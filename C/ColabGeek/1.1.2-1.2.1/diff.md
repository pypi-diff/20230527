# Comparing `tmp/ColabGeek-1.1.2.tar.gz` & `tmp/ColabGeek-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ColabGeek-1.1.2.tar", last modified: Thu Apr 20 17:18:36 2023, max compression
+gzip compressed data, was "ColabGeek-1.2.1.tar", last modified: Sat May 27 12:39:37 2023, max compression
```

## Comparing `ColabGeek-1.1.2.tar` & `ColabGeek-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:36.209597 ColabGeek-1.1.2/
--rw-rw-r--   0 root         (0) root         (0)     1067 2023-04-20 16:19:47.000000 ColabGeek-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6380 2023-04-20 17:18:36.208597 ColabGeek-1.1.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5643 2023-04-20 17:14:39.000000 ColabGeek-1.1.2/README.md
--rw-rw-r--   0 root         (0) root         (0)      939 2023-04-20 17:14:39.000000 ColabGeek-1.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 17:18:36.209597 ColabGeek-1.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:36.206596 ColabGeek-1.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:36.207596 ColabGeek-1.1.2/src/ColabGeek/
--rw-rw-r--   0 root         (0) root         (0)     7849 2023-04-20 17:14:39.000000 ColabGeek-1.1.2/src/ColabGeek/ColabGeek.py
--rw-rw-r--   0 root         (0) root         (0)       24 2023-04-20 16:19:47.000000 ColabGeek-1.1.2/src/ColabGeek/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:36.208597 ColabGeek-1.1.2/src/ColabGeek/shell_scripts/
--rw-rw-r--   0 root         (0) root         (0)      382 2023-04-20 16:19:47.000000 ColabGeek-1.1.2/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
--rw-rw-r--   0 root         (0) root         (0)     1192 2023-04-20 16:19:47.000000 ColabGeek-1.1.2/src/ColabGeek/shell_scripts/Run_code_server.exp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:36.208597 ColabGeek-1.1.2/src/ColabGeek.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6380 2023-04-20 17:18:36.000000 ColabGeek-1.1.2/src/ColabGeek.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-04-20 17:18:36.000000 ColabGeek-1.1.2/src/ColabGeek.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 17:18:36.000000 ColabGeek-1.1.2/src/ColabGeek.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-20 17:18:36.000000 ColabGeek-1.1.2/src/ColabGeek.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 12:39:37.282796 ColabGeek-1.2.1/
+-rw-rw-r--   0 root         (0) root         (0)     1067 2023-05-27 12:10:14.000000 ColabGeek-1.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7171 2023-05-27 12:39:37.281796 ColabGeek-1.2.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6434 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/README.md
+-rw-rw-r--   0 root         (0) root         (0)      939 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 12:39:37.282796 ColabGeek-1.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 12:39:37.278796 ColabGeek-1.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 12:39:37.280796 ColabGeek-1.2.1/src/ColabGeek/
+-rw-rw-r--   0 root         (0) root         (0)    11496 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/src/ColabGeek/ColabGeek.py
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-05-27 12:10:14.000000 ColabGeek-1.2.1/src/ColabGeek/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 12:39:37.281796 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/
+-rw-rw-r--   0 root         (0) root         (0)      816 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Install_Homebrew.exp
+-rw-rw-r--   0 root         (0) root         (0)      324 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Install_Jekyll.exp
+-rw-rw-r--   0 root         (0) root         (0)      485 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Install_Ruby.exp
+-rw-rw-r--   0 root         (0) root         (0)      442 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Install_rbenv.exp
+-rw-rw-r--   0 root         (0) root         (0)      382 2023-05-27 12:10:14.000000 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
+-rw-rw-r--   0 root         (0) root         (0)     1192 2023-05-27 12:10:14.000000 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Run_code_server.exp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 12:39:37.280796 ColabGeek-1.2.1/src/ColabGeek.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7171 2023-05-27 12:39:37.000000 ColabGeek-1.2.1/src/ColabGeek.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      518 2023-05-27 12:39:37.000000 ColabGeek-1.2.1/src/ColabGeek.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 12:39:37.000000 ColabGeek-1.2.1/src/ColabGeek.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-27 12:39:37.000000 ColabGeek-1.2.1/src/ColabGeek.egg-info/top_level.txt
```

### Comparing `ColabGeek-1.1.2/LICENSE` & `ColabGeek-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.1.2/PKG-INFO` & `ColabGeek-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.1.2
+Version: 1.2.1
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -126,10 +126,22 @@
 # - port The server port of shadowsocks, set to None and you will use the default port.
 # - password The shadowsocks password.
 # - encrypt The shadowsocks encrypt method.
 
 main.Run_shadowsocks()
 ```
 
+### Jekyll
+
+[Jekyll](https://jekyllrb.com/) is a simple, blog-aware, static site generator that allows users to create their own websites or blogs without the need for databases or server-side programming languages. It takes text written in Markdown, processes it through a template engine, and generates a ready-to-publish static website. ColabGeek now provides a method to automatically install Jekyll and all of its dependencies. Users can easily access their Jekyll sites using tunneling methods, also provided by ColabGeek.
+
+```python
+# ColabGeek.Install_Jekyll has the following parameters:
+# - version Which version of Ruby you would like to install? The latest stable version is recommended.
+# - verbose Show the running logs.
+
+main.Install_Jekyll(version='3.2.2',verbose=True)
+```
+
 ## Statement
 
 ColabGeek violated numerous community rules of Google Colab. But still, I developed ColabGeek, because the simple Jupyter interface just does not meet the requirements of many software applications and is not user-friendly for coding in non-Python languages. I recommend all ColabGeek users purchase Colab Pro or Pro+ to support the excellent services provided by Google. Keep in mind, avoid misuse and Don't Be Evil.
```

