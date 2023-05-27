# Comparing `tmp/ss_logger-0.1.1.tar.gz` & `tmp/ss_logger-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ss_logger-0.1.1.tar", last modified: Sat May 27 17:16:48 2023, max compression
+gzip compressed data, was "ss_logger-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ss_logger-0.1.1.tar` & `ss_logger-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,4 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 17:16:48.866037 ss_logger-0.1.1/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-05-27 17:16:48.865758 ss_logger-0.1.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-27 17:16:48.866122 ss_logger-0.1.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      302 2023-05-27 17:16:13.000000 ss_logger-0.1.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 17:16:48.863214 ss_logger-0.1.1/ss_logger/
--rwxrwxrwx   0 root         (0) root         (0)     1295 2023-05-27 17:11:46.000000 ss_logger-0.1.1/ss_logger/CommonLogger.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 17:12:25.000000 ss_logger-0.1.1/ss_logger/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 17:16:48.865286 ss_logger-0.1.1/ss_logger.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-05-27 17:16:48.000000 ss_logger-0.1.1/ss_logger.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      220 2023-05-27 17:16:48.000000 ss_logger-0.1.1/ss_logger.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-27 17:16:48.000000 ss_logger-0.1.1/ss_logger.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2023-05-27 17:16:48.000000 ss_logger-0.1.1/ss_logger.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2023-05-27 17:16:48.000000 ss_logger-0.1.1/ss_logger.egg-info/top_level.txt
+-rwxr-xr-x   0        0        0       37 2023-05-27 17:28:57.645959 ss_logger-0.2.1/README.md
+-rwxr-xr-x   0        0        0      385 2023-05-27 17:28:57.650892 ss_logger-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0     1298 2023-05-27 17:33:11.722880 ss_logger-0.2.1/ss_logger/__init__.py
+-rw-r--r--   0        0        0      299 1970-01-01 00:00:00.000000 ss_logger-0.2.1/PKG-INFO
```

### Comparing `ss_logger-0.1.1/ss_logger/CommonLogger.py` & `ss_logger-0.2.1/ss_logger/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+"""
+This is the ss_logger module.
+Here you can add a description of what your module does.
+"""
+__version__ = "0.2.1"
+
 import logging
 import os
 from snakecase import convert
 from logging.handlers import RotatingFileHandler
-projectRootDirPath = os.path.dirname(os.path.abspath(__file__))
 
 def get_log_file_name(class_obj_or_name):
     if isinstance(class_obj_or_name, str):
         class_name = class_obj_or_name
     else:
         class_name = class_obj_or_name.__name__
     return convert(class_name) + '.log'
 
-def config_common_logger(filename, log_level=logging.DEBUG,
-                         log_format='%(asctime)s - %(name)s - %(levelname)s - %(message)s'):
+def config_common_logger(filename,projectRootDirPath,log_level=logging.DEBUG, log_format='%(asctime)s - %(name)s - %(levelname)s - %(message)s'):
     # Configure rotating file handler
     log_path = os.path.join(projectRootDirPath, 'logs', filename)
     max_file_size = 1000000 # 1 MB
     backup_count = 10
-    rotating_handler = RotatingFileHandler(log_path, maxBytes=max_file_size,
-                                            backupCount=backup_count)
+    rotating_handler = RotatingFileHandler(log_path, maxBytes=max_file_size, backupCount=backup_count)
     rotating_handler.setFormatter(logging.Formatter(log_format))
 
     # Configure console handler
     console_handler = logging.StreamHandler()
     console_handler.setLevel(log_level)
     console_handler.setFormatter(logging.Formatter(log_format))
```

