# Comparing `tmp/unlimitedgpt-0.0.5.tar.gz` & `tmp/unlimitedgpt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unlimitedgpt-0.0.5.tar", max compression
+gzip compressed data, was "unlimitedgpt-0.0.6.tar", max compression
```

## Comparing `unlimitedgpt-0.0.5.tar` & `unlimitedgpt-0.0.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3889 2023-05-27 11:49:13.069369 unlimitedgpt-0.0.5/README.md
--rw-r--r--   0        0        0     1220 2023-05-27 11:49:13.069369 unlimitedgpt-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4580 1970-01-01 00:00:00.000000 unlimitedgpt-0.0.5/setup.py
--rw-r--r--   0        0        0     5316 1970-01-01 00:00:00.000000 unlimitedgpt-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3889 2023-05-27 11:57:44.166522 unlimitedgpt-0.0.6/README.md
+-rw-r--r--   0        0        0     1262 2023-05-27 11:57:44.166522 unlimitedgpt-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 unlimitedgpt-0.0.6/setup.py
+-rw-r--r--   0        0        0     5325 1970-01-01 00:00:00.000000 unlimitedgpt-0.0.6/PKG-INFO
```

### Comparing `unlimitedgpt-0.0.5/README.md` & `unlimitedgpt-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `unlimitedgpt-0.0.5/pyproject.toml` & `unlimitedgpt-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-[build-system]
-requires = ["setuptools>=42", "wheel"]
-build-backend = "setuptools.build_meta"
-
 [tool.poetry]
 name = "UnlimitedGPT"
-version = "0.0.5"
+version = "0.0.6"
 description = "An unofficial Python wrapper for OpenAI's ChatGPT API"
-authors = ["Sxvxge <sxvxge69@gmail.com>"]
 license = "GPL-3.0 license"
 readme = "README.md"
-homepage = "https://github.com/Sxvxgee/UnlimitedGPT"
 repository = "https://github.com/Sxvxgee/UnlimitedGPT"
 documentation = "https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md"
+authors = ["Sxvxge <sxvxge69@gmail.com>"]
+maintainers = ["Sxvxge <sxvxge69@gmail.com>"]
+packages = [
+    { include = "UnlimitedGPT" },
+]
+homepage = "https://github.com/Sxvxgee/UnlimitedGPT"
 keywords = ["OpenAI", "ChatGPT", "wrapper"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
@@ -24,13 +24,13 @@
     "Programming Language :: Python :: 3.10",
     "Topic :: Internet",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-packages = [
-    { include = "UnlimitedGPT" }
-]
 
 [tool.poetry.dependencies]
-python = ">=3.8.0"
+python = "^3.9"
+
+[build-system]
+requires = ["setuptools", "wheel", "markdownify", "undetected-chromedriver"]
```

