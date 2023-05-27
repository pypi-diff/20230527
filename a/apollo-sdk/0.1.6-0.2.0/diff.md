# Comparing `tmp/apollo-sdk-0.1.6.tar.gz` & `tmp/apollo-sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-sdk-0.1.6.tar", last modified: Sat May  6 03:15:36 2023, max compression
+gzip compressed data, was "apollo-sdk-0.2.0.tar", last modified: Sat May 27 06:14:29 2023, max compression
```

## Comparing `apollo-sdk-0.1.6.tar` & `apollo-sdk-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,65 @@
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.622763 apollo-sdk-0.1.6/
--rw-r--r--   0 adrianbrown   (501) staff       (20)     3793 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/LICENSE
--rw-r--r--   0 adrianbrown   (501) staff       (20)     5909 2023-05-06 03:15:36.622834 apollo-sdk-0.1.6/PKG-INFO
--rw-r--r--   0 adrianbrown   (501) staff       (20)     5259 2023-05-06 02:32:52.000000 apollo-sdk-0.1.6/README.md
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.618934 apollo-sdk-0.1.6/apollo/
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1419 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/__init__.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     3778 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/client.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.619058 apollo-sdk-0.1.6/apollo/connectors/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/connectors/__init__.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.619182 apollo-sdk-0.1.6/apollo/connectors/aws/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/connectors/aws/__init__.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.619347 apollo-sdk-0.1.6/apollo/connectors/google/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/connectors/google/__init__.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.619480 apollo-sdk-0.1.6/apollo/connectors/microsoft/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/connectors/microsoft/__init__.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.619597 apollo-sdk-0.1.6/apollo/connectors/openai/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/connectors/openai/__init__.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1450 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/const.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.619728 apollo-sdk-0.1.6/apollo/database/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/__init__.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.620233 apollo-sdk-0.1.6/apollo/database/firebase/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      770 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/firebase/__init__.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1488 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/firebase/base.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     3494 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/firebase/cloud.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1438 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/firebase/local.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.620361 apollo-sdk-0.1.6/apollo/database/mongo/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/mongo/__init__.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.620490 apollo-sdk-0.1.6/apollo/database/mysql/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/mysql/__init__.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.620645 apollo-sdk-0.1.6/apollo/database/postgres/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/postgres/__init__.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.621161 apollo-sdk-0.1.6/apollo/database/supabase/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      770 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/supabase/__init__.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)      739 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/supabase/base.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1553 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/supabase/cloud.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)      810 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/supabase/local.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     4197 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/exceptions.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1389 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/manager.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1230 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/resource.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.621294 apollo-sdk-0.1.6/apollo/service/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/service/__init__.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.621417 apollo-sdk-0.1.6/apollo/service/graphql/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/service/graphql/__init__.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.621919 apollo-sdk-0.1.6/apollo/service/json/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      754 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/service/json/__init__.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)      859 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/service/json/base.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1209 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/service/json/cloud.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)      888 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/service/json/local.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.622036 apollo-sdk-0.1.6/apollo/tests/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/tests/__init__.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.622647 apollo-sdk-0.1.6/apollo_sdk.egg-info/
--rw-r--r--   0 adrianbrown   (501) staff       (20)     5909 2023-05-06 03:15:36.000000 apollo-sdk-0.1.6/apollo_sdk.egg-info/PKG-INFO
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1107 2023-05-06 03:15:36.000000 apollo-sdk-0.1.6/apollo_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 adrianbrown   (501) staff       (20)        1 2023-05-06 03:15:36.000000 apollo-sdk-0.1.6/apollo_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 adrianbrown   (501) staff       (20)      266 2023-05-06 03:15:36.000000 apollo-sdk-0.1.6/apollo_sdk.egg-info/requires.txt
--rw-r--r--   0 adrianbrown   (501) staff       (20)        7 2023-05-06 03:15:36.000000 apollo-sdk-0.1.6/apollo_sdk.egg-info/top_level.txt
--rw-r--r--   0 adrianbrown   (501) staff       (20)      103 2023-05-06 03:15:36.623064 apollo-sdk-0.1.6/setup.cfg
--rw-r--r--   0 adrianbrown   (501) staff       (20)     2092 2023-05-06 03:15:18.000000 apollo-sdk-0.1.6/setup.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.565208 apollo-sdk-0.2.0/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3793 2023-04-29 17:42:09.000000 apollo-sdk-0.2.0/LICENSE
+-rw-r--r--   0 abpyguru   (501) staff       (20)     6096 2023-05-27 06:14:29.565287 apollo-sdk-0.2.0/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5635 2023-05-26 15:53:50.000000 apollo-sdk-0.2.0/README.md
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.558088 apollo-sdk-0.2.0/apollo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2250 2023-05-27 05:36:11.000000 apollo-sdk-0.2.0/apollo/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5275 2023-05-27 05:36:10.000000 apollo-sdk-0.2.0/apollo/client.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.558434 apollo-sdk-0.2.0/apollo/connectors/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/connectors/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.558759 apollo-sdk-0.2.0/apollo/connectors/aws/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/connectors/aws/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.558991 apollo-sdk-0.2.0/apollo/connectors/google/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/connectors/google/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.559252 apollo-sdk-0.2.0/apollo/connectors/microsoft/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/connectors/microsoft/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.560438 apollo-sdk-0.2.0/apollo/connectors/openai/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      801 2023-05-26 16:56:46.000000 apollo-sdk-0.2.0/apollo/connectors/openai/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1023 2023-05-27 05:36:11.000000 apollo-sdk-0.2.0/apollo/connectors/openai/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2574 2023-05-27 05:36:11.000000 apollo-sdk-0.2.0/apollo/connectors/openai/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      956 2023-05-27 05:36:11.000000 apollo-sdk-0.2.0/apollo/connectors/openai/local.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1585 2023-05-26 17:12:47.000000 apollo-sdk-0.2.0/apollo/const.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.560615 apollo-sdk-0.2.0/apollo/database/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/database/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.561360 apollo-sdk-0.2.0/apollo/database/firebase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/database/firebase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/database/firebase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3494 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/database/firebase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1438 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/database/firebase/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.561529 apollo-sdk-0.2.0/apollo/database/mongo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/database/mongo/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.561693 apollo-sdk-0.2.0/apollo/database/mysql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/database/mysql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.561870 apollo-sdk-0.2.0/apollo/database/postgres/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/database/postgres/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.562472 apollo-sdk-0.2.0/apollo/database/supabase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/database/supabase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      739 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/database/supabase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1553 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/database/supabase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      810 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/database/supabase/local.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4197 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/exceptions.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1578 2023-05-27 05:36:11.000000 apollo-sdk-0.2.0/apollo/manager.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.563241 apollo-sdk-0.2.0/apollo/plugins/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-05-26 17:55:34.000000 apollo-sdk-0.2.0/apollo/plugins/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4796 2023-05-27 05:36:11.000000 apollo-sdk-0.2.0/apollo/plugins/utils.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5165 2023-05-27 05:36:11.000000 apollo-sdk-0.2.0/apollo/plugins/validation.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1426 2023-05-27 05:36:10.000000 apollo-sdk-0.2.0/apollo/resource.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.563493 apollo-sdk-0.2.0/apollo/service/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/service/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.563645 apollo-sdk-0.2.0/apollo/service/graphql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/service/graphql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.564252 apollo-sdk-0.2.0/apollo/service/json/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      754 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/service/json/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      947 2023-05-27 05:36:11.000000 apollo-sdk-0.2.0/apollo/service/json/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1272 2023-05-27 05:36:10.000000 apollo-sdk-0.2.0/apollo/service/json/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      926 2023-05-27 05:36:10.000000 apollo-sdk-0.2.0/apollo/service/json/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.564468 apollo-sdk-0.2.0/apollo/tests/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.0/apollo/tests/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 06:14:29.565099 apollo-sdk-0.2.0/apollo_sdk.egg-info/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     6096 2023-05-27 06:14:29.000000 apollo-sdk-0.2.0/apollo_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1288 2023-05-27 06:14:29.000000 apollo-sdk-0.2.0/apollo_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-05-27 06:14:29.000000 apollo-sdk-0.2.0/apollo_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1710 2023-05-27 06:14:29.000000 apollo-sdk-0.2.0/apollo_sdk.egg-info/requires.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        7 2023-05-27 06:14:29.000000 apollo-sdk-0.2.0/apollo_sdk.egg-info/top_level.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)      103 2023-05-27 06:14:29.565497 apollo-sdk-0.2.0/setup.cfg
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1631 2023-05-27 06:13:29.000000 apollo-sdk-0.2.0/setup.py
```

### Comparing `apollo-sdk-0.1.6/LICENSE` & `apollo-sdk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/PKG-INFO` & `apollo-sdk-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,120 +1,130 @@
 Metadata-Version: 2.1
 Name: apollo-sdk
