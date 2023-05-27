# Comparing `tmp/xpanther-1.1.1.tar.gz` & `tmp/xpanther-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpanther-1.1.1.tar", last modified: Thu May 25 14:47:49 2023, max compression
+gzip compressed data, was "xpanther-1.1.2.tar", last modified: Sat May 27 17:58:31 2023, max compression
```

## Comparing `xpanther-1.1.1.tar` & `xpanther-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 14:47:49.173689 xpanther-1.1.1/
--rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     5539 2023-05-25 14:47:49.173689 xpanther-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5071 2023-05-20 14:06:27.000000 xpanther-1.1.1/README.md
--rw-rw-rw-   0        0        0      650 2023-05-25 14:47:11.000000 xpanther-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 14:47:49.173689 xpanther-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 14:47:49.123041 xpanther-1.1.1/xpanther/
--rw-rw-rw-   0        0        0       79 2023-05-07 13:19:03.000000 xpanther-1.1.1/xpanther/__init__.py
--rw-rw-rw-   0        0        0    20899 2023-05-25 12:52:00.000000 xpanther-1.1.1/xpanther/main.py
--rw-rw-rw-   0        0        0     5109 2023-05-25 14:46:29.000000 xpanther-1.1.1/xpanther/main_ide.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:47:49.172671 xpanther-1.1.1/xpanther.egg-info/
--rw-rw-rw-   0        0        0     5539 2023-05-25 14:47:49.000000 xpanther-1.1.1/xpanther.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-05-25 14:47:49.000000 xpanther-1.1.1/xpanther.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 14:47:49.000000 xpanther-1.1.1/xpanther.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-25 14:47:49.000000 xpanther-1.1.1/xpanther.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 14:47:49.000000 xpanther-1.1.1/xpanther.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 17:58:31.834891 xpanther-1.1.2/
+-rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5684 2023-05-27 17:58:31.834891 xpanther-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5216 2023-05-27 17:57:46.000000 xpanther-1.1.2/README.md
+-rw-rw-rw-   0        0        0      650 2023-05-27 17:57:46.000000 xpanther-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 17:58:31.836792 xpanther-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 17:58:31.794644 xpanther-1.1.2/xpanther/
+-rw-rw-rw-   0        0        0       79 2023-05-07 13:19:03.000000 xpanther-1.1.2/xpanther/__init__.py
+-rw-rw-rw-   0        0        0    20899 2023-05-25 12:52:00.000000 xpanther-1.1.2/xpanther/main.py
+-rw-rw-rw-   0        0        0     5241 2023-05-27 17:57:46.000000 xpanther-1.1.2/xpanther/main_ide.py
+drwxrwxrwx   0        0        0        0 2023-05-27 17:58:31.826824 xpanther-1.1.2/xpanther.egg-info/
+-rw-rw-rw-   0        0        0     5684 2023-05-27 17:58:31.000000 xpanther-1.1.2/xpanther.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-27 17:58:31.000000 xpanther-1.1.2/xpanther.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 17:58:31.000000 xpanther-1.1.2/xpanther.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-27 17:58:31.000000 xpanther-1.1.2/xpanther.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 17:58:31.000000 xpanther-1.1.2/xpanther.egg-info/top_level.txt
```

### Comparing `xpanther-1.1.1/LICENSE` & `xpanther-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xpanther-1.1.1/PKG-INFO` & `xpanther-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanther
-Version: 1.1.1
+Version: 1.1.2
 Summary: Find Unique Xpath of any HTML/XML element
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/XPanther
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -100,14 +100,16 @@
 Use:
 ```python
 XPantherIDE('page_url').start()
 ```   
     
 #### After you run the program, the browser will open, and you can start finding xpaths by `right-clicking` over elements. A pop up alert will appear showing the xpath, you must accept/close the pop up before trying again. You can then just close the browser and the program terminates.
 
+#### The program will test each xpath if it works, it is corresponding to clicked element, and output it in the console along with its speed.
+
 ### **Both programs are open to improvements or new ideas!**
```

### Comparing `xpanther-1.1.1/README.md` & `xpanther-1.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,16 @@
 Use:
 ```python
 XPantherIDE('page_url').start()
 ```   
     
 #### After you run the program, the browser will open, and you can start finding xpaths by `right-clicking` over elements. A pop up alert will appear showing the xpath, you must accept/close the pop up before trying again. You can then just close the browser and the program terminates.
 
+#### The program will test each xpath if it works, it is corresponding to clicked element, and output it in the console along with its speed.
+
 ### **Both programs are open to improvements or new ideas!**
