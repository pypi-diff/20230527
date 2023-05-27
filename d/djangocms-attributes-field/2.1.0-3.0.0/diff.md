# Comparing `tmp/djangocms-attributes-field-2.1.0.tar.gz` & `tmp/djangocms-attributes-field-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-attributes-field-2.1.0.tar", last modified: Tue Apr  5 13:48:30 2022, max compression
+gzip compressed data, was "djangocms-attributes-field-3.0.0.tar", last modified: Sat May 27 06:47:59 2023, max compression
```

## Comparing `djangocms-attributes-field-2.1.0.tar` & `djangocms-attributes-field-3.0.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 mwalker    (501) staff       (20)        0 2022-04-05 13:48:30.195633 djangocms-attributes-field-2.1.0/
--rw-r--r--   0 mwalker    (501) staff       (20)     1475 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/LICENSE
--rw-r--r--   0 mwalker    (501) staff       (20)     7626 2022-04-05 13:48:30.194939 djangocms-attributes-field-2.1.0/PKG-INFO
--rw-r--r--   0 mwalker    (501) staff       (20)     6241 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/README.rst
-drwxr-xr-x   0 mwalker    (501) staff       (20)        0 2022-04-05 13:48:30.166459 djangocms-attributes-field-2.1.0/djangocms_attributes_field/
--rw-r--r--   0 mwalker    (501) staff       (20)       22 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/djangocms_attributes_field/__init__.py
--rw-r--r--   0 mwalker    (501) staff       (20)     8348 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/djangocms_attributes_field/fields.py
--rw-r--r--   0 mwalker    (501) staff       (20)       27 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/djangocms_attributes_field/models.py
--rw-r--r--   0 mwalker    (501) staff       (20)     8318 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/djangocms_attributes_field/widgets.py
-drwxr-xr-x   0 mwalker    (501) staff       (20)        0 2022-04-05 13:48:30.181830 djangocms-attributes-field-2.1.0/djangocms_attributes_field.egg-info/
--rw-r--r--   0 mwalker    (501) staff       (20)     7626 2022-04-05 13:48:29.000000 djangocms-attributes-field-2.1.0/djangocms_attributes_field.egg-info/PKG-INFO
--rw-r--r--   0 mwalker    (501) staff       (20)      788 2022-04-05 13:48:30.000000 djangocms-attributes-field-2.1.0/djangocms_attributes_field.egg-info/SOURCES.txt
--rw-r--r--   0 mwalker    (501) staff       (20)        1 2022-04-05 13:48:29.000000 djangocms-attributes-field-2.1.0/djangocms_attributes_field.egg-info/dependency_links.txt
--rw-r--r--   0 mwalker    (501) staff       (20)        1 2022-04-05 13:44:12.000000 djangocms-attributes-field-2.1.0/djangocms_attributes_field.egg-info/not-zip-safe
--rw-r--r--   0 mwalker    (501) staff       (20)       43 2022-04-05 13:48:29.000000 djangocms-attributes-field-2.1.0/djangocms_attributes_field.egg-info/requires.txt
--rw-r--r--   0 mwalker    (501) staff       (20)       33 2022-04-05 13:48:30.000000 djangocms-attributes-field-2.1.0/djangocms_attributes_field.egg-info/top_level.txt
--rw-r--r--   0 mwalker    (501) staff       (20)       38 2022-04-05 13:48:30.195844 djangocms-attributes-field-2.1.0/setup.cfg
--rw-r--r--   0 mwalker    (501) staff       (20)     1723 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/setup.py
-drwxr-xr-x   0 mwalker    (501) staff       (20)        0 2022-04-05 13:48:30.187787 djangocms-attributes-field-2.1.0/tests/
--rw-r--r--   0 mwalker    (501) staff       (20)        0 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/tests/__init__.py
--rwxr-xr-x   0 mwalker    (501) staff       (20)      445 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/tests/settings.py
-drwxr-xr-x   0 mwalker    (501) staff       (20)        0 2022-04-05 13:48:30.191969 djangocms-attributes-field-2.1.0/tests/test_app/
--rw-r--r--   0 mwalker    (501) staff       (20)       22 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/tests/test_app/__init__.py
--rw-r--r--   0 mwalker    (501) staff       (20)      354 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/tests/test_app/cms_plugins.py
--rw-r--r--   0 mwalker    (501) staff       (20)      506 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/tests/test_app/forms.py
-drwxr-xr-x   0 mwalker    (501) staff       (20)        0 2022-04-05 13:48:30.194233 djangocms-attributes-field-2.1.0/tests/test_app/migrations/
--rw-r--r--   0 mwalker    (501) staff       (20)     1048 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/tests/test_app/migrations/0001_initial.py
--rw-r--r--   0 mwalker    (501) staff       (20)        0 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/tests/test_app/migrations/__init__.py
--rw-r--r--   0 mwalker    (501) staff       (20)      373 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/tests/test_app/models.py
--rw-r--r--   0 mwalker    (501) staff       (20)     3688 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/tests/test_fields.py
--rw-r--r--   0 mwalker    (501) staff       (20)      874 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/tests/test_migrations.py
--rw-r--r--   0 mwalker    (501) staff       (20)     4022 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/tests/test_plugins.py
--rw-r--r--   0 mwalker    (501) staff       (20)      703 2022-04-05 13:42:22.000000 djangocms-attributes-field-2.1.0/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:47:59.816245 djangocms-attributes-field-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-27 06:47:59.816245 djangocms-attributes-field-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:47:59.816245 djangocms-attributes-field-3.0.0/djangocms_attributes_field/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/djangocms_attributes_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/djangocms_attributes_field/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/djangocms_attributes_field/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/djangocms_attributes_field/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:47:59.816245 djangocms-attributes-field-3.0.0/djangocms_attributes_field.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-27 06:47:59.000000 djangocms-attributes-field-3.0.0/djangocms_attributes_field.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-27 06:47:59.000000 djangocms-attributes-field-3.0.0/djangocms_attributes_field.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:47:59.000000 djangocms-attributes-field-3.0.0/djangocms_attributes_field.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:47:59.000000 djangocms-attributes-field-3.0.0/djangocms_attributes_field.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 06:47:59.000000 djangocms-attributes-field-3.0.0/djangocms_attributes_field.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-27 06:47:59.000000 djangocms-attributes-field-3.0.0/djangocms_attributes_field.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 06:47:59.816245 djangocms-attributes-field-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:47:59.816245 djangocms-attributes-field-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:47:59.816245 djangocms-attributes-field-3.0.0/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/tests/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/tests/test_app/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/tests/test_app/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:47:59.816245 djangocms-attributes-field-3.0.0/tests/test_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/tests/test_app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/tests/test_app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/tests/test_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-27 06:47:50.000000 djangocms-attributes-field-3.0.0/tests/test_widgets.py
```

### Comparing `djangocms-attributes-field-2.1.0/LICENSE` & `djangocms-attributes-field-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-attributes-field-2.1.0/PKG-INFO` & `djangocms-attributes-field-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 Metadata-Version: 2.1
 Name: djangocms-attributes-field
