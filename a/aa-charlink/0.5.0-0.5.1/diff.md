# Comparing `tmp/aa-charlink-0.5.0.tar.gz` & `tmp/aa-charlink-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-charlink-0.5.0.tar", last modified: Thu May 25 12:54:43 2023, max compression
+gzip compressed data, was "aa-charlink-0.5.1.tar", last modified: Fri May 26 13:15:11 2023, max compression
```

## Comparing `aa-charlink-0.5.0.tar` & `aa-charlink-0.5.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.776608 aa-charlink-0.5.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-25 12:54:43.776608 aa-charlink-0.5.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.768608 aa-charlink-0.5.0/aa_charlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-25 12:54:43.000000 aa-charlink-0.5.0/aa_charlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-25 12:54:43.000000 aa-charlink-0.5.0/aa_charlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:54:43.000000 aa-charlink-0.5.0/aa_charlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:54:43.000000 aa-charlink-0.5.0/aa_charlink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 12:54:43.000000 aa-charlink-0.5.0/aa_charlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 12:54:43.000000 aa-charlink-0.5.0/aa_charlink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.772608 aa-charlink-0.5.0/charlink/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1703 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/app_imports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      108 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/app_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/apps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/auth_hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.772608 aa-charlink-0.5.0/charlink/imports/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.772608 aa-charlink-0.5.0/charlink/imports/allianceauth/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/allianceauth/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/allianceauth/corputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/corpstats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/corptools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1319 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/memberaudit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      844 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/miningtaxes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/moonmining.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/moonstuff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4599 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.772608 aa-charlink-0.5.0/charlink/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/migrations/0001_initial.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/migrations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.768608 aa-charlink-0.5.0/charlink/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.776608 aa-charlink-0.5.0/charlink/templates/charlink/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templates/charlink/app_audit.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3656 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templates/charlink/audit.html
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templates/charlink/base_audit.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3786 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templates/charlink/charlink.html
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templates/charlink/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templates/charlink/user_audit.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.776608 aa-charlink-0.5.0/charlink/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templatetags/charlinkutils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/urls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8715 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-05-25 12:54:43.776608 aa-charlink-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:15:11.680012 aa-charlink-0.5.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-26 13:15:11.680012 aa-charlink-0.5.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:15:11.680012 aa-charlink-0.5.1/aa_charlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-26 13:15:11.000000 aa-charlink-0.5.1/aa_charlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-26 13:15:11.000000 aa-charlink-0.5.1/aa_charlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:15:11.000000 aa-charlink-0.5.1/aa_charlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:15:11.000000 aa-charlink-0.5.1/aa_charlink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 13:15:11.000000 aa-charlink-0.5.1/aa_charlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 13:15:11.000000 aa-charlink-0.5.1/aa_charlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:15:11.680012 aa-charlink-0.5.1/charlink/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1703 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/app_imports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      108 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/app_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/apps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/auth_hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:15:11.680012 aa-charlink-0.5.1/charlink/imports/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/imports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:15:11.680012 aa-charlink-0.5.1/charlink/imports/allianceauth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/imports/allianceauth/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/imports/allianceauth/corputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/imports/corpstats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/imports/corptools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1319 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/imports/memberaudit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      844 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/imports/miningtaxes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/imports/moonmining.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/imports/moonstuff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4599 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/imports/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:15:11.680012 aa-charlink-0.5.1/charlink/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/migrations/0001_initial.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/migrations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:15:11.676012 aa-charlink-0.5.1/charlink/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:15:11.680012 aa-charlink-0.5.1/charlink/templates/charlink/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/templates/charlink/app_audit.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3656 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/templates/charlink/audit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/templates/charlink/base_audit.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3786 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/templates/charlink/charlink.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/templates/charlink/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/templates/charlink/user_audit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:15:11.680012 aa-charlink-0.5.1/charlink/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/templatetags/charlinkutils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9274 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/charlink/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-05-26 13:14:56.000000 aa-charlink-0.5.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1607 2023-05-26 13:15:11.684012 aa-charlink-0.5.1/setup.cfg
```

### Comparing `aa-charlink-0.5.0/LICENSE` & `aa-charlink-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/PKG-INFO` & `aa-charlink-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-charlink
-Version: 0.5.0
+Version: 0.5.1
 Summary: Character Linker for Alliance Auth
 Home-page: https://github.com/Maestro-Zacht/aa-charlink
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,allianceauth_charlink,charlink,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `aa-charlink-0.5.0/README.md` & `aa-charlink-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/aa_charlink.egg-info/PKG-INFO` & `aa-charlink-0.5.1/aa_charlink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-charlink
-Version: 0.5.0
+Version: 0.5.1
 Summary: Character Linker for Alliance Auth
 Home-page: https://github.com/Maestro-Zacht/aa-charlink
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,allianceauth_charlink,charlink,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `aa-charlink-0.5.0/aa_charlink.egg-info/SOURCES.txt` & `aa-charlink-0.5.1/aa_charlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/app_imports.py` & `aa-charlink-0.5.1/charlink/app_imports.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/forms.py` & `aa-charlink-0.5.1/charlink/forms.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/imports/allianceauth/corputils.py` & `aa-charlink-0.5.1/charlink/imports/allianceauth/corputils.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/imports/corpstats.py` & `aa-charlink-0.5.1/charlink/imports/corpstats.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/imports/corptools.py` & `aa-charlink-0.5.1/charlink/imports/corptools.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/imports/memberaudit.py` & `aa-charlink-0.5.1/charlink/imports/memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/imports/miningtaxes.py` & `aa-charlink-0.5.1/charlink/imports/miningtaxes.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/imports/moonmining.py` & `aa-charlink-0.5.1/charlink/imports/moonmining.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/imports/moonstuff.py` & `aa-charlink-0.5.1/charlink/imports/moonstuff.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/imports/structures.py` & `aa-charlink-0.5.1/charlink/imports/structures.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/migrations/0001_initial.py` & `aa-charlink-0.5.1/charlink/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/templates/charlink/app_audit.html` & `aa-charlink-0.5.1/charlink/templates/charlink/app_audit.html`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/templates/charlink/audit.html` & `aa-charlink-0.5.1/charlink/templates/charlink/audit.html`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/templates/charlink/base_audit.html` & `aa-charlink-0.5.1/charlink/templates/charlink/base_audit.html`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/templates/charlink/charlink.html` & `aa-charlink-0.5.1/charlink/templates/charlink/charlink.html`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/templates/charlink/search.html` & `aa-charlink-0.5.1/charlink/templates/charlink/search.html`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/templates/charlink/user_audit.html` & `aa-charlink-0.5.1/charlink/templates/charlink/user_audit.html`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/templatetags/charlinkutils.py` & `aa-charlink-0.5.1/charlink/templatetags/charlinkutils.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.5.0/charlink/views.py` & `aa-charlink-0.5.1/charlink/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from django.shortcuts import render, redirect, get_object_or_404
 from django.contrib.auth.decorators import login_required
