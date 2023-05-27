# Comparing `tmp/edge_addons_api-0.3.0.tar.gz` & `tmp/edge_addons_api-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_addons_api-0.3.0.tar", max compression
+gzip compressed data, was "edge_addons_api-0.3.1.tar", max compression
```

## Comparing `edge_addons_api-0.3.0.tar` & `edge_addons_api-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-01-22 22:42:11.927242 edge_addons_api-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-01-22 22:42:11.927242 edge_addons_api-0.3.0/edge_addons_api/__init__.py
--rw-r--r--   0        0        0     4417 2023-01-22 22:42:11.931242 edge_addons_api-0.3.0/edge_addons_api/client.py
--rw-r--r--   0        0        0      272 2023-01-22 22:42:11.931242 edge_addons_api-0.3.0/edge_addons_api/exceptions.py
--rw-r--r--   0        0        0      488 2023-01-22 22:42:11.931242 edge_addons_api-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 edge_addons_api-0.3.0/setup.py
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 edge_addons_api-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-27 06:58:29.715550 edge_addons_api-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 06:58:29.715550 edge_addons_api-0.3.1/edge_addons_api/__init__.py
+-rw-r--r--   0        0        0     4435 2023-05-27 06:58:29.715550 edge_addons_api-0.3.1/edge_addons_api/client.py
+-rw-r--r--   0        0        0      272 2023-05-27 06:58:29.715550 edge_addons_api-0.3.1/edge_addons_api/exceptions.py
+-rw-r--r--   0        0        0      496 2023-05-27 06:58:29.715550 edge_addons_api-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 edge_addons_api-0.3.1/setup.py
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 edge_addons_api-0.3.1/PKG-INFO
```

### Comparing `edge_addons_api-0.3.0/README.md` & `edge_addons_api-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `edge_addons_api-0.3.0/edge_addons_api/client.py` & `edge_addons_api-0.3.1/edge_addons_api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,25 +64,23 @@
         response.raise_for_status()
 
         logger.debug(f"Publish response: {response.content.decode()}")
 
         return response.headers["Location"]
 
     def _upload(self, file_path: str, access_token: str) -> str:
-
-        files = {"file": open(file_path, "rb")}
-
-        response = requests.post(
-            self._upload_endpoint(),
-            files=files,
-            headers={
-                "Authorization": f"Bearer {access_token}",
-                "Content-Type": "application/zip",
-            },
-        )
+        with open(file_path, "rb") as f:
+            response = requests.post(
+                self._upload_endpoint(),
+                data=f,
+                headers={
+                    "Authorization": f"Bearer {access_token}",
+                    "Content-Type": "application/zip",
+                },
+            )
 
         response.raise_for_status()
 
         return response.headers["Location"]
 
     def _check_upload(
         self,
```

### Comparing `edge_addons_api-0.3.0/setup.py` & `edge_addons_api-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'edge-addons-api',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'API client for uploading addons to the Edge store',
     'long_description': '# Edge Addons API\n\n[![CI](https://github.com/inverse/python-edge-addons-api/actions/workflows/main.yml/badge.svg)](https://github.com/inverse/python-edge-addons-api/actions/workflows/main.yml)\n\nAn API client for publishing addons to the Edge store.\n\nBased on the [PlasmHQ Edge Addons API](https://github.com/PlasmoHQ/edge-addons-api).\n\n## Usage\n\nObtain the required options for your project. These can be obtained by following the [Microsoft Edge Add-Ons API guide](https://learn.microsoft.com/en-us/microsoft-edge/extensions-chromium/publish/api/using-addons-api).\n\nOnce obtained you can submit you addon like below:\n\n\n```python\nfrom edge_addons_api.client import Options, Client\n\noptions = Options(\n    product_id="Your product ID",\n    client_id="Your client ID",\n    client_secret="Your client secret",\n    access_token_url="Your access token URL"\n)\n\nclient = Client(options)\n\n# Upload extension\noperation_id = client.submit(\n    file_path="/path/to/extension.zip",\n    notes="Your upload notes"\n)\n\n# Check publish status\nclient.fetch_publish_status(operation_id)\n```\n\n## License\n\nMIT\n',
     'author': 'Malachi Soord',
     'author_email': 'inverse.chi@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `edge_addons_api-0.3.0/PKG-INFO` & `edge_addons_api-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-addons-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: API client for uploading addons to the Edge store
 License: MIT
 Author: Malachi Soord
 Author-email: inverse.chi@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

