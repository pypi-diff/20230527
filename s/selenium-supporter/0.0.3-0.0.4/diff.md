# Comparing `tmp/selenium-supporter-0.0.3.tar.gz` & `tmp/selenium-supporter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-supporter-0.0.3.tar", last modified: Thu Mar 30 00:49:43 2023, max compression
+gzip compressed data, was "selenium-supporter-0.0.4.tar", last modified: Sat May 27 16:56:31 2023, max compression
```

## Comparing `selenium-supporter-0.0.3.tar` & `selenium-supporter-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 00:49:43.922892 selenium-supporter-0.0.3/
--rw-r--r--   0 root         (0) root         (0)     1885 2023-03-30 00:49:43.921892 selenium-supporter-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1603 2023-03-30 00:49:42.000000 selenium-supporter-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 00:49:43.920892 selenium-supporter-0.0.3/selenium_supporter/
--rw-r--r--   0 root         (0) root         (0)       44 2023-03-30 00:49:42.000000 selenium-supporter-0.0.3/selenium_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9181 2023-03-30 00:49:42.000000 selenium-supporter-0.0.3/selenium_supporter/drivers.py
--rw-r--r--   0 root         (0) root         (0)     8913 2023-03-30 00:49:42.000000 selenium-supporter-0.0.3/selenium_supporter/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 00:49:43.921892 selenium-supporter-0.0.3/selenium_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1885 2023-03-30 00:49:43.000000 selenium-supporter-0.0.3/selenium_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2023-03-30 00:49:43.000000 selenium-supporter-0.0.3/selenium_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 00:49:43.000000 selenium-supporter-0.0.3/selenium_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 00:49:43.000000 selenium-supporter-0.0.3/selenium_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       68 2023-03-30 00:49:43.000000 selenium-supporter-0.0.3/selenium_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-30 00:49:43.000000 selenium-supporter-0.0.3/selenium_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 00:49:43.922892 selenium-supporter-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      606 2023-03-30 00:49:42.000000 selenium-supporter-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 16:56:31.086913 selenium-supporter-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-05-27 16:56:31.085913 selenium-supporter-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 16:56:31.084913 selenium-supporter-0.0.4/selenium_supporter/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9181 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter/drivers.py
+-rw-r--r--   0 root         (0) root         (0)     8913 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 16:56:31.085913 selenium-supporter-0.0.4/selenium_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      357 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 16:56:31.086913 selenium-supporter-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      606 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/setup.py
```

### Comparing `selenium-supporter-0.0.3/PKG-INFO` & `selenium-supporter-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: selenium-supporter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Selenium supporter
 Home-page: https://github.com/automatethem/selenium-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # selenium-supporter
 
 https://pypi.org/project/selenium-supporter
 <pre>
 pip install selenium-supporter
@@ -21,14 +20,15 @@
 import selenium_supporter
 
 selenium_supporter.drivers.ChromeDriver()
 selenium_supporter.drivers.ChromeDebuggingDriver()
 
 selenium_supporter.utils.get_chrome_web_browser_path()
 selenium_supporter.utils.kill_all_chrome_web_browser_processes()
+selenium_supporter.utils.kill_all_chrome_web_browser_driver_processes()
 selenium_supporter.utils.open_chrome_web_browser(user_data_dir=None, proxy_server=None)
 selenium_supporter.utils.open_chrome_web_browser_with_remote_debugging_mode(remote_debugging_port, remote_debugging_address, user_data_dir=None, proxy_server=None, headless=False)
 selenium_supporter.utils.check_port_open(ip, port)
 selenium_supporter.utils.save_partial_screenshot(element, image_file)
 selenium_supporter.utils.save_full_screenshot(driver, image_file)     
 selenium_supporter.utils.save_full_screenshot_with_scroll(driver, image_file)
 selenium_supporter.utils.save_partial_screenshot_with_scroll(driver, partial_element, image_file)
```

### Comparing `selenium-supporter-0.0.3/README.md` & `selenium-supporter-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import selenium_supporter
 
 selenium_supporter.drivers.ChromeDriver()
 selenium_supporter.drivers.ChromeDebuggingDriver()
 
 selenium_supporter.utils.get_chrome_web_browser_path()
 selenium_supporter.utils.kill_all_chrome_web_browser_processes()
+selenium_supporter.utils.kill_all_chrome_web_browser_driver_processes()
 selenium_supporter.utils.open_chrome_web_browser(user_data_dir=None, proxy_server=None)
 selenium_supporter.utils.open_chrome_web_browser_with_remote_debugging_mode(remote_debugging_port, remote_debugging_address, user_data_dir=None, proxy_server=None, headless=False)
 selenium_supporter.utils.check_port_open(ip, port)
 selenium_supporter.utils.save_partial_screenshot(element, image_file)
 selenium_supporter.utils.save_full_screenshot(driver, image_file)     
 selenium_supporter.utils.save_full_screenshot_with_scroll(driver, image_file)
 selenium_supporter.utils.save_partial_screenshot_with_scroll(driver, partial_element, image_file)
```

### Comparing `selenium-supporter-0.0.3/selenium_supporter/drivers.py` & `selenium-supporter-0.0.4/selenium_supporter/drivers.py`

 * *Files identical despite different names*

### Comparing `selenium-supporter-0.0.3/selenium_supporter/utils.py` & `selenium-supporter-0.0.4/selenium_supporter/utils.py`

 * *Files identical despite different names*

### Comparing `selenium-supporter-0.0.3/selenium_supporter.egg-info/PKG-INFO` & `selenium-supporter-0.0.4/selenium_supporter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: selenium-supporter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Selenium supporter
 Home-page: https://github.com/automatethem/selenium-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # selenium-supporter
 
 https://pypi.org/project/selenium-supporter
 <pre>
 pip install selenium-supporter
@@ -21,14 +20,15 @@
 import selenium_supporter
 
 selenium_supporter.drivers.ChromeDriver()
 selenium_supporter.drivers.ChromeDebuggingDriver()
 
 selenium_supporter.utils.get_chrome_web_browser_path()
 selenium_supporter.utils.kill_all_chrome_web_browser_processes()
+selenium_supporter.utils.kill_all_chrome_web_browser_driver_processes()
 selenium_supporter.utils.open_chrome_web_browser(user_data_dir=None, proxy_server=None)
 selenium_supporter.utils.open_chrome_web_browser_with_remote_debugging_mode(remote_debugging_port, remote_debugging_address, user_data_dir=None, proxy_server=None, headless=False)
 selenium_supporter.utils.check_port_open(ip, port)
 selenium_supporter.utils.save_partial_screenshot(element, image_file)
 selenium_supporter.utils.save_full_screenshot(driver, image_file)     
 selenium_supporter.utils.save_full_screenshot_with_scroll(driver, image_file)
 selenium_supporter.utils.save_partial_screenshot_with_scroll(driver, partial_element, image_file)
```

### Comparing `selenium-supporter-0.0.3/setup.py` & `selenium-supporter-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='selenium-supporter',
-	version='0.0.3',
+	version='0.0.4',
 	description='Selenium supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/selenium-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