### Comparing `ColabGeek-1.1.2/README.md` & `ColabGeek-1.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -112,10 +112,22 @@
 # - port The server port of shadowsocks, set to None and you will use the default port.
 # - password The shadowsocks password.
 # - encrypt The shadowsocks encrypt method.
 
 main.Run_shadowsocks()
 ```
 
+### Jekyll
+
+[Jekyll](https://jekyllrb.com/) is a simple, blog-aware, static site generator that allows users to create their own websites or blogs without the need for databases or server-side programming languages. It takes text written in Markdown, processes it through a template engine, and generates a ready-to-publish static website. ColabGeek now provides a method to automatically install Jekyll and all of its dependencies. Users can easily access their Jekyll sites using tunneling methods, also provided by ColabGeek.
+
+```python
+# ColabGeek.Install_Jekyll has the following parameters:
+# - version Which version of Ruby you would like to install? The latest stable version is recommended.
+# - verbose Show the running logs.
+
+main.Install_Jekyll(version='3.2.2',verbose=True)
+```
+
 ## Statement
 
 ColabGeek violated numerous community rules of Google Colab. But still, I developed ColabGeek, because the simple Jupyter interface just does not meet the requirements of many software applications and is not user-friendly for coding in non-Python languages. I recommend all ColabGeek users purchase Colab Pro or Pro+ to support the excellent services provided by Google. Keep in mind, avoid misuse and Don't Be Evil.
```

### Comparing `ColabGeek-1.1.2/pyproject.toml` & `ColabGeek-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 "ColabGeek.shell_scripts" = ["*"]
 
 [project]
 name = "ColabGeek"
-version = "1.1.2"
+version = "1.2.1"
 authors = [
     {name = "Yiming Sun",email = "yiming.sun12138@gmail.com"},
 ]
 description = "ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ColabGeek-1.1.2/src/ColabGeek/ColabGeek.py` & `ColabGeek-1.2.1/src/ColabGeek/ColabGeek.py`

 * *Files 20% similar despite different names*

