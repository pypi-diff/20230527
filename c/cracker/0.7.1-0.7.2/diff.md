# Comparing `tmp/cracker-0.7.1.tar.gz` & `tmp/cracker-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cracker-0.7.1.tar", last modified: Thu May 25 03:41:32 2023, max compression
+gzip compressed data, was "cracker-0.7.2.tar", last modified: Sat May 27 00:29:51 2023, max compression
```

## Comparing `cracker-0.7.1.tar` & `cracker-0.7.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.583131 cracker-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.571131 cracker-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.575131 cracker-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-25 03:41:17.000000 cracker-0.7.1/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 03:41:17.000000 cracker-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 03:41:17.000000 cracker-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 03:41:17.000000 cracker-0.7.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-25 03:41:32.583131 cracker-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-25 03:41:17.000000 cracker-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.575131 cracker-0.7.1/cracker/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/cracker/config/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/config/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/config/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/config/parser.json
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/cracker_gui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2206 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/icon.jpeg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4856 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/keylogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/mp3_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/cracker/speaker/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/speaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/speaker/abstract_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/speaker/espeak.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/speaker/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/speaker/polly.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/ssml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/cracker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/tests/test_text_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/text_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   425242 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/cracker/view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/view/config_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/view/parser_config_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/view/speaker_config_tab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/cracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-25 03:41:32.000000 cracker-0.7.1/cracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-25 03:41:32.000000 cracker-0.7.1/cracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 03:41:32.000000 cracker-0.7.1/cracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 03:41:32.000000 cracker-0.7.1/cracker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 03:41:32.000000 cracker-0.7.1/cracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 03:41:32.000000 cracker-0.7.1/cracker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-25 03:41:17.000000 cracker-0.7.1/docs/macos.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 03:41:17.000000 cracker-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 03:41:32.583131 cracker-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/ubuntu/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-25 03:41:17.000000 cracker-0.7.1/ubuntu/cracker.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-25 03:41:17.000000 cracker-0.7.1/ubuntu/icon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-05-25 03:41:17.000000 cracker-0.7.1/ubuntu/install_ubuntu.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.601784 cracker-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.589784 cracker-0.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.593784 cracker-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-27 00:29:31.000000 cracker-0.7.2/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 00:29:31.000000 cracker-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-27 00:29:31.000000 cracker-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-27 00:29:31.000000 cracker-0.7.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-27 00:29:51.601784 cracker-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-27 00:29:31.000000 cracker-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.597784 cracker-0.7.2/cracker/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.597784 cracker-0.7.2/cracker/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/config/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/config/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/config/parser.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/cracker_gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2206 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/icon.jpeg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4856 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/keylogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/mp3_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.597784 cracker-0.7.2/cracker/speaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/speaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/speaker/abstract_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/speaker/espeak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/speaker/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/speaker/polly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/ssml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.597784 cracker-0.7.2/cracker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/tests/test_text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   425242 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.601784 cracker-0.7.2/cracker/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/view/config_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/view/parser_config_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/view/speaker_config_tab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.597784 cracker-0.7.2/cracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-27 00:29:51.000000 cracker-0.7.2/cracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-27 00:29:51.000000 cracker-0.7.2/cracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 00:29:51.000000 cracker-0.7.2/cracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-27 00:29:51.000000 cracker-0.7.2/cracker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-27 00:29:51.000000 cracker-0.7.2/cracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-27 00:29:51.000000 cracker-0.7.2/cracker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.601784 cracker-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-27 00:29:31.000000 cracker-0.7.2/docs/macos.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 00:29:31.000000 cracker-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 00:29:51.601784 cracker-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.601784 cracker-0.7.2/ubuntu/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-27 00:29:31.000000 cracker-0.7.2/ubuntu/cracker.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-27 00:29:31.000000 cracker-0.7.2/ubuntu/icon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-05-27 00:29:31.000000 cracker-0.7.2/ubuntu/install_ubuntu.sh
```

### Comparing `cracker-0.7.1/.github/workflows/publish-pypi.yml` & `cracker-0.7.2/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/LICENSE` & `cracker-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/PKG-INFO` & `cracker-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cracker
-Version: 0.7.1
+Version: 0.7.2
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: build
 Provides-Extra: test
 License-File: LICENSE
 
 # Cracker
