# Comparing `tmp/bs4_web_scraper-0.0.2a0.tar.gz` & `tmp/bs4_web_scraper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs4_web_scraper-0.0.2a0.tar", last modified: Sat May 27 13:17:27 2023, max compression
+gzip compressed data, was "bs4_web_scraper-0.1.1.tar", last modified: Sat May 27 19:21:37 2023, max compression
```

## Comparing `bs4_web_scraper-0.0.2a0.tar` & `bs4_web_scraper-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 13:17:27.724143 bs4_web_scraper-0.0.2a0/
--rw-rw-rw-   0        0        0     1104 2023-03-07 14:14:59.000000 bs4_web_scraper-0.0.2a0/LICENSE.md
--rw-rw-rw-   0        0        0    19317 2023-05-27 13:17:27.721146 bs4_web_scraper-0.0.2a0/PKG-INFO
--rw-rw-rw-   0        0        0    17975 2023-05-27 12:26:05.000000 bs4_web_scraper-0.0.2a0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 13:17:27.461665 bs4_web_scraper-0.0.2a0/bs4_web_scraper/
--rw-rw-rw-   0        0        0     3623 2023-05-27 13:15:42.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/__init__.py
--rw-rw-rw-   0        0        0    41404 2023-05-27 13:07:58.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/base.py
--rw-rw-rw-   0        0        0     2102 2023-03-29 00:08:41.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/exceptions.py
--rw-rw-rw-   0        0        0    12777 2023-05-23 09:26:13.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/file_handler.py
--rw-rw-rw-   0        0        0     5642 2023-05-27 10:03:10.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/logging.py
--rw-rw-rw-   0        0        0     4858 2023-03-29 00:08:41.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/request_limiter.py
--rw-rw-rw-   0        0        0    35513 2023-05-27 13:08:15.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/scraper.py
--rw-rw-rw-   0        0        0    22737 2023-05-27 12:41:04.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/translate.py
--rw-rw-rw-   0        0        0     3906 2023-03-29 00:08:41.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:17:27.712146 bs4_web_scraper-0.0.2a0/bs4_web_scraper.egg-info/
--rw-rw-rw-   0        0        0    19317 2023-05-27 13:17:27.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-05-27 13:17:27.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 13:17:27.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2023-05-27 13:17:27.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-27 13:17:27.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1732 2023-05-27 13:15:22.000000 bs4_web_scraper-0.0.2a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 13:17:27.725142 bs4_web_scraper-0.0.2a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 19:21:37.715564 bs4_web_scraper-0.1.1/
+-rw-rw-rw-   0        0        0     1104 2023-03-07 14:14:59.000000 bs4_web_scraper-0.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0    19379 2023-05-27 19:21:37.712561 bs4_web_scraper-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    18039 2023-05-27 19:11:56.000000 bs4_web_scraper-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 19:21:37.532407 bs4_web_scraper-0.1.1/bs4_web_scraper/
+-rw-rw-rw-   0        0        0     3635 2023-05-27 19:20:08.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/__init__.py
+-rw-rw-rw-   0        0        0    41404 2023-05-27 13:07:58.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/base.py
+-rw-rw-rw-   0        0        0     2102 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/exceptions.py
+-rw-rw-rw-   0        0        0    12777 2023-05-23 09:26:13.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/file_handler.py
+-rw-rw-rw-   0        0        0     5642 2023-05-27 10:03:10.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/logging.py
+-rw-rw-rw-   0        0        0     4858 2023-05-27 19:09:12.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/request_limiter.py
+-rw-rw-rw-   0        0        0    39119 2023-05-27 19:20:26.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/scraper.py
+-rw-rw-rw-   0        0        0    22737 2023-05-27 12:41:04.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/translate.py
+-rw-rw-rw-   0        0        0     3906 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-27 19:21:37.704508 bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/
+-rw-rw-rw-   0        0        0    19379 2023-05-27 19:21:37.000000 bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2023-05-27 19:21:37.000000 bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 19:21:37.000000 bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2023-05-27 19:21:37.000000 bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-27 19:21:37.000000 bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1731 2023-05-27 19:19:47.000000 bs4_web_scraper-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 19:21:37.715564 bs4_web_scraper-0.1.1/setup.cfg
```

### Comparing `bs4_web_scraper-0.0.2a0/LICENSE.md` & `bs4_web_scraper-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.0.2a0/PKG-INFO` & `bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bs4_web_scraper
-Version: 0.0.2a0
+Name: bs4-web-scraper
+Version: 0.1.1
 Summary: A web scraper based on the BeautifulSoup4 library and translators package.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/bs4_web_scraper
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/bs4_web_scraper/issues
 Project-URL: Repository, https://github.com/ti-oluwa/bs4_web_scraper
 Keywords: web scraper,bs4,beautifulsoup4,web scraping,web scraping with python,web scraping with bs4,web scraping with beautifulsoup4,web scraping with translation,web scraping with translation to other languages,web scraping with translation to other languages with python,web scraping with translation to other languages with bs4,web scraping with translation to other languages with beautifulsoup4,web scraping with translation to other languages with python and bs4,web scraping with translation to other languages with python and beautifulsoup4
