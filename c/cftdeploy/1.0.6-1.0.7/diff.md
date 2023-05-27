# Comparing `tmp/cftdeploy-1.0.6.tar.gz` & `tmp/cftdeploy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cftdeploy-1.0.6.tar", last modified: Fri Apr 14 12:11:10 2023, max compression
+gzip compressed data, was "cftdeploy-1.0.7.tar", last modified: Sat May 27 21:28:14 2023, max compression
```

## Comparing `cftdeploy-1.0.6.tar` & `cftdeploy-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-14 12:11:10.076722 cftdeploy-1.0.6/
--rw-r--r--   0 chris      (501) staff       (20)    11357 2019-04-06 19:02:14.000000 cftdeploy-1.0.6/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)       15 2019-04-13 22:31:50.000000 cftdeploy-1.0.6/MANIFEST.in
--rw-r--r--   0 chris      (501) staff       (20)     8975 2023-04-14 12:11:10.076797 cftdeploy-1.0.6/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     8629 2019-04-13 21:28:10.000000 cftdeploy-1.0.6/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-14 12:11:10.075942 cftdeploy-1.0.6/cftdeploy/
--rw-r--r--   0 chris      (501) staff       (20)      302 2019-12-30 01:13:59.000000 cftdeploy-1.0.6/cftdeploy/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      137 2023-04-14 12:06:08.000000 cftdeploy-1.0.6/cftdeploy/_version.py
--rw-r--r--   0 chris      (501) staff       (20)    19631 2023-01-13 01:09:20.000000 cftdeploy-1.0.6/cftdeploy/entry_points.py
--rw-r--r--   0 chris      (501) staff       (20)    10417 2020-12-11 14:51:29.000000 cftdeploy-1.0.6/cftdeploy/manifest.py
--rw-r--r--   0 chris      (501) staff       (20)     2068 2019-12-30 01:13:59.000000 cftdeploy-1.0.6/cftdeploy/skeleton.py
--rw-r--r--   0 chris      (501) staff       (20)    12426 2020-12-24 15:31:43.000000 cftdeploy-1.0.6/cftdeploy/stack.py
--rw-r--r--   0 chris      (501) staff       (20)     7496 2020-12-11 01:47:04.000000 cftdeploy-1.0.6/cftdeploy/template.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-14 12:11:10.076614 cftdeploy-1.0.6/cftdeploy.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     8975 2023-04-14 12:11:10.000000 cftdeploy-1.0.6/cftdeploy.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      403 2023-04-14 12:11:10.000000 cftdeploy-1.0.6/cftdeploy.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-04-14 12:11:10.000000 cftdeploy-1.0.6/cftdeploy.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)      430 2023-04-14 12:11:10.000000 cftdeploy-1.0.6/cftdeploy.egg-info/entry_points.txt
--rw-r--r--   0 chris      (501) staff       (20)       38 2023-04-14 12:11:10.000000 cftdeploy-1.0.6/cftdeploy.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       10 2023-04-14 12:11:10.000000 cftdeploy-1.0.6/cftdeploy.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)      131 2023-04-14 12:11:10.077071 cftdeploy-1.0.6/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)     1339 2023-04-14 12:02:59.000000 cftdeploy-1.0.6/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-27 21:28:14.076684 cftdeploy-1.0.7/
+-rw-r--r--   0 chris      (501) staff       (20)    11357 2019-04-06 19:02:14.000000 cftdeploy-1.0.7/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)       15 2019-04-13 22:31:50.000000 cftdeploy-1.0.7/MANIFEST.in
+-rw-r--r--   0 chris      (501) staff       (20)     8975 2023-05-27 21:28:14.076769 cftdeploy-1.0.7/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     8629 2019-04-13 21:28:10.000000 cftdeploy-1.0.7/README.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-27 21:28:14.075372 cftdeploy-1.0.7/cftdeploy/
+-rw-r--r--   0 chris      (501) staff       (20)      302 2019-12-30 01:13:59.000000 cftdeploy-1.0.7/cftdeploy/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      137 2023-05-27 21:27:41.000000 cftdeploy-1.0.7/cftdeploy/_version.py
+-rw-r--r--   0 chris      (501) staff       (20)    19631 2023-01-13 01:09:20.000000 cftdeploy-1.0.7/cftdeploy/entry_points.py
+-rw-r--r--   0 chris      (501) staff       (20)    10417 2020-12-11 14:51:29.000000 cftdeploy-1.0.7/cftdeploy/manifest.py
+-rw-r--r--   0 chris      (501) staff       (20)     2068 2019-12-30 01:13:59.000000 cftdeploy-1.0.7/cftdeploy/skeleton.py
+-rw-r--r--   0 chris      (501) staff       (20)    12426 2020-12-24 15:31:43.000000 cftdeploy-1.0.7/cftdeploy/stack.py
+-rw-r--r--   0 chris      (501) staff       (20)     7906 2023-05-27 21:27:32.000000 cftdeploy-1.0.7/cftdeploy/template.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-27 21:28:14.076547 cftdeploy-1.0.7/cftdeploy.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     8975 2023-05-27 21:28:14.000000 cftdeploy-1.0.7/cftdeploy.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      403 2023-05-27 21:28:14.000000 cftdeploy-1.0.7/cftdeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-27 21:28:14.000000 cftdeploy-1.0.7/cftdeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)      430 2023-05-27 21:28:14.000000 cftdeploy-1.0.7/cftdeploy.egg-info/entry_points.txt
+-rw-r--r--   0 chris      (501) staff       (20)       38 2023-05-27 21:28:14.000000 cftdeploy-1.0.7/cftdeploy.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       10 2023-05-27 21:28:14.000000 cftdeploy-1.0.7/cftdeploy.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)      131 2023-05-27 21:28:14.077106 cftdeploy-1.0.7/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)     1339 2023-04-14 12:02:59.000000 cftdeploy-1.0.7/setup.py
```

### Comparing `cftdeploy-1.0.6/LICENSE` & `cftdeploy-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cftdeploy-1.0.6/PKG-INFO` & `cftdeploy-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cftdeploy
-Version: 1.0.6
+Version: 1.0.7
 Summary: Tools and modules for managing CloudFormation Templates & Stacks
 Home-page: http://github.com/jchrisfarris/cft-deploy
 Author: Chris Farris
 Author-email: chris@room17.com
 License: Apache License 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cftdeploy-1.0.6/README.md` & `cftdeploy-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cftdeploy-1.0.6/cftdeploy/entry_points.py` & `cftdeploy-1.0.7/cftdeploy/entry_points.py`

 * *Files identical despite different names*

### Comparing `cftdeploy-1.0.6/cftdeploy/manifest.py` & `cftdeploy-1.0.7/cftdeploy/manifest.py`

 * *Files identical despite different names*

### Comparing `cftdeploy-1.0.6/cftdeploy/skeleton.py` & `cftdeploy-1.0.7/cftdeploy/skeleton.py`

 * *Files identical despite different names*

### Comparing `cftdeploy-1.0.6/cftdeploy/stack.py` & `cftdeploy-1.0.7/cftdeploy/stack.py`

 * *Files identical despite different names*

### Comparing `cftdeploy-1.0.6/cftdeploy/template.py` & `cftdeploy-1.0.7/cftdeploy/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,21 @@
             return(self.filename)
         else:
             return("A Template has no name")
 
     @classmethod
     def read(cls, filename, region, session=None):
         """Read the template from filename and then initialize."""