-Version: 2.1.0
+Version: 3.0.0
 Summary: Adds attributes to Django models.
 Home-page: https://github.com/django-cms/djangocms-attributes-field/
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django CMS
-Classifier: Framework :: Django CMS :: 3.7
-Classifier: Framework :: Django CMS :: 3.8
+Classifier: Framework :: Django CMS :: 3.9
+Classifier: Framework :: Django CMS :: 3.10
+Classifier: Framework :: Django CMS :: 3.11
+Classifier: Framework :: Django CMS :: 4.1
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 ===========================
 django CMS Attributes Field
 ===========================
 
-|pypi| |build| |coverage|
+|pypi| |coverage|  |python| |django| |djangocms| |djangocms4|
+
 
 This project is an opinionated implementation of JSONField for arbitrary HTML
 element attributes.
 
 It aims to provide a sensible means of storing and managing
 arbitrary HTML element attributes for later emitting them into templates.
 
@@ -53,30 +56,30 @@
 
 To avoid these pitfalls, this package allows all of these attributes to be
 stored together in a single text field in the database as a JSON blob, but
 provides a nice widget to provide an intuitive, key/value pair interface
 and provide sensible validation of the keys used.
 
 
-.. note:: 
+.. note::
 
     This project is considered 3rd party (no supervision by the `django CMS Association <https://www.django-cms.org/en/about-us/>`_). Join us on `Slack                 <https://www.django-cms.org/slack/>`_ for more information.
 
 
 .. image:: preview.gif
 
 
 *******************************************
 Contribute to this project and win rewards
 *******************************************
 
 Because this is a an open-source project, we welcome everyone to
 `get involved in the project <https://www.django-cms.org/en/contribute/>`_ and
