# Comparing `tmp/apollo-sdk-0.2.4.tar.gz` & `tmp/apollo-sdk-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-sdk-0.2.4.tar", last modified: Sat May 27 07:14:26 2023, max compression
+gzip compressed data, was "apollo-sdk-0.2.8.tar", last modified: Sat May 27 07:48:49 2023, max compression
```

## Comparing `apollo-sdk-0.2.4.tar` & `apollo-sdk-0.2.8.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.251846 apollo-sdk-0.2.4/
--rw-r--r--   0 abpyguru   (501) staff       (20)     3793 2023-04-29 17:42:09.000000 apollo-sdk-0.2.4/LICENSE
--rw-r--r--   0 abpyguru   (501) staff       (20)     6096 2023-05-27 07:14:26.251933 apollo-sdk-0.2.4/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     5635 2023-05-26 15:53:50.000000 apollo-sdk-0.2.4/README.md
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.245193 apollo-sdk-0.2.4/apollo/
--rw-r--r--   0 abpyguru   (501) staff       (20)     2250 2023-05-27 05:36:11.000000 apollo-sdk-0.2.4/apollo/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     5275 2023-05-27 05:36:10.000000 apollo-sdk-0.2.4/apollo/client.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.245496 apollo-sdk-0.2.4/apollo/connectors/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/connectors/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.245999 apollo-sdk-0.2.4/apollo/connectors/aws/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/connectors/aws/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.246299 apollo-sdk-0.2.4/apollo/connectors/google/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/connectors/google/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.246517 apollo-sdk-0.2.4/apollo/connectors/microsoft/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/connectors/microsoft/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.247245 apollo-sdk-0.2.4/apollo/connectors/openai/
--rw-r--r--   0 abpyguru   (501) staff       (20)      801 2023-05-26 16:56:46.000000 apollo-sdk-0.2.4/apollo/connectors/openai/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1023 2023-05-27 05:36:11.000000 apollo-sdk-0.2.4/apollo/connectors/openai/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2574 2023-05-27 05:36:11.000000 apollo-sdk-0.2.4/apollo/connectors/openai/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      956 2023-05-27 05:36:11.000000 apollo-sdk-0.2.4/apollo/connectors/openai/local.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1585 2023-05-26 17:12:47.000000 apollo-sdk-0.2.4/apollo/const.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.247392 apollo-sdk-0.2.4/apollo/database/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/database/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.247944 apollo-sdk-0.2.4/apollo/database/firebase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/database/firebase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/database/firebase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     3494 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/database/firebase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1438 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/database/firebase/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.248080 apollo-sdk-0.2.4/apollo/database/mongo/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/database/mongo/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.248215 apollo-sdk-0.2.4/apollo/database/mysql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/database/mysql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.248352 apollo-sdk-0.2.4/apollo/database/postgres/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/database/postgres/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.248898 apollo-sdk-0.2.4/apollo/database/supabase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/database/supabase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      739 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/database/supabase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1553 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/database/supabase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      810 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/database/supabase/local.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4197 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/exceptions.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1578 2023-05-27 05:36:11.000000 apollo-sdk-0.2.4/apollo/manager.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.249549 apollo-sdk-0.2.4/apollo/plugins/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-05-26 17:55:34.000000 apollo-sdk-0.2.4/apollo/plugins/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4796 2023-05-27 05:36:11.000000 apollo-sdk-0.2.4/apollo/plugins/utils.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     5165 2023-05-27 05:36:11.000000 apollo-sdk-0.2.4/apollo/plugins/validation.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1426 2023-05-27 05:36:10.000000 apollo-sdk-0.2.4/apollo/resource.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.249900 apollo-sdk-0.2.4/apollo/service/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/service/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.250069 apollo-sdk-0.2.4/apollo/service/graphql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/service/graphql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.250691 apollo-sdk-0.2.4/apollo/service/json/
--rw-r--r--   0 abpyguru   (501) staff       (20)      754 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/service/json/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      947 2023-05-27 05:36:11.000000 apollo-sdk-0.2.4/apollo/service/json/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1272 2023-05-27 05:36:10.000000 apollo-sdk-0.2.4/apollo/service/json/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      926 2023-05-27 05:36:10.000000 apollo-sdk-0.2.4/apollo/service/json/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.250936 apollo-sdk-0.2.4/apollo/tests/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.4/apollo/tests/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:14:26.251737 apollo-sdk-0.2.4/apollo_sdk.egg-info/
--rw-r--r--   0 abpyguru   (501) staff       (20)     6096 2023-05-27 07:14:26.000000 apollo-sdk-0.2.4/apollo_sdk.egg-info/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     1325 2023-05-27 07:14:26.000000 apollo-sdk-0.2.4/apollo_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-05-27 07:14:26.000000 apollo-sdk-0.2.4/apollo_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       53 2023-05-27 07:14:26.000000 apollo-sdk-0.2.4/apollo_sdk.egg-info/entry_points.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)     1798 2023-05-27 07:14:26.000000 apollo-sdk-0.2.4/apollo_sdk.egg-info/requires.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)        7 2023-05-27 07:14:26.000000 apollo-sdk-0.2.4/apollo_sdk.egg-info/top_level.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)      103 2023-05-27 07:14:26.252148 apollo-sdk-0.2.4/setup.cfg
--rw-r--r--   0 abpyguru   (501) staff       (20)     1623 2023-05-27 07:14:10.000000 apollo-sdk-0.2.4/setup.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.372126 apollo-sdk-0.2.8/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3793 2023-04-29 17:42:09.000000 apollo-sdk-0.2.8/LICENSE
+-rw-r--r--   0 abpyguru   (501) staff       (20)     6096 2023-05-27 07:48:49.371992 apollo-sdk-0.2.8/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5635 2023-05-26 15:53:50.000000 apollo-sdk-0.2.8/README.md
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.364799 apollo-sdk-0.2.8/apollo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2250 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5275 2023-05-27 05:36:10.000000 apollo-sdk-0.2.8/apollo/client.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.365069 apollo-sdk-0.2.8/apollo/connectors/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/connectors/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.365462 apollo-sdk-0.2.8/apollo/connectors/aws/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/connectors/aws/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.365687 apollo-sdk-0.2.8/apollo/connectors/google/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/connectors/google/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.365933 apollo-sdk-0.2.8/apollo/connectors/microsoft/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/connectors/microsoft/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.366848 apollo-sdk-0.2.8/apollo/connectors/openai/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      801 2023-05-26 16:56:46.000000 apollo-sdk-0.2.8/apollo/connectors/openai/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1023 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/connectors/openai/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2574 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/connectors/openai/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      956 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/connectors/openai/local.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1585 2023-05-26 17:12:47.000000 apollo-sdk-0.2.8/apollo/const.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.367004 apollo-sdk-0.2.8/apollo/database/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.367574 apollo-sdk-0.2.8/apollo/database/firebase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/firebase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/firebase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3494 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/firebase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1438 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/firebase/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.367712 apollo-sdk-0.2.8/apollo/database/mongo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/mongo/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.367852 apollo-sdk-0.2.8/apollo/database/mysql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/mysql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.367986 apollo-sdk-0.2.8/apollo/database/postgres/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/postgres/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.368642 apollo-sdk-0.2.8/apollo/database/supabase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/supabase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      739 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/supabase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1553 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/supabase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      810 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/supabase/local.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4197 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/exceptions.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1578 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/manager.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.369416 apollo-sdk-0.2.8/apollo/plugins/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-05-26 17:55:34.000000 apollo-sdk-0.2.8/apollo/plugins/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4796 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/plugins/utils.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5165 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/plugins/validation.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1426 2023-05-27 05:36:10.000000 apollo-sdk-0.2.8/apollo/resource.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.369781 apollo-sdk-0.2.8/apollo/service/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/service/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.369940 apollo-sdk-0.2.8/apollo/service/graphql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/service/graphql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.370653 apollo-sdk-0.2.8/apollo/service/json/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      754 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/service/json/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      947 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/service/json/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1272 2023-05-27 05:36:10.000000 apollo-sdk-0.2.8/apollo/service/json/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      926 2023-05-27 05:36:10.000000 apollo-sdk-0.2.8/apollo/service/json/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.370968 apollo-sdk-0.2.8/apollo/tests/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/tests/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.371773 apollo-sdk-0.2.8/apollo_sdk.egg-info/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     6096 2023-05-27 07:48:49.000000 apollo-sdk-0.2.8/apollo_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1322 2023-05-27 07:48:49.000000 apollo-sdk-0.2.8/apollo_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-05-27 07:48:49.000000 apollo-sdk-0.2.8/apollo_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       47 2023-05-27 07:48:49.000000 apollo-sdk-0.2.8/apollo_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1798 2023-05-27 07:48:49.000000 apollo-sdk-0.2.8/apollo_sdk.egg-info/requires.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       11 2023-05-27 07:48:49.000000 apollo-sdk-0.2.8/apollo_sdk.egg-info/top_level.txt
+-rwxr-xr-x   0 abpyguru   (501) staff       (20)      176 2023-05-27 06:38:58.000000 apollo-sdk-0.2.8/cli.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)       38 2023-05-27 07:48:49.372169 apollo-sdk-0.2.8/setup.cfg
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1592 2023-05-27 07:46:44.000000 apollo-sdk-0.2.8/setup.py
```

### Comparing `apollo-sdk-0.2.4/LICENSE` & `apollo-sdk-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/PKG-INFO` & `apollo-sdk-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-sdk
-Version: 0.2.4
+Version: 0.2.8
 Summary: Build automated decision making workflows by aggregating your AI models and data into one api.
 Home-page: https://github.com/apolloapi/apolloapi
 Author: Apollo API
 Author-email: adrbrownx@gmail.com
 License: Elastic License v2
 Platform: Any
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: apollo-sdk Version: 0.2.4 Summary: Build automated
+Metadata-Version: 2.1 Name: apollo-sdk Version: 0.2.8 Summary: Build automated
 decision making workflows by aggregating your AI models and data into one api.
 Home-page: https://github.com/apolloapi/apolloapi Author: Apollo API Author-
 email: adrbrownx@gmail.com License: Elastic License v2 Platform: Any
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Description-Content-Type: text/markdown License-File: LICENSE
     ![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/
   643fffb82419ac18d39e3e4e_Screenshot%202023-04-19%20at%2010.50.13%20AM.png)