-from django.contrib.auth.models import User
+from django.contrib.auth.models import User, Permission
 from django.contrib import messages
 from django.db.models import Exists, OuterRef, Q
 from django.core.exceptions import PermissionDenied
 from django.http import Http404
 
 from allianceauth.services.hooks import get_extension_logger
 from allianceauth.eveonline.models import EveCharacter, EveCorporationInfo
 from allianceauth.authentication.decorators import permissions_required
 from allianceauth.authentication.models import CharacterOwnership
 
+from app_utils.allianceauth import users_with_permission
+
 from .forms import LinkForm
 from .app_imports import import_apps
 from .decorators import charlink
 from .app_settings import CHARLINK_IGNORE_APPS
 
 logger = get_extension_logger(__name__)
 
@@ -269,18 +271,34 @@
     app_data = imported_apps[app]
 
     if not request.user.has_perms(app_data['permissions']):
         raise PermissionDenied('You do not have permission to view the selected application statistics.')
 
     corps = get_visible_corps(request.user)
 
+    queries = []
+    for perm in app_data['permissions']:
+        app_label, codename = perm.split('.')
+        perm_obj = Permission.objects.get(content_type__app_label=app_label, codename=codename)
+
+        queries.append(Q(character_ownership__user__in=users_with_permission(perm_obj)))
+
+    if len(queries) == 0:
+        perm_query = Q(character_ownership__isnull=False)
+    else:
+        perm_query = queries.pop()
+        for query in queries:
+            perm_query |= query
+
     visible_characters = EveCharacter.objects.filter(
-        Q(corporation_id__in=corps.values('corporation_id')) |
-        Q(character_ownership__user__profile__main_character__corporation_id__in=corps.values('corporation_id')),
-        character_ownership__isnull=False,
+        (
+            Q(corporation_id__in=corps.values('corporation_id')) |
+            Q(character_ownership__user__profile__main_character__corporation_id__in=corps.values('corporation_id'))
+        ) &
+        perm_query,
     ).select_related('character_ownership__user__profile__main_character')
 
     visible_characters = chars_annotate_linked_apps(
         visible_characters,
         {app: app_data}
     ).order_by(app, 'character_name')
```

### Comparing `aa-charlink-0.5.0/setup.cfg` & `aa-charlink-0.5.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.5.0
+current_version = 0.5.1
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(b(?P<beta>\d+))?
 serialize = 
 	{major}.{minor}.{patch}b{beta}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
 sign_tags = True
@@ -45,14 +45,15 @@
 url = https://github.com/Maestro-Zacht/aa-charlink
 
 [options]
 packages = find:
 python_requires = ~=3.8
 install_requires = 
 	allianceauth~=3.0
+	allianceauth-app-utils~=1.14
 include_package_data = True
 zip_safe = False
 
 [options.packages.find]
 include = charlink*
 
 [bdist_wheel]
```

