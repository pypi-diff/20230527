# Comparing `tmp/robotframework-kubelibrary-0.8.5.tar.gz` & `tmp/robotframework-kubelibrary-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-kubelibrary-0.8.5.tar", last modified: Sat Apr 22 07:04:23 2023, max compression
+gzip compressed data, was "robotframework-kubelibrary-0.8.6.tar", last modified: Sat May 27 07:57:23 2023, max compression
```

## Comparing `robotframework-kubelibrary-0.8.5.tar` & `robotframework-kubelibrary-0.8.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6871 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6213 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/src/KubeLibrary/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61132 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/src/KubeLibrary/KubeLibrary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/src/KubeLibrary/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/src/KubeLibrary/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/src/KubeLibrary/version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6871 2023-04-22 07:04:23.000000 robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-04-22 07:04:23.000000 robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-22 07:04:23.000000 robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2023-04-22 07:04:23.000000 robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-04-22 07:04:23.000000 robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42996 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/test/test_KubeLibrary.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-27 07:57:23.290898 robotframework-kubelibrary-0.8.6/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2023-05-27 07:57:17.000000 robotframework-kubelibrary-0.8.6/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6871 2023-05-27 07:57:23.290898 robotframework-kubelibrary-0.8.6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6213 2023-05-27 07:57:17.000000 robotframework-kubelibrary-0.8.6/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-27 07:57:23.290898 robotframework-kubelibrary-0.8.6/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-05-27 07:57:17.000000 robotframework-kubelibrary-0.8.6/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-27 07:57:23.286898 robotframework-kubelibrary-0.8.6/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-27 07:57:23.286898 robotframework-kubelibrary-0.8.6/src/KubeLibrary/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61815 2023-05-27 07:57:17.000000 robotframework-kubelibrary-0.8.6/src/KubeLibrary/KubeLibrary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2023-05-27 07:57:17.000000 robotframework-kubelibrary-0.8.6/src/KubeLibrary/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-05-27 07:57:17.000000 robotframework-kubelibrary-0.8.6/src/KubeLibrary/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2023-05-27 07:57:17.000000 robotframework-kubelibrary-0.8.6/src/KubeLibrary/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-27 07:57:23.286898 robotframework-kubelibrary-0.8.6/src/robotframework_kubelibrary.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6871 2023-05-27 07:57:23.000000 robotframework-kubelibrary-0.8.6/src/robotframework_kubelibrary.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-05-27 07:57:23.000000 robotframework-kubelibrary-0.8.6/src/robotframework_kubelibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-27 07:57:23.000000 robotframework-kubelibrary-0.8.6/src/robotframework_kubelibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2023-05-27 07:57:23.000000 robotframework-kubelibrary-0.8.6/src/robotframework_kubelibrary.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-27 07:57:23.000000 robotframework-kubelibrary-0.8.6/src/robotframework_kubelibrary.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-27 07:57:23.290898 robotframework-kubelibrary-0.8.6/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42996 2023-05-27 07:57:17.000000 robotframework-kubelibrary-0.8.6/test/test_KubeLibrary.py
```

### Comparing `robotframework-kubelibrary-0.8.5/LICENSE` & `robotframework-kubelibrary-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-kubelibrary-0.8.5/PKG-INFO` & `robotframework-kubelibrary-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-kubelibrary
-Version: 0.8.5
+Version: 0.8.6
 Summary: Kubernetes library for Robot Framework
 Home-page: https://github.com/devopsspiral/KubeLibrary
 Author: Michał Wcisło
 Author-email: mwcislo999@gmail.com
 License: MIT
 Keywords: robotframework testing test automation kubernetes
 Platform: UNKNOWN
```

### Comparing `robotframework-kubelibrary-0.8.5/README.md` & `robotframework-kubelibrary-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-kubelibrary-0.8.5/setup.py` & `robotframework-kubelibrary-0.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-kubelibrary-0.8.5/src/KubeLibrary/KubeLibrary.py` & `robotframework-kubelibrary-0.8.6/src/KubeLibrary/KubeLibrary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1590,14 +1590,34 @@
 
         As in ``GET /apis/{group}/{version}/namespaces/{namespace}/{plural}/{name}``
 
         https://github.com/kubernetes-client/python/blob/master/kubernetes/README.md
         """
         return self.custom_object.get_namespaced_custom_object(group, version, namespace, plural, name)
 
+    def list_namespaced_custom_object(self, group, version, namespace, plural):
+        """List custom objects in namespace.
+
+        Returns an object.
+
+        - ``group``:
+          API Group, e.g. 'k8s.cni.cncf.io'
+        - ``version``:
+          API version, e.g. 'v1'
+        - ``namespace``:
+          Namespace, e.g. 'default'
+        - ``plural``:
+          e.g. 'network-attachment-definitions'
+
+        As in ``GET /apis/{group}/{version}/namespaces/{namespace}/{plural}``
+
+        https://github.com/kubernetes-client/python/blob/master/kubernetes/README.md
+        """
+        return self.custom_object.list_namespaced_custom_object(group, version, namespace, plural)
+
     def get_custom_object_in_namespace(self, group, version, namespace, plural, name):
         """*DEPRECATED* Will be removed in v1.0.0. Use get_namespaced_custom_object.
 
         Get custom object in namespace.
 
         Returns an object.
```

### Comparing `robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/PKG-INFO` & `robotframework-kubelibrary-0.8.6/src/robotframework_kubelibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-kubelibrary
-Version: 0.8.5
+Version: 0.8.6
 Summary: Kubernetes library for Robot Framework
 Home-page: https://github.com/devopsspiral/KubeLibrary
 Author: Michał Wcisło
 Author-email: mwcislo999@gmail.com
 License: MIT
 Keywords: robotframework testing test automation kubernetes
 Platform: UNKNOWN
```

### Comparing `robotframework-kubelibrary-0.8.5/test/test_KubeLibrary.py` & `robotframework-kubelibrary-0.8.6/test/test_KubeLibrary.py`

 * *Files identical despite different names*