```

### Comparing `apollo-sdk-0.2.4/README.md` & `apollo-sdk-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/__init__.py` & `apollo-sdk-0.2.8/apollo/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/client.py` & `apollo-sdk-0.2.8/apollo/client.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/connectors/__init__.py` & `apollo-sdk-0.2.8/apollo/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/connectors/aws/__init__.py` & `apollo-sdk-0.2.8/apollo/connectors/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/connectors/google/__init__.py` & `apollo-sdk-0.2.8/apollo/connectors/google/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/connectors/microsoft/__init__.py` & `apollo-sdk-0.2.8/apollo/connectors/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/connectors/openai/__init__.py` & `apollo-sdk-0.2.8/apollo/connectors/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/connectors/openai/base.py` & `apollo-sdk-0.2.8/apollo/connectors/openai/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/connectors/openai/cloud.py` & `apollo-sdk-0.2.8/apollo/connectors/openai/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/connectors/openai/local.py` & `apollo-sdk-0.2.8/apollo/connectors/openai/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/const.py` & `apollo-sdk-0.2.8/apollo/const.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/database/__init__.py` & `apollo-sdk-0.2.8/apollo/database/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/database/firebase/__init__.py` & `apollo-sdk-0.2.8/apollo/database/firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/database/firebase/base.py` & `apollo-sdk-0.2.8/apollo/database/firebase/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/database/firebase/cloud.py` & `apollo-sdk-0.2.8/apollo/database/firebase/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/database/firebase/local.py` & `apollo-sdk-0.2.8/apollo/database/firebase/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/database/mongo/__init__.py` & `apollo-sdk-0.2.8/apollo/database/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/database/mysql/__init__.py` & `apollo-sdk-0.2.8/apollo/database/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/database/postgres/__init__.py` & `apollo-sdk-0.2.8/apollo/database/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/database/supabase/__init__.py` & `apollo-sdk-0.2.8/apollo/database/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/database/supabase/base.py` & `apollo-sdk-0.2.8/apollo/database/supabase/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/database/supabase/cloud.py` & `apollo-sdk-0.2.8/apollo/database/supabase/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/database/supabase/local.py` & `apollo-sdk-0.2.8/apollo/database/supabase/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/exceptions.py` & `apollo-sdk-0.2.8/apollo/exceptions.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/manager.py` & `apollo-sdk-0.2.8/apollo/manager.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/plugins/__init__.py` & `apollo-sdk-0.2.8/apollo/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/plugins/utils.py` & `apollo-sdk-0.2.8/apollo/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/plugins/validation.py` & `apollo-sdk-0.2.8/apollo/plugins/validation.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/resource.py` & `apollo-sdk-0.2.8/apollo/resource.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/service/__init__.py` & `apollo-sdk-0.2.8/apollo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/service/graphql/__init__.py` & `apollo-sdk-0.2.8/apollo/service/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/service/json/__init__.py` & `apollo-sdk-0.2.8/apollo/service/json/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/service/json/base.py` & `apollo-sdk-0.2.8/apollo/service/json/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/service/json/cloud.py` & `apollo-sdk-0.2.8/apollo/service/json/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/service/json/local.py` & `apollo-sdk-0.2.8/apollo/service/json/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo/tests/__init__.py` & `apollo-sdk-0.2.8/apollo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/apollo_sdk.egg-info/PKG-INFO` & `apollo-sdk-0.2.8/apollo_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-sdk
-Version: 0.2.4
+Version: 0.2.8
 Summary: Build automated decision making workflows by aggregating your AI models and data into one api.
 Home-page: https://github.com/apolloapi/apolloapi
 Author: Apollo API
 Author-email: adrbrownx@gmail.com
 License: Elastic License v2
 Platform: Any
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: apollo-sdk Version: 0.2.4 Summary: Build automated
+Metadata-Version: 2.1 Name: apollo-sdk Version: 0.2.8 Summary: Build automated
 decision making workflows by aggregating your AI models and data into one api.
 Home-page: https://github.com/apolloapi/apolloapi Author: Apollo API Author-
 email: adrbrownx@gmail.com License: Elastic License v2 Platform: Any
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Description-Content-Type: text/markdown License-File: LICENSE
     ![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/
   643fffb82419ac18d39e3e4e_Screenshot%202023-04-19%20at%2010.50.13%20AM.png)
