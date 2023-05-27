# Comparing `tmp/proxyUtil-0.1.2.tar.gz` & `tmp/proxyUtil-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxyUtil-0.1.2.tar", last modified: Fri May 26 16:10:44 2023, max compression
+gzip compressed data, was "proxyUtil-0.1.3.tar", last modified: Sat May 27 08:43:30 2023, max compression
```

## Comparing `proxyUtil-0.1.2.tar` & `proxyUtil-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-26 16:10:44.957942 proxyUtil-0.1.2/
--rw-r--r--   0 kali      (1000) kali      (1000)     1070 2023-04-16 07:27:26.000000 proxyUtil-0.1.2/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)       84 2023-05-24 12:11:07.000000 proxyUtil-0.1.2/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     3431 2023-05-26 16:10:44.957942 proxyUtil-0.1.2/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     2883 2023-04-16 07:27:26.000000 proxyUtil-0.1.2/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-26 16:10:44.957942 proxyUtil-0.1.2/proxyUtil/
--rw-r--r--   0 kali      (1000) kali      (1000)      179 2023-04-16 07:27:26.000000 proxyUtil-0.1.2/proxyUtil/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)      283 2023-04-28 16:17:30.000000 proxyUtil-0.1.2/proxyUtil/__version__.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     5039 2023-04-28 13:58:41.000000 proxyUtil-0.1.2/proxyUtil/cdnGen.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6023 2023-04-28 14:06:40.000000 proxyUtil-0.1.2/proxyUtil/cfRecorder.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-26 16:10:44.957942 proxyUtil-0.1.2/proxyUtil/data/
--rw-r--r--   0 kali      (1000) kali      (1000)     8368 2023-04-16 07:27:26.000000 proxyUtil-0.1.2/proxyUtil/data/Clash-Template.yaml
--rwxr-xr-x   0 kali      (1000) kali      (1000)     3247 2023-04-28 14:06:45.000000 proxyUtil-0.1.2/proxyUtil/dnsChecker.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6184 2023-04-16 07:27:26.000000 proxyUtil-0.1.2/proxyUtil/dnsUrl.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4953 2023-04-16 07:27:26.000000 proxyUtil-0.1.2/proxyUtil/dnsUtil.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2397 2023-04-28 14:07:31.000000 proxyUtil-0.1.2/proxyUtil/ipExtractor.py
--rw-r--r--   0 kali      (1000) kali      (1000)      834 2023-04-16 07:27:26.000000 proxyUtil-0.1.2/proxyUtil/logFormatter.py
--rw-r--r--   0 kali      (1000) kali      (1000)    29880 2023-05-11 15:55:26.000000 proxyUtil-0.1.2/proxyUtil/myUtil.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     7048 2023-05-23 07:11:13.000000 proxyUtil-0.1.2/proxyUtil/v2rayChecker.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-26 16:10:44.957942 proxyUtil-0.1.2/proxyUtil.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3431 2023-05-26 16:10:44.000000 proxyUtil-0.1.2/proxyUtil.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      654 2023-05-26 16:10:44.000000 proxyUtil-0.1.2/proxyUtil.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-26 16:10:44.000000 proxyUtil-0.1.2/proxyUtil.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      211 2023-05-26 16:10:44.000000 proxyUtil-0.1.2/proxyUtil.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      595 2023-05-26 16:10:44.000000 proxyUtil-0.1.2/proxyUtil.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-05-26 16:10:44.000000 proxyUtil-0.1.2/proxyUtil.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      570 2023-04-16 07:27:26.000000 proxyUtil-0.1.2/requirements.txt
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-26 16:10:44.957942 proxyUtil-0.1.2/scripts/
--rwxr-xr-x   0 kali      (1000) kali      (1000)     7639 2023-04-16 07:27:26.000000 proxyUtil-0.1.2/scripts/clashGen
--rwxr-xr-x   0 kali      (1000) kali      (1000)     4292 2023-05-11 15:57:25.000000 proxyUtil-0.1.2/scripts/connectMe
--rwxr-xr-x   0 kali      (1000) kali      (1000)     5346 2023-04-16 07:27:26.000000 proxyUtil-0.1.2/scripts/shadowChecker
--rwxr-xr-x   0 kali      (1000) kali      (1000)     1199 2023-04-16 07:27:26.000000 proxyUtil-0.1.2/scripts/ssURI2sslocal
--rwxr-xr-x   0 kali      (1000) kali      (1000)     1051 2023-04-16 07:27:26.000000 proxyUtil-0.1.2/scripts/sslocal2ssURI
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-05-26 16:10:44.957942 proxyUtil-0.1.2/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     2114 2023-05-24 12:26:37.000000 proxyUtil-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:43:30.178429 proxyUtil-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-27 08:43:30.178429 proxyUtil-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:43:30.174429 proxyUtil-0.1.3/proxyUtil/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/proxyUtil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/proxyUtil/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5039 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/proxyUtil/cdnGen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/proxyUtil/cfRecorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:43:30.178429 proxyUtil-0.1.3/proxyUtil/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/proxyUtil/data/Clash-Template.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3247 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/proxyUtil/dnsChecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/proxyUtil/dnsUrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/proxyUtil/dnsUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/proxyUtil/ipExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/proxyUtil/logFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29880 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/proxyUtil/myUtil.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7174 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/proxyUtil/v2rayChecker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:43:30.178429 proxyUtil-0.1.3/proxyUtil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-27 08:43:30.000000 proxyUtil-0.1.3/proxyUtil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-27 08:43:30.000000 proxyUtil-0.1.3/proxyUtil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:43:30.000000 proxyUtil-0.1.3/proxyUtil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-27 08:43:30.000000 proxyUtil-0.1.3/proxyUtil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-27 08:43:30.000000 proxyUtil-0.1.3/proxyUtil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-27 08:43:30.000000 proxyUtil-0.1.3/proxyUtil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:43:30.178429 proxyUtil-0.1.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7639 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/scripts/clashGen
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4292 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/scripts/connectMe
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5346 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/scripts/shadowChecker
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/scripts/ssURI2sslocal
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/scripts/sslocal2ssURI
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:43:30.178429 proxyUtil-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-27 08:43:11.000000 proxyUtil-0.1.3/setup.py
```

### Comparing `proxyUtil-0.1.2/LICENSE` & `proxyUtil-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/PKG-INFO` & `proxyUtil-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxyUtil
-Version: 0.1.2
+Version: 0.1.3
 Summary: some proxy tools
 Home-page: https://github.com/mheidari98/proxyUtil
 Author: Mahdi Heidari
 Author-email: mahdih3idari@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `proxyUtil-0.1.2/README.md` & `proxyUtil-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/proxyUtil/cdnGen.py` & `proxyUtil-0.1.3/proxyUtil/cdnGen.py`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/proxyUtil/cfRecorder.py` & `proxyUtil-0.1.3/proxyUtil/cfRecorder.py`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/proxyUtil/data/Clash-Template.yaml` & `proxyUtil-0.1.3/proxyUtil/data/Clash-Template.yaml`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/proxyUtil/dnsChecker.py` & `proxyUtil-0.1.3/proxyUtil/dnsChecker.py`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/proxyUtil/dnsUrl.py` & `proxyUtil-0.1.3/proxyUtil/dnsUrl.py`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/proxyUtil/dnsUtil.py` & `proxyUtil-0.1.3/proxyUtil/dnsUtil.py`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/proxyUtil/ipExtractor.py` & `proxyUtil-0.1.3/proxyUtil/ipExtractor.py`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/proxyUtil/logFormatter.py` & `proxyUtil-0.1.3/proxyUtil/logFormatter.py`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/proxyUtil/myUtil.py` & `proxyUtil-0.1.3/proxyUtil/myUtil.py`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/proxyUtil/v2rayChecker.py` & `proxyUtil-0.1.3/proxyUtil/v2rayChecker.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     parser.add_argument("-d", "--domain", help="test connect domain", default='http://www.gstatic.com/generate_204')
     parser.add_argument("-t", "--timeout", help="timeout in seconds, default is 3", default=3 , type=int)
     parser.add_argument("-l", "--lport", help="start local port, default is 1080", default=1080, type=int)
     parser.add_argument('-v', "--verbose", help="increase output verbosity", action="store_true", default=False)
     parser.add_argument('-vv', '--debug', help="debug log", action='store_true', default=False)
     parser.add_argument('-T', '--threads', help="threads number, default is 10", default=10, type=int)
     parser.add_argument('-n', '--number', help="number of proxy to check", type=int)
