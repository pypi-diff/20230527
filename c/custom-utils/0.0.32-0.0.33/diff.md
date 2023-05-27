# Comparing `tmp/custom-utils-0.0.32.tar.gz` & `tmp/custom-utils-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom-utils-0.0.32.tar", last modified: Sat May 27 14:21:03 2023, max compression
+gzip compressed data, was "custom-utils-0.0.33.tar", last modified: Sat May 27 14:30:37 2023, max compression
```

## Comparing `custom-utils-0.0.32.tar` & `custom-utils-0.0.33.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 14:21:03.162214 custom-utils-0.0.32/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1068 2023-05-18 07:57:45.000000 custom-utils-0.0.32/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16468 2023-05-27 14:21:03.162214 custom-utils-0.0.32/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15838 2023-05-27 14:19:41.000000 custom-utils-0.0.32/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 14:21:03.158214 custom-utils-0.0.32/custom_utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-05-18 07:57:45.000000 custom-utils-0.0.32/custom_utils/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 14:21:03.162214 custom-utils-0.0.32/custom_utils/alerter/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.32/custom_utils/alerter/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1245 2023-05-27 11:34:18.000000 custom-utils-0.0.32/custom_utils/alerter/slack.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-05-18 07:57:45.000000 custom-utils-0.0.32/custom_utils/config.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 14:21:03.162214 custom-utils-0.0.32/custom_utils/configurer/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.32/custom_utils/configurer/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2138 2023-05-18 07:57:45.000000 custom-utils-0.0.32/custom_utils/configurer/profiler.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2473 2023-05-18 07:57:45.000000 custom-utils-0.0.32/custom_utils/configurer/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 14:21:03.162214 custom-utils-0.0.32/custom_utils/connector/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.32/custom_utils/connector/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7285 2023-05-18 07:57:45.000000 custom-utils-0.0.32/custom_utils/connector/bigquery.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8750 2023-05-18 07:57:45.000000 custom-utils-0.0.32/custom_utils/connector/mongodb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2232 2023-05-27 13:04:17.000000 custom-utils-0.0.32/custom_utils/connector/mysql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4066 2023-05-27 13:15:15.000000 custom-utils-0.0.32/custom_utils/connector/s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1017 2023-05-27 10:52:53.000000 custom-utils-0.0.32/custom_utils/exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      568 2023-05-27 12:41:24.000000 custom-utils-0.0.32/custom_utils/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 14:21:03.158214 custom-utils-0.0.32/custom_utils.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16468 2023-05-27 14:21:03.000000 custom-utils-0.0.32/custom_utils.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      635 2023-05-27 14:21:03.000000 custom-utils-0.0.32/custom_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-27 14:21:03.000000 custom-utils-0.0.32/custom_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      511 2023-05-27 14:21:03.000000 custom-utils-0.0.32/custom_utils.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-05-27 14:21:03.000000 custom-utils-0.0.32/custom_utils.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-27 14:21:03.162214 custom-utils-0.0.32/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1438 2023-05-27 14:00:30.000000 custom-utils-0.0.32/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 14:30:37.750247 custom-utils-0.0.33/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1068 2023-05-18 07:57:45.000000 custom-utils-0.0.33/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16262 2023-05-27 14:30:37.746247 custom-utils-0.0.33/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15632 2023-05-27 14:28:51.000000 custom-utils-0.0.33/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 14:30:37.738247 custom-utils-0.0.33/custom_utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-05-18 07:57:45.000000 custom-utils-0.0.33/custom_utils/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 14:30:37.742247 custom-utils-0.0.33/custom_utils/alerter/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.33/custom_utils/alerter/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1245 2023-05-27 11:34:18.000000 custom-utils-0.0.33/custom_utils/alerter/slack.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-05-18 07:57:45.000000 custom-utils-0.0.33/custom_utils/config.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 14:30:37.742247 custom-utils-0.0.33/custom_utils/configurer/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.33/custom_utils/configurer/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2138 2023-05-18 07:57:45.000000 custom-utils-0.0.33/custom_utils/configurer/profiler.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2473 2023-05-18 07:57:45.000000 custom-utils-0.0.33/custom_utils/configurer/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 14:30:37.746247 custom-utils-0.0.33/custom_utils/connector/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.33/custom_utils/connector/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7285 2023-05-18 07:57:45.000000 custom-utils-0.0.33/custom_utils/connector/bigquery.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8750 2023-05-18 07:57:45.000000 custom-utils-0.0.33/custom_utils/connector/mongodb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2232 2023-05-27 13:04:17.000000 custom-utils-0.0.33/custom_utils/connector/mysql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4066 2023-05-27 13:15:15.000000 custom-utils-0.0.33/custom_utils/connector/s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1017 2023-05-27 10:52:53.000000 custom-utils-0.0.33/custom_utils/exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      568 2023-05-27 12:41:24.000000 custom-utils-0.0.33/custom_utils/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 14:30:37.742247 custom-utils-0.0.33/custom_utils.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16262 2023-05-27 14:30:37.000000 custom-utils-0.0.33/custom_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      635 2023-05-27 14:30:37.000000 custom-utils-0.0.33/custom_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-27 14:30:37.000000 custom-utils-0.0.33/custom_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      511 2023-05-27 14:30:37.000000 custom-utils-0.0.33/custom_utils.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-05-27 14:30:37.000000 custom-utils-0.0.33/custom_utils.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-27 14:30:37.750247 custom-utils-0.0.33/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1438 2023-05-27 14:29:44.000000 custom-utils-0.0.33/setup.py
```

### Comparing `custom-utils-0.0.32/LICENSE` & `custom-utils-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.32/PKG-INFO` & `custom-utils-0.0.33/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: custom-utils
-Version: 0.0.32
-Summary: Utilities for database connectors, slack alerter, loggers etc
-Home-page: https://github.com/RahulnKumar/custom-utils
-Author: Rahul Kumar
-Author-email: rahulnkumar7@gmail.com
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6.9
-Description-Content-Type: text/markdown
-Provides-Extra: s3
-Provides-Extra: mysql
-Provides-Extra: bigquery
-Provides-Extra: mongodb
-Provides-Extra: slack
-Provides-Extra: full
-License-File: LICENSE
-
 # custom-utils
 Pip Package for Database Connectors, Alerter, Log Formatter etc
 
 
 ***
 
 <p float="left">