```

### Comparing `apollo-sdk-0.2.4/apollo_sdk.egg-info/SOURCES.txt` & `apollo-sdk-0.2.8/apollo_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 README.md
-setup.cfg
+cli.py
 setup.py
 apollo/__init__.py
 apollo/client.py
 apollo/const.py
 apollo/exceptions.py
 apollo/manager.py
 apollo/resource.py
```

### Comparing `apollo-sdk-0.2.4/apollo_sdk.egg-info/requires.txt` & `apollo-sdk-0.2.8/apollo_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.4/setup.py` & `apollo-sdk-0.2.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,27 +20,25 @@
     long_description = f.read()
     
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="apollo-sdk",
-    version="0.2.4",
+    version="0.2.8",
     description="Build automated decision making workflows by aggregating your AI models and data into one api.",
     author="Apollo API",
     author_email="adrbrownx@gmail.com",
     packages=find_packages(),
-    # package_dir={'': ''},
+    py_modules = ['cli', 'apollo'],
     url="https://github.com/apolloapi/apolloapi",
     license="Elastic License v2",
     classifiers=[
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3"
     ],
     platforms=["Any"],
-    scripts=[],
-    provides=[],
     install_requires=requirements,
     long_description_content_type="text/markdown",
     long_description=long_description,
-    entry_points={"console_scripts": ["apollo-sdk=apolloapi:run_console"]},
+    entry_points={"console_scripts": ["apollo-sdk=cli:run_console"]},
 )
```

