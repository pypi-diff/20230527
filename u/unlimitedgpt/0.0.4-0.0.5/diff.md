# Comparing `tmp/UnlimitedGPT-0.0.4.tar.gz` & `tmp/unlimitedgpt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.0.4.tar", last modified: Sat May 27 11:07:13 2023, max compression
+gzip compressed data, was "unlimitedgpt-0.0.5.tar", max compression
```

## Comparing `UnlimitedGPT-0.0.4.tar` & `unlimitedgpt-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,4 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 11:07:13.394724 UnlimitedGPT-0.0.4/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    35149 2023-05-26 09:35:45.000000 UnlimitedGPT-0.0.4/LICENSE
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4982 2023-05-27 11:07:13.394724 UnlimitedGPT-0.0.4/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3889 2023-05-27 11:05:02.000000 UnlimitedGPT-0.0.4/README.md
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 11:07:13.390724 UnlimitedGPT-0.0.4/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4982 2023-05-27 11:07:13.000000 UnlimitedGPT-0.0.4/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      377 2023-05-27 11:07:13.000000 UnlimitedGPT-0.0.4/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-05-27 11:07:13.000000 UnlimitedGPT-0.0.4/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-05-27 11:07:13.000000 UnlimitedGPT-0.0.4/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       44 2023-05-27 11:07:13.000000 UnlimitedGPT-0.0.4/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-05-27 11:07:13.394724 UnlimitedGPT-0.0.4/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1529 2023-05-27 11:06:45.000000 UnlimitedGPT-0.0.4/setup.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 11:07:13.374723 UnlimitedGPT-0.0.4/src/
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 11:07:13.390724 UnlimitedGPT-0.0.4/src/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    13097 2023-05-27 10:02:18.000000 UnlimitedGPT-0.0.4/src/UnlimitedGPT/ChatGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      244 2023-05-27 10:00:18.000000 UnlimitedGPT-0.0.4/src/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 11:07:13.394724 UnlimitedGPT-0.0.4/src/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1710 2023-05-27 09:21:23.000000 UnlimitedGPT-0.0.4/src/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      294 2023-05-27 10:01:38.000000 UnlimitedGPT-0.0.4/src/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      494 2023-05-27 09:58:48.000000 UnlimitedGPT-0.0.4/src/UnlimitedGPT/internal/objects.py
+-rw-r--r--   0        0        0     3889 2023-05-27 11:49:13.069369 unlimitedgpt-0.0.5/README.md
+-rw-r--r--   0        0        0     1220 2023-05-27 11:49:13.069369 unlimitedgpt-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4580 1970-01-01 00:00:00.000000 unlimitedgpt-0.0.5/setup.py
+-rw-r--r--   0        0        0     5316 1970-01-01 00:00:00.000000 unlimitedgpt-0.0.5/PKG-INFO
```

### Comparing `UnlimitedGPT-0.0.4/PKG-INFO` & `unlimitedgpt-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 Metadata-Version: 2.1
-Name: UnlimitedGPT
-Version: 0.0.4
+Name: unlimitedgpt
+Version: 0.0.5
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
-Author: Sxvxge
 License: GPL-3.0 license
-Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
-Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
+Keywords: OpenAI,ChatGPT,wrapper
+Author: Sxvxge
+Author-email: sxvxge69@gmail.com
+Requires-Python: >=3.8.0
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: >=3.8.0
+Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
+Project-URL: Repository, https://github.com/Sxvxgee/UnlimitedGPT
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # UnlimitedGPT
 
 [![PyPi](https://img.shields.io/pypi/v/UnlimitedGPT.svg)](https://pypi.python.org/pypi/UnlimitedGPT)
 [![License](https://img.shields.io/github/license/Sxvxgee/UnlimitedGPT.svg?color=green)](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/LICENSE)
 
 > This is a maintained, modified and improved package of the original [pyChatGPT](https://github.com/terry3041/pyChatGPT) package. The original package is in slow development and has many issues. This package is actively maintained and updated.
@@ -125,7 +132,8 @@
 ## Disclaimer
 
 This project is not affiliated with OpenAI in any way. Use at your own risk. I am not responsible for any damage caused by this project. Please read the [OpenAI Terms of Service](https://beta.openai.com/terms) before using this project.
 
 ## License
 
 This project is licensed under the GPLv3 License - see the [LICENSE](LICENSE) file for details.
+
```

### Comparing `UnlimitedGPT-0.0.4/README.md` & `unlimitedgpt-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.0.4/UnlimitedGPT.egg-info/PKG-INFO` & `unlimitedgpt-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,131 +1,26 @@
-Metadata-Version: 2.1
-Name: UnlimitedGPT
-Version: 0.0.4
-Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
-Home-page: https://github.com/Sxvxgee/UnlimitedGPT
-Author: Sxvxge
-License: GPL-3.0 license
-Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
-Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-# UnlimitedGPT
+packages = \
+['UnlimitedGPT']
 
-[![PyPi](https://img.shields.io/pypi/v/UnlimitedGPT.svg)](https://pypi.python.org/pypi/UnlimitedGPT)
-[![License](https://img.shields.io/github/license/Sxvxgee/UnlimitedGPT.svg?color=green)](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/LICENSE)
+package_data = \
+{'': ['*']}
 
-> This is a maintained, modified and improved package of the original [pyChatGPT](https://github.com/terry3041/pyChatGPT) package. The original package is in slow development and has many issues. This package is actively maintained and updated.
+setup_kwargs = {
+    'name': 'unlimitedgpt',
+    'version': '0.0.5',
+    'description': "An unofficial Python wrapper for OpenAI's ChatGPT API",
+    'long_description': "# UnlimitedGPT\n\n[![PyPi](https://img.shields.io/pypi/v/UnlimitedGPT.svg)](https://pypi.python.org/pypi/UnlimitedGPT)\n[![License](https://img.shields.io/github/license/Sxvxgee/UnlimitedGPT.svg?color=green)](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/LICENSE)\n\n> This is a maintained, modified and improved package of the original [pyChatGPT](https://github.com/terry3041/pyChatGPT) package. The original package is in slow development and has many issues. This package is actively maintained and updated.\n\nAn unofficial Python wrapper for OpenAI's ChatGPT API\n\n## Features\n\n-   [x] Cloudflare's anti-bot protection bypass using `undetected_chromedriver`\n-   [x] [Headless machines support](#how-do-i-get-it-to-work-on-headless-linux-server)\n-   [x] [Google Colab support](#how-do-i-get-it-to-work-on-google-colab)\n-   [x] Proxy support (only without basic auth)\n\n## Getting Started\n\n> This library is using only the `undetected_chromedriver` package to bypass Cloudflare's anti-bot protection. `requests` module is not used due to the complexity of the protection. **Please make sure you have [Google Chrome](https://www.google.com/chrome/) / [Chromium](https://www.chromium.org/) before using this wrapper.**\n\n### Installation\n\n```bash\npip install -U UnlimitedGPT\n```\n\n### Usage\n\n#### Obtaining session_token\n\n1. Go to https://chat.openai.com/chat and open the developer tools by `F12`.\n2. Find the `__Secure-next-auth.session-token` cookie in `Application` > `Storage` > `Cookies` > `https://chat.openai.com`.\n3. Copy the value in the `Cookie Value` field.\n\n![image](https://user-images.githubusercontent.com/19218518/206170122-61fbe94f-4b0c-4782-a344-e26ac0d4e2a7.png)\n\n#### Interactive mode\n\n> Currently, interactive mode is not supported in this package. But it will be added in the future.\n\n#### Import as a module\n\n```python\nfrom UnlimitedGPT import ChatGPT\n\nsession_token = 'abc123'  # `__Secure-next-auth.session-token` cookie from https://chat.openai.com/chat\napi = ChatGPT(session_token)  # auth with session token\napi = ChatGPT(session_token, conversation_id='some-random-uuid')  # specify conversation id\napi = ChatGPT(session_token, proxy='https://proxy.example.com:8080')  # specify proxy\napi = ChatGPT(session_token, chrome_args=['--window-size=1920,768'])  # specify chrome args\napi = ChatGPT(session_token, disable_moderation=True)  # disable moderation\napi = ChatGPT(session_token, verbose=True)  # verbose mode (print debug messages)\n\nmessage = api.send_message('Hello, world!')\nprint(message.response, message.conversation_id)\n\napi.reset_conversation()  # reset the conversation\n```\n\n## Frequently Asked Questions\n\n### How do I get it to work on headless linux server?\n\n```bash\n# install chromium & X virtual framebuffer\nsudo apt install chromium-browser xvfb\n\n# start your script\npython3 your_script.py\n```\n\n### How do I get it to work on Google Colab?\n\nIt is normal for the seession to be crashed when installing dependencies. Just ignore the error and run your script.\n\n```python\n# install dependencies\n!apt install chromium-browser xvfb\n!pip install -U selenium_profiles UnlimitedGPT\n\n# install chromedriver\nfrom selenium_profiles.utils.installer import install_chromedriver\ninstall_chromedriver()\n```\n\n```python\n# start your script as normal\n!python3 -m UnlimitedGPT\n```\n\n## Insipration\n\nThis project is inspired by\n\n-   [ChatGPT](https://github.com/acheong08/ChatGPT)\n-   [chatgpt-api](https://github.com/transitive-bullshit/chatgpt-api)\n-   [pyChatGPT](https://github.com/terry3041/pyChatGPT)\n\n## Disclaimer\n\nThis project is not affiliated with OpenAI in any way. Use at your own risk. I am not responsible for any damage caused by this project. Please read the [OpenAI Terms of Service](https://beta.openai.com/terms) before using this project.\n\n## License\n\nThis project is licensed under the GPLv3 License - see the [LICENSE](LICENSE) file for details.\n",
+    'author': 'Sxvxge',
+    'author_email': 'sxvxge69@gmail.com',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'https://github.com/Sxvxgee/UnlimitedGPT',
+    'packages': packages,
+    'package_data': package_data,
+    'python_requires': '>=3.8.0',
+}
 
-An unofficial Python wrapper for OpenAI's ChatGPT API
 
-## Features
-
--   [x] Cloudflare's anti-bot protection bypass using `undetected_chromedriver`
--   [x] [Headless machines support](#how-do-i-get-it-to-work-on-headless-linux-server)
--   [x] [Google Colab support](#how-do-i-get-it-to-work-on-google-colab)
--   [x] Proxy support (only without basic auth)
-
-## Getting Started
-
-> This library is using only the `undetected_chromedriver` package to bypass Cloudflare's anti-bot protection. `requests` module is not used due to the complexity of the protection. **Please make sure you have [Google Chrome](https://www.google.com/chrome/) / [Chromium](https://www.chromium.org/) before using this wrapper.**
-
-### Installation
-
-```bash
-pip install -U UnlimitedGPT
-```
-
-### Usage
-
-#### Obtaining session_token
-
-1. Go to https://chat.openai.com/chat and open the developer tools by `F12`.
-2. Find the `__Secure-next-auth.session-token` cookie in `Application` > `Storage` > `Cookies` > `https://chat.openai.com`.
-3. Copy the value in the `Cookie Value` field.
-
-![image](https://user-images.githubusercontent.com/19218518/206170122-61fbe94f-4b0c-4782-a344-e26ac0d4e2a7.png)
-
-#### Interactive mode
-
-> Currently, interactive mode is not supported in this package. But it will be added in the future.
-
-#### Import as a module
-
-```python
-from UnlimitedGPT import ChatGPT
-
-session_token = 'abc123'  # `__Secure-next-auth.session-token` cookie from https://chat.openai.com/chat
-api = ChatGPT(session_token)  # auth with session token
-api = ChatGPT(session_token, conversation_id='some-random-uuid')  # specify conversation id
-api = ChatGPT(session_token, proxy='https://proxy.example.com:8080')  # specify proxy
-api = ChatGPT(session_token, chrome_args=['--window-size=1920,768'])  # specify chrome args
-api = ChatGPT(session_token, disable_moderation=True)  # disable moderation
-api = ChatGPT(session_token, verbose=True)  # verbose mode (print debug messages)
-
-message = api.send_message('Hello, world!')
-print(message.response, message.conversation_id)
-
-api.reset_conversation()  # reset the conversation
-```
-
-## Frequently Asked Questions
-
-### How do I get it to work on headless linux server?
-
-```bash
-# install chromium & X virtual framebuffer
-sudo apt install chromium-browser xvfb
-
-# start your script
-python3 your_script.py
-```
-
-### How do I get it to work on Google Colab?
-
-It is normal for the seession to be crashed when installing dependencies. Just ignore the error and run your script.
-
-```python
-# install dependencies
-!apt install chromium-browser xvfb
-!pip install -U selenium_profiles UnlimitedGPT
-
-# install chromedriver
-from selenium_profiles.utils.installer import install_chromedriver
-install_chromedriver()
-```
-
-```python
-# start your script as normal
-!python3 -m UnlimitedGPT
-```
-
-## Insipration
-
-This project is inspired by
-
--   [ChatGPT](https://github.com/acheong08/ChatGPT)
--   [chatgpt-api](https://github.com/transitive-bullshit/chatgpt-api)
--   [pyChatGPT](https://github.com/terry3041/pyChatGPT)
-
-## Disclaimer
-
-This project is not affiliated with OpenAI in any way. Use at your own risk. I am not responsible for any damage caused by this project. Please read the [OpenAI Terms of Service](https://beta.openai.com/terms) before using this project.
-
-## License
-
-This project is licensed under the GPLv3 License - see the [LICENSE](LICENSE) file for details.
+setup(**setup_kwargs)
```