```

### Comparing `cracker-0.7.1/README.md` & `cracker-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/config/configuration.py` & `cracker-0.7.2/cracker/config/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     """Holds configuration values for the application."""
 
     singleton = None
     _logger = get_logger(__name__)
 
     language_file = "voices.json"
     DEFAULT_CONFIG_PATH = "config/default.yaml"
+    DEFAULT_PARSER_PATH = "config/parser.json"
     USER_CONFIG_DIR_PATH = os.path.expanduser("~/.config/cracker")
 
     languages = []
 
     speaker = None
     language = None
     voice = None
@@ -142,16 +143,14 @@
         # Check for different than default AWS profile_name
         _config["polly"]["profile_name"] = config_speakers.get("polly", {}).get("profile_name", "default")
 
         if self.voice not in self.lang_voices:
             _config["voice"] = self.voice = self.lang_voices[0]
 
         self.regex_config = self.load_regex_config()
-        print(f"Regex: {self.regex_config}")
-
         return _config
 
     def load_speaker_config(self, speaker, language=None):
         """Loads speaker's default and available configuration.
 
         Args:
             speaker: Name of the speaker.
@@ -178,21 +177,20 @@
         regex_config = None
 
         if not os.path.isdir(self.USER_CONFIG_DIR_PATH):
             self._logger.debug("Creating user dir in '%s'", self.USER_CONFIG_DIR_PATH)
             os.mkdir(self.USER_CONFIG_DIR_PATH)
 
         if not os.path.isfile(self.user_parser_path):
-            file_content = pkgutil.get_data("cracker", "config/parser.json")
+            file_content = pkgutil.get_data("cracker", self.DEFAULT_PARSER_PATH)
             file_content = file_content.decode("utf-8")
         else:
             with open(self.user_parser_path) as f:
                 file_content = f.read()
         regex_config = json.loads(file_content)["parser_rules"]
-        return {v["name"]: v for v in regex_config}
+        return regex_config
 
     def save_regex_config(self, parser_config_path: str) -> None:
         """Writes configuration to file system."""
         parser_rules = {"parser_rules": self.regex_config}
-        print(parser_rules)
         with open(parser_config_path, "w") as f:
             json.dump(parser_rules, f, indent=4)
```

### Comparing `cracker-0.7.1/cracker/config/parser.json` & `cracker-0.7.2/cracker/config/parser.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'parser_rules'": "{replace: OrderedDict([('citation_compact_all', OrderedDict([('name', "*

 * *                   "'citation_compact_all'), ('active', True), ('key', "*

 * *                   "'[\\\\(\\\\[](((and\\\\s)?[A-Z]\\\\w+(\\\\set\\\\sal\\\\.)?\\\\W?\\\\s)+\\\\d{4}([;]\\\\s)?)+[\\\\)\\\\]]'), "*

 * *                   "('value', '')])), ('citation_author_year', OrderedDict([('name', "*

 * *                   "'citation_author_year'), ('active', False), ('key', "*

 * *                   "'[\\\\(\\\\[](([A-Z]\\\\w+(\\\\set\ […]*

```diff
@@ -1,52 +1,52 @@
 {
-    "parser_rules": [
-        {
-            "active": true,
-            "key": "[\\(\\[](((and\\s)?[A-Z]\\w+(\\set\\sal\\.)?\\W?\\s)+\\d{4}([;]\\s)?)+[\\)\\]]",
-            "name": "citation_compact_all",
-            "value": ""
-        },
-        {
+    "parser_rules": {
+        "citation_author_year": {
             "active": false,
             "key": "[\\(\\[](([A-Z]\\w+(\\set\\sal\\.)?,\\s\\d{4})([;]\\s)?){1,}[\\]\\)]",
             "name": "citation_author_year",
             "value": ""
         },
-        {
+        "citation_compact_all": {
+            "active": true,
+            "key": "[\\(\\[](((and\\s)?[A-Z]\\w+(\\set\\sal\\.)?\\W?\\s)+\\d{4}([;]\\s)?)+[\\)\\]]",
+            "name": "citation_compact_all",
+            "value": ""
+        },
+        "citation_numbers_comma": {
             "active": false,
             "key": "\\[\\d+(,\\s*\\d+)*\\]",
             "name": "citation_numbers_comma",
             "value": ""
         },
-        {
+        "extensive_new_line": {
             "active": true,
             "key": "\\n\\s*?(?=[a-z])",
             "name": "extensive_new_line",
             "value": " "
         },
-        {
+        "hypthened_new_line": {
             "active": true,
             "key": "-\\n",
             "name": "hypthened_new_line",
             "value": ""
         },
-        {
+        "just_dash": {
             "active": true,
             "key": "- ",
             "name": "just_dash",
             "value": ""
         },
-        {
+        "tabs": {
             "active": true,
             "key": "\\t",
             "name": "tabs",
             "value": " "
         },
-        {
+        "trailing_whitespace": {
             "active": false,
             "key": "\\b\\s+\\.",
             "name": "trailing_whitespace",
             "value": "."
         }
-    ]
+    }
 }
```

### Comparing `cracker-0.7.1/cracker/cracker.py` & `cracker-0.7.2/cracker/cracker.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/cracker_gui.py` & `cracker-0.7.2/cracker/cracker_gui.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/icon.jpeg` & `cracker-0.7.2/cracker/icon.jpeg`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/icon.png` & `cracker-0.7.2/cracker/icon.png`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/keylogger.py` & `cracker-0.7.2/cracker/keylogger.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/main.py` & `cracker-0.7.2/cracker/main.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/mp3_helper.py` & `cracker-0.7.2/cracker/mp3_helper.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/speaker/__init__.py` & `cracker-0.7.2/cracker/speaker/__init__.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/speaker/abstract_speaker.py` & `cracker-0.7.2/cracker/speaker/abstract_speaker.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/speaker/espeak.py` & `cracker-0.7.2/cracker/speaker/espeak.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/speaker/google.py` & `cracker-0.7.2/cracker/speaker/google.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/speaker/polly.py` & `cracker-0.7.2/cracker/speaker/polly.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/ssml.py` & `cracker-0.7.2/cracker/ssml.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/tests/test_config.py` & `cracker-0.7.2/cracker/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/tests/test_text_parser.py` & `cracker-0.7.2/cracker/tests/test_text_parser.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/text_parser.py` & `cracker-0.7.2/cracker/text_parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,49 +9,38 @@
 class TextParser:
     _logger = logging.getLogger(__name__)
 
     citation_author_year = re.compile(r"[\(\[]\w+, \d{4}(;\s\w+, \d{4})*[\)\]]")
     citation_numbers_comma = re.compile(r"\[\d+(,\s*\d+)*\]")
 
     def __init__(self):
-        self._config = None
         self._parser_rules = None
         self._regex_rules = OrderedDict()
 
         global_config = Configuration()
-        self.config = global_config.load_regex_config()
-
-    @property
-    def config(self):
-        return self._config
-
-    @config.setter
-    def config(self, config):
-        self._config = config
-        self.update_config()
+        self.parser_rules = global_config.load_regex_config()
 
     @property
     def parser_rules(self):
         return self._parser_rules
 
     @parser_rules.setter
     def parser_rules(self, parser_rules):
-        assert self._config, "Need to provide config before parser"
-        self._config["parser_rules"] = parser_rules
+        self._parser_rules = parser_rules
         self.update_config()
 
     def update_config(self):
         """Goes through the config and extracts regex rules."""
-        if self.config is None:
+        if self.parser_rules is None:
             return
 
         # Clears all regex rules
         self._regex_rules.clear()
 
-        for rule in self.config.values():
+        for rule in self.parser_rules.values():
             if not rule["active"]:
                 continue
             self._regex_rules[rule["key"]] = rule["value"]
 
     @classmethod
     def reduce_cite(cls, text: str) -> str:
         """Removes citations from pasted text."""
```

### Comparing `cracker-0.7.1/cracker/themes.py` & `cracker-0.7.2/cracker/themes.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/utils.py` & `cracker-0.7.2/cracker/utils.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/view/config_window.py` & `cracker-0.7.2/cracker/view/config_window.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker/view/parser_config_tab.py` & `cracker-0.7.2/cracker/view/parser_config_tab.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,40 +23,22 @@
 
     def init(self):
         self.regex_config = self.config.regex_config
         self.create_options(self.regex_config)
 
     def confirm_action(self) -> List:
         self.check_update()
-        return self.get_regex_config()
+        return self.regex_config
 
     def clearLayout(layout):
         while layout.count():
             child = layout.takeAt(0)
             if child.widget():
                 child.widget().deleteLater()
 
-    def refresh_reduce_rules(self) -> Optional[Dict]:
-        """From provided path to a config it extracts configuration for the TextParser"""
-        regex_config_list = {}
-        try:
-            file_content = pkgutil.get_data("cracker", self.regex_file_path)
-            if file_content is None:
-                raise FileNotFoundError(f"Could not find config file {self.regex_file_path}")
-            regex_config_list = json.loads(file_content.decode("utf-8"))
-        except Exception:
-            self._logger.exception("While reading config")
-
-        regex_config = {}
-        for regex_entry in regex_config_list["parser_rules"]:
-            name = regex_entry["name"]
-            regex_config[name] = regex_entry
-
-        return regex_config
-
     def create_options(self, options):
         regex_config_options = RegexConfigOptions(options)
         self.layout.addWidget(regex_config_options, 0, 0, 1, 5)
 
     def check_update(self) -> None:
         """Iterate through every option and see it they're active"""
         assert self.regex_config, "Regex config hasn't been loaded"
