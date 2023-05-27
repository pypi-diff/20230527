# Comparing `tmp/pronoundb-1.2.0.tar.gz` & `tmp/pronoundb-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pronoundb-1.2.0.tar", max compression
+gzip compressed data, was "pronoundb-2.0.0.tar", max compression
```

## Comparing `pronoundb-1.2.0.tar` & `pronoundb-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1091 2022-11-18 17:05:56.697373 pronoundb-1.2.0/LICENSE
--rw-r--r--   0        0        0       93 2022-11-18 16:02:01.482088 pronoundb-1.2.0/pronoundb/__init__.py
--rw-r--r--   0        0        0     3888 2022-11-19 23:16:22.409484 pronoundb-1.2.0/pronoundb/api.py
--rw-r--r--   0        0        0      202 2022-11-18 16:02:01.468729 pronoundb-1.2.0/pronoundb/platform.py
--rw-r--r--   0        0        0      641 2022-11-19 23:19:17.580807 pronoundb-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1145 2022-11-19 23:05:03.364270 pronoundb-1.2.0/README.md
--rw-r--r--   0        0        0     1850 1970-01-01 00:00:00.000000 pronoundb-1.2.0/setup.py
--rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 pronoundb-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-11-18 17:05:56.697373 pronoundb-2.0.0/LICENSE
+-rw-r--r--   0        0        0       93 2022-11-18 16:02:01.482088 pronoundb-2.0.0/pronoundb/__init__.py
+-rw-r--r--   0        0        0     3026 2023-05-27 21:33:50.816512 pronoundb-2.0.0/pronoundb/api.py
+-rw-r--r--   0        0        0      175 2023-05-27 21:01:46.113572 pronoundb-2.0.0/pronoundb/platform.py
+-rw-r--r--   0        0        0      664 2023-05-27 21:40:24.484655 pronoundb-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1889 2023-05-27 21:42:02.059224 pronoundb-2.0.0/README.md
+-rw-r--r--   0        0        0     2596 1970-01-01 00:00:00.000000 pronoundb-2.0.0/setup.py
+-rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 pronoundb-2.0.0/PKG-INFO
```

### Comparing `pronoundb-1.2.0/LICENSE` & `pronoundb-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pronoundb-1.2.0/pronoundb/api.py` & `pronoundb-2.0.0/pronoundb/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,102 +1,78 @@
 import typing
 import urllib.parse
+
 import aiohttp
 
 from .platform import Platform
 
 _english_pronouns: dict[str, list[str]] = {
     "unspecified": [],
-    "hh": ["he", "him"],
-    "hi": ["he", "it"],
-    "hs": ["he", "she"],
-    "ht": ["he", "they"],
-    "ih": ["it", "he"],
-    "ii": ["it", "its"],
-    "is": ["it", "she"],
-    "it": ["it", "they"],
-    "shh": ["she", "he"],
-    "sh": ["she", "her"],
-    "si": ["she", "it"],
-    "st": ["she", "they"],
-    "th": ["they", "he"],
-    "ti": ["they", "it"],
-    "ts": ["they", "she"],
-    "tt": ["they", "them"],
+    "he": ["he", "him"],
+    "she": ["she", "her"],
+    "they": ["they", "them"],
     "any": ["any"],
     "other": ["other"],
     "ask": ["ask"],
     "avoid": ["use name"],
 }
 
 
-async def lookup(platform: Platform, identifiers: typing.Union[str, int, list[str], list[int]]) -> typing.Union[dict[str, list[str]], dict[int, list[str]]]:
+async def lookup(platform: Platform, identifiers: typing.Union[str, int, list[str], list[int]], pronouns=None) -> \
+        typing.Union[dict[str, list[str]], dict[int, list[str]]]:
     """
     Sends a request to the PronounDB API to get the pronouns of one or multiple users.
     If more than 50 identifiers are passed, the wrapper will automatically split the request into multiple requests.
 
     :param platform: One of the supported platforms (see the Platform enum)
     :param identifiers: Account IDs on the platform
+    :param pronouns: An optional parameter that allows specifying the desired language for the returned pronouns.
+                     By default, English pronouns are used (see _english_pronouns).
+                     You can use this argument to retrieve pronouns in other languages by providing
+                     a dictionary with the corresponding pronouns for the desired language.
     :return: The pronouns of the users as a list of all the pronouns the users use
     """
 