-`receive a reward <https://www.django-cms.org/en/bounty-program/>`_ for their contribution. 
-Become part of a fantastic community and help us make django CMS the best CMS in the world.   
+`receive a reward <https://www.django-cms.org/en/bounty-program/>`_ for their contribution.
+Become part of a fantastic community and help us make django CMS the best CMS in the world.
 
 We'll be delighted to receive your
 feedback in the form of issues and pull requests. Before submitting your
 pull request, please review our `contribution guidelines
 <http://docs.django-cms.org/en/latest/contributing/index.html>`_.
 
 We're grateful to all contributors who have helped create and maintain this package.
@@ -86,16 +89,14 @@
 
 Documentation
 =============
 
 See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-attributes-field/blob/master/setup.py>`_
 file for additional dependencies:
 
-|python| |django| |djangocms|
-
 
 Installation
 ------------
 
 For a manual install:
 
 * run ``pip install djangocms-attributes-field``
@@ -197,20 +198,17 @@
     source env/bin/activate
     pip install -r tests/requirements.txt
     python setup.py test
 
 
 .. |pypi| image:: https://badge.fury.io/py/djangocms-attributes-field.svg
     :target: http://badge.fury.io/py/djangocms-attributes-field
-.. |build| image:: https://travis-ci.org/divio/djangocms-attributes-field.svg?branch=master
-    :target: https://travis-ci.org/divio/djangocms-attributes-field
-.. |coverage| image:: https://codecov.io/gh/divio/djangocms-attributes-field/branch/master/graph/badge.svg
+.. |coverage| image:: https://codecov.io/gh/django-cms/djangocms-attributes-field/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/divio/djangocms-attributes-field
-
-.. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
+.. |python| image:: https://img.shields.io/badge/python-3.8+-blue.svg
     :target: https://pypi.org/project/djangocms-attributes-field/
-.. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
+.. |django| image:: https://img.shields.io/badge/django-3.2,%204.0--%204.2-blue.svg
     :target: https://www.djangoproject.com/
-.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
+.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.9%2B-blue.svg
+    :target: https://www.django-cms.org/
+.. |djangocms4| image:: https://img.shields.io/badge/django%20CMS-4-blue.svg
     :target: https://www.django-cms.org/
-
-
```

### Comparing `djangocms-attributes-field-2.1.0/README.rst` & `djangocms-attributes-field-3.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ===========================
 django CMS Attributes Field
 ===========================
 
-|pypi| |build| |coverage|
+|pypi| |coverage|  |python| |django| |djangocms| |djangocms4|
+
 
 This project is an opinionated implementation of JSONField for arbitrary HTML
 element attributes.
 
 It aims to provide a sensible means of storing and managing
 arbitrary HTML element attributes for later emitting them into templates.
 
@@ -18,30 +19,30 @@
 
 To avoid these pitfalls, this package allows all of these attributes to be
 stored together in a single text field in the database as a JSON blob, but
 provides a nice widget to provide an intuitive, key/value pair interface
 and provide sensible validation of the keys used.
 
 
-.. note:: 
+.. note::
 
     This project is considered 3rd party (no supervision by the `django CMS Association <https://www.django-cms.org/en/about-us/>`_). Join us on `Slack                 <https://www.django-cms.org/slack/>`_ for more information.
 
 
 .. image:: preview.gif
 
 
 *******************************************
 Contribute to this project and win rewards
 *******************************************
 
 Because this is a an open-source project, we welcome everyone to
 `get involved in the project <https://www.django-cms.org/en/contribute/>`_ and