@@ -222,14 +222,17 @@
 
 The following are some useful methods for scraping web data using the scraper class.
 
 - `download_url`
 - `download_urls`
 - `find_urls`
 - `find_all_tags`
+- `find_tags_by_id`
+- `find_tags_by_class`
+- `find_comments`
 - `find_links`
 - `find_stylesheets`
 - `find_scripts`
 - `find_videos`
 - `find_images`
 - `find_audios`
 - `find_fonts`
```

### Comparing `bs4_web_scraper-0.0.2a0/README.md` & `bs4_web_scraper-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,17 @@
 
 The following are some useful methods for scraping web data using the scraper class.
 
 - `download_url`
 - `download_urls`
 - `find_urls`
 - `find_all_tags`
+- `find_tags_by_id`
+- `find_tags_by_class`
+- `find_comments`
 - `find_links`
 - `find_stylesheets`
 - `find_scripts`
 - `find_videos`
 - `find_images`
 - `find_audios`
 - `find_fonts`
```

### Comparing `bs4_web_scraper-0.0.2a0/bs4_web_scraper/__init__.py` & `bs4_web_scraper-0.1.1/bs4_web_scraper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = '0.0.2'
-__date__ = ''
+__version__ = '0.1.1'
+__date__ = '27-05-2023'
 __author__ = 'ti-oluwa'
-__doc__ = 'A web scraper that uses BeautifulSoup4 to scrape web pages and can translate them to other languages.'
+__doc__ = 'A web scraper that uses BeautifulSoup4 to scrape web pages and can translate them to__ other languages.'
 __license__ = 'MIT'
 __title__ = 'bs4_web_scraper'
 __url__ = 'https://github.com/ti-oluwa/bs4_web_scraper'
 __description__ = 'A web scraper that uses BeautifulSoup4 to scrape web pages and can translates them to other languages.'
 __keywords__ = 'web scraper, bs4, beautifulsoup4, web scraping, web scraping with python, web scraping with bs4, web scraping with beautifulsoup4, web scraping with translation, web scraping with translation to other languages, web scraping with translation to other languages with python, web scraping with translation to other languages with bs4, web scraping with translation to other languages with beautifulsoup4, web scraping with translation to other languages with python and bs4, web scraping with translation to other languages with python and beautifulsoup4,'
 __maintainer__ = 'ti-oluwa'
 __maintainer_email__ = 'tioluwa.dev@gmail.com'
```

### Comparing `bs4_web_scraper-0.0.2a0/bs4_web_scraper/base.py` & `bs4_web_scraper-0.1.1/bs4_web_scraper/base.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.0.2a0/bs4_web_scraper/exceptions.py` & `bs4_web_scraper-0.1.1/bs4_web_scraper/exceptions.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.0.2a0/bs4_web_scraper/file_handler.py` & `bs4_web_scraper-0.1.1/bs4_web_scraper/file_handler.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.0.2a0/bs4_web_scraper/logging.py` & `bs4_web_scraper-0.1.1/bs4_web_scraper/logging.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.0.2a0/bs4_web_scraper/request_limiter.py` & `bs4_web_scraper-0.1.1/bs4_web_scraper/request_limiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,14 @@
         return self.no_of_available_retries > 0
 
 
     def pause(self) -> None:
         '''Disallows request making for the specified pause duration.'''
         self.requests_paused = True
         self._log("REQUESTS PAUSED \n")