```diff
@@ -127,21 +127,23 @@
         # get shell script path
         script_path = os.path.dirname(__file__)
         script_path = os.path.join(script_path,'shell_scripts','Run_Rstudio_server.sh')
 
         # run Rstudio server
         char_cmd = "bash" + " " + str(script_path) + " " + str(self.path) + " " + str(port)
         exec_logging = os.popen(char_cmd)
+        exec_logging = ''.join(exec_logging.readlines())
         if verbose:
-            exec_logging = ''.join(exec_logging.readlines())
             print(exec_logging)
 
     # run code server
     def Run_code_server(self,port = None,password = None,verbose = True):
         # check param
+        if (str(self.user) == 'root'):
+            raise RootUserError()
         if (port is None):
             port = self.port
         if (password is None):
             password = self.password
 
         # install expect
         os.system("apt install expect -y")
@@ -149,23 +151,23 @@
         # get shell script path
         script_path = os.path.dirname(__file__)
         script_path = os.path.join(script_path,'shell_scripts','Run_code_server.exp')
 
         # run code server
         char_cmd = "expect" + " " + str(script_path) + " " + str(self.user) + " " + str(self.password) + " " + str(port) + " " + str(password) + " " + str(self.path)
         exec_logging = os.popen(char_cmd)
+        exec_logging = ''.join(exec_logging.readlines())
         if verbose:
-            exec_logging = ''.join(exec_logging.readlines())
             print(exec_logging)
 
     def Install_code_server_extension(self,extension,verbose = True):
         char_cmd = "sudo -u" + " " + str(self.user) + " " + "code-server --install-extension" + " " + str(extension)
         exec_logging = os.popen(char_cmd)
+        exec_logging = ''.join(exec_logging.readlines())
         if verbose:
-            exec_logging = ''.join(exec_logging.readlines())
             print(exec_logging)
 
     def Config_code_server(self,property,value):
         # check whether settings.json exists
         file_path = "/home/" + str(self.user) + "/.local/share/code-server/User"
         char_cmd = "sudo -u" + " " + str(self.user) + " " + "mkdir -p" + " " + file_path
         os.system(char_cmd)
@@ -201,14 +203,108 @@
 
         # run shadowsocks
         char_cmd = "ss-server" + " " + "-s 0.0.0.0" + " " + "-p" + " " + str(port) + " " + "-k" + " " + str(password) + " " + "-m" + " " + str(encrypt)
         char_cmd = "nohup" + " " + char_cmd + " " + ">" + " " + "/tmp/" + str(self.path) + "/shadowsocks.log 2>&1 &"
         os.system(char_cmd)
 
     '''
+    Jekyll method
+    '''
+    # install Homebrew
+    def Install_Homebrew(self,verbose = True):
+        # check param
+        if (str(self.user) == 'root'):
+            raise RootUserError()
+
+        # install expect
+        os.system("apt install expect -y")
+
+        # get shell script path
+        script_path = os.path.dirname(__file__)
+        script_path = os.path.join(script_path,'shell_scripts','Install_Homebrew.exp')
+
+        # run expect script
+        char_cmd = "expect" + " " + str(script_path) + " " + str(self.user) + " " + str(self.password) + " " + str(self.path)
+        exec_logging = os.popen(char_cmd)
+        exec_logging = ''.join(exec_logging.readlines())
+        if verbose:
+            print(exec_logging)
+
+    # install rbenv
+    def Install_rbenv(self,verbose = True):
+        # check param
+        if (str(self.user) == 'root'):
+            raise RootUserError()
+
+        # install expect
+        os.system("apt install expect -y")
+
+        # get shell script path
+        script_path = os.path.dirname(__file__)
+        script_path = os.path.join(script_path,'shell_scripts','Install_rbenv.exp')
+
+        # run expect script
+        char_cmd = "expect" + " " + str(script_path) + " " + str(self.user) + " " + str(self.password) + " " + str(self.path)
+        exec_logging = os.popen(char_cmd)
+        exec_logging = ''.join(exec_logging.readlines())
+        if verbose:
+            print(exec_logging)
+
+    # install Ruby
+    def Install_Ruby(self,version = None,verbose = True):
+        # check param
+        if (str(self.user) == 'root'):
+            raise RootUserError()
+        if (version is None):
+            version = input("Input the Ruby version to install: ")
+
+        # install expect
+        os.system("apt install expect -y")
+
+        # get shell script path
+        script_path = os.path.dirname(__file__)
+        script_path = os.path.join(script_path,'shell_scripts','Install_Ruby.exp')
+
+        # run expect script
+        char_cmd = "expect" + " " + str(script_path) + " " + str(self.user) + " " + str(self.password) + " " + str(version) + " " + str(self.path)
+        exec_logging = os.popen(char_cmd)
+        exec_logging = ''.join(exec_logging.readlines())
+        if verbose:
+            print(exec_logging)
+
+    # install Jekyll
+    def Install_Jekyll(self,version = None,verbose = True):
+        # check param
+        if (str(self.user) == 'root'):
+            raise RootUserError()
+            
+        # install dependency
+        if verbose:
+            print("Install Homebrew: \n")
+        self.Install_Homebrew(verbose = verbose)
+        if verbose:
+            print("Install rbenv: \n")
+        self.Install_rbenv(verbose = verbose)
+        if verbose:
+            print("Install Ruby: \n")
+        self.Install_Ruby(version = version,verbose = verbose)
+
+        # get shell script path
+        script_path = os.path.dirname(__file__)
+        script_path = os.path.join(script_path,'shell_scripts','Install_Jekyll.exp')
+
+        # run expect script
+        char_cmd = "expect" + " " + str(script_path) + " " + str(self.user) + " " + str(self.password) + " " + str(self.path)
+        exec_logging = os.popen(char_cmd)
+        exec_logging = ''.join(exec_logging.readlines())
+        if verbose:
+            print("Install Jekyll: \n")
+            print(exec_logging)
+            
+    '''
     other method
     '''
     # keep Colab session busy
     def busy_session(self,busy = None):
         # check param
         if (busy is None):
             busy = self.keep_busy
@@ -224,8 +320,18 @@
 '''
 define other method
 '''
 # update environment
 def update_environment():
     os.system("apt update")
     os.system("apt upgrade -y")
-    os.system("apt autoremove -y")
+    os.system("apt autoremove -y")
+
+'''
+define Exception class
+'''
+# RootUserError
+class RootUserError(Exception):
+    """Exception raised when the user is root."""
+
+    def __init__(self,message = 'Cannot proceed under user root!'):
+        super().__init__(message)
```