```

### Comparing `xpanther-1.1.1/pyproject.toml` & `xpanther-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xpanther"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
 description = "Find Unique Xpath of any HTML/XML element"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `xpanther-1.1.1/xpanther/main.py` & `xpanther-1.1.2/xpanther/main.py`

 * *Files identical despite different names*

### Comparing `xpanther-1.1.1/xpanther/main_ide.py` & `xpanther-1.1.2/xpanther/main_ide.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as ec
 from selenium import webdriver
 from xpanther import XPanther
 
 
 class XPantherIDE:
-    def __init__(self, page_url, turbo=True):
+    def __init__(self, page_url, advanced=True):
         self.__driver = webdriver.Chrome()
         self.__page_url = page_url
 
-        self.turbo = turbo
+        self.advanced = advanced
 
     def wait_for_alert(self):
         for _ in range(100):
             try:
                 WebDriverWait(self.__driver, 1).until(ec.alert_is_present())
                 sleep(1)
             except TimeoutException or NoAlertPresentException:
@@ -28,36 +28,37 @@
             self.__driver.switch_to.alert.accept()
         except NoAlertPresentException:
             return None
 
     def find_and_alert_xpath(self, return_value):
         self.__driver.execute_script("alert('Capturing...')")
         xpath_s = XPanther(
-            return_value[1], print_output=False, speed='fast', show_all=self.turbo
+            return_value[1], print_output=False, speed='fast', show_all=self.advanced
         ).capture(return_value[0])[0]
         index = 0
         elapsed_time = 0
         if not xpath_s:
             result = 'Could not find XPATH...'
             self.accept_alert()
         else:
-            if not self.turbo:
+            if not self.advanced:
                 xpath_s = [xpath_s]
             result = 'No XPATH found worked with selenium...'
             self.accept_alert()
             for xpath in xpath_s:
                 try:
                     start_time = time()
-                    WebDriverWait(self.__driver, 0.2).until(ec.presence_of_element_located((By.XPATH, xpath)))
+                    element = WebDriverWait(self.__driver, 0.2).until(ec.presence_of_element_located((By.XPATH, xpath)))
                     elapsed_time = (time() - start_time) * 1000
                 except TimeoutException:
                     index += 1
                 else:
-                    result = xpath
-                    break
+                    if element == return_value[2]:
+                        result = xpath
+                        break
         self.__driver.execute_script(f"alert('{result}')")
         return xpath_s, elapsed_time, index
 
     def start(self):
         program_return = []
         self.__driver.get(self.__page_url)
         print("\033[95m---XPantherIDE Started---\033[0m")
@@ -68,14 +69,15 @@
             e.preventDefault();
             array_events[0] = e.target.outerHTML
             window.array_events = array_events
             }
         var registerUrl = (e) => {
             e.preventDefault();
             array_events[1] = document.documentElement.outerHTML
+            array_events[2] = e.target
             }
 
         getElementHtml = document.addEventListener("contextmenu", registerOuterHtml, true)
         getDOMHtml = document.addEventListener("contextmenu", registerUrl, true)
 
         """
         return_js = """
@@ -98,15 +100,15 @@
                     return_value = WebDriverWait(self.__driver, 1).until(
                         lambda driver: self.__driver.execute_script(return_js)
                     )
                     if return_value:
                         xpath, time_, nr = self.find_and_alert_xpath(return_value)
                         index += 1
                         if xpath:
-                            print(f"\033[97m\n#{index} SELECTION -> \033[0m\033[92mWORKING XPATH:\033[0m")
+                            print(f"\033[97m\n#{index} SELECTION -> \033[0m\033[92mTESTED WORKING XPATH:\033[0m")
                             if time_:
                                 print(f'\033[96m                 SPEED =< {time_} ms\033[0m')
                                 print(f'----------------{xpath[nr]}')
                             else:
                                 print(f'----------------None')
                             if len(xpath) > 1 or not time_:
                                 print('\033[91m                NOT TESTED/WORKING:\033[0m')
```

### Comparing `xpanther-1.1.1/xpanther.egg-info/PKG-INFO` & `xpanther-1.1.2/xpanther.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanther
-Version: 1.1.1
+Version: 1.1.2
 Summary: Find Unique Xpath of any HTML/XML element
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/XPanther
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -100,14 +100,16 @@
 Use:
 ```python
 XPantherIDE('page_url').start()
 ```   
     
 #### After you run the program, the browser will open, and you can start finding xpaths by `right-clicking` over elements. A pop up alert will appear showing the xpath, you must accept/close the pop up before trying again. You can then just close the browser and the program terminates.
 
+#### The program will test each xpath if it works, it is corresponding to clicked element, and output it in the console along with its speed.
+
 ### **Both programs are open to improvements or new ideas!**
```

