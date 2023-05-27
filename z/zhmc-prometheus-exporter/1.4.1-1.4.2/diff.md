# Comparing `tmp/zhmc_prometheus_exporter-1.4.1.tar.gz` & `tmp/zhmc_prometheus_exporter-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhmc_prometheus_exporter-1.4.1.tar", last modified: Thu Apr 27 07:05:47 2023, max compression
+gzip compressed data, was "zhmc_prometheus_exporter-1.4.2.tar", last modified: Sat May 27 03:30:56 2023, max compression
```

## Comparing `zhmc_prometheus_exporter-1.4.1.tar` & `zhmc_prometheus_exporter-1.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:05:47.139525 zhmc_prometheus_exporter-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-27 07:04:49.000000 zhmc_prometheus_exporter-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-27 07:05:24.000000 zhmc_prometheus_exporter-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-27 07:05:47.139525 zhmc_prometheus_exporter-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-04-27 07:04:49.000000 zhmc_prometheus_exporter-1.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-27 07:04:49.000000 zhmc_prometheus_exporter-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 07:05:47.139525 zhmc_prometheus_exporter-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-27 07:04:49.000000 zhmc_prometheus_exporter-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:05:47.139525 zhmc_prometheus_exporter-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18580 2023-04-27 07:04:49.000000 zhmc_prometheus_exporter-1.4.1/tests/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:05:47.139525 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-27 07:04:49.000000 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-27 07:04:49.000000 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:05:47.139525 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-27 07:04:49.000000 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter/schemas/hmccreds_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-04-27 07:04:49.000000 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter/schemas/metrics_schema.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    69323 2023-04-27 07:04:49.000000 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter/zhmc_prometheus_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:05:47.139525 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-27 07:05:47.000000 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-27 07:05:47.000000 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:05:47.000000 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-27 07:05:47.000000 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-27 07:05:47.000000 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 07:05:47.000000 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:05:46.000000 zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:30:56.122473 zhmc_prometheus_exporter-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-27 03:30:13.000000 zhmc_prometheus_exporter-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-27 03:30:45.000000 zhmc_prometheus_exporter-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-27 03:30:56.122473 zhmc_prometheus_exporter-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-27 03:30:13.000000 zhmc_prometheus_exporter-1.4.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-27 03:30:13.000000 zhmc_prometheus_exporter-1.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 03:30:56.122473 zhmc_prometheus_exporter-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-27 03:30:13.000000 zhmc_prometheus_exporter-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:30:56.118473 zhmc_prometheus_exporter-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18580 2023-05-27 03:30:13.000000 zhmc_prometheus_exporter-1.4.2/tests/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:30:56.118473 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-27 03:30:13.000000 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-27 03:30:13.000000 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:30:56.122473 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-27 03:30:13.000000 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter/schemas/hmccreds_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-05-27 03:30:13.000000 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter/schemas/metrics_schema.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    69813 2023-05-27 03:30:13.000000 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter/zhmc_prometheus_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:30:56.122473 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-27 03:30:56.000000 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-27 03:30:56.000000 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 03:30:56.000000 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-27 03:30:56.000000 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-27 03:30:56.000000 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 03:30:56.000000 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 03:30:55.000000 zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter.egg-info/zip-safe
```

### Comparing `zhmc_prometheus_exporter-1.4.1/LICENSE` & `zhmc_prometheus_exporter-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.4.1/PKG-INFO` & `zhmc_prometheus_exporter-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmc_prometheus_exporter
-Version: 1.4.1
+Version: 1.4.2
 Summary: IBM Z HMC Prometheus Exporter
 Home-page: https://github.com/zhmcclient/zhmc-prometheus-exporter
 Author: Jakob Naucke
 Author-email: jakob.naucke@ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmc_prometheus_exporter-1.4.1/README.rst` & `zhmc_prometheus_exporter-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.4.1/requirements.txt` & `zhmc_prometheus_exporter-1.4.2/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 #
 # The order of packages is significant, because pip processes them in the order
 # of appearance.
 #
 
 # Direct dependencies for runtime (must be consistent with minimum-constraints.txt)
 