-`receive a reward <https://www.django-cms.org/en/bounty-program/>`_ for their contribution. 
-Become part of a fantastic community and help us make django CMS the best CMS in the world.   
+`receive a reward <https://www.django-cms.org/en/bounty-program/>`_ for their contribution.
+Become part of a fantastic community and help us make django CMS the best CMS in the world.
 
 We'll be delighted to receive your
 feedback in the form of issues and pull requests. Before submitting your
 pull request, please review our `contribution guidelines
 <http://docs.django-cms.org/en/latest/contributing/index.html>`_.
 
 We're grateful to all contributors who have helped create and maintain this package.
@@ -51,16 +52,14 @@
 
 Documentation
 =============
 
 See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-attributes-field/blob/master/setup.py>`_
 file for additional dependencies:
 
-|python| |django| |djangocms|
-
 
 Installation
 ------------
 
 For a manual install:
 
 * run ``pip install djangocms-attributes-field``
@@ -162,18 +161,17 @@
     source env/bin/activate
     pip install -r tests/requirements.txt
     python setup.py test
 
 
 .. |pypi| image:: https://badge.fury.io/py/djangocms-attributes-field.svg
     :target: http://badge.fury.io/py/djangocms-attributes-field
-.. |build| image:: https://travis-ci.org/divio/djangocms-attributes-field.svg?branch=master
-    :target: https://travis-ci.org/divio/djangocms-attributes-field
-.. |coverage| image:: https://codecov.io/gh/divio/djangocms-attributes-field/branch/master/graph/badge.svg
+.. |coverage| image:: https://codecov.io/gh/django-cms/djangocms-attributes-field/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/divio/djangocms-attributes-field
-
-.. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
+.. |python| image:: https://img.shields.io/badge/python-3.8+-blue.svg
     :target: https://pypi.org/project/djangocms-attributes-field/
-.. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
+.. |django| image:: https://img.shields.io/badge/django-3.2,%204.0--%204.2-blue.svg
     :target: https://www.djangoproject.com/
-.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
+.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.9%2B-blue.svg
+    :target: https://www.django-cms.org/
+.. |djangocms4| image:: https://img.shields.io/badge/django%20CMS-4-blue.svg
     :target: https://www.django-cms.org/
```

### Comparing `djangocms-attributes-field-2.1.0/djangocms_attributes_field/fields.py` & `djangocms-attributes-field-3.0.0/djangocms_attributes_field/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from django.core.validators import RegexValidator
 from django.db import models
 from django.utils.html import conditional_escape, mark_safe
 from django.utils.translation import gettext_lazy as _
 
 from .widgets import AttributesWidget
 