@@ -46,15 +26,15 @@
     - [1. Profile Decorator](#1-profile-decorator)
     - [2.  Log Formatter](#2--log-formatter)
   - [4. Alerter](#4-alerter)
     - [1.  Slack Alerter](#1--slack-alerter)
 
 ***
 
-## 1.  Installation<a id="Installation" name="Installation">    
+## 1.  Installation<a id="1--installation">    
 
 - **Installation from Pypi repository** (Any one)
 	
     `pip install custom-utils`  --> minimal installation  
     `pip install custom-utils[full]` --> full installation  
     `pip install custom-utils[s3,mysql,bigquery,mongodb,slack]`  --> selective installation 
 - **Installation from github repository** (Any one)  
@@ -62,18 +42,18 @@
     `pip install git+https://github.com/rahulnkumar/custom-utils.git`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<tag_no>`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<branch_name>`    
     
 ---
     
 	
-## 2. Connector<a id="2-connector" name="Connector">
+## 2. Connector<a id="2-connector">
 
     
-### 1. S3 Connector<a id="S3_Connector" name="S3_Connector">     
+### 1. S3 Connector<a id="1-s3-connector">     
 
 **Code Snippet Sample :**
 ```python
 ## To use S3 either setup AWS CLI or set the credentials from pip package only
 
 ## Setup AWS CLI
 sudo apt install awscli && aws configure
@@ -133,15 +113,15 @@
   
 ```
 ---
     
 
 ---
    
-### 2. MySQL Connector<a id="MySQL_Connector" name="MySQL_Connector">  
+### 2. MySQL Connector<a id="2-mysql-connector">  
   
 **Code Snippet Sample :**  
 ```python
 # Query from Custom MySQL Database
 from custom_utils.connector.mysql import MySQL 
 user = "***"
 password = "***"
@@ -184,15 +164,15 @@
  |      :param string query: query for fetching data from table
  |      :return pd.DataFrame data
 ```
     
 ---
     
     
-### 3.  MongoDB Connector<a id="MongoDB_Connector" name="MongoDB_Connector">
+### 3.  MongoDB Connector<a id="3--mongodb-connector">
     
 **Code Snippet Sample :**  
 ```python
 from custom_utils.connector.mongodb import MongoDB
 uri = "****"
 db = "***"
 collection = "****"
@@ -289,15 +269,15 @@
  |      :param list upsert_keys : keys to be upserted
  |      :return:
  |  
  |  ----------------------------------------------------------------------
 ```
 ---
 	
-### 4.  BigQuery Connector<a id="BigQuery_Connector" name="BigQuery_Connector">
+### 4.  BigQuery Connector<a id="4--bigquery-connector">
     
 **Code Snippet Sample :**  
 ```python
 
 # Fetching data from BigQuery
 from custom_utils.connector.bigquery import BigQuery
 bq = BigQuery(read_big_query_project = "****",
@@ -369,17 +349,17 @@
  |      :param string table: target table name
  |      :param  rows_to_insert: list of dictionaries where each dictionary is a
  |                              row with keys as column names
 ```
 ---
 	
 	
-## 3. Configurer<a id="Configurer" name="Configurer">   
+## 3. Configurer<a id="3-configurer">   
 	
-### 1. Profile Decorator<a id="Profile_Decorator" name="Profile_Decorator">    
+### 1. Profile Decorator<a id="1-profile-decorator">    
     
 **Code Snippet Sample :**  
 ```python
 from custom_utils.configurer.profiler import profiler
 @profiler(sort_by='cumulative', lines_to_print=10, strip_dirs=True)
 def product_counter_v3():
     return [1, 2, 3, 4, 5]
@@ -398,15 +378,15 @@
     the size of the printout, especially that sorting by 'cumulative', the time consuming operations are printed toward
     the top of the file.
     :param bool strip_dirs: Whether to remove the leading path info from file names. This is also useful in reducing the
     size of the printout
     :return: Profile of the decorated function
     """
 ```
-###  2.  Log Formatter<a id="Log_Formatter" name="Log_Formatter">
+###  2.  Log Formatter<a id="2--log-formatter">
  
 **Code Snippet Sample :**
 ```python
 from custom_utils.configurer.utils import LogFormatter
 LogFormatter.apply()
 ```
     
@@ -422,17 +402,17 @@
         """
         Start logging in json format.
         :return:
 ```
 ---
 	
 	
-## 4. Alerter<a id="Alerter" name="Alerter">    
+## 4. Alerter<a id="4-alerter">    
 	
-###  1.  Slack Alerter<a id="Slack_Alerter" name="Slack_Alerter">  
+###  1.  Slack Alerter<a id="1--slack-alerter">  
     
     
 **Code Snippet Sample :**
 ```python3
 from custom_utils.alerter.slack import Slack
 slack = Slack(token=SLACK_BOT_TOKEN) # OR Slack() with  SLACK_BOT_TOKEN as env variable
 channel="#shield"
```

#### html2text {}

```diff
@@ -1,17 +1,9 @@
-Metadata-Version: 2.1 Name: custom-utils Version: 0.0.32 Summary: Utilities for
-database connectors, slack alerter, loggers etc Home-page: https://github.com/
-RahulnKumar/custom-utils Author: Rahul Kumar Author-email:
-rahulnkumar7@gmail.com Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.6.9
-Description-Content-Type: text/markdown Provides-Extra: s3 Provides-Extra:
-mysql Provides-Extra: bigquery Provides-Extra: mongodb Provides-Extra: slack
-Provides-Extra: full License-File: LICENSE # custom-utils Pip Package for
-Database Connectors, Alerter, Log Formatter etc ***
+# custom-utils Pip Package for Database Connectors, Alerter, Log Formatter etc
+***
 [https://img.shields.io/pypi/v/custom-utils] [https://www.code-inspector.com/
 project/29426/score/svg] [https://img.shields.io/pypi/dm/custom-
 utils?logo=Python&style=social] [GitHub_license]
 ## Table of Contents - [custom-utils](#custom-utils) - [Table of Contents]
 (#table-of-contents) - [1. Installation](#1--installation) - [2. Connector](#2-
 connector) - [1. S3 Connector](#1-s3-connector) - [2. MySQL Connector](#2-
 mysql-connector) - [3. MongoDB Connector](#3--mongodb-connector) - [4. BigQuery
```

### Comparing `custom-utils-0.0.32/README.md` & `custom-utils-0.0.33/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: custom-utils
+Version: 0.0.33
+Summary: Utilities for database connectors, slack alerter, loggers etc
+Home-page: https://github.com/RahulnKumar/custom-utils
+Author: Rahul Kumar
+Author-email: rahulnkumar7@gmail.com
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.6.9
+Description-Content-Type: text/markdown
+Provides-Extra: s3
+Provides-Extra: mysql
+Provides-Extra: bigquery
+Provides-Extra: mongodb
+Provides-Extra: slack
+Provides-Extra: full
+License-File: LICENSE
+
 # custom-utils
 Pip Package for Database Connectors, Alerter, Log Formatter etc
 
 
 ***
 
 <p float="left">
@@ -26,15 +46,15 @@
     - [1. Profile Decorator](#1-profile-decorator)
     - [2.  Log Formatter](#2--log-formatter)
   - [4. Alerter](#4-alerter)
     - [1.  Slack Alerter](#1--slack-alerter)
 
 ***
 
-## 1.  Installation<a id="Installation" name="Installation">    
+## 1.  Installation<a id="1--installation">    
 
 - **Installation from Pypi repository** (Any one)
 	
     `pip install custom-utils`  --> minimal installation  
     `pip install custom-utils[full]` --> full installation  
     `pip install custom-utils[s3,mysql,bigquery,mongodb,slack]`  --> selective installation 
 - **Installation from github repository** (Any one)  
@@ -42,18 +62,18 @@
     `pip install git+https://github.com/rahulnkumar/custom-utils.git`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<tag_no>`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<branch_name>`    
     
 ---
     
 	
-## 2. Connector<a id="2-connector" name="Connector">
+## 2. Connector<a id="2-connector">
 
     
-### 1. S3 Connector<a id="S3_Connector" name="S3_Connector">     
+### 1. S3 Connector<a id="1-s3-connector">     
 
 **Code Snippet Sample :**
 ```python
 ## To use S3 either setup AWS CLI or set the credentials from pip package only
 
 ## Setup AWS CLI
 sudo apt install awscli && aws configure
@@ -113,15 +133,15 @@
   
 ```
 ---
     
 
 ---
    
-### 2. MySQL Connector<a id="MySQL_Connector" name="MySQL_Connector">  
+### 2. MySQL Connector<a id="2-mysql-connector">  
   
 **Code Snippet Sample :**  
 ```python
 # Query from Custom MySQL Database
 from custom_utils.connector.mysql import MySQL 
 user = "***"
 password = "***"
@@ -164,15 +184,15 @@
  |      :param string query: query for fetching data from table
  |      :return pd.DataFrame data
 ```
     
 ---
     
     
-### 3.  MongoDB Connector<a id="MongoDB_Connector" name="MongoDB_Connector">
+### 3.  MongoDB Connector<a id="3--mongodb-connector">
     
 **Code Snippet Sample :**  
 ```python
 from custom_utils.connector.mongodb import MongoDB
 uri = "****"
 db = "***"
 collection = "****"
@@ -269,15 +289,15 @@
  |      :param list upsert_keys : keys to be upserted
  |      :return:
  |  
  |  ----------------------------------------------------------------------
 ```
 ---
 	
-### 4.  BigQuery Connector<a id="BigQuery_Connector" name="BigQuery_Connector">
+### 4.  BigQuery Connector<a id="4--bigquery-connector">
     
 **Code Snippet Sample :**  
 ```python
 
 # Fetching data from BigQuery
 from custom_utils.connector.bigquery import BigQuery
 bq = BigQuery(read_big_query_project = "****",
@@ -349,17 +369,17 @@
  |      :param string table: target table name
  |      :param  rows_to_insert: list of dictionaries where each dictionary is a
  |                              row with keys as column names
 ```
 ---
 	
 	
-## 3. Configurer<a id="Configurer" name="Configurer">   
+## 3. Configurer<a id="3-configurer">   
 	
-### 1. Profile Decorator<a id="Profile_Decorator" name="Profile_Decorator">    
+### 1. Profile Decorator<a id="1-profile-decorator">    
     
 **Code Snippet Sample :**  
 ```python
 from custom_utils.configurer.profiler import profiler
 @profiler(sort_by='cumulative', lines_to_print=10, strip_dirs=True)
 def product_counter_v3():
     return [1, 2, 3, 4, 5]
@@ -378,15 +398,15 @@
     the size of the printout, especially that sorting by 'cumulative', the time consuming operations are printed toward
     the top of the file.
     :param bool strip_dirs: Whether to remove the leading path info from file names. This is also useful in reducing the
     size of the printout
     :return: Profile of the decorated function
     """
 ```
-###  2.  Log Formatter<a id="Log_Formatter" name="Log_Formatter">
+###  2.  Log Formatter<a id="2--log-formatter">
  
 **Code Snippet Sample :**
 ```python
 from custom_utils.configurer.utils import LogFormatter
 LogFormatter.apply()
 ```
     
@@ -402,17 +422,17 @@
         """
         Start logging in json format.
         :return:
 ```
 ---
 	
 	
-## 4. Alerter<a id="Alerter" name="Alerter">    
+## 4. Alerter<a id="4-alerter">    
 	
-###  1.  Slack Alerter<a id="Slack_Alerter" name="Slack_Alerter">  
+###  1.  Slack Alerter<a id="1--slack-alerter">  
     
     
 **Code Snippet Sample :**
 ```python3
 from custom_utils.alerter.slack import Slack
 slack = Slack(token=SLACK_BOT_TOKEN) # OR Slack() with  SLACK_BOT_TOKEN as env variable
 channel="#shield"
```

#### html2text {}

```diff
@@ -1,9 +1,17 @@
-# custom-utils Pip Package for Database Connectors, Alerter, Log Formatter etc
-***
+Metadata-Version: 2.1 Name: custom-utils Version: 0.0.33 Summary: Utilities for
+database connectors, slack alerter, loggers etc Home-page: https://github.com/
+RahulnKumar/custom-utils Author: Rahul Kumar Author-email:
+rahulnkumar7@gmail.com Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.6.9
+Description-Content-Type: text/markdown Provides-Extra: s3 Provides-Extra:
+mysql Provides-Extra: bigquery Provides-Extra: mongodb Provides-Extra: slack
+Provides-Extra: full License-File: LICENSE # custom-utils Pip Package for
+Database Connectors, Alerter, Log Formatter etc ***
 [https://img.shields.io/pypi/v/custom-utils] [https://www.code-inspector.com/
 project/29426/score/svg] [https://img.shields.io/pypi/dm/custom-
 utils?logo=Python&style=social] [GitHub_license]
 ## Table of Contents - [custom-utils](#custom-utils) - [Table of Contents]
 (#table-of-contents) - [1. Installation](#1--installation) - [2. Connector](#2-
 connector) - [1. S3 Connector](#1-s3-connector) - [2. MySQL Connector](#2-
 mysql-connector) - [3. MongoDB Connector](#3--mongodb-connector) - [4. BigQuery
```

### Comparing `custom-utils-0.0.32/custom_utils/alerter/slack.py` & `custom-utils-0.0.33/custom_utils/alerter/slack.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.32/custom_utils/configurer/profiler.py` & `custom-utils-0.0.33/custom_utils/configurer/profiler.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.32/custom_utils/configurer/utils.py` & `custom-utils-0.0.33/custom_utils/configurer/utils.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.32/custom_utils/connector/bigquery.py` & `custom-utils-0.0.33/custom_utils/connector/bigquery.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.32/custom_utils/connector/mongodb.py` & `custom-utils-0.0.33/custom_utils/connector/mongodb.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.32/custom_utils/connector/mysql.py` & `custom-utils-0.0.33/custom_utils/connector/mysql.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.32/custom_utils/connector/s3.py` & `custom-utils-0.0.33/custom_utils/connector/s3.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.32/custom_utils/exceptions.py` & `custom-utils-0.0.33/custom_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.32/custom_utils/utils.py` & `custom-utils-0.0.33/custom_utils/utils.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.32/custom_utils.egg-info/PKG-INFO` & `custom-utils-0.0.33/custom_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-utils
-Version: 0.0.32
+Version: 0.0.33
 Summary: Utilities for database connectors, slack alerter, loggers etc
 Home-page: https://github.com/RahulnKumar/custom-utils
 Author: Rahul Kumar
 Author-email: rahulnkumar7@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -46,15 +46,15 @@
     - [1. Profile Decorator](#1-profile-decorator)
     - [2.  Log Formatter](#2--log-formatter)
   - [4. Alerter](#4-alerter)
     - [1.  Slack Alerter](#1--slack-alerter)
 
 ***
 
-## 1.  Installation<a id="Installation" name="Installation">    
+## 1.  Installation<a id="1--installation">    
 
 - **Installation from Pypi repository** (Any one)
 	
     `pip install custom-utils`  --> minimal installation  
     `pip install custom-utils[full]` --> full installation  
     `pip install custom-utils[s3,mysql,bigquery,mongodb,slack]`  --> selective installation 
 - **Installation from github repository** (Any one)  
@@ -62,18 +62,18 @@
     `pip install git+https://github.com/rahulnkumar/custom-utils.git`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<tag_no>`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<branch_name>`    
     
 ---
     
 	
-## 2. Connector<a id="2-connector" name="Connector">
+## 2. Connector<a id="2-connector">
 
     
-### 1. S3 Connector<a id="S3_Connector" name="S3_Connector">     
+### 1. S3 Connector<a id="1-s3-connector">     
 
 **Code Snippet Sample :**
 ```python
 ## To use S3 either setup AWS CLI or set the credentials from pip package only
 
 ## Setup AWS CLI
 sudo apt install awscli && aws configure
@@ -133,15 +133,15 @@
   
 ```
 ---
     
 
 ---
    
-### 2. MySQL Connector<a id="MySQL_Connector" name="MySQL_Connector">  
+### 2. MySQL Connector<a id="2-mysql-connector">  
   
 **Code Snippet Sample :**  
 ```python
 # Query from Custom MySQL Database
 from custom_utils.connector.mysql import MySQL 
 user = "***"
 password = "***"
@@ -184,15 +184,15 @@
  |      :param string query: query for fetching data from table
  |      :return pd.DataFrame data
 ```
     
 ---
     
     
-### 3.  MongoDB Connector<a id="MongoDB_Connector" name="MongoDB_Connector">
+### 3.  MongoDB Connector<a id="3--mongodb-connector">
     
 **Code Snippet Sample :**  
 ```python
 from custom_utils.connector.mongodb import MongoDB
 uri = "****"
 db = "***"
 collection = "****"
@@ -289,15 +289,15 @@
  |      :param list upsert_keys : keys to be upserted
  |      :return:
  |  
  |  ----------------------------------------------------------------------
 ```
 ---
 	
-### 4.  BigQuery Connector<a id="BigQuery_Connector" name="BigQuery_Connector">
+### 4.  BigQuery Connector<a id="4--bigquery-connector">
     
 **Code Snippet Sample :**  
 ```python
 
 # Fetching data from BigQuery
 from custom_utils.connector.bigquery import BigQuery
 bq = BigQuery(read_big_query_project = "****",
@@ -369,17 +369,17 @@
  |      :param string table: target table name
  |      :param  rows_to_insert: list of dictionaries where each dictionary is a
  |                              row with keys as column names
 ```
 ---
 	
 	
-## 3. Configurer<a id="Configurer" name="Configurer">   
+## 3. Configurer<a id="3-configurer">   
 	
-### 1. Profile Decorator<a id="Profile_Decorator" name="Profile_Decorator">    
+### 1. Profile Decorator<a id="1-profile-decorator">    
     
 **Code Snippet Sample :**  
 ```python
 from custom_utils.configurer.profiler import profiler
 @profiler(sort_by='cumulative', lines_to_print=10, strip_dirs=True)
 def product_counter_v3():
     return [1, 2, 3, 4, 5]
@@ -398,15 +398,15 @@
     the size of the printout, especially that sorting by 'cumulative', the time consuming operations are printed toward
     the top of the file.
     :param bool strip_dirs: Whether to remove the leading path info from file names. This is also useful in reducing the
     size of the printout
     :return: Profile of the decorated function
     """
 ```
-###  2.  Log Formatter<a id="Log_Formatter" name="Log_Formatter">
+###  2.  Log Formatter<a id="2--log-formatter">
  
 **Code Snippet Sample :**
 ```python
 from custom_utils.configurer.utils import LogFormatter
 LogFormatter.apply()
 ```
     
@@ -422,17 +422,17 @@
         """
         Start logging in json format.
         :return:
 ```
 ---
 	
 	
-## 4. Alerter<a id="Alerter" name="Alerter">    
+## 4. Alerter<a id="4-alerter">    
 	
-###  1.  Slack Alerter<a id="Slack_Alerter" name="Slack_Alerter">  
+###  1.  Slack Alerter<a id="1--slack-alerter">  
     
     
 **Code Snippet Sample :**
 ```python3
 from custom_utils.alerter.slack import Slack
 slack = Slack(token=SLACK_BOT_TOKEN) # OR Slack() with  SLACK_BOT_TOKEN as env variable
 channel="#shield"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: custom-utils Version: 0.0.32 Summary: Utilities for
+Metadata-Version: 2.1 Name: custom-utils Version: 0.0.33 Summary: Utilities for
 database connectors, slack alerter, loggers etc Home-page: https://github.com/
 RahulnKumar/custom-utils Author: Rahul Kumar Author-email:
 rahulnkumar7@gmail.com Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown Provides-Extra: s3 Provides-Extra:
 mysql Provides-Extra: bigquery Provides-Extra: mongodb Provides-Extra: slack
```

### Comparing `custom-utils-0.0.32/custom_utils.egg-info/SOURCES.txt` & `custom-utils-0.0.33/custom_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.32/setup.py` & `custom-utils-0.0.33/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 EXTRAS_REQUIRE['full'] = list(set(chain(*EXTRAS_REQUIRE.values())))
 
 setup(
     author="Rahul Kumar",
     author_email="rahulnkumar7@gmail.com",
     name='custom-utils',
     description='Utilities for database connectors, slack alerter, loggers etc',
-    version="0.0.32",
+    version="0.0.33",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RahulnKumar/custom-utils',
     packages=find_packages(),
     python_requires=">=3.6.9",
     install_requires=['requests', 'json-utils', 'python-dotenv', 'subprocess32', 'psutil',],
     extras_require=EXTRAS_REQUIRE,
```