### Comparing `unlimitedgpt-0.0.5/setup.py` & `unlimitedgpt-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 ['UnlimitedGPT']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'unlimitedgpt',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': "An unofficial Python wrapper for OpenAI's ChatGPT API",
     'long_description': "# UnlimitedGPT\n\n[![PyPi](https://img.shields.io/pypi/v/UnlimitedGPT.svg)](https://pypi.python.org/pypi/UnlimitedGPT)\n[![License](https://img.shields.io/github/license/Sxvxgee/UnlimitedGPT.svg?color=green)](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/LICENSE)\n\n> This is a maintained, modified and improved package of the original [pyChatGPT](https://github.com/terry3041/pyChatGPT) package. The original package is in slow development and has many issues. This package is actively maintained and updated.\n\nAn unofficial Python wrapper for OpenAI's ChatGPT API\n\n## Features\n\n-   [x] Cloudflare's anti-bot protection bypass using `undetected_chromedriver`\n-   [x] [Headless machines support](#how-do-i-get-it-to-work-on-headless-linux-server)\n-   [x] [Google Colab support](#how-do-i-get-it-to-work-on-google-colab)\n-   [x] Proxy support (only without basic auth)\n\n## Getting Started\n\n> This library is using only the `undetected_chromedriver` package to bypass Cloudflare's anti-bot protection. `requests` module is not used due to the complexity of the protection. **Please make sure you have [Google Chrome](https://www.google.com/chrome/) / [Chromium](https://www.chromium.org/) before using this wrapper.**\n\n### Installation\n\n```bash\npip install -U UnlimitedGPT\n```\n\n### Usage\n\n#### Obtaining session_token\n\n1. Go to https://chat.openai.com/chat and open the developer tools by `F12`.\n2. Find the `__Secure-next-auth.session-token` cookie in `Application` > `Storage` > `Cookies` > `https://chat.openai.com`.\n3. Copy the value in the `Cookie Value` field.\n\n![image](https://user-images.githubusercontent.com/19218518/206170122-61fbe94f-4b0c-4782-a344-e26ac0d4e2a7.png)\n\n#### Interactive mode\n\n> Currently, interactive mode is not supported in this package. But it will be added in the future.\n\n#### Import as a module\n\n```python\nfrom UnlimitedGPT import ChatGPT\n\nsession_token = 'abc123'  # `__Secure-next-auth.session-token` cookie from https://chat.openai.com/chat\napi = ChatGPT(session_token)  # auth with session token\napi = ChatGPT(session_token, conversation_id='some-random-uuid')  # specify conversation id\napi = ChatGPT(session_token, proxy='https://proxy.example.com:8080')  # specify proxy\napi = ChatGPT(session_token, chrome_args=['--window-size=1920,768'])  # specify chrome args\napi = ChatGPT(session_token, disable_moderation=True)  # disable moderation\napi = ChatGPT(session_token, verbose=True)  # verbose mode (print debug messages)\n\nmessage = api.send_message('Hello, world!')\nprint(message.response, message.conversation_id)\n\napi.reset_conversation()  # reset the conversation\n```\n\n## Frequently Asked Questions\n\n### How do I get it to work on headless linux server?\n\n```bash\n# install chromium & X virtual framebuffer\nsudo apt install chromium-browser xvfb\n\n# start your script\npython3 your_script.py\n```\n\n### How do I get it to work on Google Colab?\n\nIt is normal for the seession to be crashed when installing dependencies. Just ignore the error and run your script.\n\n```python\n# install dependencies\n!apt install chromium-browser xvfb\n!pip install -U selenium_profiles UnlimitedGPT\n\n# install chromedriver\nfrom selenium_profiles.utils.installer import install_chromedriver\ninstall_chromedriver()\n```\n\n```python\n# start your script as normal\n!python3 -m UnlimitedGPT\n```\n\n## Insipration\n\nThis project is inspired by\n\n-   [ChatGPT](https://github.com/acheong08/ChatGPT)\n-   [chatgpt-api](https://github.com/transitive-bullshit/chatgpt-api)\n-   [pyChatGPT](https://github.com/terry3041/pyChatGPT)\n\n## Disclaimer\n\nThis project is not affiliated with OpenAI in any way. Use at your own risk. I am not responsible for any damage caused by this project. Please read the [OpenAI Terms of Service](https://beta.openai.com/terms) before using this project.\n\n## License\n\nThis project is licensed under the GPLv3 License - see the [LICENSE](LICENSE) file for details.\n",
     'author': 'Sxvxge',
     'author_email': 'sxvxge69@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
+    'maintainer': 'Sxvxge',
+    'maintainer_email': 'sxvxge69@gmail.com',
     'url': 'https://github.com/Sxvxgee/UnlimitedGPT',
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.8.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `unlimitedgpt-0.0.5/PKG-INFO` & `unlimitedgpt-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: unlimitedgpt
-Version: 0.0.5
+Version: 0.0.6
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 License: GPL-3.0 license
 Keywords: OpenAI,ChatGPT,wrapper
 Author: Sxvxge
 Author-email: sxvxge69@gmail.com
-Requires-Python: >=3.8.0
+Maintainer: Sxvxge
+Maintainer-email: sxvxge69@gmail.com
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
```