-Version: 0.1.6
+Version: 0.2.0
 Summary: Build automated decision making workflows by aggregating your AI models and data into one api.
 Home-page: https://github.com/apolloapi/apolloapi
-Author: Apollo API, Inc.
+Author: Apollo API
 Author-email: adrbrownx@gmail.com
 License: Elastic License v2
-Classifier: Intended Audience :: Developers
+Platform: Any
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
-![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/6455b1fd3d8642575f793c94_header.png)
+![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/643fffb82419ac18d39e3e4e_Screenshot%202023-04-19%20at%2010.50.13%20AM.png)
 
 </div>
 
-<h1 align="center">Open-source Task Automation</h1>
+<h1 align="center">The easiest way to build custom decision making workflows</h1>
 
 <div align="center">
-Apollo is an open-source no-code platform that helps you build automated workflows in minutes. Our SDK allows you to automate tasks such as; onboarding, compliance, trust & safety, fraud detection, code generation and more.
+Apollo gives you access to custom machine learning models, no-code platform and continuously syncs data from any API or Database to centralize investigations and allow you to automate the detection of harm in images, videos, audio and text.
 </div>
 
 <p align="center">
     <br />
-    <a href="https://docs.apolloapi.io/" rel="dofollow"><strong>Docs »</strong></a>
+    <a href="https://apolloapi-doc.vercel.app/" rel="dofollow"><strong>Docs »</strong></a>
     <br />
 
   <br/>
+    <a href="https://apolloapi-doc.vercel.app/">Examples</a>
     <a href="https://www.apolloapi.io/">Join the waitlist</a>
     ·
     <a href="https://github.com/apolloapi/apolloapi/issues">Report Bug</a>
     ·
     <a href="https://discord.gg/ZUH7f7AzUY">Community Discord</a>
 </p>
 
-## Why Apollo API?
+## ⭐ Can you show me an example?
 
-Before Apollo, integrating AI models and building automated workflows could be time-consuming and complex, with Apollo, teams can simplify and accelerate the process, making it easier to deploy AI models, sync data, and develop insights in minutes.
+In your code you can write:
 
-## 🚀 Interesting, how can I try it?
+```ts
+Apollo.connect('postgres://username:password@hostnam...', ...) // Starts syncing content forever!
 
-Lets install the SDK first...
+Apollo.use('OpenAI', "moderation", ...) // Connect to existing providers!
+
+Apollo.rule('Phrase1', '>=', '0.8') // Create custom rules!
+
+Apollo.use('Apollo', "violence", ...) // Connect with our internal models!
+
+// Detect bad actors at scale!
+Apollo.detectImage('Image1', 'contains', 'VERY_LIKELY') // Image Analysis/OCR
+Apollo.detectSpeech('Audio1', 'contains', 'UNLIKELY') // Audio Processing
+Apollo.detectVideo('Video1', 'contains', 'POSSIBLE') // Video Analysis
+Apollo.detectText('Phrase1', 'contains', 'UNKNOWN') // Text Analysis
 
-```bash
-pip install apollo-sdk
 ```
 
-Let's setup your first Integration!
+Apollo then takes care of:
+
+- Detecting real-time changes in user experience
+- Automated detection against image, video, audio or text
+- Connecting policy to product
+- Making sure your integration is robust, so you never again have to worry about stuck/stale data or false-positives
+
+## 🧑‍💻 Cool, what can I build with it?
+
+- Trust & Safety teams in companies use Apollo to **build native in-app connections** related to active response, content moderation, fraud detection, etc.
+- Some **automate their personal lives** with Apollo by integrating against discord communities or other decentralized networks for safety
+- Apollo can help you **quickly build trust** for hobby projects, communities or business
+
+## 🚀 Interesting, how can I try it?
+
+Let's setup your first Integration in 2 minutes!
 
 It will pull from your local database (and keep it in sync).
 
+To start:
+
+```bash
+# install the cli-toolkit
+pip install apollo-sdk
+
+# enter a python repl or create a python file, up to you! (repl is easiest)
+python3
+```
+
 ```python
 # import the package
 from apollo.client import Apollo
 
 # sync data from your database instance
 # (we support supabase at the current moment or postgresql via uri format)
 Apollo.connect("postgres://username:password@hostname:port/database_name")
 
 # If you want to test out operation on your external connection
 Apollo.fetch_tables()
 Apollo.query("desc", "table", "column")
 ```
 
-...and create a workflow with a simple command:
+Test sending your content to our API!
 
-_Note: you can obtain a Auth token [here](https://docs.apolloapi.io/docs/api/authentication), sign up today on our [Site](https://app.apolloapi.io/)_
+...and create a workflow with a simple command:
 
 ```python
 # import the package
 from apollo.client import Apollo
 
 # Use our custom model to test building decisions
 Apollo.use("apollo", token="YOUR_API_TOKEN_HERE")
 
-# Lets check to see if a phrase contains threats
+# We support video, speech, image and text. Try text!
 Apollo.detectText("Phrase1", "contains", "Threats")
-
-# Create custom rules which creates a task!
-Apollo.rule('Phrase1', '>=', '0.8')
-
-# Connect with other models!
-Apollo.use('Google', "violence", ...)
-
-Apollo.detectImage('Image1', 'contains', 'VERY_LIKELY') # Image Analysis/OCR
-Apollo.detectSpeech('Audio1', 'contains', 'UNLIKELY') # Audio Processing
-Apollo.detectVideo('Video1', 'contains', 'POSSIBLE') # Video Analysis
-Apollo.detectText('Phrase1', 'contains', 'UNKNOWN') # Text Analysis
 ```
 
 That's all it takes!
 
-## Apollo then takes care of:
-
-- Detecting real-time changes in your data
-- Automating tasks against image, video, audio or text
-- Simplifying the process of deploying AI models
-- Making sure your integration is robust, so you never again have to worry about stuck/stale data or false-positives
-
-In practice, you probably want to use one of our native SDKs to interact with Apollo's API or use our custom browser client so you dont have to write code. If so, sign up at [Apollo API](https://app.apolloapi.io/signup)!
+That's all it takes! You can check out [more on our notion page](https://cloudguruab.notion.site/Apollo-e5e347745c1e43798d849d79cce90aba).
 
-## 🧑‍💻 Cool, what can I build with it?
-
-- Trust & Safety teams can use Apollo to **build native in-app connections** related to active response, content moderation, fraud detection, etc.
-- Some **automate their personal lives** with Apollo by integrating against discord communities or their personal lives
-- Apollo can help you **quickly automate tasks** for hobby projects, communities or business
+In practice, you probably want to use one of our native SDKs to interact with Apollo's API or use our custom browser client so you dont have to write code. If so, ping us at adrian@apolloapi.io!
 
 ## Contributing
 
 ### 📦 pre-commit config
 
 As an open source project, Apollo welcomes contributions from the community at large. This isn’t an exhaustive reference and is a living document subject to change as needed when the project formalizes any practice or pattern.
 
@@ -159,7 +169,11 @@
 
 ⭐ Follow our development by starring us here on GitHub ⭐
 
 - Share feedback or ask questions on the [Discord community](https://discord.gg/ZUH7f7AzUY)
 - [Chat with a member of the team](https://apolloapi.io) 👋
 - Check our [blog on Trust & Safety](https://www.thebriefnewsletter.com)
 - Look at our docs on how to get started [here!](https://apolloapi-doc.vercel.app/)
+
+## NOTES CLI TEST
+
+- set env variables for provider (openai) either in .env file or by exports
```

#### html2text {}