-        self._log('------------------- \n')
+        self._log('=================== \n')
         self._log("WAITING... \n")
-        self._log('------------------- \n')
+        self._log('=================== \n')
         time.sleep(self.pause_duration)
         self.requests_paused = False
         self._log("REQUESTS RESTARTED \n")
```

### Comparing `bs4_web_scraper-0.0.2a0/bs4_web_scraper/scraper.py` & `bs4_web_scraper-0.1.1/bs4_web_scraper/scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     websites you are scraping by making a donation.
 """
 import os
 import re
 from typing import (AnyStr, Dict, List, Tuple)
 from collections.abc import Iterable
 import time
+from bs4 import Comment
 from concurrent.futures import ThreadPoolExecutor
 from urllib3.util.url import parse_url
 
 from . import utils
 from .base import BS4BaseScraper
 from .file_handler import FileHandler
 
@@ -338,26 +339,26 @@
                         depth: int = 0, count: int = None, recursive: bool = True):
         """
         Gets all markup elements with the target name in specified url.
 
         Returns a list of the markup elements with the target name as bs4.element.Tag objects.
 
         Args::
-            * url (str): url of page to be parsed and scanned for target element.
+            * url (str): url of page to be parsed and scanned for target elements.
             * target (str): name of markup element (with a url related attribute).
             * attrs (Dict[str, str] | Iterable[Dict[str, str]]): A dictionary or list of dictionaries of filters on attribute values.
             * depth (int): Number of levels to recursively search for target items. Defaults to 0.
             * count (int): Number of target items to be found on a url page before stopping.
             * recursive (bool): Performs a recursive search of url page's children
         """
         self.set_base_url(url)
         base_url_obj = parse_url(self.base_url)
         soup = self.make_soup_from_url(url)
+        tags = []
         if soup is not None:
-            tags = []
             if isinstance(attrs, Iterable) and not isinstance(attrs, dict):
                 for attr in attrs:
                     tags.extend(soup.find_all(target, attr, recursive=recursive, limit=count))
             else:
                 tags.extend(soup.find_all(target, attrs, recursive=recursive, limit=count))
 
             while depth > 0:
@@ -365,21 +366,89 @@
                 link_tags = soup.find_all('a', recursive=recursive)
                 links = [ self.get_link_tag(link_tag, download=False) for link_tag in link_tags ]
                 links = filter(lambda link: bool(link), links)   
                 link_objs = [ (link, parse_url(link)) for link in links ]
                 links = [ link_obj[0] for link_obj in link_objs if (base_url_obj.netloc and link_obj[1].netloc) and (base_url_obj.netloc in link_obj[1].netloc) ] 
 
                 with ThreadPoolExecutor() as executor:
-                    results = executor.map(lambda args: self.find_urls_tags(*args), map(lambda link: (link, target, attrs, depth, count, recursive), links))
+                    results = executor.map(lambda args: self.find_all_tags(*args), map(lambda link: (link, target, attrs, depth, count, recursive), links))
                     for result in results:
                         if result:
                             tags.extend(result)
                 continue
         return tags
 
+
+    def find_tags_by_id(self, url: str, id: str, depth: int = 0, count: int = None, recursive: bool = True):
+        """
+        Gets all markup elements with the target id in specified url.
+
+        Returns a list of the markup elements with the target id as bs4.element.Tag objects.
+
+        Args::
+            * url (str): url of page to be parsed and scanned for target elements.
+            * id (str): id of markup element(s).
+            * depth (int): Number of levels to recursively search for target items. Defaults to 0.
+            * count (int): Number of target items to be found on a url page before stopping.
+            * recursive (bool): Performs a recursive search of url page's children
+        """
+        return self.find_all_tags(url, target=None, attrs={"id": id}, depth=depth, count=count, recursive=recursive)
+
+
+    def find_tags_by_class(self, url: str, class_: str, depth: int = 0, count: int = None, recursive: bool = True):
+        """
+        Gets all markup elements with the target class name in specified url.
+
+        Returns a list of the markup elements with the target name as bs4.element.Tag objects.
+
+        Args::
+            * url (str): url of page to be parsed and scanned for target elements.
+            * class (str): class name of markup elements.
+            * depth (int): Number of levels to recursively search for target items. Defaults to 0.
+            * count (int): Number of target items to be found on a url page before stopping.
+            * recursive (bool): Performs a recursive search of url page's children
+        """
+        return self.find_all_tags(url, target=None, attrs={"class": class_}, depth=depth, count=count, recursive=recursive)
+
+
+    def find_comments(self, url: str, depth: int = 0, count: int = None, recursive: bool = True):
+        """
+        Gets all comments in specified url.
+
+        Returns a list of the comments as bs4.element.Comment objects.
+
+        Args::
+            * url (str): url of page to be parsed and scanned for target elements.
+            * depth (int): Number of levels to recursively search for target items. Defaults to 0.
+            * count (int): Number of target items to be found on a url page before stopping.
+            * recursive (bool): Performs a recursive search of url page's children
+        """
+        self.set_base_url(url)
+        base_url_obj = parse_url(self.base_url)
+        soup = self.make_soup_from_url(url)
+        comments = []
+        if soup is not None:
+            comments = soup.find_all(text=lambda text: isinstance(text, Comment), limit=count, recursive=recursive)
+
+            while depth > 0:
+                depth -= 1
+                link_tags = soup.find_all('a', recursive=recursive)
+                links = [ self.get_link_tag(link_tag, download=False) for link_tag in link_tags ]
+                links = filter(lambda link: bool(link), links)   
+                link_objs = [ (link, parse_url(link)) for link in links ]
+                links = [ link_obj[0] for link_obj in link_objs if (base_url_obj.netloc and link_obj[1].netloc) and (base_url_obj.netloc in link_obj[1].netloc) ] 
+
+                with ThreadPoolExecutor() as executor:
+                    results = executor.map(lambda args: self.find_comments(*args), map(lambda link: (link, depth, count, recursive), links))
+                    for result in results:
+                        if result:
+                            comments.extend(result)
+                continue
+        return comments
+
     
     def find_links(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "links.csv", **kwargs) -> List[str]:
         """
         Gets all the links from the given url.
 
         Removes duplicates and returns a list of links and saves the links to a file if `save_to_file` is set to True.
