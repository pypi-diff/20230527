# Comparing `tmp/django-grip-3.2.0.tar.gz` & `tmp/django-grip-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-grip-3.2.0.tar", last modified: Wed Aug 17 01:15:50 2022, max compression
+gzip compressed data, was "django-grip-3.3.0.tar", last modified: Sat May 27 00:49:53 2023, max compression
```

## Comparing `django-grip-3.2.0.tar` & `django-grip-3.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2022-08-17 01:15:50.896367 django-grip-3.2.0/
--rw-r--r--   0 jkarneges   (501) staff       (20)     1056 2022-06-17 18:20:45.000000 django-grip-3.2.0/COPYING
--rw-r--r--   0 jkarneges   (501) staff       (20)      333 2022-08-17 01:15:50.896539 django-grip-3.2.0/PKG-INFO
--rw-r--r--   0 jkarneges   (501) staff       (20)     5974 2022-06-17 18:20:45.000000 django-grip-3.2.0/README.md
-drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2022-08-17 01:15:50.896120 django-grip-3.2.0/django_grip.egg-info/
--rw-r--r--   0 jkarneges   (501) staff       (20)      333 2022-08-17 01:15:50.000000 django-grip-3.2.0/django_grip.egg-info/PKG-INFO
--rw-r--r--   0 jkarneges   (501) staff       (20)      225 2022-08-17 01:15:50.000000 django-grip-3.2.0/django_grip.egg-info/SOURCES.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)        1 2022-08-17 01:15:50.000000 django-grip-3.2.0/django_grip.egg-info/dependency_links.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)       83 2022-08-17 01:15:50.000000 django-grip-3.2.0/django_grip.egg-info/requires.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)       12 2022-08-17 01:15:50.000000 django-grip-3.2.0/django_grip.egg-info/top_level.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)    10731 2022-08-17 01:15:17.000000 django-grip-3.2.0/django_grip.py
--rw-r--r--   0 jkarneges   (501) staff       (20)       79 2022-08-17 01:15:50.897003 django-grip-3.2.0/setup.cfg
--rw-r--r--   0 jkarneges   (501) staff       (20)      479 2022-08-17 01:15:17.000000 django-grip-3.2.0/setup.py
+drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-05-27 00:49:53.182755 django-grip-3.3.0/
+-rw-r--r--   0 jkarneges   (501) staff       (20)     1056 2022-06-17 18:20:45.000000 django-grip-3.3.0/COPYING
+-rw-r--r--   0 jkarneges   (501) staff       (20)      333 2023-05-27 00:49:53.182944 django-grip-3.3.0/PKG-INFO
+-rw-r--r--   0 jkarneges   (501) staff       (20)     5974 2022-06-17 18:20:45.000000 django-grip-3.3.0/README.md
+drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-05-27 00:49:53.182368 django-grip-3.3.0/django_grip.egg-info/
+-rw-r--r--   0 jkarneges   (501) staff       (20)      333 2023-05-27 00:49:52.000000 django-grip-3.3.0/django_grip.egg-info/PKG-INFO
+-rw-r--r--   0 jkarneges   (501) staff       (20)      225 2023-05-27 00:49:53.000000 django-grip-3.3.0/django_grip.egg-info/SOURCES.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)        1 2023-05-27 00:49:52.000000 django-grip-3.3.0/django_grip.egg-info/dependency_links.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)       81 2023-05-27 00:49:53.000000 django-grip-3.3.0/django_grip.egg-info/requires.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)       12 2023-05-27 00:49:53.000000 django-grip-3.3.0/django_grip.egg-info/top_level.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)    10731 2022-08-17 01:15:17.000000 django-grip-3.3.0/django_grip.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)       79 2023-05-27 00:49:53.183564 django-grip-3.3.0/setup.cfg
+-rw-r--r--   0 jkarneges   (501) staff       (20)      477 2023-05-27 00:49:47.000000 django-grip-3.3.0/setup.py
```

### Comparing `django-grip-3.2.0/COPYING` & `django-grip-3.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `django-grip-3.2.0/README.md` & `django-grip-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-grip-3.2.0/django_grip.py` & `django-grip-3.3.0/django_grip.py`

 * *Files identical despite different names*

