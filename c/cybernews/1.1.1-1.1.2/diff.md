# Comparing `tmp/cybernews-1.1.1.tar.gz` & `tmp/cybernews-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybernews-1.1.1.tar", last modified: Mon Apr  3 19:10:06 2023, max compression
+gzip compressed data, was "cybernews-1.1.2.tar", last modified: Fri May 26 22:30:57 2023, max compression
```

## Comparing `cybernews-1.1.1.tar` & `cybernews-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 19:10:06.250262 cybernews-1.1.1/
--rw-rw-rw-   0        0        0     1085 2023-02-14 15:43:47.000000 cybernews-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2600 2023-04-03 19:10:06.249619 cybernews-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-02-14 20:27:18.000000 cybernews-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 19:10:06.237489 cybernews-1.1.1/cybernews/
--rw-rw-rw-   0        0        0        0 2023-02-14 17:22:32.000000 cybernews-1.1.1/cybernews/__init__.py
--rw-rw-rw-   0        0        0    12744 2023-04-03 18:54:53.000000 cybernews-1.1.1/cybernews/cybernews.py
-drwxrwxrwx   0        0        0        0 2023-04-03 19:10:06.243202 cybernews-1.1.1/cybernews.egg-info/
--rw-rw-rw-   0        0        0     2600 2023-04-03 19:10:06.000000 cybernews-1.1.1/cybernews.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-03 19:10:06.000000 cybernews-1.1.1/cybernews.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 19:10:06.000000 cybernews-1.1.1/cybernews.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-03 19:10:06.000000 cybernews-1.1.1/cybernews.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-03 19:10:06.000000 cybernews-1.1.1/cybernews.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 19:10:06.250262 cybernews-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1638 2023-04-03 19:07:56.000000 cybernews-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-03 19:10:06.244228 cybernews-1.1.1/test/
--rw-rw-rw-   0        0        0        0 2023-02-14 18:19:04.000000 cybernews-1.1.1/test/__init__.py
--rw-rw-rw-   0        0        0      734 2023-04-03 18:59:36.000000 cybernews-1.1.1/test/unit.py
-drwxrwxrwx   0        0        0        0 2023-04-03 19:10:06.247770 cybernews-1.1.1/utils/
--rw-rw-rw-   0        0        0       51 2023-02-14 18:00:18.000000 cybernews-1.1.1/utils/__init__.py
--rw-rw-rw-   0        0        0     5319 2023-02-14 20:05:26.000000 cybernews-1.1.1/utils/extractor.py
--rw-rw-rw-   0        0        0     1636 2023-02-14 20:09:33.000000 cybernews-1.1.1/utils/performance.py
--rw-rw-rw-   0        0        0     1616 2023-02-14 18:04:38.000000 cybernews-1.1.1/utils/sorting.py
+drwxrwxrwx   0        0        0        0 2023-05-26 22:30:57.895651 cybernews-1.1.2/
+-rw-rw-rw-   0        0        0     1085 2023-02-14 15:43:47.000000 cybernews-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2600 2023-05-26 22:30:57.895651 cybernews-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-02-14 20:27:18.000000 cybernews-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 22:30:57.883738 cybernews-1.1.2/cybernews/
+-rw-rw-rw-   0        0        0        0 2023-02-14 17:22:32.000000 cybernews-1.1.2/cybernews/__init__.py
+-rw-rw-rw-   0        0        0    13449 2023-05-26 22:23:06.000000 cybernews-1.1.2/cybernews/cybernews.py
+drwxrwxrwx   0        0        0        0 2023-05-26 22:30:57.889089 cybernews-1.1.2/cybernews.egg-info/
+-rw-rw-rw-   0        0        0     2600 2023-05-26 22:30:57.000000 cybernews-1.1.2/cybernews.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-05-26 22:30:57.000000 cybernews-1.1.2/cybernews.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 22:30:57.000000 cybernews-1.1.2/cybernews.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-26 22:30:57.000000 cybernews-1.1.2/cybernews.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-26 22:30:57.000000 cybernews-1.1.2/cybernews.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 22:30:57.895651 cybernews-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1638 2023-05-26 22:26:28.000000 cybernews-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 22:30:57.890624 cybernews-1.1.2/test/
+-rw-rw-rw-   0        0        0        0 2023-02-14 18:19:04.000000 cybernews-1.1.2/test/__init__.py
+-rw-rw-rw-   0        0        0      734 2023-05-26 22:23:12.000000 cybernews-1.1.2/test/unit.py
+drwxrwxrwx   0        0        0        0 2023-05-26 22:30:57.894636 cybernews-1.1.2/utils/
+-rw-rw-rw-   0        0        0       51 2023-02-14 18:00:18.000000 cybernews-1.1.2/utils/__init__.py
+-rw-rw-rw-   0        0        0     5644 2023-05-26 22:23:16.000000 cybernews-1.1.2/utils/extractor.py
+-rw-rw-rw-   0        0        0     1613 2023-05-26 22:23:16.000000 cybernews-1.1.2/utils/performance.py
+-rw-rw-rw-   0        0        0     1777 2023-05-26 22:23:16.000000 cybernews-1.1.2/utils/sorting.py
```

### Comparing `cybernews-1.1.1/LICENSE` & `cybernews-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cybernews-1.1.1/PKG-INFO` & `cybernews-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybernews
-Version: 1.1.1
+Version: 1.1.2
 Summary: Get the latest Cyber Security updates curated from different sources under one roof.
 Author: GhoulBond
 Author-email: hitesh22rana@gmail.com
 Keywords: python,web scraping,news,cyber news,hacker news,hacking,cyber,free,open source,latest news,project,api,REST-API,cyber security,cybersecurity,updates,news,cyber attacks,cyber threats,online security
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cybernews-1.1.1/README.md` & `cybernews-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cybernews-1.1.1/cybernews.egg-info/PKG-INFO` & `cybernews-1.1.2/cybernews.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybernews
-Version: 1.1.1
+Version: 1.1.2
 Summary: Get the latest Cyber Security updates curated from different sources under one roof.
 Author: GhoulBond
 Author-email: hitesh22rana@gmail.com
 Keywords: python,web scraping,news,cyber news,hacker news,hacking,cyber,free,open source,latest news,project,api,REST-API,cyber security,cybersecurity,updates,news,cyber attacks,cyber threats,online security
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cybernews-1.1.1/setup.py` & `cybernews-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 _directory = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(_directory, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.1'
+VERSION = '1.1.2'
 DESCRIPTION = 'Get the latest Cyber Security updates curated from different sources under one roof.'
 LONG_DESCRIPTION = 'Python package and API that make use of Web-Scraping under the hood and provides a variety of curated news related to cyberspace from various sources under one roof. It is designed to help technology enthusiasts stay up-to-date with the latest updates in the field.'
 
 """
     Setting up
 """
```

### Comparing `cybernews-1.1.1/test/unit.py` & `cybernews-1.1.2/test/unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 
     def test_get_news_invalid_type(self):
         for news in self.invalid_news:
             with self.assertRaises(ValueError):
                 self.news.get_news(news)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `cybernews-1.1.1/utils/extractor.py` & `cybernews-1.1.2/utils/extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
     Class for Exception Handling and Extracting data out of complex strings
 """
 import concurrent.futures
-from bs4 import BeautifulSoup
+
 import httpx
+from bs4 import BeautifulSoup
 
-from .sorting import Sorting
 from .performance import Performance
+from .sorting import Sorting
 
 
 class Extractor(Performance):
     def __init__(self):
         """
         Initializing the Extractor class
         """
@@ -31,18 +32,18 @@
         Args:
         name (str): the name to extract from.
 
         Returns:
         str: the extracted author name.
         """
         # Use the '_pattern1' regular expression to remove unwanted characters
-        author_name = self.remove_symbols(self._pattern1.sub('', name))
-        
+        author_name = self.remove_symbols(self._pattern1.sub("", name))
+
         if not self.is_valid_author_name(author_name):
-            return 'N/A'
+            return "N/A"
         return self.format_author_name(author_name)
 
     # Checking is news or some random advertisement
     def _check_ad(self, news_date: str):
         """
         Check if a given date string represents an advertisement.
 
@@ -64,49 +65,58 @@
         date (str): the string to extract the news date from.
         news_date (str): an additional string to use in the extraction process.
 
         Returns:
         str: the extracted news date, or 'N/A' if the date could not be extracted.
         """
         # Use two regular expressions to remove unwanted characters
-        date = self._pattern3.sub('', self._pattern2.sub('', date))
+        date = self._pattern3.sub("", self._pattern2.sub("", date))
         # Use the '_pattern5' regular expression to match the news date
-        return self._pattern5.match(date).group() if news_date != '' else 'N/A'
+        return self._pattern5.match(date).group() if news_date != "" else "N/A"
 
     # Extracting Data From Single News
     def _extract_data_from_single_news(self, url: str, value: dict):
         news_data_from_single_news = []
         response = self.session.get(url, timeout=20, headers=self.headers)
-        soup = BeautifulSoup(response.text, 'lxml')
-        news_headlines = soup.select(value['headlines'])
-        news_author = soup.select(value['author'])
-        news_full_news = soup.select(value['fullNews'])
-        news_url = soup.select(value['newsURL'])
-        news_img_url = soup.select(value['newsImg'])
-        raw_news_date = soup.select(
-            value['date']) if value['date'] is not None else ''
+        soup = BeautifulSoup(response.text, "lxml")
+        news_headlines = soup.select(value["headlines"])
+        raw_news_author = (
+            soup.select(value["author"]) if value["author"] is not None else ""
+        )
+        news_full_news = soup.select(value["fullNews"])
+        news_url = soup.select(value["newsURL"])
+        news_img_url = soup.select(value["newsImg"])
+        raw_news_date = soup.select(value["date"]) if value["date"] is not None else ""
 
         for index in range(len(news_headlines)):
             if raw_news_date:
                 news_date = self._news_date_extractor(
-                    raw_news_date[index].text.strip(), raw_news_date)
+                    raw_news_date[index].text.strip(), raw_news_date
+                )
+            else:
+                news_date = "N/A"
+
+            if raw_news_author:
+                news_author = self._author_name_extractor(
+                    raw_news_author[index].text.strip()
+                )
             else:
-                news_date = 'N/A'
+                news_author = "N/A"
 
             if self._check_ad(news_date):
                 continue
 
             complete_news = {
-                'id': self.sorting.ordering_date(news_date),
-                'headlines': news_headlines[index].text.strip(),
-                'author': self._author_name_extractor(news_author[index].text.strip()),
-                'fullNews': news_full_news[index].text.strip(),
-                'newsURL': news_url[index]['href'],
-                'newsImgURL': news_img_url[index]['data-src'],
-                'newsDate': news_date
+                "id": self.sorting.ordering_date(news_date),
+                "headlines": news_headlines[index].text.strip(),
+                "author": news_author,
+                "fullNews": news_full_news[index].text.strip(),
+                "newsURL": news_url[index]["href"],
+                "newsImgURL": news_img_url[index]["data-src"],
+                "newsDate": news_date,
             }
             news_data_from_single_news.append(complete_news)
 
         return news_data_from_single_news
 
     # Extracting Data Using Tags
     def data_extractor(self, news: list) -> list:
@@ -120,19 +130,24 @@
         list: a list of dictionaries containing the extracted news data.
         """
 
         # Initialize an empty list to store the extracted news data
         news_data = []
 
         with concurrent.futures.ThreadPoolExecutor() as executor:
-            future_to_news = {executor.submit(
-                self._extract_data_from_single_news, url, value): (url, value) for single_news in news for url, value in
-                              single_news.items()}
+            future_to_news = {
+                executor.submit(self._extract_data_from_single_news, url, value): (
+                    url,
+                    value,
+                )
+                for single_news in news
+                for url, value in single_news.items()
+            }
             for future in concurrent.futures.as_completed(future_to_news):
                 url = future_to_news[future]
                 try:
                     news_data_from_single_news = future.result()
                     news_data.extend(news_data_from_single_news)
                 except Exception as exc:
-                    print(f'{url} generated an exception: {exc}')
+                    print(f"{url} generated an exception: {exc}")
 
         return self.sorting.ordering_news(news_data)
```

### Comparing `cybernews-1.1.1/utils/sorting.py` & `cybernews-1.1.2/utils/sorting.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,62 +2,74 @@
     Class for Sorting News According to the date
 """
 import uuid
 
 
 class Sorting:
     """
-        Months Dictionary
+    Months Dictionary
     """
+
     def __init__(self) -> None:
         self._months = {
-            'january': '01',
-            'february': '02',
-            'march': '03',
-            'april': '04',
-            'may': '05',
-            'june': '06',
-            'july': '07',
-            'august': '08',
-            'september': '09',
-            'october': '10',
-            'november': '11',
-            'december': '12'
+            "january": "01",
+            "february": "02",
+            "march": "03",
+            "april": "04",
+            "may": "05",
+            "june": "06",
+            "july": "07",
+            "august": "08",
+            "september": "09",
+            "october": "10",
+            "november": "11",
+            "december": "12",
         }
 
     """
         Giving UUID as _id for each news so that id is distinct
     """
+
     def _ordering_id(self, news):
         for individual_news in news:
-            individual_news['id'] = uuid.uuid4().int
+            individual_news["id"] = uuid.uuid4().int
 
         return news
 
     """
         Ordering Date
     """
+
     def ordering_date(self, individual_news):
-        if individual_news == 'N/A':
+        if individual_news == "N/A":
             return 1
 
-        individual_news = individual_news.lower().replace(',', '').split(' ')
+        individual_news = individual_news.lower().replace(",", "").split(" ")
 
         try:
             if individual_news[0].isnumeric():
-                return int(individual_news[2] + self._months[individual_news[1]] + individual_news[0])
-
-            return int(individual_news[2] + self._months[individual_news[0]] + individual_news[1])
+                return int(
+                    individual_news[2]
+                    + self._months[individual_news[1]]
+                    + individual_news[0]
+                )
+
+            return int(
+                individual_news[2]
+                + self._months[individual_news[0]]
+                + individual_news[1]
+            )
 
         except Exception as _:
             return 1
 
     """
         Ordering News By Latest Date
     """
-    def ordering_news(self, news):
 
+    def ordering_news(self, news):
         data = sorted(
-            news, key=lambda individual_news: individual_news['id'], reverse=True)
+            news, key=lambda individual_news: individual_news["id"], reverse=True
+        )
 
         data = self._ordering_id(data)
         return data
```