```diff
@@ -1,78 +1,78 @@
-Metadata-Version: 2.1 Name: apollo-sdk Version: 0.1.6 Summary: Build automated
+Metadata-Version: 2.1 Name: apollo-sdk Version: 0.2.0 Summary: Build automated
 decision making workflows by aggregating your AI models and data into one api.
-Home-page: https://github.com/apolloapi/apolloapi Author: Apollo API, Inc.
-Author-email: adrbrownx@gmail.com License: Elastic License v2 Classifier:
-Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
-text/markdown License-File: LICENSE
+Home-page: https://github.com/apolloapi/apolloapi Author: Apollo API Author-
+email: adrbrownx@gmail.com License: Elastic License v2 Platform: Any
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Description-Content-Type: text/markdown License-File: LICENSE
     ![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/
-                     6455b1fd3d8642575f793c94_header.png)
-                   ****** Open-source Task Automation ******
-   Apollo is an open-source no-code platform that helps you build automated
-workflows in minutes. Our SDK allows you to automate tasks such as; onboarding,
-    compliance, trust & safety, fraud detection, code generation and more.
+  643fffb82419ac18d39e3e4e_Screenshot%202023-04-19%20at%2010.50.13%20AM.png)
+    ****** The easiest way to build custom decision making workflows ******
+Apollo gives you access to custom machine learning models, no-code platform and
+ continuously syncs data from any API or Database to centralize investigations
+ and allow you to automate the detection of harm in images, videos, audio and
+                                     text.
 
                                    Docs_Â»
 
-             Join_the_waitlist Â· Report_Bug Â· Community_Discord
-## Why Apollo API? Before Apollo, integrating AI models and building automated
-workflows could be time-consuming and complex, with Apollo, teams can simplify
-and accelerate the process, making it easier to deploy AI models, sync data,
-and develop insights in minutes. ## ð Interesting, how can I try it? Lets
-install the SDK first... ```bash pip install apollo-sdk ``` Let's setup your
-first Integration! It will pull from your local database (and keep it in sync).
-```python # import the package from apollo.client import Apollo # sync data
-from your database instance # (we support supabase at the current moment or
-postgresql via uri format) Apollo.connect("postgres://username:
-password@hostname:port/database_name") # If you want to test out operation on
-your external connection Apollo.fetch_tables() Apollo.query("desc", "table",
-"column") ``` ...and create a workflow with a simple command: _Note: you can
-obtain a Auth token [here](https://docs.apolloapi.io/docs/api/authentication),
-sign up today on our [Site](https://app.apolloapi.io/)_ ```python # import the
+         Examples Join_the_waitlist Â· Report_Bug Â· Community_Discord
+## â­ Can you show me an example? In your code you can write: ```ts
+Apollo.connect('postgres://username:password@hostnam...', ...) // Starts
+syncing content forever! Apollo.use('OpenAI', "moderation", ...) // Connect to
+existing providers! Apollo.rule('Phrase1', '>=', '0.8') // Create custom rules!
+Apollo.use('Apollo', "violence", ...) // Connect with our internal models! /
+/ Detect bad actors at scale! Apollo.detectImage('Image1', 'contains',
+'VERY_LIKELY') // Image Analysis/OCR Apollo.detectSpeech('Audio1', 'contains',
+'UNLIKELY') // Audio Processing Apollo.detectVideo('Video1', 'contains',
+'POSSIBLE') // Video Analysis Apollo.detectText('Phrase1', 'contains',
+'UNKNOWN') // Text Analysis ``` Apollo then takes care of: - Detecting real-
+time changes in user experience - Automated detection against image, video,
+audio or text - Connecting policy to product - Making sure your integration is
+robust, so you never again have to worry about stuck/stale data or false-
+positives ## ð§âð» Cool, what can I build with it? - Trust & Safety teams
+in companies use Apollo to **build native in-app connections** related to
+active response, content moderation, fraud detection, etc. - Some **automate
+their personal lives** with Apollo by integrating against discord communities
+or other decentralized networks for safety - Apollo can help you **quickly
+build trust** for hobby projects, communities or business ## ð Interesting,
+how can I try it? Let's setup your first Integration in 2 minutes! It will pull
+from your local database (and keep it in sync). To start: ```bash # install the
+cli-toolkit pip install apollo-sdk # enter a python repl or create a python
+file, up to you! (repl is easiest) python3 ``` ```python # import the package
+from apollo.client import Apollo # sync data from your database instance # (we
+support supabase at the current moment or postgresql via uri format)
+Apollo.connect("postgres://username:password@hostname:port/database_name") # If
+you want to test out operation on your external connection Apollo.fetch_tables
+() Apollo.query("desc", "table", "column") ``` Test sending your content to our
+API! ...and create a workflow with a simple command: ```python # import the
 package from apollo.client import Apollo # Use our custom model to test
-building decisions Apollo.use("apollo", token="YOUR_API_TOKEN_HERE") # Lets
-check to see if a phrase contains threats Apollo.detectText("Phrase1",
-"contains", "Threats") # Create custom rules which creates a task! Apollo.rule
-('Phrase1', '>=', '0.8') # Connect with other models! Apollo.use('Google',
-"violence", ...) Apollo.detectImage('Image1', 'contains', 'VERY_LIKELY') #
-Image Analysis/OCR Apollo.detectSpeech('Audio1', 'contains', 'UNLIKELY') #
-Audio Processing Apollo.detectVideo('Video1', 'contains', 'POSSIBLE') # Video
-Analysis Apollo.detectText('Phrase1', 'contains', 'UNKNOWN') # Text Analysis
-``` That's all it takes! ## Apollo then takes care of: - Detecting real-time
-changes in your data - Automating tasks against image, video, audio or text -
-Simplifying the process of deploying AI models - Making sure your integration
-is robust, so you never again have to worry about stuck/stale data or false-
-positives In practice, you probably want to use one of our native SDKs to
-interact with Apollo's API or use our custom browser client so you dont have to
-write code. If so, sign up at [Apollo API](https://app.apolloapi.io/signup)! ##
-ð§âð» Cool, what can I build with it? - Trust & Safety teams can use
-Apollo to **build native in-app connections** related to active response,
-content moderation, fraud detection, etc. - Some **automate their personal
-lives** with Apollo by integrating against discord communities or their
-personal lives - Apollo can help you **quickly automate tasks** for hobby
-projects, communities or business ## Contributing ### ð¦ pre-commit config As
-an open source project, Apollo welcomes contributions from the community at
-large. This isnât an exhaustive reference and is a living document subject to
-change as needed when the project formalizes any practice or pattern. Clone the
-repo and start Apollo locally... ```bash git clone https://github.com/
-apolloapi/apolloapi.git cd apolloapi && python3 -m venv env && source env/bin/
-activate && pip install -r requirements.txt ``` - After installing system
-dependencies be sure to install pre-commit for lint checks ```bash pip install
-pre-commit pre-commit install pre-commit run --all-files ``` Apollo uses commit
-messages for automated generation of project changelog. For every pull request
-we request contributors to be compliant with the following commit message
-notation. ``` :
+building decisions Apollo.use("apollo", token="YOUR_API_TOKEN_HERE") # We
+support video, speech, image and text. Try text! Apollo.detectText("Phrase1",
+"contains", "Threats") ``` That's all it takes! That's all it takes! You can
+check out [more on our notion page](https://cloudguruab.notion.site/Apollo-
+e5e347745c1e43798d849d79cce90aba). In practice, you probably want to use one of
+our native SDKs to interact with Apollo's API or use our custom browser client
+so you dont have to write code. If so, ping us at adrian@apolloapi.io! ##
+Contributing ### ð¦ pre-commit config As an open source project, Apollo
+welcomes contributions from the community at large. This isnât an exhaustive
+reference and is a living document subject to change as needed when the project
+formalizes any practice or pattern. Clone the repo and start Apollo locally...
+```bash git clone https://github.com/apolloapi/apolloapi.git cd apolloapi &&
+python3 -m venv env && source env/bin/activate && pip install -
+r requirements.txt ``` - After installing system dependencies be sure to
+install pre-commit for lint checks ```bash pip install pre-commit pre-commit
+install pre-commit run --all-files ``` Apollo uses commit messages for
+automated generation of project changelog. For every pull request we request
+contributors to be compliant with the following commit message notation. ``` :
 ``` Accepted `` values: - new = newly implemented user-facing features - chg =
 changes in existing user-facing features - fix = user-facing bugfixes - oth =
 other changes which users should know about - dev = any developer-facing
 changes, regardless of new/chg/fix status #### Summary (The first line) The
 first line should not be longer than 75 characters, the second line is always
 blank and other lines should be wrapped at 80 characters. ## ð Neat, I would
 like to learn more â­ Follow our development by starring us here on GitHub â­
 - Share feedback or ask questions on the [Discord community](https://
 discord.gg/ZUH7f7AzUY) - [Chat with a member of the team](https://apolloapi.io)
 ð - Check our [blog on Trust & Safety](https://www.thebriefnewsletter.com) -
 Look at our docs on how to get started [here!](https://apolloapi-
-doc.vercel.app/)
+doc.vercel.app/) ## NOTES CLI TEST - set env variables for provider (openai)
+either in .env file or by exports
```

### Comparing `apollo-sdk-0.1.6/README.md` & `apollo-sdk-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,116 @@
 <div align="center">
 
-![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/6455b1fd3d8642575f793c94_header.png)
+![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/643fffb82419ac18d39e3e4e_Screenshot%202023-04-19%20at%2010.50.13%20AM.png)
 
 </div>
 
-<h1 align="center">Open-source Task Automation</h1>
+<h1 align="center">The easiest way to build custom decision making workflows</h1>
 
 <div align="center">
-Apollo is an open-source no-code platform that helps you build automated workflows in minutes. Our SDK allows you to automate tasks such as; onboarding, compliance, trust & safety, fraud detection, code generation and more.
+Apollo gives you access to custom machine learning models, no-code platform and continuously syncs data from any API or Database to centralize investigations and allow you to automate the detection of harm in images, videos, audio and text.
 </div>
 
 <p align="center">
     <br />
-    <a href="https://docs.apolloapi.io/" rel="dofollow"><strong>Docs »</strong></a>
+    <a href="https://apolloapi-doc.vercel.app/" rel="dofollow"><strong>Docs »</strong></a>
     <br />
 
   <br/>
+    <a href="https://apolloapi-doc.vercel.app/">Examples</a>
     <a href="https://www.apolloapi.io/">Join the waitlist</a>
     ·
     <a href="https://github.com/apolloapi/apolloapi/issues">Report Bug</a>
     ·
     <a href="https://discord.gg/ZUH7f7AzUY">Community Discord</a>
 </p>
 
-## Why Apollo API?
+## ⭐ Can you show me an example?
 
-Before Apollo, integrating AI models and building automated workflows could be time-consuming and complex, with Apollo, teams can simplify and accelerate the process, making it easier to deploy AI models, sync data, and develop insights in minutes.
+In your code you can write:
 
-## 🚀 Interesting, how can I try it?
+```ts
+Apollo.connect('postgres://username:password@hostnam...', ...) // Starts syncing content forever!
 
-Lets install the SDK first...
+Apollo.use('OpenAI', "moderation", ...) // Connect to existing providers!
+
+Apollo.rule('Phrase1', '>=', '0.8') // Create custom rules!
+
+Apollo.use('Apollo', "violence", ...) // Connect with our internal models!
+
+// Detect bad actors at scale!
+Apollo.detectImage('Image1', 'contains', 'VERY_LIKELY') // Image Analysis/OCR
+Apollo.detectSpeech('Audio1', 'contains', 'UNLIKELY') // Audio Processing
+Apollo.detectVideo('Video1', 'contains', 'POSSIBLE') // Video Analysis
+Apollo.detectText('Phrase1', 'contains', 'UNKNOWN') // Text Analysis
 
-```bash
-pip install apollo-sdk
 ```
 
-Let's setup your first Integration!
+Apollo then takes care of:
+
+- Detecting real-time changes in user experience
+- Automated detection against image, video, audio or text
+- Connecting policy to product
+- Making sure your integration is robust, so you never again have to worry about stuck/stale data or false-positives
+
+## 🧑‍💻 Cool, what can I build with it?
+
+- Trust & Safety teams in companies use Apollo to **build native in-app connections** related to active response, content moderation, fraud detection, etc.
+- Some **automate their personal lives** with Apollo by integrating against discord communities or other decentralized networks for safety
+- Apollo can help you **quickly build trust** for hobby projects, communities or business
+
+## 🚀 Interesting, how can I try it?
+
+Let's setup your first Integration in 2 minutes!
 
 It will pull from your local database (and keep it in sync).
 
+To start:
+
+```bash
+# install the cli-toolkit
+pip install apollo-sdk
+
+# enter a python repl or create a python file, up to you! (repl is easiest)
+python3
+```
+
 ```python
 # import the package
 from apollo.client import Apollo
 
 # sync data from your database instance
 # (we support supabase at the current moment or postgresql via uri format)
 Apollo.connect("postgres://username:password@hostname:port/database_name")
 
 # If you want to test out operation on your external connection
 Apollo.fetch_tables()
 Apollo.query("desc", "table", "column")
 ```
 
-...and create a workflow with a simple command:
+Test sending your content to our API!
 
-_Note: you can obtain a Auth token [here](https://docs.apolloapi.io/docs/api/authentication), sign up today on our [Site](https://app.apolloapi.io/)_
+...and create a workflow with a simple command:
 
 ```python
 # import the package
 from apollo.client import Apollo
 
 # Use our custom model to test building decisions
 Apollo.use("apollo", token="YOUR_API_TOKEN_HERE")
 
-# Lets check to see if a phrase contains threats
+# We support video, speech, image and text. Try text!
 Apollo.detectText("Phrase1", "contains", "Threats")
-
-# Create custom rules which creates a task!
-Apollo.rule('Phrase1', '>=', '0.8')
-
-# Connect with other models!
-Apollo.use('Google', "violence", ...)
-
-Apollo.detectImage('Image1', 'contains', 'VERY_LIKELY') # Image Analysis/OCR
-Apollo.detectSpeech('Audio1', 'contains', 'UNLIKELY') # Audio Processing
-Apollo.detectVideo('Video1', 'contains', 'POSSIBLE') # Video Analysis
-Apollo.detectText('Phrase1', 'contains', 'UNKNOWN') # Text Analysis
 ```
 
 That's all it takes!
 
-## Apollo then takes care of:
-
-- Detecting real-time changes in your data
-- Automating tasks against image, video, audio or text
-- Simplifying the process of deploying AI models
-- Making sure your integration is robust, so you never again have to worry about stuck/stale data or false-positives
-
-In practice, you probably want to use one of our native SDKs to interact with Apollo's API or use our custom browser client so you dont have to write code. If so, sign up at [Apollo API](https://app.apolloapi.io/signup)!
+That's all it takes! You can check out [more on our notion page](https://cloudguruab.notion.site/Apollo-e5e347745c1e43798d849d79cce90aba).
 
-## 🧑‍💻 Cool, what can I build with it?
-
-- Trust & Safety teams can use Apollo to **build native in-app connections** related to active response, content moderation, fraud detection, etc.
-- Some **automate their personal lives** with Apollo by integrating against discord communities or their personal lives
-- Apollo can help you **quickly automate tasks** for hobby projects, communities or business
+In practice, you probably want to use one of our native SDKs to interact with Apollo's API or use our custom browser client so you dont have to write code. If so, ping us at adrian@apolloapi.io!
 
 ## Contributing
 
 ### 📦 pre-commit config
 
 As an open source project, Apollo welcomes contributions from the community at large. This isn’t an exhaustive reference and is a living document subject to change as needed when the project formalizes any practice or pattern.
 
@@ -142,7 +155,11 @@
 
 ⭐ Follow our development by starring us here on GitHub ⭐
 
 - Share feedback or ask questions on the [Discord community](https://discord.gg/ZUH7f7AzUY)
 - [Chat with a member of the team](https://apolloapi.io) 👋
 - Check our [blog on Trust & Safety](https://www.thebriefnewsletter.com)
 - Look at our docs on how to get started [here!](https://apolloapi-doc.vercel.app/)
+
+## NOTES CLI TEST
+
+- set env variables for provider (openai) either in .env file or by exports
```

#### html2text {}

```diff
@@ -1,69 +1,72 @@
     ![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/
-                     6455b1fd3d8642575f793c94_header.png)
-                   ****** Open-source Task Automation ******
-   Apollo is an open-source no-code platform that helps you build automated
-workflows in minutes. Our SDK allows you to automate tasks such as; onboarding,
-    compliance, trust & safety, fraud detection, code generation and more.
+  643fffb82419ac18d39e3e4e_Screenshot%202023-04-19%20at%2010.50.13%20AM.png)
+    ****** The easiest way to build custom decision making workflows ******
+Apollo gives you access to custom machine learning models, no-code platform and
+ continuously syncs data from any API or Database to centralize investigations
+ and allow you to automate the detection of harm in images, videos, audio and
+                                     text.
 
                                    Docs_Â»
 
-             Join_the_waitlist Â· Report_Bug Â· Community_Discord
-## Why Apollo API? Before Apollo, integrating AI models and building automated
-workflows could be time-consuming and complex, with Apollo, teams can simplify
-and accelerate the process, making it easier to deploy AI models, sync data,
-and develop insights in minutes. ## ð Interesting, how can I try it? Lets
-install the SDK first... ```bash pip install apollo-sdk ``` Let's setup your
-first Integration! It will pull from your local database (and keep it in sync).
-```python # import the package from apollo.client import Apollo # sync data
-from your database instance # (we support supabase at the current moment or
-postgresql via uri format) Apollo.connect("postgres://username:
-password@hostname:port/database_name") # If you want to test out operation on
-your external connection Apollo.fetch_tables() Apollo.query("desc", "table",
-"column") ``` ...and create a workflow with a simple command: _Note: you can
-obtain a Auth token [here](https://docs.apolloapi.io/docs/api/authentication),
-sign up today on our [Site](https://app.apolloapi.io/)_ ```python # import the
+         Examples Join_the_waitlist Â· Report_Bug Â· Community_Discord
+## â­ Can you show me an example? In your code you can write: ```ts
+Apollo.connect('postgres://username:password@hostnam...', ...) // Starts
+syncing content forever! Apollo.use('OpenAI', "moderation", ...) // Connect to
+existing providers! Apollo.rule('Phrase1', '>=', '0.8') // Create custom rules!
+Apollo.use('Apollo', "violence", ...) // Connect with our internal models! /
+/ Detect bad actors at scale! Apollo.detectImage('Image1', 'contains',
+'VERY_LIKELY') // Image Analysis/OCR Apollo.detectSpeech('Audio1', 'contains',
+'UNLIKELY') // Audio Processing Apollo.detectVideo('Video1', 'contains',
+'POSSIBLE') // Video Analysis Apollo.detectText('Phrase1', 'contains',
+'UNKNOWN') // Text Analysis ``` Apollo then takes care of: - Detecting real-
+time changes in user experience - Automated detection against image, video,
+audio or text - Connecting policy to product - Making sure your integration is
+robust, so you never again have to worry about stuck/stale data or false-
+positives ## ð§âð» Cool, what can I build with it? - Trust & Safety teams
+in companies use Apollo to **build native in-app connections** related to
+active response, content moderation, fraud detection, etc. - Some **automate
+their personal lives** with Apollo by integrating against discord communities
+or other decentralized networks for safety - Apollo can help you **quickly
+build trust** for hobby projects, communities or business ## ð Interesting,
+how can I try it? Let's setup your first Integration in 2 minutes! It will pull
+from your local database (and keep it in sync). To start: ```bash # install the
+cli-toolkit pip install apollo-sdk # enter a python repl or create a python
+file, up to you! (repl is easiest) python3 ``` ```python # import the package
+from apollo.client import Apollo # sync data from your database instance # (we
+support supabase at the current moment or postgresql via uri format)
+Apollo.connect("postgres://username:password@hostname:port/database_name") # If
+you want to test out operation on your external connection Apollo.fetch_tables
+() Apollo.query("desc", "table", "column") ``` Test sending your content to our
+API! ...and create a workflow with a simple command: ```python # import the
 package from apollo.client import Apollo # Use our custom model to test
-building decisions Apollo.use("apollo", token="YOUR_API_TOKEN_HERE") # Lets
-check to see if a phrase contains threats Apollo.detectText("Phrase1",
-"contains", "Threats") # Create custom rules which creates a task! Apollo.rule
-('Phrase1', '>=', '0.8') # Connect with other models! Apollo.use('Google',
-"violence", ...) Apollo.detectImage('Image1', 'contains', 'VERY_LIKELY') #
-Image Analysis/OCR Apollo.detectSpeech('Audio1', 'contains', 'UNLIKELY') #
-Audio Processing Apollo.detectVideo('Video1', 'contains', 'POSSIBLE') # Video
-Analysis Apollo.detectText('Phrase1', 'contains', 'UNKNOWN') # Text Analysis
-``` That's all it takes! ## Apollo then takes care of: - Detecting real-time
-changes in your data - Automating tasks against image, video, audio or text -
-Simplifying the process of deploying AI models - Making sure your integration
-is robust, so you never again have to worry about stuck/stale data or false-
-positives In practice, you probably want to use one of our native SDKs to
-interact with Apollo's API or use our custom browser client so you dont have to
-write code. If so, sign up at [Apollo API](https://app.apolloapi.io/signup)! ##
-ð§âð» Cool, what can I build with it? - Trust & Safety teams can use
-Apollo to **build native in-app connections** related to active response,
-content moderation, fraud detection, etc. - Some **automate their personal
-lives** with Apollo by integrating against discord communities or their
-personal lives - Apollo can help you **quickly automate tasks** for hobby
-projects, communities or business ## Contributing ### ð¦ pre-commit config As
-an open source project, Apollo welcomes contributions from the community at
-large. This isnât an exhaustive reference and is a living document subject to
-change as needed when the project formalizes any practice or pattern. Clone the
-repo and start Apollo locally... ```bash git clone https://github.com/
-apolloapi/apolloapi.git cd apolloapi && python3 -m venv env && source env/bin/
-activate && pip install -r requirements.txt ``` - After installing system
-dependencies be sure to install pre-commit for lint checks ```bash pip install
-pre-commit pre-commit install pre-commit run --all-files ``` Apollo uses commit
-messages for automated generation of project changelog. For every pull request
-we request contributors to be compliant with the following commit message
-notation. ``` :
+building decisions Apollo.use("apollo", token="YOUR_API_TOKEN_HERE") # We
+support video, speech, image and text. Try text! Apollo.detectText("Phrase1",
+"contains", "Threats") ``` That's all it takes! That's all it takes! You can
+check out [more on our notion page](https://cloudguruab.notion.site/Apollo-
+e5e347745c1e43798d849d79cce90aba). In practice, you probably want to use one of
+our native SDKs to interact with Apollo's API or use our custom browser client
+so you dont have to write code. If so, ping us at adrian@apolloapi.io! ##
+Contributing ### ð¦ pre-commit config As an open source project, Apollo
+welcomes contributions from the community at large. This isnât an exhaustive
+reference and is a living document subject to change as needed when the project
+formalizes any practice or pattern. Clone the repo and start Apollo locally...
+```bash git clone https://github.com/apolloapi/apolloapi.git cd apolloapi &&
+python3 -m venv env && source env/bin/activate && pip install -
+r requirements.txt ``` - After installing system dependencies be sure to
+install pre-commit for lint checks ```bash pip install pre-commit pre-commit
+install pre-commit run --all-files ``` Apollo uses commit messages for
+automated generation of project changelog. For every pull request we request
+contributors to be compliant with the following commit message notation. ``` :
 ``` Accepted `` values: - new = newly implemented user-facing features - chg =
 changes in existing user-facing features - fix = user-facing bugfixes - oth =
 other changes which users should know about - dev = any developer-facing
 changes, regardless of new/chg/fix status #### Summary (The first line) The
 first line should not be longer than 75 characters, the second line is always
 blank and other lines should be wrapped at 80 characters. ## ð Neat, I would
 like to learn more â­ Follow our development by starring us here on GitHub â­
 - Share feedback or ask questions on the [Discord community](https://
 discord.gg/ZUH7f7AzUY) - [Chat with a member of the team](https://apolloapi.io)
 ð - Check our [blog on Trust & Safety](https://www.thebriefnewsletter.com) -
 Look at our docs on how to get started [here!](https://apolloapi-
-doc.vercel.app/)
+doc.vercel.app/) ## NOTES CLI TEST - set env variables for provider (openai)
+either in .env file or by exports
```

### Comparing `apollo-sdk-0.1.6/apollo/__init__.py` & `apollo-sdk-0.2.0/apollo/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,27 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
+import importlib
+
 from apollo.database.supabase.base import AbstractSupabaseClient
 from apollo.database.firebase.base import AbstractFirebaseClient
 from apollo.service.json.base import AbstractRestClient
-from .const import SUPABASE_CLIENT_CLASS, FIREBASE_CLIENT_CLASS, REST_CLIENT_CLASS
+from apollo.connectors.openai.base import AbstractOpenAIProvider
+
+from .const import (
+    SUPABASE_CLIENT_CLASS,
+    FIREBASE_CLIENT_CLASS,
+    REST_CLIENT_CLASS,
+    OPENAI_CLIENT_CLASS,
+)
 
 from django.utils.module_loading import import_string
 
 
 def get_supabase_client(connection_string) -> AbstractSupabaseClient:
     client = import_string(SUPABASE_CLIENT_CLASS)
     return client(connection_string)
@@ -30,7 +39,25 @@
     client = import_string(FIREBASE_CLIENT_CLASS)
     return client(service_account_key)
 
 
 def get_json_client(api_key) -> AbstractRestClient:
     client = import_string(REST_CLIENT_CLASS)
     return client(api_key)
+
+
+def get_openai_client(provider_path: str) -> AbstractOpenAIProvider:
+    client = import_string(OPENAI_CLIENT_CLASS)
+    if provider_path.startswith("openai:"):
+        path_parts = provider_path.split(":")
+        model_name = path_parts[0]
+        model_type = path_parts[1]
+        if model_type == "chat":
+            print(f"Connected to {provider_path}")
+            return client("gpt-3.5-turbo")
+        elif model_type == "completion":
+            print(f"Connected to {provider_path}")
+            return client("text-davinci-003")
+        else:
+            raise ValueError(f"Unknown OpenAI model type: {model_type}")
+    else:
+        return importlib.import_module(provider_path).default()
```

### Comparing `apollo-sdk-0.1.6/apollo/connectors/__init__.py` & `apollo-sdk-0.2.0/apollo/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/connectors/aws/__init__.py` & `apollo-sdk-0.2.0/apollo/connectors/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/connectors/google/__init__.py` & `apollo-sdk-0.2.0/apollo/connectors/google/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/connectors/microsoft/__init__.py` & `apollo-sdk-0.2.0/apollo/connectors/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/connectors/openai/__init__.py` & `apollo-sdk-0.2.0/apollo/database/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/const.py` & `apollo-sdk-0.2.0/apollo/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,19 @@
 )
 
 # Service client
 REST_CLIENT_CLASS = os.environ.get(
     "REST_CLIENT_CLASS", "apollo.service.json.RestClient"
 )
 
+# OPENAI Provider
+OPENAI_CLIENT_CLASS = os.environ.get(
+    "OPENAI_CLIENT_CLASS", "apollo.connectors.openai.OpenAiGenericProvider"
+)
+
 # Hard code sql queries to prevent injection
 QUERY_CONTEXT = {
     "asc": "",
     "desc": "",
     "all_tables": "select table_name from information_schema.tables where table_schema='public'",
 }
```

### Comparing `apollo-sdk-0.1.6/apollo/database/__init__.py` & `apollo-sdk-0.2.0/apollo/database/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/database/firebase/__init__.py` & `apollo-sdk-0.2.0/apollo/database/firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/database/firebase/base.py` & `apollo-sdk-0.2.0/apollo/database/firebase/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/database/firebase/cloud.py` & `apollo-sdk-0.2.0/apollo/database/firebase/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/database/firebase/local.py` & `apollo-sdk-0.2.0/apollo/database/firebase/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/database/mongo/__init__.py` & `apollo-sdk-0.2.0/apollo/database/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/database/mysql/__init__.py` & `apollo-sdk-0.2.0/apollo/database/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/database/postgres/__init__.py` & `apollo-sdk-0.2.0/apollo/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/database/supabase/__init__.py` & `apollo-sdk-0.2.0/apollo/database/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/database/supabase/base.py` & `apollo-sdk-0.2.0/apollo/database/supabase/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/database/supabase/cloud.py` & `apollo-sdk-0.2.0/apollo/database/supabase/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/database/supabase/local.py` & `apollo-sdk-0.2.0/apollo/database/supabase/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/exceptions.py` & `apollo-sdk-0.2.0/apollo/exceptions.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/manager.py` & `apollo-sdk-0.2.0/apollo/manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-from apollo import get_supabase_client, get_firebase_client, get_json_client
+from apollo import (
+    get_supabase_client,
+    get_firebase_client,
+    get_json_client,
+    get_openai_client,
+)
 from apollo.exceptions import EmptyResultsWarning
 
 
 class PostgresConnectionManager:
     @staticmethod
     def connect_to_prefix(uri):
         return get_supabase_client(uri)
@@ -41,7 +46,13 @@
         return get_firebase_client(service_account_key)
 
 
 class JSONConnectionManager:
     @staticmethod
     def connect(api_key):
         return get_json_client(api_key)
+
+
+class OpenAIConnectionManager:
+    @staticmethod
+    def load_openai_provider(provider_path: str):
+        return get_openai_client(provider_path)
```

### Comparing `apollo-sdk-0.1.6/apollo/resource.py` & `apollo-sdk-0.2.0/apollo/resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from apollo.manager import (
     PostgresConnectionManager,
     FirebaseConnectionManager,
     JSONConnectionManager,
+    OpenAIConnectionManager,
 )
 from apollo.const import QUERY_CONTEXT
 
 
 class Postgres:
 
     # Specific sql queries
@@ -33,20 +34,29 @@
     psql_curs = None
 
 
 class Firebase:
     pass
 
 
-class JSON:
+class JSONService:
 
     # Service utility class
     _service_manager = JSONConnectionManager()
 
     # Token
     _auth_token = None
 
 
-class General(Postgres, JSON):
+class OpenAI:
+
+    # connection manager
+    _openai_manager = OpenAIConnectionManager()
+
+    # model type definition
+    _provider_path = None
+
+
+class General(Postgres, JSONService, OpenAI):
 
     # Current LLM to be used
     model = None
```

### Comparing `apollo-sdk-0.1.6/apollo/service/__init__.py` & `apollo-sdk-0.2.0/apollo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/service/graphql/__init__.py` & `apollo-sdk-0.2.0/apollo/service/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/service/json/__init__.py` & `apollo-sdk-0.2.0/apollo/service/json/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo/service/json/base.py` & `apollo-sdk-0.2.0/apollo/service/json/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,7 +16,11 @@
 
 class AbstractRestClient:
     def make_http_request(self, body, header, endpoint):
         return NotImplementedError
 
     def make_https_request(self, body, header, endpoint):
         return NotImplementedError
+
+    # general request module
+    def call_api(self):
+        raise NotImplementedError
```

### Comparing `apollo-sdk-0.1.6/apollo/service/json/cloud.py` & `apollo-sdk-0.2.0/apollo/service/json/cloud.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     def __init__(self, api_key):
         self.api_key = api_key
 
     @staticmethod
     def make_http_request():
         return None
 
+    @staticmethod
+    def call_api(self):
+        return None
+
     def make_https_request(self, body):
         response = requests.post(
             "https://api.apolloapi.io/api/v1/apollo/",
             headers={"Authorization": f"Token {self.api_key}"},
             json=body,
             timeout=10,
         )
```

### Comparing `apollo-sdk-0.1.6/apollo/service/json/local.py` & `apollo-sdk-0.2.0/apollo/service/json/local.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,7 +18,10 @@
 
 class FakeRestClient(AbstractRestClient):
     def make_http_request(self, body, header, endpoint):
         pass
 
     def make_https_request(self, body, header, endpoint):
         pass
+
+    def call_api(self):
+        pass
```

### Comparing `apollo-sdk-0.1.6/apollo/tests/__init__.py` & `apollo-sdk-0.2.0/apollo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.6/apollo_sdk.egg-info/PKG-INFO` & `apollo-sdk-0.2.0/apollo_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,120 +1,130 @@
 Metadata-Version: 2.1
 Name: apollo-sdk
-Version: 0.1.6
+Version: 0.2.0
 Summary: Build automated decision making workflows by aggregating your AI models and data into one api.
 Home-page: https://github.com/apolloapi/apolloapi
-Author: Apollo API, Inc.
+Author: Apollo API
 Author-email: adrbrownx@gmail.com
 License: Elastic License v2
-Classifier: Intended Audience :: Developers
+Platform: Any
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
-![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/6455b1fd3d8642575f793c94_header.png)
+![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/643fffb82419ac18d39e3e4e_Screenshot%202023-04-19%20at%2010.50.13%20AM.png)
 
 </div>
 
-<h1 align="center">Open-source Task Automation</h1>
+<h1 align="center">The easiest way to build custom decision making workflows</h1>
 
 <div align="center">
-Apollo is an open-source no-code platform that helps you build automated workflows in minutes. Our SDK allows you to automate tasks such as; onboarding, compliance, trust & safety, fraud detection, code generation and more.
+Apollo gives you access to custom machine learning models, no-code platform and continuously syncs data from any API or Database to centralize investigations and allow you to automate the detection of harm in images, videos, audio and text.
 </div>
 
 <p align="center">
     <br />
-    <a href="https://docs.apolloapi.io/" rel="dofollow"><strong>Docs »</strong></a>
+    <a href="https://apolloapi-doc.vercel.app/" rel="dofollow"><strong>Docs »</strong></a>
     <br />
 
   <br/>
+    <a href="https://apolloapi-doc.vercel.app/">Examples</a>
     <a href="https://www.apolloapi.io/">Join the waitlist</a>
     ·
     <a href="https://github.com/apolloapi/apolloapi/issues">Report Bug</a>
     ·
     <a href="https://discord.gg/ZUH7f7AzUY">Community Discord</a>
 </p>
 
-## Why Apollo API?
+## ⭐ Can you show me an example?
 
-Before Apollo, integrating AI models and building automated workflows could be time-consuming and complex, with Apollo, teams can simplify and accelerate the process, making it easier to deploy AI models, sync data, and develop insights in minutes.
+In your code you can write:
 
-## 🚀 Interesting, how can I try it?
+```ts
+Apollo.connect('postgres://username:password@hostnam...', ...) // Starts syncing content forever!
 
-Lets install the SDK first...
+Apollo.use('OpenAI', "moderation", ...) // Connect to existing providers!
+
+Apollo.rule('Phrase1', '>=', '0.8') // Create custom rules!
+
+Apollo.use('Apollo', "violence", ...) // Connect with our internal models!
+
+// Detect bad actors at scale!
+Apollo.detectImage('Image1', 'contains', 'VERY_LIKELY') // Image Analysis/OCR
+Apollo.detectSpeech('Audio1', 'contains', 'UNLIKELY') // Audio Processing
+Apollo.detectVideo('Video1', 'contains', 'POSSIBLE') // Video Analysis
+Apollo.detectText('Phrase1', 'contains', 'UNKNOWN') // Text Analysis
 
-```bash
-pip install apollo-sdk
 ```
 
-Let's setup your first Integration!
+Apollo then takes care of:
+
+- Detecting real-time changes in user experience
+- Automated detection against image, video, audio or text
+- Connecting policy to product
+- Making sure your integration is robust, so you never again have to worry about stuck/stale data or false-positives
+
+## 🧑‍💻 Cool, what can I build with it?
+
+- Trust & Safety teams in companies use Apollo to **build native in-app connections** related to active response, content moderation, fraud detection, etc.
+- Some **automate their personal lives** with Apollo by integrating against discord communities or other decentralized networks for safety
+- Apollo can help you **quickly build trust** for hobby projects, communities or business
+
+## 🚀 Interesting, how can I try it?
+
+Let's setup your first Integration in 2 minutes!
 
 It will pull from your local database (and keep it in sync).
 
+To start:
+
+```bash
+# install the cli-toolkit
+pip install apollo-sdk
+
+# enter a python repl or create a python file, up to you! (repl is easiest)
+python3
+```
+
 ```python
 # import the package
 from apollo.client import Apollo
 
 # sync data from your database instance
 # (we support supabase at the current moment or postgresql via uri format)
 Apollo.connect("postgres://username:password@hostname:port/database_name")
 
 # If you want to test out operation on your external connection
 Apollo.fetch_tables()
 Apollo.query("desc", "table", "column")
 ```
 
-...and create a workflow with a simple command:
+Test sending your content to our API!
 
-_Note: you can obtain a Auth token [here](https://docs.apolloapi.io/docs/api/authentication), sign up today on our [Site](https://app.apolloapi.io/)_
+...and create a workflow with a simple command:
 
 ```python
 # import the package
 from apollo.client import Apollo
 
 # Use our custom model to test building decisions
 Apollo.use("apollo", token="YOUR_API_TOKEN_HERE")
 
-# Lets check to see if a phrase contains threats
+# We support video, speech, image and text. Try text!
 Apollo.detectText("Phrase1", "contains", "Threats")
-
-# Create custom rules which creates a task!
-Apollo.rule('Phrase1', '>=', '0.8')
-
-# Connect with other models!
-Apollo.use('Google', "violence", ...)
-
-Apollo.detectImage('Image1', 'contains', 'VERY_LIKELY') # Image Analysis/OCR
-Apollo.detectSpeech('Audio1', 'contains', 'UNLIKELY') # Audio Processing
-Apollo.detectVideo('Video1', 'contains', 'POSSIBLE') # Video Analysis
-Apollo.detectText('Phrase1', 'contains', 'UNKNOWN') # Text Analysis
 ```
 
 That's all it takes!
 
-## Apollo then takes care of:
-
-- Detecting real-time changes in your data
-- Automating tasks against image, video, audio or text
-- Simplifying the process of deploying AI models
-- Making sure your integration is robust, so you never again have to worry about stuck/stale data or false-positives
-
-In practice, you probably want to use one of our native SDKs to interact with Apollo's API or use our custom browser client so you dont have to write code. If so, sign up at [Apollo API](https://app.apolloapi.io/signup)!
+That's all it takes! You can check out [more on our notion page](https://cloudguruab.notion.site/Apollo-e5e347745c1e43798d849d79cce90aba).
 
-## 🧑‍💻 Cool, what can I build with it?
-
-- Trust & Safety teams can use Apollo to **build native in-app connections** related to active response, content moderation, fraud detection, etc.
-- Some **automate their personal lives** with Apollo by integrating against discord communities or their personal lives
-- Apollo can help you **quickly automate tasks** for hobby projects, communities or business
+In practice, you probably want to use one of our native SDKs to interact with Apollo's API or use our custom browser client so you dont have to write code. If so, ping us at adrian@apolloapi.io!
 
 ## Contributing
 
 ### 📦 pre-commit config
 
 As an open source project, Apollo welcomes contributions from the community at large. This isn’t an exhaustive reference and is a living document subject to change as needed when the project formalizes any practice or pattern.
 
@@ -159,7 +169,11 @@
 
 ⭐ Follow our development by starring us here on GitHub ⭐
 
 - Share feedback or ask questions on the [Discord community](https://discord.gg/ZUH7f7AzUY)
 - [Chat with a member of the team](https://apolloapi.io) 👋
 - Check our [blog on Trust & Safety](https://www.thebriefnewsletter.com)
 - Look at our docs on how to get started [here!](https://apolloapi-doc.vercel.app/)
+
+## NOTES CLI TEST
+
+- set env variables for provider (openai) either in .env file or by exports
```

#### html2text {}

```diff
@@ -1,78 +1,78 @@
-Metadata-Version: 2.1 Name: apollo-sdk Version: 0.1.6 Summary: Build automated
+Metadata-Version: 2.1 Name: apollo-sdk Version: 0.2.0 Summary: Build automated
 decision making workflows by aggregating your AI models and data into one api.
-Home-page: https://github.com/apolloapi/apolloapi Author: Apollo API, Inc.
-Author-email: adrbrownx@gmail.com License: Elastic License v2 Classifier:
-Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
-text/markdown License-File: LICENSE
+Home-page: https://github.com/apolloapi/apolloapi Author: Apollo API Author-
+email: adrbrownx@gmail.com License: Elastic License v2 Platform: Any
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Description-Content-Type: text/markdown License-File: LICENSE
     ![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/
-                     6455b1fd3d8642575f793c94_header.png)
-                   ****** Open-source Task Automation ******
-   Apollo is an open-source no-code platform that helps you build automated
-workflows in minutes. Our SDK allows you to automate tasks such as; onboarding,
-    compliance, trust & safety, fraud detection, code generation and more.
+  643fffb82419ac18d39e3e4e_Screenshot%202023-04-19%20at%2010.50.13%20AM.png)
+    ****** The easiest way to build custom decision making workflows ******
+Apollo gives you access to custom machine learning models, no-code platform and
+ continuously syncs data from any API or Database to centralize investigations
+ and allow you to automate the detection of harm in images, videos, audio and
+                                     text.
 
                                    Docs_Â»
 
-             Join_the_waitlist Â· Report_Bug Â· Community_Discord
-## Why Apollo API? Before Apollo, integrating AI models and building automated
-workflows could be time-consuming and complex, with Apollo, teams can simplify
-and accelerate the process, making it easier to deploy AI models, sync data,
-and develop insights in minutes. ## ð Interesting, how can I try it? Lets
-install the SDK first... ```bash pip install apollo-sdk ``` Let's setup your
-first Integration! It will pull from your local database (and keep it in sync).
-```python # import the package from apollo.client import Apollo # sync data
-from your database instance # (we support supabase at the current moment or
-postgresql via uri format) Apollo.connect("postgres://username:
-password@hostname:port/database_name") # If you want to test out operation on
-your external connection Apollo.fetch_tables() Apollo.query("desc", "table",
-"column") ``` ...and create a workflow with a simple command: _Note: you can
-obtain a Auth token [here](https://docs.apolloapi.io/docs/api/authentication),
-sign up today on our [Site](https://app.apolloapi.io/)_ ```python # import the
+         Examples Join_the_waitlist Â· Report_Bug Â· Community_Discord
+## â­ Can you show me an example? In your code you can write: ```ts
+Apollo.connect('postgres://username:password@hostnam...', ...) // Starts
+syncing content forever! Apollo.use('OpenAI', "moderation", ...) // Connect to
+existing providers! Apollo.rule('Phrase1', '>=', '0.8') // Create custom rules!
+Apollo.use('Apollo', "violence", ...) // Connect with our internal models! /
+/ Detect bad actors at scale! Apollo.detectImage('Image1', 'contains',
+'VERY_LIKELY') // Image Analysis/OCR Apollo.detectSpeech('Audio1', 'contains',
+'UNLIKELY') // Audio Processing Apollo.detectVideo('Video1', 'contains',
+'POSSIBLE') // Video Analysis Apollo.detectText('Phrase1', 'contains',
+'UNKNOWN') // Text Analysis ``` Apollo then takes care of: - Detecting real-
+time changes in user experience - Automated detection against image, video,
+audio or text - Connecting policy to product - Making sure your integration is
+robust, so you never again have to worry about stuck/stale data or false-
+positives ## ð§âð» Cool, what can I build with it? - Trust & Safety teams
+in companies use Apollo to **build native in-app connections** related to
+active response, content moderation, fraud detection, etc. - Some **automate
+their personal lives** with Apollo by integrating against discord communities
+or other decentralized networks for safety - Apollo can help you **quickly
+build trust** for hobby projects, communities or business ## ð Interesting,
+how can I try it? Let's setup your first Integration in 2 minutes! It will pull
+from your local database (and keep it in sync). To start: ```bash # install the
+cli-toolkit pip install apollo-sdk # enter a python repl or create a python
+file, up to you! (repl is easiest) python3 ``` ```python # import the package
+from apollo.client import Apollo # sync data from your database instance # (we
+support supabase at the current moment or postgresql via uri format)
+Apollo.connect("postgres://username:password@hostname:port/database_name") # If
+you want to test out operation on your external connection Apollo.fetch_tables
+() Apollo.query("desc", "table", "column") ``` Test sending your content to our
+API! ...and create a workflow with a simple command: ```python # import the
 package from apollo.client import Apollo # Use our custom model to test
-building decisions Apollo.use("apollo", token="YOUR_API_TOKEN_HERE") # Lets
-check to see if a phrase contains threats Apollo.detectText("Phrase1",
-"contains", "Threats") # Create custom rules which creates a task! Apollo.rule
-('Phrase1', '>=', '0.8') # Connect with other models! Apollo.use('Google',
-"violence", ...) Apollo.detectImage('Image1', 'contains', 'VERY_LIKELY') #
-Image Analysis/OCR Apollo.detectSpeech('Audio1', 'contains', 'UNLIKELY') #
-Audio Processing Apollo.detectVideo('Video1', 'contains', 'POSSIBLE') # Video
-Analysis Apollo.detectText('Phrase1', 'contains', 'UNKNOWN') # Text Analysis
-``` That's all it takes! ## Apollo then takes care of: - Detecting real-time
-changes in your data - Automating tasks against image, video, audio or text -
-Simplifying the process of deploying AI models - Making sure your integration
-is robust, so you never again have to worry about stuck/stale data or false-
-positives In practice, you probably want to use one of our native SDKs to
-interact with Apollo's API or use our custom browser client so you dont have to
-write code. If so, sign up at [Apollo API](https://app.apolloapi.io/signup)! ##
-ð§âð» Cool, what can I build with it? - Trust & Safety teams can use
-Apollo to **build native in-app connections** related to active response,
-content moderation, fraud detection, etc. - Some **automate their personal
-lives** with Apollo by integrating against discord communities or their
-personal lives - Apollo can help you **quickly automate tasks** for hobby
-projects, communities or business ## Contributing ### ð¦ pre-commit config As
-an open source project, Apollo welcomes contributions from the community at
-large. This isnât an exhaustive reference and is a living document subject to
-change as needed when the project formalizes any practice or pattern. Clone the
-repo and start Apollo locally... ```bash git clone https://github.com/
-apolloapi/apolloapi.git cd apolloapi && python3 -m venv env && source env/bin/
-activate && pip install -r requirements.txt ``` - After installing system
-dependencies be sure to install pre-commit for lint checks ```bash pip install
-pre-commit pre-commit install pre-commit run --all-files ``` Apollo uses commit
-messages for automated generation of project changelog. For every pull request
-we request contributors to be compliant with the following commit message
-notation. ``` :
+building decisions Apollo.use("apollo", token="YOUR_API_TOKEN_HERE") # We
+support video, speech, image and text. Try text! Apollo.detectText("Phrase1",
+"contains", "Threats") ``` That's all it takes! That's all it takes! You can
+check out [more on our notion page](https://cloudguruab.notion.site/Apollo-
+e5e347745c1e43798d849d79cce90aba). In practice, you probably want to use one of
+our native SDKs to interact with Apollo's API or use our custom browser client
+so you dont have to write code. If so, ping us at adrian@apolloapi.io! ##
+Contributing ### ð¦ pre-commit config As an open source project, Apollo
+welcomes contributions from the community at large. This isnât an exhaustive
+reference and is a living document subject to change as needed when the project
+formalizes any practice or pattern. Clone the repo and start Apollo locally...
+```bash git clone https://github.com/apolloapi/apolloapi.git cd apolloapi &&
+python3 -m venv env && source env/bin/activate && pip install -
+r requirements.txt ``` - After installing system dependencies be sure to
+install pre-commit for lint checks ```bash pip install pre-commit pre-commit
+install pre-commit run --all-files ``` Apollo uses commit messages for
+automated generation of project changelog. For every pull request we request
+contributors to be compliant with the following commit message notation. ``` :
 ``` Accepted `` values: - new = newly implemented user-facing features - chg =
 changes in existing user-facing features - fix = user-facing bugfixes - oth =
 other changes which users should know about - dev = any developer-facing
 changes, regardless of new/chg/fix status #### Summary (The first line) The
 first line should not be longer than 75 characters, the second line is always
 blank and other lines should be wrapped at 80 characters. ## ð Neat, I would
 like to learn more â­ Follow our development by starring us here on GitHub â­
 - Share feedback or ask questions on the [Discord community](https://
 discord.gg/ZUH7f7AzUY) - [Chat with a member of the team](https://apolloapi.io)
 ð - Check our [blog on Trust & Safety](https://www.thebriefnewsletter.com) -
 Look at our docs on how to get started [here!](https://apolloapi-
-doc.vercel.app/)
+doc.vercel.app/) ## NOTES CLI TEST - set env variables for provider (openai)
+either in .env file or by exports
```

### Comparing `apollo-sdk-0.1.6/apollo_sdk.egg-info/SOURCES.txt` & `apollo-sdk-0.2.0/apollo_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,26 +9,32 @@
 apollo/manager.py
 apollo/resource.py
 apollo/connectors/__init__.py
 apollo/connectors/aws/__init__.py
 apollo/connectors/google/__init__.py
 apollo/connectors/microsoft/__init__.py
 apollo/connectors/openai/__init__.py
+apollo/connectors/openai/base.py
+apollo/connectors/openai/cloud.py
+apollo/connectors/openai/local.py
 apollo/database/__init__.py
 apollo/database/firebase/__init__.py
 apollo/database/firebase/base.py
 apollo/database/firebase/cloud.py
 apollo/database/firebase/local.py
 apollo/database/mongo/__init__.py
 apollo/database/mysql/__init__.py
 apollo/database/postgres/__init__.py
 apollo/database/supabase/__init__.py
 apollo/database/supabase/base.py
 apollo/database/supabase/cloud.py
 apollo/database/supabase/local.py
+apollo/plugins/__init__.py
+apollo/plugins/utils.py
+apollo/plugins/validation.py
 apollo/service/__init__.py
 apollo/service/graphql/__init__.py
 apollo/service/json/__init__.py
 apollo/service/json/base.py
 apollo/service/json/cloud.py
 apollo/service/json/local.py
 apollo/tests/__init__.py
```

### Comparing `apollo-sdk-0.1.6/setup.py` & `apollo-sdk-0.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,50 +11,36 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from setuptools import setup, find_packages
-from pathlib import Path
-this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
+
+with open("README.md", encoding="utf-8") as f:
+    long_description = f.read()
+    
+with open("requirements.txt") as f:
+    requirements = f.read().splitlines()
 
 setup(
     name="apollo-sdk",
-    version="0.1.6",
+    version="0.2.0",
     description="Build automated decision making workflows by aggregating your AI models and data into one api.",
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author="Apollo API, Inc.",
+    author="Apollo API",
     author_email="adrbrownx@gmail.com",
-    packages=find_packages(),
+    packages=find_packages(exclude=("scripts")),
     # package_dir={'': ''},
     url="https://github.com/apolloapi/apolloapi",
     license="Elastic License v2",
-    install_requires=[
-        "Django==4.1.2",
-        "firebase-admin==6.1.0",
-        "grpcio==1.53.0",
-        "httplib2==0.21.0",
-        "protobuf==4.22.3",
-        "psycopg2-binary==2.9.6",
-        "python-dotenv==1.0.0",
-        "psycopg==3.1.6",
-        "requests==2.28.1",
-        "psycopg2==2.9.3",
-        "pytest==7.2.0",
-        "PyJWT==2.6.0",
-        "requests==2.28.1",
-        "six==1.16.0",
-        "sqlparse==0.4.3",
-        "urllib3==1.26.13",
-    ],
     classifiers=[
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3"
     ],
+    platforms=["Any"],
+    scripts=[],
+    provides=[],
+    install_requires=requirements,
+    long_description_content_type="text/markdown",
+    long_description=long_description,
+    # entry_points={"console_scripts": ["apolloapi=apolloapi"]},
 )
```