+    parser.add_argument('-s', '--shuffle', help="shuffle proxies", action='store_true', default=False)
     parser.add_argument('-x', '--xray', help="use xray core instead v2ray", action='store_true', default=False)
     parser.add_argument('-c', '--core', help="select core from [v2ray, xray]", choices=["v2ray", "xray", "wxray"], default="xray")
     parser.add_argument('--t2exec', help="time to execute core, default is 1", default=1, type=float)
     parser.add_argument('--t2kill', help="time to kill core, default is 0.1", default=0.1, type=float)
     parser.add_argument('--url', help="get proxy from url")
     parser.add_argument('--free', help="get free proxy", action='store_true', default=False)
     parser.add_argument('--stdin', help="get proxy from stdin", action='store_true', default=False)
@@ -132,16 +133,20 @@
     if args.free :
         lines.update( ScrapURL('https://raw.githubusercontent.com/mheidari98/.proxy/main/all') )
 
     if args.stdin :
         lines.update( parseContent(sys.stdin.read()) )
     
     lines = list(lines)
+
+    if args.shuffle :
+        random.shuffle(lines)
+
     if args.number :
-        lines = random.sample(lines, min(args.number, len(lines)))
+        lines = lines[:args.number]
     logging.info(f"We have {len(lines)} proxy to check")
     
     if not lines:
         logging.error("No proxy to check")
         return
     
     N = min(args.threads, len(lines))
```

### Comparing `proxyUtil-0.1.2/proxyUtil.egg-info/PKG-INFO` & `proxyUtil-0.1.3/proxyUtil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxyUtil
-Version: 0.1.2
+Version: 0.1.3
 Summary: some proxy tools
 Home-page: https://github.com/mheidari98/proxyUtil
 Author: Mahdi Heidari
 Author-email: mahdih3idari@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `proxyUtil-0.1.2/proxyUtil.egg-info/SOURCES.txt` & `proxyUtil-0.1.3/proxyUtil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/proxyUtil.egg-info/requires.txt` & `proxyUtil-0.1.3/proxyUtil.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/requirements.txt` & `proxyUtil-0.1.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/scripts/clashGen` & `proxyUtil-0.1.3/scripts/clashGen`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/scripts/connectMe` & `proxyUtil-0.1.3/scripts/connectMe`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/scripts/shadowChecker` & `proxyUtil-0.1.3/scripts/shadowChecker`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/scripts/ssURI2sslocal` & `proxyUtil-0.1.3/scripts/ssURI2sslocal`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/scripts/sslocal2ssURI` & `proxyUtil-0.1.3/scripts/sslocal2ssURI`

 * *Files identical despite different names*

### Comparing `proxyUtil-0.1.2/setup.py` & `proxyUtil-0.1.3/setup.py`

 * *Files identical despite different names*

