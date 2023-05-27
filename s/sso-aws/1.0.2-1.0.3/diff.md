# Comparing `tmp/sso-aws-1.0.2.tar.gz` & `tmp/sso-aws-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sso-aws-1.0.2.tar", last modified: Sat May 27 08:05:52 2023, max compression
+gzip compressed data, was "sso-aws-1.0.3.tar", last modified: Sat May 27 08:08:02 2023, max compression
```

## Comparing `sso-aws-1.0.2.tar` & `sso-aws-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 08:05:52.355877 sso-aws-1.0.2/
--rw-rw-rw-   0        0        0     1055 2023-05-27 07:46:17.000000 sso-aws-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2899 2023-05-27 08:05:52.355877 sso-aws-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2519 2023-05-27 08:05:04.000000 sso-aws-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 08:05:52.355877 sso-aws-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      573 2023-05-27 08:03:41.000000 sso-aws-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:05:52.355877 sso-aws-1.0.2/sso_aws.egg-info/
--rw-rw-rw-   0        0        0     2899 2023-05-27 08:05:52.000000 sso-aws-1.0.2/sso_aws.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-05-27 08:05:52.000000 sso-aws-1.0.2/sso_aws.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 08:05:52.000000 sso-aws-1.0.2/sso_aws.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-27 08:05:52.000000 sso-aws-1.0.2/sso_aws.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 08:05:52.000000 sso-aws-1.0.2/sso_aws.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 08:08:02.767725 sso-aws-1.0.3/
+-rw-rw-rw-   0        0        0     1055 2023-05-27 07:46:17.000000 sso-aws-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2904 2023-05-27 08:08:02.766724 sso-aws-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2519 2023-05-27 08:05:04.000000 sso-aws-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 08:08:02.767725 sso-aws-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      578 2023-05-27 08:08:00.000000 sso-aws-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:08:02.765725 sso-aws-1.0.3/sso_aws.egg-info/
+-rw-rw-rw-   0        0        0     2904 2023-05-27 08:08:02.000000 sso-aws-1.0.3/sso_aws.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-05-27 08:08:02.000000 sso-aws-1.0.3/sso_aws.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 08:08:02.000000 sso-aws-1.0.3/sso_aws.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-27 08:08:02.000000 sso-aws-1.0.3/sso_aws.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 08:08:02.000000 sso-aws-1.0.3/sso_aws.egg-info/top_level.txt
```

### Comparing `sso-aws-1.0.2/LICENSE` & `sso-aws-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sso-aws-1.0.2/PKG-INFO` & `sso-aws-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sso-aws
-Version: 1.0.2
-Summary: Login to AWS SSO with this simple utility - just invoke get_aws_session with: region, role_name, account_id, sso_endpoint. Then use the returned aws session instead of boto3
+Version: 1.0.3
+Summary: TEST Login to AWS SSO with this simple utility - just invoke get_aws_session with: region, role_name, account_id, sso_endpoint. Then use the returned aws session instead of boto3
 Home-page: UNKNOWN
 Author: Tom R
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sso-aws-1.0.2/README.md` & `sso-aws-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sso-aws-1.0.2/setup.py` & `sso-aws-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sso-aws',
-    version='1.0.2',
+    version='1.0.3',
     author='Tom R',
-    description='Login to AWS SSO with this simple utility - just invoke get_aws_session '
+    description='TEST Login to AWS SSO with this simple utility - just invoke get_aws_session '
                 'with: region, role_name, account_id, sso_endpoint. Then use the returned aws session '
                 'instead of boto3',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'boto3',
     ],
```

### Comparing `sso-aws-1.0.2/sso_aws.egg-info/PKG-INFO` & `sso-aws-1.0.3/sso_aws.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sso-aws
-Version: 1.0.2
-Summary: Login to AWS SSO with this simple utility - just invoke get_aws_session with: region, role_name, account_id, sso_endpoint. Then use the returned aws session instead of boto3
+Version: 1.0.3
+Summary: TEST Login to AWS SSO with this simple utility - just invoke get_aws_session with: region, role_name, account_id, sso_endpoint. Then use the returned aws session instead of boto3
 Home-page: UNKNOWN
 Author: Tom R
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

