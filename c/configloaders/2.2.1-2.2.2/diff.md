# Comparing `tmp/configloaders-2.2.1.tar.gz` & `tmp/configloaders-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configloaders-2.2.1.tar", max compression
+gzip compressed data, was "configloaders-2.2.2.tar", max compression
```

## Comparing `configloaders-2.2.1.tar` & `configloaders-2.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     4352 2023-05-19 09:32:04.370261 configloaders-2.2.1/configloaders/__core.py
--rw-r--r--   0        0        0      162 2023-05-18 01:08:47.253489 configloaders-2.2.1/configloaders/__init__.py
--rw-r--r--   0        0        0     1505 2023-05-17 06:42:37.555364 configloaders-2.2.1/configloaders/__main__.py
--rw-r--r--   0        0        0     4484 2023-05-22 07:40:20.708475 configloaders-2.2.1/configloaders/__type.py
--rw-r--r--   0        0        0     1936 2023-05-17 06:57:28.206529 configloaders-2.2.1/configloaders/providers/__pycache__/ini_provider.cpython-37.pyc
--rw-r--r--   0        0        0      942 2023-05-22 01:42:21.856533 configloaders-2.2.1/configloaders/providers/__pycache__/json_provider.cpython-310.pyc
--rw-r--r--   0        0        0      843 2023-05-17 06:57:28.216261 configloaders-2.2.1/configloaders/providers/__pycache__/json_provider.cpython-37.pyc
--rw-r--r--   0        0        0      855 2023-05-17 06:57:28.244261 configloaders-2.2.1/configloaders/providers/__pycache__/pickle_provider.cpython-37.pyc
--rw-r--r--   0        0        0     1215 2023-05-17 06:57:28.251261 configloaders-2.2.1/configloaders/providers/__pycache__/py_provider.cpython-37.pyc
--rw-r--r--   0        0        0      843 2023-05-17 06:57:28.255298 configloaders-2.2.1/configloaders/providers/__pycache__/toml_provider.cpython-37.pyc
--rw-r--r--   0        0        0     1619 2023-05-17 06:57:28.346825 configloaders-2.2.1/configloaders/providers/__pycache__/txt_provider.cpython-37.pyc
--rw-r--r--   0        0        0     1689 2023-05-17 06:57:28.348830 configloaders-2.2.1/configloaders/providers/__pycache__/xml_provider.cpython-37.pyc
--rw-r--r--   0        0        0      853 2023-05-17 06:57:28.458830 configloaders-2.2.1/configloaders/providers/__pycache__/yaml_provider.cpython-37.pyc
--rw-r--r--   0        0        0     1029 2023-05-22 01:42:37.354421 configloaders-2.2.1/configloaders/providers/ini_provider.py
--rw-r--r--   0        0        0      403 2023-05-22 01:42:20.261678 configloaders-2.2.1/configloaders/providers/json_provider.py
--rw-r--r--   0        0        0      351 2023-05-17 06:42:37.083912 configloaders-2.2.1/configloaders/providers/pickle_provider.py
--rw-r--r--   0        0        0      657 2023-05-17 06:42:37.206904 configloaders-2.2.1/configloaders/providers/py_provider.py
--rw-r--r--   0        0        0      379 2023-05-22 01:43:44.359388 configloaders-2.2.1/configloaders/providers/toml_provider.py
--rw-r--r--   0        0        0      661 2023-05-22 01:43:44.446581 configloaders-2.2.1/configloaders/providers/txt_provider.py
--rw-r--r--   0        0        0     1387 2023-05-22 01:43:40.948700 configloaders-2.2.1/configloaders/providers/xml_provider.py
--rw-r--r--   0        0        0      389 2023-05-22 01:43:44.414281 configloaders-2.2.1/configloaders/providers/yaml_provider.py
--rw-r--r--   0        0        0     1079 2023-05-18 10:09:54.036619 configloaders-2.2.1/LICENSE
--rw-r--r--   0        0        0      611 2023-05-22 07:41:18.385980 configloaders-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     1756 2023-05-18 10:08:59.013294 configloaders-2.2.1/README.md
--rw-r--r--   0        0        0     2627 1970-01-01 00:00:00.000000 configloaders-2.2.1/setup.py
--rw-r--r--   0        0        0     2380 1970-01-01 00:00:00.000000 configloaders-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4352 2023-05-19 09:32:04.370261 configloaders-2.2.2/configloaders/__core.py
+-rw-r--r--   0        0        0      162 2023-05-18 01:08:47.253489 configloaders-2.2.2/configloaders/__init__.py
+-rw-r--r--   0        0        0     1505 2023-05-17 06:42:37.555364 configloaders-2.2.2/configloaders/__main__.py
+-rw-r--r--   0        0        0     4897 2023-05-27 14:32:55.657888 configloaders-2.2.2/configloaders/__type.py
+-rw-r--r--   0        0        0     1936 2023-05-17 06:57:28.206529 configloaders-2.2.2/configloaders/providers/__pycache__/ini_provider.cpython-37.pyc
+-rw-r--r--   0        0        0      942 2023-05-22 01:42:21.856533 configloaders-2.2.2/configloaders/providers/__pycache__/json_provider.cpython-310.pyc
+-rw-r--r--   0        0        0      843 2023-05-17 06:57:28.216261 configloaders-2.2.2/configloaders/providers/__pycache__/json_provider.cpython-37.pyc
+-rw-r--r--   0        0        0      855 2023-05-17 06:57:28.244261 configloaders-2.2.2/configloaders/providers/__pycache__/pickle_provider.cpython-37.pyc
+-rw-r--r--   0        0        0     1215 2023-05-17 06:57:28.251261 configloaders-2.2.2/configloaders/providers/__pycache__/py_provider.cpython-37.pyc
+-rw-r--r--   0        0        0      843 2023-05-17 06:57:28.255298 configloaders-2.2.2/configloaders/providers/__pycache__/toml_provider.cpython-37.pyc
+-rw-r--r--   0        0        0     1619 2023-05-17 06:57:28.346825 configloaders-2.2.2/configloaders/providers/__pycache__/txt_provider.cpython-37.pyc
+-rw-r--r--   0        0        0     1689 2023-05-17 06:57:28.348830 configloaders-2.2.2/configloaders/providers/__pycache__/xml_provider.cpython-37.pyc
+-rw-r--r--   0        0        0      853 2023-05-17 06:57:28.458830 configloaders-2.2.2/configloaders/providers/__pycache__/yaml_provider.cpython-37.pyc
+-rw-r--r--   0        0        0     1029 2023-05-22 01:42:37.354421 configloaders-2.2.2/configloaders/providers/ini_provider.py
+-rw-r--r--   0        0        0      403 2023-05-22 01:42:20.261678 configloaders-2.2.2/configloaders/providers/json_provider.py
+-rw-r--r--   0        0        0      351 2023-05-17 06:42:37.083912 configloaders-2.2.2/configloaders/providers/pickle_provider.py
+-rw-r--r--   0        0        0      657 2023-05-17 06:42:37.206904 configloaders-2.2.2/configloaders/providers/py_provider.py
+-rw-r--r--   0        0        0      379 2023-05-22 01:43:44.359388 configloaders-2.2.2/configloaders/providers/toml_provider.py
+-rw-r--r--   0        0        0      661 2023-05-22 01:43:44.446581 configloaders-2.2.2/configloaders/providers/txt_provider.py
+-rw-r--r--   0        0        0     1387 2023-05-22 01:43:40.948700 configloaders-2.2.2/configloaders/providers/xml_provider.py
+-rw-r--r--   0        0        0      389 2023-05-22 01:43:44.414281 configloaders-2.2.2/configloaders/providers/yaml_provider.py
+-rw-r--r--   0        0        0     1079 2023-05-18 10:09:54.036619 configloaders-2.2.2/LICENSE
+-rw-r--r--   0        0        0      611 2023-05-27 14:23:42.478415 configloaders-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1756 2023-05-18 10:08:59.013294 configloaders-2.2.2/README.md
+-rw-r--r--   0        0        0     2627 1970-01-01 00:00:00.000000 configloaders-2.2.2/setup.py
+-rw-r--r--   0        0        0     2380 1970-01-01 00:00:00.000000 configloaders-2.2.2/PKG-INFO
```

### Comparing `configloaders-2.2.1/configloaders/__core.py` & `configloaders-2.2.2/configloaders/__core.py`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/__main__.py` & `configloaders-2.2.2/configloaders/__main__.py`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/__type.py` & `configloaders-2.2.2/configloaders/__type.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,41 +63,47 @@
                 if isinstance(val, (int, float, str, bool, list, set, tuple, type(None))):
                     dat[key] = val
                 elif not inspect.ismodule(val):
                     dat[key] = {}
                     items.append((Namespace(val), dat[key]))
         return data
 