### Comparing `ColabGeek-1.1.2/src/ColabGeek/shell_scripts/Run_code_server.exp` & `ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Run_code_server.exp`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.1.2/src/ColabGeek.egg-info/PKG-INFO` & `ColabGeek-1.2.1/src/ColabGeek.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.1.2
+Version: 1.2.1
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -126,10 +126,22 @@
 # - port The server port of shadowsocks, set to None and you will use the default port.
 # - password The shadowsocks password.
 # - encrypt The shadowsocks encrypt method.
 
 main.Run_shadowsocks()
 ```
 
+### Jekyll
+
+[Jekyll](https://jekyllrb.com/) is a simple, blog-aware, static site generator that allows users to create their own websites or blogs without the need for databases or server-side programming languages. It takes text written in Markdown, processes it through a template engine, and generates a ready-to-publish static website. ColabGeek now provides a method to automatically install Jekyll and all of its dependencies. Users can easily access their Jekyll sites using tunneling methods, also provided by ColabGeek.
+
+```python
+# ColabGeek.Install_Jekyll has the following parameters:
+# - version Which version of Ruby you would like to install? The latest stable version is recommended.
+# - verbose Show the running logs.
+
+main.Install_Jekyll(version='3.2.2',verbose=True)
+```
+
 ## Statement
 
 ColabGeek violated numerous community rules of Google Colab. But still, I developed ColabGeek, because the simple Jupyter interface just does not meet the requirements of many software applications and is not user-friendly for coding in non-Python languages. I recommend all ColabGeek users purchase Colab Pro or Pro+ to support the excellent services provided by Google. Keep in mind, avoid misuse and Don't Be Evil.
```