-
-regex_key_validator = RegexValidator(regex=r'^[a-z][-a-z0-9_]*\Z',
+regex_key_validator = RegexValidator(regex=r'^[a-z][-a-z0-9_:]*\Z',
                                      flags=re.IGNORECASE, code='invalid')
 
 
 class AttributesFormField(forms.CharField):
     empty_values = [None, '']
 
     def __init__(self, *args, **kwargs):
@@ -25,15 +24,15 @@
 
     def to_python(self, value):
         if isinstance(value, str) and value:
             try:
                 return json.loads(value)
             except ValueError as exc:
                 raise forms.ValidationError(
-                    'JSON decode error: %s' % (str(exc.args[0]),)
+                    'JSON decode error: {}'.format(str(exc.args[0]))
                 )
         else:
             return value
 
     def validate(self, value):
         # This is required in older django versions.
         if value in self.empty_values and self.required:
@@ -118,15 +117,15 @@
     def contribute_to_class(self, cls, name, **kwargs):
         """
         Adds a @property: «name»_str that returns a string representation of
         the attributes ready for inclusion on an HTML element.
         """
         super().contribute_to_class(cls, name, **kwargs)
         # Make sure we're not going to clobber something that already exists.
-        property_name = '{name}_str'.format(name=name)
+        property_name = f'{name}_str'
         if not hasattr(cls, property_name):
             str_property = partial(self.to_str, field_name=name)
             setattr(cls, property_name, property(str_property))
 
     def validate(self, value, model_instance):
         if not self.null and value is None:
             raise ValidationError(self.error_messages['null'])
@@ -138,15 +137,15 @@
         for key, val in value.items():
             self.validate_key(key)
             self.validate_value(key, val)
 
     def validate_key(self, key):
         """
         A key must start with a letter, but can otherwise contain letters,
-        numbers, dashes or underscores. It must not also be part of
+        numbers, dashes, colons or underscores. It must not also be part of
         `excluded_keys` as configured in the field.
 
         :param key: (str) The key to validate
         """
         # Verify the key is not one of `excluded_keys`.
         if key.lower() in self.excluded_keys:
             raise ValidationError(
@@ -212,11 +211,11 @@
         except AttributeError:
             value_items = [value]
 
         attrs = []
         for key, val in value_items:
             if key.lower() not in excluded_keys:
                 if val:
-                    attrs.append('{key}="{value}"'.format(key=key, value=conditional_escape(val)))
+                    attrs.append(f'{key}="{conditional_escape(val)}"')
                 else:
-                    attrs.append('{key}'.format(key=key))
+                    attrs.append(f'{key}')
         return mark_safe(" ".join(attrs))
```

### Comparing `djangocms-attributes-field-2.1.0/djangocms_attributes_field/widgets.py` & `djangocms-attributes-field-3.0.0/djangocms_attributes_field/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         output = '<div class="djangocms-attributes-field">'
         if value and isinstance(value, dict) and len(value) > 0:
             for key in self.sorted(value):
                 output += self._render_row(key, value[key], name, flatatt(self.key_attrs), flatatt(self.val_attrs))
 
         # Add empty template
         output += """
-        <div class="template hidden">{0}
+        <div class="template hidden">{}
         </div>""".format(self._render_row('', '', name, flatatt(self.key_attrs), flatatt(self.val_attrs)))
 
         # Add "+" button
         output += """
         <div class="related-widget-wrapper">
             <a class="add-attributes-pair addlink" href="#" title="{title}"></a>
         </div>
@@ -190,16 +190,16 @@
         Returns the dict-representation of the key-value pairs
         sent in the POST parameters
 
         :param data: (dict) request.POST or request.GET parameters.
         :param files: (list) request.FILES
         :param name: (str) the name of the field associated with this widget.
         """
-        key_field = 'attributes_key[{0}]'.format(name)
-        val_field = 'attributes_value[{0}]'.format(name)
+        key_field = f'attributes_key[{name}]'
+        val_field = f'attributes_value[{name}]'
         if key_field in data and val_field in data:
             keys = data.getlist(key_field)
             values = data.getlist(val_field)
             return dict([item for item in zip(keys, values) if not item[0] == ''])
         return {}
 
     def value_omitted_from_data(self, data, files, name):
```

### Comparing `djangocms-attributes-field-2.1.0/djangocms_attributes_field.egg-info/PKG-INFO` & `djangocms-attributes-field-3.0.0/djangocms_attributes_field.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 Metadata-Version: 2.1
 Name: djangocms-attributes-field
-Version: 2.1.0
+Version: 3.0.0
 Summary: Adds attributes to Django models.
 Home-page: https://github.com/django-cms/djangocms-attributes-field/
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django CMS
-Classifier: Framework :: Django CMS :: 3.7
-Classifier: Framework :: Django CMS :: 3.8
+Classifier: Framework :: Django CMS :: 3.9
+Classifier: Framework :: Django CMS :: 3.10
+Classifier: Framework :: Django CMS :: 3.11
+Classifier: Framework :: Django CMS :: 4.1
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 ===========================
 django CMS Attributes Field
 ===========================
 
-|pypi| |build| |coverage|
+|pypi| |coverage|  |python| |django| |djangocms| |djangocms4|
+
 
 This project is an opinionated implementation of JSONField for arbitrary HTML
 element attributes.
 
 It aims to provide a sensible means of storing and managing
 arbitrary HTML element attributes for later emitting them into templates.
 
@@ -53,30 +56,30 @@
 
 To avoid these pitfalls, this package allows all of these attributes to be
 stored together in a single text field in the database as a JSON blob, but
 provides a nice widget to provide an intuitive, key/value pair interface
 and provide sensible validation of the keys used.
 
 
-.. note:: 
+.. note::
 
     This project is considered 3rd party (no supervision by the `django CMS Association <https://www.django-cms.org/en/about-us/>`_). Join us on `Slack                 <https://www.django-cms.org/slack/>`_ for more information.
 
 
 .. image:: preview.gif
 
 
 *******************************************
 Contribute to this project and win rewards
 *******************************************
 
 Because this is a an open-source project, we welcome everyone to
 `get involved in the project <https://www.django-cms.org/en/contribute/>`_ and
-`receive a reward <https://www.django-cms.org/en/bounty-program/>`_ for their contribution. 
-Become part of a fantastic community and help us make django CMS the best CMS in the world.   
+`receive a reward <https://www.django-cms.org/en/bounty-program/>`_ for their contribution.
+Become part of a fantastic community and help us make django CMS the best CMS in the world.
 
 We'll be delighted to receive your
 feedback in the form of issues and pull requests. Before submitting your
 pull request, please review our `contribution guidelines
 <http://docs.django-cms.org/en/latest/contributing/index.html>`_.
 
 We're grateful to all contributors who have helped create and maintain this package.
@@ -86,16 +89,14 @@
 
 Documentation
 =============
 
 See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-attributes-field/blob/master/setup.py>`_
 file for additional dependencies:
 
-|python| |django| |djangocms|
-
 
 Installation
 ------------
 
 For a manual install:
 
 * run ``pip install djangocms-attributes-field``
@@ -197,20 +198,17 @@
     source env/bin/activate
     pip install -r tests/requirements.txt
     python setup.py test
 
 
 .. |pypi| image:: https://badge.fury.io/py/djangocms-attributes-field.svg
     :target: http://badge.fury.io/py/djangocms-attributes-field
-.. |build| image:: https://travis-ci.org/divio/djangocms-attributes-field.svg?branch=master
-    :target: https://travis-ci.org/divio/djangocms-attributes-field
-.. |coverage| image:: https://codecov.io/gh/divio/djangocms-attributes-field/branch/master/graph/badge.svg
+.. |coverage| image:: https://codecov.io/gh/django-cms/djangocms-attributes-field/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/divio/djangocms-attributes-field
-
-.. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
+.. |python| image:: https://img.shields.io/badge/python-3.8+-blue.svg
     :target: https://pypi.org/project/djangocms-attributes-field/
-.. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
+.. |django| image:: https://img.shields.io/badge/django-3.2,%204.0--%204.2-blue.svg
     :target: https://www.djangoproject.com/
-.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
+.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.9%2B-blue.svg
+    :target: https://www.django-cms.org/
+.. |djangocms4| image:: https://img.shields.io/badge/django%20CMS-4-blue.svg
     :target: https://www.django-cms.org/
-
-
```

### Comparing `djangocms-attributes-field-2.1.0/djangocms_attributes_field.egg-info/SOURCES.txt` & `djangocms-attributes-field-3.0.0/djangocms_attributes_field.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.rst
+pyproject.toml
 setup.py
 djangocms_attributes_field/__init__.py
 djangocms_attributes_field/fields.py
 djangocms_attributes_field/models.py
 djangocms_attributes_field/widgets.py
 djangocms_attributes_field.egg-info/PKG-INFO
 djangocms_attributes_field.egg-info/SOURCES.txt
```

### Comparing `djangocms-attributes-field-2.1.0/setup.py` & `djangocms-attributes-field-3.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,37 +2,39 @@
 from setuptools import find_packages, setup
 
 from djangocms_attributes_field import __version__
 
 
 REQUIREMENTS = [
     'django-cms>=3.7',
-    'django-treebeard>=4.3,<4.5',
 ]
 
 
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.5',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Framework :: Django',
-    'Framework :: Django :: 2.2',
-    'Framework :: Django :: 3.0',
-    'Framework :: Django :: 3.1',
+    'Framework :: Django :: 3.2',
+    'Framework :: Django :: 4.0',
+    'Framework :: Django :: 4.1',
+    'Framework :: Django :: 4.2',
     'Framework :: Django CMS',
-    'Framework :: Django CMS :: 3.7',
-    'Framework :: Django CMS :: 3.8',
+    'Framework :: Django CMS :: 3.9',
+    'Framework :: Django CMS :: 3.10',
+    'Framework :: Django CMS :: 3.11',
+    'Framework :: Django CMS :: 4.1',
     'Topic :: Internet :: WWW/HTTP',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Topic :: Software Development',
     'Topic :: Software Development :: Libraries',
 ]
```

### Comparing `djangocms-attributes-field-2.1.0/tests/test_app/migrations/0001_initial.py` & `djangocms-attributes-field-3.0.0/tests/test_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-attributes-field-2.1.0/tests/test_fields.py` & `djangocms-attributes-field-3.0.0/tests/test_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.core.exceptions import ValidationError
 from django.db.models.fields import NOT_PROVIDED
 from django.test.testcases import TestCase
 
 from djangocms_attributes_field.fields import (
-    AttributesField, AttributesFormField,
+    AttributesField,
+    AttributesFormField,
 )
 
 
 class Noop:
     pass
 
 
@@ -21,14 +22,15 @@
             field.validate_key('a')
             field.validate_key('A')
             field.validate_key('a1')
             field.validate_key('A1')
             field.validate_key('a-1')
             field.validate_key('a_1')
             field.validate_key('a-A1_')
+            field.validate_key('v-on:click')
         except ValidationError:
             self.fail('Keys that pass have failed.')
 
         # We don't accept these though...
         with self.assertRaises(ValidationError):
             field.validate_key('-abc')
         with self.assertRaises(ValidationError):
```

### Comparing `djangocms-attributes-field-2.1.0/tests/test_migrations.py` & `djangocms-attributes-field-3.0.0/tests/test_migrations.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             'interactive': False,
             'dry_run': True,
             'stdout': output,
             'check_changes': True,
         }
 
         try:
-            call_command('makemigrations', **options)
+            call_command('makemigrations', 'djangocms_attributes_field', **options)
         except SystemExit as e:
             status_code = str(e)
         else:
             # the "no changes" exit code is 0
             status_code = '0'
 
         if status_code == '1':
```

### Comparing `djangocms-attributes-field-2.1.0/tests/test_plugins.py` & `djangocms-attributes-field-3.0.0/tests/test_plugins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import warnings
 
+from cms import __version__
 from cms.api import add_plugin, create_page
 from cms.test_utils.testcases import CMSTestCase
 
 from .test_app.cms_plugins import TestPluginPlugin
 
 
 # we're testing the plugin generation from a sample django CMS addon in
@@ -13,33 +14,36 @@
     def setUp(self):
         self.language = "en"
         self.page = create_page(
             title="page",
             template="page.html",
             language=self.language,
         )
-        self.page.publish(self.language)
-        self.placeholder = self.page.placeholders.get(slot="content")
+        if __version__ < "4":
+            self.page.publish(self.language)
+            self.placeholder = self.page.placeholders.get(slot="content")
+        else:
+            self.placeholder = self.page.get_placeholders(self.language).get(slot="content")
         self.superuser = self.get_superuser()
 
     def tearDown(self):
         self.page.delete()
         self.superuser.delete()
 
     def test_plugin_rendering(self):
         request_url = self.page.get_absolute_url(self.language) + "?toolbar_off=true"
-
         add_plugin(
             placeholder=self.placeholder,
             plugin_type=TestPluginPlugin.__name__,
             language=self.language,
             attributes1={"data-tracking": "google"},
             attributes2={"class": "some new classes"},
         )
-        self.page.publish(self.language)
+        if __version__ < "4":
+            self.page.publish(self.language)
 
         with self.login_user_context(self.superuser):
             response = self.client.get(request_url)
 
         self.assertContains(response, "data-tracking")
         self.assertContains(response, "google")
         self.assertContains(response, "class")
```

### Comparing `djangocms-attributes-field-2.1.0/tests/test_widgets.py` & `djangocms-attributes-field-3.0.0/tests/test_widgets.py`

 * *Files identical despite different names*