+    @staticmethod
+    def private_key(key):
+        if isinstance(key, str) and key.startswith('__'): return '__private' + key
+        return key
+
     def __setitem_func(self, key, value):
-        self.__target = functools.partial(self.__target, **dict.fromkeys([key], value))
+        self.__target = functools.partial(self.__target, **dict.fromkeys([self.private_key(key)], value))
 
     def __getitem_func(self, item):
+        item = self.private_key(item)
         if item in self.__target.keywords: return self.__target.keywords.get(item)
         else: return self.__signature[item].default
 
     def __iter_func(self):
-        return iter(self.__signature)
+        return iter(filter(lambda k: self.private_key(k) == k, self.__signature))
 
     def __setitem_dict(self, key, value):
-        self.__target[key] = value
+        self.__target[self.private_key(key)] = value
 
     def __getitem_dict(self, item):
-        return self.__target[item]
+        return self.__target[self.private_key(item)]
 
     def __iter_dict(self):
-        return iter(self.__target)
+        return iter(filter(lambda k: self.private_key(k) == k, self.__target))
 
     def __setitem_arg(self, key, value):
-        self.__target.add_argument(f'--{key}', type=type(value), default=value, metavar=str(value))
+        self.__target.add_argument(f'--{self.private_key(key)}', type=type(value), default=value, metavar=str(value))
 
     def __getitem_arg(self, item):