```

### Comparing `bs4_web_scraper-0.0.2a0/bs4_web_scraper/translate.py` & `bs4_web_scraper-0.1.1/bs4_web_scraper/translate.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.0.2a0/bs4_web_scraper/utils.py` & `bs4_web_scraper-0.1.1/bs4_web_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.0.2a0/bs4_web_scraper.egg-info/PKG-INFO` & `bs4_web_scraper-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bs4-web-scraper
-Version: 0.0.2a0
+Name: bs4_web_scraper
+Version: 0.1.1
 Summary: A web scraper based on the BeautifulSoup4 library and translators package.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/bs4_web_scraper
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/bs4_web_scraper/issues
 Project-URL: Repository, https://github.com/ti-oluwa/bs4_web_scraper
 Keywords: web scraper,bs4,beautifulsoup4,web scraping,web scraping with python,web scraping with bs4,web scraping with beautifulsoup4,web scraping with translation,web scraping with translation to other languages,web scraping with translation to other languages with python,web scraping with translation to other languages with bs4,web scraping with translation to other languages with beautifulsoup4,web scraping with translation to other languages with python and bs4,web scraping with translation to other languages with python and beautifulsoup4
@@ -222,14 +222,17 @@
 
 The following are some useful methods for scraping web data using the scraper class.
 
 - `download_url`
 - `download_urls`
 - `find_urls`
 - `find_all_tags`
+- `find_tags_by_id`
+- `find_tags_by_class`
+- `find_comments`
 - `find_links`
 - `find_stylesheets`
 - `find_scripts`
 - `find_videos`
 - `find_images`
 - `find_audios`
 - `find_fonts`
```

### Comparing `bs4_web_scraper-0.0.2a0/pyproject.toml` & `bs4_web_scraper-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bs4_web_scraper"
-version = "0.0.2a"
+version = "0.1.1"
 authors = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 maintainers = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 description = "A web scraper based on the BeautifulSoup4 library and translators package."
```