-        f = open(filename, "r")
-        template_body = f.read()
-        return(CFTemplate(template_body, region, filename=filename, session=session))
+        try:
+            f = open(filename, "r")
+            template_body = f.read()
+            return(CFTemplate(template_body, region, filename=filename, session=session))
+        except FileNotFoundError as e:
+            print(e)
+            exit(1)
 
     @classmethod
     def download(cls, bucket, object_key, region, session=None):
         """Downloads the template from S3 and then initialize."""
         try:
             s3 = boto3.client('s3')  # FIXME will fail for cross-account roles
             response = s3.get_object(
@@ -72,14 +76,17 @@
         except ClientError as e:
             if e.response['Error']['Code'] == 'ValidationError':
                 if "Member must have length less than or equal to 51200" in e.response['Error']['Message']:
                     raise CFTemplateTooLargeError(e)
                 else:
                     logger.error(f"Invalid Template: {e}")
                     return(None)
+            if e.response['Error']['Code'] == 'ExpiredToken':
+                logger.error(f"Credentials Expired: {e}")
+                return(None)
             else:
                 raise
 
     def generate_manifest(self, manifest_file_name, substitutions=None, overwrite=False):
         """Generates a stub manifest file for this template and writes it to manifest_file_name.
         If substitutions are specified, these are populated into the stub manifest file.
         """
@@ -105,18 +112,21 @@
 
         # Default Value to be subsituted into the skeleton
         manifest_values = {
             'parameter_yaml': parameter_string,
             'my_stack_name': "CHANGEME",
             'term_protection': "false",  # Use yaml formatting which is lowercase
             'template_line': "# WARNING - No Template Source Defined.",
-            'template_description': params['Description'],
             'timestamp': datetime.datetime.now(),
             'region': "CHANGEME"
         }
+        if 'Description' in params:
+            manifest_values['template_description'] = params['Description']
+        else:
+            manifest_values['template_description'] = "No Template Description Provided"
 
         # Set the Template Line value
         if self.filename is not None:
             manifest_values['template_line'] = f"LocalTemplate: {self.filename}"
         elif self.s3url is not None:
             (bucket, object_key) = self.parse_s3_url(self.s3url)
             template_url = f"https://s3.amazonaws.com/{bucket}/{object_key}"
```

### Comparing `cftdeploy-1.0.6/cftdeploy.egg-info/PKG-INFO` & `cftdeploy-1.0.7/cftdeploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cftdeploy
-Version: 1.0.6
+Version: 1.0.7
 Summary: Tools and modules for managing CloudFormation Templates & Stacks
 Home-page: http://github.com/jchrisfarris/cft-deploy
 Author: Chris Farris
 Author-email: chris@room17.com
 License: Apache License 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cftdeploy-1.0.6/setup.py` & `cftdeploy-1.0.7/setup.py`

 * *Files identical despite different names*