-        return next(filter(lambda x: x.dest == item, self.__target._actions)).default
+        return next(filter(lambda x: x.dest == self.private_key(item), self.__target._actions)).default
 
     def __iter_arg(self):
-        return iter(map(lambda x: x.dest, self.__target._actions))
+        return iter(filter(lambda k: self.private_key(k) == k, map(lambda x: x.dest, self.__target._actions)))
 
     def __setitem_obj(self, key, value):
         setattr(self.__target, key, value)
 
     def __getitem_obj(self, item):
         return getattr(self.__target, item)
```

### Comparing `configloaders-2.2.1/configloaders/providers/__pycache__/ini_provider.cpython-37.pyc` & `configloaders-2.2.2/configloaders/providers/__pycache__/ini_provider.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/providers/__pycache__/json_provider.cpython-310.pyc` & `configloaders-2.2.2/configloaders/providers/__pycache__/json_provider.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/providers/__pycache__/json_provider.cpython-37.pyc` & `configloaders-2.2.2/configloaders/providers/__pycache__/json_provider.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/providers/__pycache__/pickle_provider.cpython-37.pyc` & `configloaders-2.2.2/configloaders/providers/__pycache__/pickle_provider.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/providers/__pycache__/py_provider.cpython-37.pyc` & `configloaders-2.2.2/configloaders/providers/__pycache__/py_provider.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/providers/__pycache__/toml_provider.cpython-37.pyc` & `configloaders-2.2.2/configloaders/providers/__pycache__/toml_provider.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/providers/__pycache__/txt_provider.cpython-37.pyc` & `configloaders-2.2.2/configloaders/providers/__pycache__/txt_provider.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/providers/__pycache__/xml_provider.cpython-37.pyc` & `configloaders-2.2.2/configloaders/providers/__pycache__/xml_provider.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/providers/__pycache__/yaml_provider.cpython-37.pyc` & `configloaders-2.2.2/configloaders/providers/__pycache__/yaml_provider.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/providers/ini_provider.py` & `configloaders-2.2.2/configloaders/providers/ini_provider.py`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/providers/py_provider.py` & `configloaders-2.2.2/configloaders/providers/py_provider.py`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/providers/txt_provider.py` & `configloaders-2.2.2/configloaders/providers/txt_provider.py`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/configloaders/providers/xml_provider.py` & `configloaders-2.2.2/configloaders/providers/xml_provider.py`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/LICENSE` & `configloaders-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/pyproject.toml` & `configloaders-2.2.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configloaders"
-version = "2.2.1"
+version = "2.2.2"
 description = "Configloaders is a Python library that allows you to easily load configuration from various types of configuration files and inject them into various types of objects, such as classes, dictionaries, functions, and methods."
 authors = ["jawide <596929059@qq.com>"]
 readme = "README.md"
 packages = [{include = "configloaders"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `configloaders-2.2.1/README.md` & `configloaders-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `configloaders-2.2.1/setup.py` & `configloaders-2.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['configloaders = configloaders.__main__:main']}
 
 setup_kwargs = {
     'name': 'configloaders',
-    'version': '2.2.1',
+    'version': '2.2.2',
     'description': 'Configloaders is a Python library that allows you to easily load configuration from various types of configuration files and inject them into various types of objects, such as classes, dictionaries, functions, and methods.',
     'long_description': "# Configloaders\n\nConfigloaders is a Python library that allows you to easily load configuration from various types of configuration files and inject them into various types of objects, such as classes, dictionaries, functions, and methods.\n\n## Installation\n\nYou can install Configloaders using pip:\n\n```bash\npip install configloaders\n```\n\n## Usage\n\n### Loading configuration from a file\n\nConfigloaders supports loading configuration from various types of configuration files, including YAML, JSON, INI, and Python files.\n\n```python\nimport configloaders\n\nname = 'jack'\nage = 18\n\nconfigloaders.load(globals())\n```\n\n### Injecting configuration into an object or class\n\nConfigloaders supports injecting configuration into various types of objects, including classes, dictionaries, functions, and methods.\n\n```python\nimport configloaders\n\n@configloaders.config\nclass config:\n    name = 'jack'\n    age = 18\n```\n\n### Using configuration in a function or method\n\nConfigloaders supports using configuration in a function or method by using the `@config` decorator.\n\n```python\nimport configloaders\n\n@configloaders.config\ndef hello(name, age):\n    print(name, age)\n```\n\n### Supported file formats\n\nConfigloaders supports the following file formats:\n\n- JSON\n- INI\n- PICKLE\n- PY\n- TOML\n- TXT\n- XML\n- YAML\n\n### Supported object types\n\nConfigloaders supports the following object types:\n\n- Classes\n- Dictionaries\n- Functions\n- Methods\n- argparse.ArgumentParser\n\n## Contributing\n\nIf you would like to contribute to Configloaders, please submit a pull request or open an issue on GitHub.\n\n## License\n\nConfigloaders is licensed under the MIT License. See the LICENSE file for more information.",
     'author': 'jawide',
     'author_email': '596929059@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `configloaders-2.2.1/PKG-INFO` & `configloaders-2.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configloaders
-Version: 2.2.1
+Version: 2.2.2
 Summary: Configloaders is a Python library that allows you to easily load configuration from various types of configuration files and inject them into various types of objects, such as classes, dictionaries, functions, and methods.
 Author: jawide
 Author-email: 596929059@qq.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