-# zhmcclient @ git+https://github.com/zhmcclient/python-zhmcclient.git@master
-zhmcclient>=1.7.0
+# zhmcclient @ git+https://github.com/zhmcclient/python-zhmcclient.git@stable_1.8
+zhmcclient>=1.8.1
 
 prometheus-client>=0.9.0
 urllib3>=1.25.9; python_version <= '3.9'
 urllib3>=1.26.5; python_version >= '3.10'
 jsonschema>=3.2.0
 six>=1.14.0; python_version <= '3.9'
 six>=1.16.0; python_version >= '3.10'
```

### Comparing `zhmc_prometheus_exporter-1.4.1/setup.py` & `zhmc_prometheus_exporter-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.4.1/tests/test_all.py` & `zhmc_prometheus_exporter-1.4.2/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter/__init__.py` & `zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter/_version.py` & `zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter/_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.P.dev1": A not yet released version M.N.P
 #: * "M.N.P": A released version M.N.P
-__version__ = '1.4.1'
+__version__ = '1.4.2'
```

### Comparing `zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter/schemas/hmccreds_schema.yaml` & `zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter/schemas/hmccreds_schema.yaml`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter/schemas/metrics_schema.yaml` & `zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter/schemas/metrics_schema.yaml`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter/zhmc_prometheus_exporter.py` & `zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter/zhmc_prometheus_exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1307,35 +1307,43 @@
             while True:
                 logprint(logging.DEBUG, None,
                          "Fetching metrics from HMC")
                 try:
                     metrics_object = retrieve_metrics(self.context)
                 except zhmcclient.HTTPError as exc:
                     if exc.http_status == 404 and exc.reason == 1:
-                        logprint(logging.INFO, PRINT_V,
+                        logprint(logging.WARNING, PRINT_ALWAYS,
                                  "Recreating the metrics context after HTTP "
                                  "status {}.{}".
                                  format(exc.http_status, exc.reason))
                         self.context, _ = create_metrics_context(
                             self.session, self.yaml_metric_groups,
                             self.hmc_version)
                         continue
                     logprint(logging.WARNING, PRINT_ALWAYS,
                              "Retrying after HTTP status {}.{}: {}".
                              format(exc.http_status, exc.reason, exc))
                     time.sleep(RETRY_SLEEP_TIME)
                     continue
                 except zhmcclient.ConnectionError as exc:
                     logprint(logging.WARNING, PRINT_ALWAYS,
-                             "Retrying after Connection error: {}".format(exc))
+                             "Retrying after connection error: {}".format(exc))
                     time.sleep(RETRY_SLEEP_TIME)
                     continue
-                except zhmcclient.AuthError as exc:
+                except zhmcclient.ServerAuthError as exc:
+                    http_exc = exc.details  # zhmcclient.HTTPError
+                    logprint(logging.WARNING, PRINT_ALWAYS,
+                             "Retrying after server authentication error with "
+                             "HTTP status {}.{}".
+                             format(http_exc.http_status, http_exc.reason))
+                    time.sleep(RETRY_SLEEP_TIME)
+                    continue
+                except zhmcclient.ClientAuthError as exc:
                     logprint(logging.ERROR, PRINT_ALWAYS,
-                             "Abandoning after Authentication error: {}".
+                             "Abandoning after client authentication error: {}".
                              format(exc))
                     raise
                 # pylint: disable=broad-exception-caught,broad-except
                 except Exception as exc:
                     logprint(logging.ERROR, PRINT_ALWAYS,
                              "Abandoning after exception {}: {}".
                              format(exc.__class__.__name__, exc))
```

### Comparing `zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter.egg-info/PKG-INFO` & `zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmc-prometheus-exporter
-Version: 1.4.1
+Version: 1.4.2
 Summary: IBM Z HMC Prometheus Exporter
 Home-page: https://github.com/zhmcclient/zhmc-prometheus-exporter
 Author: Jakob Naucke
 Author-email: jakob.naucke@ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmc_prometheus_exporter-1.4.1/zhmc_prometheus_exporter.egg-info/SOURCES.txt` & `zhmc_prometheus_exporter-1.4.2/zhmc_prometheus_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