@@ -70,18 +52,14 @@
 
             # TODO: Oopsy! Can't change name!
             if name in self.regex_config:
                 self.regex_config[name]["active"] = active_box.isChecked()
                 self.regex_config[name]["key"] = key_box.text()
                 self.regex_config[name]["value"] = value_box.text()
 
-    def get_regex_config(self) -> List:
-        assert self.regex_config, "Regex config hasn't been loaded"
-        return list(self.regex_config.values())
-
 
 class RegexConfigOptions(QWidget):
     ACTIVE_POS = 1
     NAME_POS = 2
     KEY_POS = 6
     VALUE_POS = 10
```

### Comparing `cracker-0.7.1/cracker/view/speaker_config_tab.py` & `cracker-0.7.2/cracker/view/speaker_config_tab.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/cracker.egg-info/PKG-INFO` & `cracker-0.7.2/cracker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cracker
-Version: 0.7.1
+Version: 0.7.2
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: build
 Provides-Extra: test
 License-File: LICENSE
 
 # Cracker
```

### Comparing `cracker-0.7.1/cracker.egg-info/SOURCES.txt` & `cracker-0.7.2/cracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/pyproject.toml` & `cracker-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/ubuntu/icon.png` & `cracker-0.7.2/ubuntu/icon.png`

 * *Files identical despite different names*

### Comparing `cracker-0.7.1/ubuntu/install_ubuntu.sh` & `cracker-0.7.2/ubuntu/install_ubuntu.sh`

 * *Files identical despite different names*