-    if isinstance(identifiers, list) and len(identifiers) == 1:
-        identifiers = identifiers[0]
-
-    if isinstance(identifiers, list):
-        return await _lookup_bulk(platform, identifiers)
-    else:
-        return await _lookup_single(platform, identifiers)
-
-
-async def _lookup_single(platform: Platform, identifier: typing.Union[str, int]) -> typing.Union[dict[str, list[str]], dict[int, list[str]]]:
-    """
-    Sends a request to the PronounDB API to get the pronouns of a user.
-
-    :param platform: One of the supported platforms (see the Platform enum)
-    :param identifier: Account ID on the platform
-    :return: The pronouns of the user as specified in the PronounDB docs
-    """
+    if pronouns is None:
+        pronouns = _english_pronouns
 
-    async with aiohttp.ClientSession() as session:
-        async with session.get("https://pronoundb.org/api/v1/lookup?platform={0}&id={1}".format(
-                platform.value,
-                urllib.parse.quote_plus(str(identifier))
-        )) as resp:
-            data = await resp.json()
+    if not isinstance(identifiers, list):
+        identifiers = [identifiers]
 
-            if "error" in data:
-                raise ValueError(f'{data["error"]}: {data["message"]}')
+    def get_pronouns_set(pronoun: str) -> list[str]:
+        if not pronoun in pronouns:
+            raise ValueError(f'{pronoun} not in pronouns parameter.')
 
-            return {identifier: _english_pronouns[data["pronouns"]]}
-
-
-async def _lookup_bulk(platform: Platform, identifiers: typing.Union[list[str], list[int]]) -> typing.Union[dict[str, list[str]], dict[int, list[str]]]:
-    """
-    Sends a request to the PronounDB API to get the pronouns of multiple users.
-    If more than 50 identifiers are passed, the wrapper will automatically split the request into multiple requests.
-
-    :param platform: One of the supported platforms (see the Platform enum)
-    :param identifiers: A list of account IDs on the platform
-    :return: A dict with the account IDs as keys and the pronouns as values
-    """
-    # Make bulk requests of 50 users at a time
+        return pronouns[pronoun]
 
     all_results = {}
 
     for i in range(0, len(identifiers), 50):
         batch: typing.Union[list[str], list[int]] = identifiers[i:i + 50]
 
         async with aiohttp.ClientSession() as session:
-            async with session.get("https://pronoundb.org/api/v1/lookup-bulk?platform={0}&ids={1}".format(
+            async with session.get("https://pronoundb.org/api/v2/lookup?platform={0}&ids={1}".format(
                     platform.value,
                     urllib.parse.quote_plus(",".join(map(str, batch)))
             )) as resp:
                 data = await resp.json()
 
                 if "error" in data:
                     raise ValueError(f'{data["error"]}: {data["message"]}')
 
                 for identifier in batch:
-                    all_results[identifier] = _english_pronouns[data[str(identifier)]]
+                    if len(data) == 0:
+                        all_results[identifier] = get_pronouns_set("unspecified")
+                        continue
+
+                    user_data = data[str(identifier)]
+                    english_set = user_data["sets"]["en"]
+
+                    if len(english_set) == 1:
+                        all_results[identifier] = get_pronouns_set(english_set[0])
+                    else:
+                        all_results[identifier] = [
+                            get_pronouns_set(english_set[0])[0],
+                            get_pronouns_set(english_set[1])[0]
+                        ]
 
     return all_results
```

### Comparing `pronoundb-1.2.0/pyproject.toml` & `pronoundb-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pronoundb"
-version = "1.2.0"
+version = "2.0.0"
 description = "API wrapper for the pronoundb.org API."
 license = "MIT"
 authors = ["SteffoSpieler <steffo@steffospieler.de>"]
 maintainers = ["SteffoSpieler <steffo@steffospieler.de>"]
 readme = "README.md"
 repository = "https://gitlab.com/SteffoSpieler/pronoundb-library"
 keywords = ["pronouns", "pronoundb", "api"]
@@ -13,11 +13,12 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 aiohttp = "^3.8"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 pytest-runner = "^6.0"
+pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pronoundb-1.2.0/setup.py` & `pronoundb-2.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8,<4.0']
 
 setup_kwargs = {
     'name': 'pronoundb',
-    'version': '1.2.0',
+    'version': '2.0.0',
     'description': 'API wrapper for the pronoundb.org API.',
-    'long_description': '# PronounDB Python API\n\nAPI wrapper for the pronoundb.org API.\n\n## Installation\n\n```bash\npip install pronoundb\n```\n\n## Examples\n\nlookup someones pronouns by their discord id:\n\n```py\nfrom pronoundb import lookup, Platform\n\nlookup(Platform.DISCORD, 123456789012345678)\n# -> {123456789012345678: ["he", "him"]}\n```\n\nlookup someones pronouns by their minecraft (java) uuid:\n\n```py\nfrom pronoundb import lookup, Platform\n\nlookup(Platform.MINECRAFT, "12345678-1234-1234-1234-123456789012")\n# -> {"12345678-1234-1234-1234-123456789012": ["they", "them"]}\n```\n\nlookup multiple users pronouns by their discord id:\n\n```py\nfrom pronoundb import lookup, Platform\n\nlookup(Platform.DISCORD, [123456789012345678, 987654321098765432])\n# -> {123456789012345678: ["he", "him"], 987654321098765432: ["she", "her"]}\n```\n\n## Supported Platforms\n\n- Discord\n- Facebook\n- GitHub\n- Minecraft (Java)\n- Twitch\n- Twitter\n\n## Contributing\n\nContributions to this library are always welcome and highly encouraged.\n\n## License\n\nThis project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.\n',
+    'long_description': '# PronounDB Python API\n\n![PyPI](https://img.shields.io/pypi/v/pronoundb?style=flat-square)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pronoundb?style=flat-square)\n![PyPI - License](https://img.shields.io/pypi/l/pronoundb?style=flat-square)\n\nAPI wrapper for the pronoundb.org API.\n\n## Installation\n\n```bash\npip install pronoundb\n```\n\n## Examples\n\nlookup someone\'s pronouns by their discord id:\n\n```py\nfrom pronoundb import lookup, Platform\n\nlookup(Platform.DISCORD, 123456789012345678)\n# -> {123456789012345678: ["he", "him"]}\n```\n\nlookup someone\'s pronouns by their minecraft (java) uuid:\n\n```py\nfrom pronoundb import lookup, Platform\n\nlookup(Platform.MINECRAFT, "12345678-1234-1234-1234-123456789012")\n# -> {"12345678-1234-1234-1234-123456789012": ["they", "them"]}\n```\n\nlookup multiple users pronouns by their discord id:\n\n```py\nfrom pronoundb import lookup, Platform\n\nlookup(Platform.DISCORD, [123456789012345678, 987654321098765432])\n# -> {123456789012345678: ["he", "him"], 987654321098765432: ["she", "her"]}\n```\n\n## Supported Platforms\n\n- Discord\n- GitHub\n- Minecraft (Java)\n- Twitch\n- Twitter\n\n## Custom Pronouns (Version 2.0.0)\n\nBeginning with version 2.0.0 you can give the lookup function a list of pronouns to translate them for example.\n\n```py\nfrom pronoundb import lookup, Platform\n\nlookup(Platform.DISCORD, 123456789012345678, {\n    "unspecified": [],\n    "he": ["Er", "Ihn"],\n    "she": ["Sie", "Ihr"],\n    "they": ["They", "Them"],\n    "any": ["Jede"],\n    "other": ["Anderes"],\n    "ask": ["Frag"],\n    "avoid": ["Nutz Name"],\n})\n# -> {123456789012345678: ["Er", "Ihn"]}\n```\n\n## Contributing\n\nContributions to this library are always welcome and highly encouraged.\n\n## License\n\nThis project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.\n',
     'author': 'SteffoSpieler',
     'author_email': 'steffo@steffospieler.de',
     'maintainer': 'SteffoSpieler',
     'maintainer_email': 'steffo@steffospieler.de',
     'url': 'https://gitlab.com/SteffoSpieler/pronoundb-library',
     'packages': packages,
     'package_data': package_data,
```

