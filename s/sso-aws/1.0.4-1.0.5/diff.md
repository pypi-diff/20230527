# Comparing `tmp/sso-aws-1.0.4.tar.gz` & `tmp/sso-aws-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sso-aws-1.0.4.tar", last modified: Sat May 27 08:11:22 2023, max compression
+gzip compressed data, was "sso-aws-1.0.5.tar", last modified: Sat May 27 08:13:46 2023, max compression
```

## Comparing `sso-aws-1.0.4.tar` & `sso-aws-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 08:11:22.295981 sso-aws-1.0.4/
--rw-rw-rw-   0        0        0     1055 2023-05-27 07:46:17.000000 sso-aws-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     2899 2023-05-27 08:11:22.294979 sso-aws-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2519 2023-05-27 08:09:55.000000 sso-aws-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 08:11:22.295981 sso-aws-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      573 2023-05-27 08:09:55.000000 sso-aws-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:11:22.293980 sso-aws-1.0.4/sso_aws.egg-info/
--rw-rw-rw-   0        0        0     2899 2023-05-27 08:11:22.000000 sso-aws-1.0.4/sso_aws.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-05-27 08:11:22.000000 sso-aws-1.0.4/sso_aws.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 08:11:22.000000 sso-aws-1.0.4/sso_aws.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-27 08:11:22.000000 sso-aws-1.0.4/sso_aws.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 08:11:22.000000 sso-aws-1.0.4/sso_aws.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 08:13:46.964256 sso-aws-1.0.5/
+-rw-rw-rw-   0        0        0     1055 2023-05-27 07:46:17.000000 sso-aws-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2899 2023-05-27 08:13:46.964256 sso-aws-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2519 2023-05-27 08:09:55.000000 sso-aws-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 08:13:46.964256 sso-aws-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      573 2023-05-27 08:13:32.000000 sso-aws-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:13:46.963256 sso-aws-1.0.5/sso_aws.egg-info/
+-rw-rw-rw-   0        0        0     2899 2023-05-27 08:13:46.000000 sso-aws-1.0.5/sso_aws.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-05-27 08:13:46.000000 sso-aws-1.0.5/sso_aws.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 08:13:46.000000 sso-aws-1.0.5/sso_aws.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-27 08:13:46.000000 sso-aws-1.0.5/sso_aws.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 08:13:46.000000 sso-aws-1.0.5/sso_aws.egg-info/top_level.txt
```

### Comparing `sso-aws-1.0.4/LICENSE` & `sso-aws-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sso-aws-1.0.4/PKG-INFO` & `sso-aws-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sso-aws
-Version: 1.0.4
+Version: 1.0.5
 Summary: Login to AWS SSO with this simple utility - just invoke get_aws_session with: region, role_name, account_id, sso_endpoint. Then use the returned aws session instead of boto3
 Home-page: UNKNOWN
 Author: Tom R
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sso-aws-1.0.4/README.md` & `sso-aws-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sso-aws-1.0.4/setup.py` & `sso-aws-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sso-aws',
-    version='1.0.4',
+    version='1.0.5',
     author='Tom R',
     description='Login to AWS SSO with this simple utility - just invoke get_aws_session '
                 'with: region, role_name, account_id, sso_endpoint. Then use the returned aws session '
                 'instead of boto3',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
```

### Comparing `sso-aws-1.0.4/sso_aws.egg-info/PKG-INFO` & `sso-aws-1.0.5/sso_aws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sso-aws
-Version: 1.0.4
+Version: 1.0.5
 Summary: Login to AWS SSO with this simple utility - just invoke get_aws_session with: region, role_name, account_id, sso_endpoint. Then use the returned aws session instead of boto3
 Home-page: UNKNOWN
 Author: Tom R
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

