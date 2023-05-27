# Comparing `tmp/django-daraja-1.2.0.tar.gz` & `tmp/django-daraja-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-daraja-1.2.0.tar", last modified: Mon Nov 16 23:06:10 2020, max compression
+gzip compressed data, was "django-daraja-1.3.0.tar", last modified: Sat May 27 11:49:41 2023, max compression
```

## Comparing `django-daraja-1.2.0.tar` & `django-daraja-1.3.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxrwxrwx   0        0        0        0 2020-11-16 23:06:10.823799 django-daraja-1.2.0/
--rw-rw-rw-   0        0        0      169 2020-09-23 19:40:20.000000 django-daraja-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1367 2020-11-16 23:06:10.821403 django-daraja-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1964 2020-11-16 22:55:29.000000 django-daraja-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2020-11-16 23:06:10.522762 django-daraja-1.2.0/django_daraja/
--rw-rw-rw-   0        0        0        0 2020-09-23 19:40:20.000000 django-daraja-1.2.0/django_daraja/__init__.py
--rw-rw-rw-   0        0        0      128 2020-09-23 19:40:20.000000 django-daraja-1.2.0/django_daraja/admin.py
--rw-rw-rw-   0        0        0      165 2020-09-23 19:40:20.000000 django-daraja-1.2.0/django_daraja/apps.py
-drwxrwxrwx   0        0        0        0 2020-11-16 23:06:10.605314 django-daraja-1.2.0/django_daraja/migrations/
--rw-rw-rw-   0        0        0      644 2020-09-23 19:40:20.000000 django-daraja-1.2.0/django_daraja/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      398 2020-09-23 19:40:21.000000 django-daraja-1.2.0/django_daraja/migrations/0002_auto_20181108_1219.py
--rw-rw-rw-   0        0        0        0 2020-09-23 19:40:21.000000 django-daraja-1.2.0/django_daraja/migrations/__init__.py
--rw-rw-rw-   0        0        0      309 2020-09-23 19:40:21.000000 django-daraja-1.2.0/django_daraja/models.py
-drwxrwxrwx   0        0        0        0 2020-11-16 23:06:10.637174 django-daraja-1.2.0/django_daraja/mpesa/
--rw-rw-rw-   0        0        0        0 2020-09-23 19:40:21.000000 django-daraja-1.2.0/django_daraja/mpesa/__init__.py
--rw-rw-rw-   0        0        0     7451 2020-11-16 22:39:39.000000 django-daraja-1.2.0/django_daraja/mpesa/core.py
--rw-rw-rw-   0        0        0      652 2020-09-23 19:40:21.000000 django-daraja-1.2.0/django_daraja/mpesa/exceptions.py
--rw-rw-rw-   0        0        0     5914 2020-11-16 21:40:29.000000 django-daraja-1.2.0/django_daraja/mpesa/utils.py
--rw-rw-rw-   0        0        0      709 2020-11-16 21:48:46.000000 django-daraja-1.2.0/django_daraja/urls.py
--rw-rw-rw-   0        0        0     2090 2020-11-16 22:03:28.000000 django-daraja-1.2.0/django_daraja/views.py
-drwxrwxrwx   0        0        0        0 2020-11-16 23:06:10.587145 django-daraja-1.2.0/django_daraja.egg-info/
--rw-rw-rw-   0        0        0     1367 2020-11-16 23:06:10.000000 django-daraja-1.2.0/django_daraja.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1111 2020-11-16 23:06:10.000000 django-daraja-1.2.0/django_daraja.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-11-16 23:06:10.000000 django-daraja-1.2.0/django_daraja.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-09-23 19:59:11.000000 django-daraja-1.2.0/django_daraja.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       51 2020-11-16 23:06:10.000000 django-daraja-1.2.0/django_daraja.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2020-11-16 23:06:10.000000 django-daraja-1.2.0/django_daraja.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2020-11-16 23:06:10.675077 django-daraja-1.2.0/docs/
--rw-rw-rw-   0        0        0      580 2020-09-23 19:40:21.000000 django-daraja-1.2.0/docs/Makefile
--rw-rw-rw-   0        0        0     5337 2020-09-23 19:40:21.000000 django-daraja-1.2.0/docs/conf.py
--rw-rw-rw-   0        0        0      891 2020-09-23 19:40:21.000000 django-daraja-1.2.0/docs/index.rst
--rwxrwxrwx   0        0        0      752 2020-09-23 19:40:21.000000 django-daraja-1.2.0/docs/make.bat
-drwxrwxrwx   0        0        0        0 2020-11-16 23:06:10.690277 django-daraja-1.2.0/docs/pages/
-drwxrwxrwx   0        0        0        0 2020-11-16 23:06:10.739133 django-daraja-1.2.0/docs/pages/apis/
--rw-rw-rw-   0        0        0     2616 2020-11-16 23:02:32.000000 django-daraja-1.2.0/docs/pages/apis/b2c_payment.rst
--rw-rw-rw-   0        0        0      212 2020-11-16 22:45:40.000000 django-daraja-1.2.0/docs/pages/apis/index.rst
--rw-rw-rw-   0        0        0      836 2020-09-23 19:40:21.000000 django-daraja-1.2.0/docs/pages/apis/oauth.rst
--rw-rw-rw-   0        0        0     1708 2020-09-23 19:40:21.000000 django-daraja-1.2.0/docs/pages/apis/stk_push.rst
--rw-rw-rw-   0        0        0     1339 2020-09-23 19:40:21.000000 django-daraja-1.2.0/docs/pages/introduction.rst
--rw-rw-rw-   0        0        0    10153 2020-11-16 22:53:55.000000 django-daraja-1.2.0/docs/pages/quick_start.rst
--rw-rw-rw-   0        0        0       78 2020-11-16 21:56:24.000000 django-daraja-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2020-11-16 23:06:10.824334 django-daraja-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2016 2020-11-16 22:56:02.000000 django-daraja-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-11-16 23:06:10.818618 django-daraja-1.2.0/tests/
--rw-rw-rw-   0        0        0      803 2020-09-23 19:40:21.000000 django-daraja-1.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0      552 2020-09-23 19:40:21.000000 django-daraja-1.2.0/tests/runtests.py
--rw-rw-rw-   0        0        0     3139 2020-09-23 19:40:21.000000 django-daraja-1.2.0/tests/settings.py
--rw-rw-rw-   0        0        0     2808 2020-11-16 22:39:55.000000 django-daraja-1.2.0/tests/test_b2c_payment.py
--rw-rw-rw-   0        0        0      409 2020-09-23 19:40:22.000000 django-daraja-1.2.0/tests/test_client.py
--rw-rw-rw-   0        0        0     1090 2020-11-16 14:34:35.000000 django-daraja-1.2.0/tests/test_oauth.py
--rw-rw-rw-   0        0        0     2323 2020-09-23 19:40:23.000000 django-daraja-1.2.0/tests/test_parse_result.py
--rw-rw-rw-   0        0        0     2164 2020-11-16 22:06:09.000000 django-daraja-1.2.0/tests/test_stk_push.py
--rw-rw-rw-   0        0        0      371 2020-09-23 19:40:23.000000 django-daraja-1.2.0/tests/test_views.py
--rw-rw-rw-   0        0        0      824 2020-09-23 19:40:23.000000 django-daraja-1.2.0/tests/urls.py
--rw-rw-rw-   0        0        0      388 2020-09-23 19:40:23.000000 django-daraja-1.2.0/tests/wsgi.py
--rw-rw-rw-   0        0        0      673 2020-11-16 13:00:57.000000 django-daraja-1.2.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-27 11:49:41.324972 django-daraja-1.3.0/
+-rw-rw-rw-   0        0        0     1052 2020-09-23 19:40:20.000000 django-daraja-1.3.0/LICENCE.txt
+-rw-rw-rw-   0        0        0      169 2020-09-23 19:40:20.000000 django-daraja-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1324 2023-05-27 11:49:41.324972 django-daraja-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3299 2023-01-03 22:17:14.000000 django-daraja-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 11:49:41.258317 django-daraja-1.3.0/django_daraja/
+-rw-rw-rw-   0        0        0        0 2020-09-23 19:40:20.000000 django-daraja-1.3.0/django_daraja/__init__.py
+-rw-rw-rw-   0        0        0      128 2020-09-23 19:40:20.000000 django-daraja-1.3.0/django_daraja/admin.py
+-rw-rw-rw-   0        0        0      165 2020-09-23 19:40:20.000000 django-daraja-1.3.0/django_daraja/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:49:41.277582 django-daraja-1.3.0/django_daraja/migrations/
+-rw-rw-rw-   0        0        0      644 2020-09-23 19:40:20.000000 django-daraja-1.3.0/django_daraja/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      398 2020-09-23 19:40:21.000000 django-daraja-1.3.0/django_daraja/migrations/0002_auto_20181108_1219.py
+-rw-rw-rw-   0        0        0        0 2020-09-23 19:40:21.000000 django-daraja-1.3.0/django_daraja/migrations/__init__.py
+-rw-rw-rw-   0        0        0      309 2020-09-23 19:40:21.000000 django-daraja-1.3.0/django_daraja/models.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:49:41.277582 django-daraja-1.3.0/django_daraja/mpesa/
+-rw-rw-rw-   0        0        0        0 2020-09-23 19:40:21.000000 django-daraja-1.3.0/django_daraja/mpesa/__init__.py
+-rw-rw-rw-   0        0        0     7451 2020-11-16 22:39:39.000000 django-daraja-1.3.0/django_daraja/mpesa/core.py
+-rw-rw-rw-   0        0        0      652 2020-09-23 19:40:21.000000 django-daraja-1.3.0/django_daraja/mpesa/exceptions.py
+-rw-rw-rw-   0        0        0     6464 2023-05-27 11:30:24.000000 django-daraja-1.3.0/django_daraja/mpesa/utils.py
+-rw-rw-rw-   0        0        0      732 2023-01-03 17:17:38.000000 django-daraja-1.3.0/django_daraja/urls.py
+-rw-rw-rw-   0        0        0     2078 2023-01-03 17:06:04.000000 django-daraja-1.3.0/django_daraja/views.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:49:41.277582 django-daraja-1.3.0/django_daraja.egg-info/
+-rw-rw-rw-   0        0        0     1324 2023-05-27 11:49:40.000000 django-daraja-1.3.0/django_daraja.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1123 2023-05-27 11:49:41.000000 django-daraja-1.3.0/django_daraja.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:49:40.000000 django-daraja-1.3.0/django_daraja.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-09-23 19:59:11.000000 django-daraja-1.3.0/django_daraja.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       51 2023-05-27 11:49:40.000000 django-daraja-1.3.0/django_daraja.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-27 11:49:40.000000 django-daraja-1.3.0/django_daraja.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 11:49:41.293210 django-daraja-1.3.0/docs/
+-rw-rw-rw-   0        0        0      580 2020-09-23 19:40:21.000000 django-daraja-1.3.0/docs/Makefile
+-rw-rw-rw-   0        0        0     5337 2020-09-23 19:40:21.000000 django-daraja-1.3.0/docs/conf.py
+-rw-rw-rw-   0        0        0      890 2020-11-16 23:11:36.000000 django-daraja-1.3.0/docs/index.rst
+-rwxrwxrwx   0        0        0      752 2020-09-23 19:40:21.000000 django-daraja-1.3.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-27 11:49:41.293210 django-daraja-1.3.0/docs/pages/
+drwxrwxrwx   0        0        0        0 2023-05-27 11:49:41.308832 django-daraja-1.3.0/docs/pages/apis/
+-rw-rw-rw-   0        0        0     2425 2023-01-03 22:17:14.000000 django-daraja-1.3.0/docs/pages/apis/b2c_payment.rst
+-rw-rw-rw-   0        0        0      212 2020-11-16 22:45:40.000000 django-daraja-1.3.0/docs/pages/apis/index.rst
+-rw-rw-rw-   0        0        0      836 2020-09-23 19:40:21.000000 django-daraja-1.3.0/docs/pages/apis/oauth.rst
+-rw-rw-rw-   0        0        0     1331 2023-05-27 11:38:21.000000 django-daraja-1.3.0/docs/pages/apis/stk_push.rst
+-rw-rw-rw-   0        0        0     1476 2023-05-27 11:38:21.000000 django-daraja-1.3.0/docs/pages/introduction.rst
+-rw-rw-rw-   0        0        0     7331 2023-01-03 22:17:14.000000 django-daraja-1.3.0/docs/pages/quick_start.rst
+-rw-rw-rw-   0        0        0       78 2020-11-16 21:56:24.000000 django-daraja-1.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 11:49:41.324972 django-daraja-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2051 2023-05-27 11:46:04.000000 django-daraja-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:49:41.324972 django-daraja-1.3.0/tests/
+-rw-rw-rw-   0        0        0      803 2020-09-23 19:40:21.000000 django-daraja-1.3.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      552 2020-09-23 19:40:21.000000 django-daraja-1.3.0/tests/runtests.py
+-rw-rw-rw-   0        0        0     3253 2023-01-03 20:39:52.000000 django-daraja-1.3.0/tests/settings.py
+-rw-rw-rw-   0        0        0     2544 2023-01-03 20:20:32.000000 django-daraja-1.3.0/tests/test_b2c_payment.py
+-rw-rw-rw-   0        0        0      409 2020-09-23 19:40:22.000000 django-daraja-1.3.0/tests/test_client.py
+-rw-rw-rw-   0        0        0     1090 2020-11-16 14:34:35.000000 django-daraja-1.3.0/tests/test_oauth.py
+-rw-rw-rw-   0        0        0     2323 2020-09-23 19:40:23.000000 django-daraja-1.3.0/tests/test_parse_result.py
+-rw-rw-rw-   0        0        0     2306 2023-01-03 21:28:26.000000 django-daraja-1.3.0/tests/test_stk_push.py
+-rw-rw-rw-   0        0        0      371 2020-09-23 19:40:23.000000 django-daraja-1.3.0/tests/test_views.py
+-rw-rw-rw-   0        0        0      858 2023-01-03 22:17:14.000000 django-daraja-1.3.0/tests/urls.py
+-rw-rw-rw-   0        0        0      388 2020-09-23 19:40:23.000000 django-daraja-1.3.0/tests/wsgi.py
+-rw-rw-rw-   0        0        0      584 2023-01-03 20:39:52.000000 django-daraja-1.3.0/tox.ini
```

### Comparing `django-daraja-1.2.0/PKG-INFO` & `django-daraja-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-daraja
-Version: 1.2.0
+Version: 1.3.0
 Summary: A python django library for interacting with the Safaricom MPESA Daraja API.
 Home-page: https://github.com/martinmogusu/django-daraja
+Download-URL: https://github.com/martinmogusu/django-daraja.git
 Author: Martin Mogusu
 Author-email: martinmogusu@gmail.com
 License: MIT License
-Download-URL: https://github.com/martinmogusu/django-daraja.git
 Project-URL: Documentation, https://django-daraja.readthedocs.io/
 Project-URL: Source, https://github.com/martinmogusu/django-daraja
-Description: 
-        This is a django library based on the Safaricom MPESA daraja API. Use it for a simplified experience, spend less time setting up...
-        
-        Read the full documentation at https://django-daraja.readthedocs.io
-        
-        MPESA Daraja API documentation can be found at https://developer.safaricom.co.ke
 Keywords: mpesa django daraja finance mobile-money safaricom api
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENCE.txt
+
+
+This is a django library based on the Safaricom MPESA daraja API. Use it for a simplified experience, spend less time setting up...
+
+Read the full documentation at https://django-daraja.readthedocs.io
+
+MPESA Daraja API documentation can be found at https://developer.safaricom.co.ke
```

### Comparing `django-daraja-1.2.0/django_daraja/migrations/0001_initial.py` & `django-daraja-1.3.0/django_daraja/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daraja-1.2.0/django_daraja/mpesa/core.py` & `django-daraja-1.3.0/django_daraja/mpesa/core.py`

 * *Files identical despite different names*

### Comparing `django-daraja-1.2.0/django_daraja/mpesa/exceptions.py` & `django-daraja-1.3.0/django_daraja/mpesa/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-daraja-1.2.0/django_daraja/mpesa/utils.py` & `django-daraja-1.3.0/django_daraja/mpesa/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,222 +1,218 @@
-"""
-General utilities for the MPESA functions
-"""
-
-from __future__ import print_function
-from .exceptions import MpesaConfigurationException, IllegalPhoneNumberException, MpesaConnectionError, MpesaError
-from django_daraja.models import AccessToken
-import requests
-from django.utils import timezone
-from decouple import config, UndefinedValueError
-import os
-from requests import Response
-import time
-from django.conf import settings
-import os
-from django.conf import settings
-import base64
-from cryptography import x509
-from cryptography.hazmat.primitives.asymmetric.padding import PKCS1v15
-
-
-class MpesaResponse(Response):
-	response_description = ""
-	error_code = None
-	error_message = ''
-
-
-def mpesa_response(r):
-	"""
-	Create MpesaResponse object from requests.Response object
-	
-	Arguments:
-		r (requests.Response) -- The response to convert
-	"""
-
-	r.__class__ = MpesaResponse
-	json_response = r.json()
-	r.response_description = json_response.get('ResponseDescription', '')
-	r.error_code = json_response.get('errorCode')
-	r.error_message = json_response.get('errorMessage', '')
-	return r
-
-
-def mpesa_config(key):
-	"""
-	Get Mpesa configuration variable with the matching key
-	
-	Arguments:
-		key (str) -- The configuration key
-
-	Returns:
-		str: Mpesa configuration variable with the matching key
-
-	Raises:
-		MpesaConfigurationException: Key not found
-	"""
-
-	value = getattr(settings, key, None)
-	if value is None:
-		try:
-			value = config(key)
-		except UndefinedValueError:
-			# Check key in settings file
-			raise MpesaConfigurationException('Mpesa environment not configured properly - ' + key + ' not found')
-
-	return value
-
-
-def api_base_url():
-	"""
-	Gets the base URL for making API calls
-
-	Returns:
-		The base URL depending on development environment (sandbox or production)
-
-	Raises:
-		MpesaConfigurationException: Environment not sandbox or production
-	"""
-
-	mpesa_environment = mpesa_config('MPESA_ENVIRONMENT')
-
-	if mpesa_environment == 'sandbox':
-		return 'https://sandbox.safaricom.co.ke/'
-	elif mpesa_environment == 'production':
-		return 'https://api.safaricom.co.ke/'
-	else:
-		raise MpesaConfigurationException('Mpesa environment not configured properly - MPESA_ENVIRONMENT should be sandbox or production')
-
-def generate_access_token_request(consumer_key = None, consumer_secret = None):
-	"""
-	Make a call to OAuth API to generate access token
-	
-	Arguments:
-		consumer_key (str) -- (Optional) The Consumer Key to use
-		consumer_secret (str) -- (Optional) The Consumer Secret to use
-
-	Returns:
-		requests.Response: Response object with the response details
-
-	Raises:
-		MpesaConnectionError: Connection error
-	"""
-
-	url = api_base_url() + 'oauth/v1/generate?grant_type=client_credentials'
-	consumer_key = consumer_key if consumer_key is not None else mpesa_config('MPESA_CONSUMER_KEY') 
-	consumer_secret = consumer_secret if consumer_secret is not None else mpesa_config('MPESA_CONSUMER_SECRET')
-
-	try:
-		r = requests.get(url, auth=(consumer_key, consumer_secret))
-	except requests.exceptions.ConnectionError:
-		raise MpesaConnectionError('Connection failed')
-	except Exception as ex:
-		return ex.message
-	
-	return r
-
-def generate_access_token():
-	"""
-	Parse generated OAuth access token, then updates database access token value
-
-	Returns:
-		AccessToken: The AccessToken object from the database
-
-	Raises:
-		MpesaError: Error generating access token
-	"""
-
-	r = generate_access_token_request()
-	if r.status_code != 200:
-		# Retry to generate access token
-		r = generate_access_token_request()
-		if r.status_code != 200:
-			raise MpesaError('Unable to generate access token')
-
-	token = r.json()['access_token']
-
-	AccessToken.objects.all().delete()
-	access_token = AccessToken.objects.create(token=token)
-
-	return access_token
-
-def mpesa_access_token():
-	"""
-	Generate access token if the current one has expired or if token is non-existent
-	Otherwise return existing access token
-
-	Returns:
-		str: A valid access token
-	"""
-
-	access_token = AccessToken.objects.first()
-	if access_token == None:
-		# No access token found
-		access_token = generate_access_token()
-	else:
-		delta = timezone.now() - access_token.created_at
-		minutes = (delta.total_seconds()//60)%60
-		print('minutes: ', minutes)
-		if minutes > 50:
-			# Access token expired
-			access_token = generate_access_token()	
-	
-	return access_token.token
-
-def format_phone_number(phone_number):
-	"""
-	Format phone number into the format 2547XXXXXXXX
-	
-	Arguments:
-		phone_number (str) -- The phone number to format
-	"""
-
-	if len(phone_number) < 9:
-		raise IllegalPhoneNumberException('Phone number too short')
-	else:
-		return '254' + phone_number[-9:]
-
-def sleep(seconds, message=''):
-	"""
-	Sleep for the specified number of seconds
-	
-	Arguments:
-		seconds (float) -- Number of seconds to sleep, can be a float
-		message (str) -- (Optional) message to display
-	"""
-
-	print()
-	print('===')
-	print(message, end="")
-	for i in range(seconds * 2):
-		time.sleep(0.5)
-		print('.', end="")
-	print()
-	print('===')
-	print()
-
-def encrypt_security_credential(credential):
-	"""
-	Generate an encrypted security credential from a plaintext value
-	
-	Arguments:
-		credential (str) -- The plaintext credential display
-	"""
-
-	mpesa_environment = mpesa_config('MPESA_ENVIRONMENT')
-
-	if mpesa_environment in ('sandbox', 'production'):
-		certificate_name = mpesa_environment + '.cer'
-	else:
-		raise MpesaConfigurationException('Mpesa environment not configured properly - MPESA_ENVIRONMENT should be sandbox or production')
-
-	certificate_path = os.path.join(settings.BASE_DIR, 'certs', certificate_name)
-	return encrypt_rsa(certificate_path, credential)
-
-def encrypt_rsa(certificate_path, input):
-	message = input.encode('ascii')
-	with open(certificate_path, "rb") as cert_file:
-		cert = x509.load_pem_x509_certificate(cert_file.read())
-		encrypted = cert.public_key().encrypt(message, PKCS1v15())
-		output = base64.b64encode(encrypted).decode('ascii')
-
-	return output
+"""
+General utilities for the MPESA functions
+"""
+
+from __future__ import print_function
+from .exceptions import MpesaConfigurationException, IllegalPhoneNumberException, MpesaConnectionError, MpesaError
+from django_daraja.models import AccessToken
+import requests
+from django.utils import timezone
+from decouple import config, UndefinedValueError
+import os
+from requests import Response
+import time
+from django.conf import settings
+import os
+from django.conf import settings
+import base64
+from cryptography import x509
+from cryptography.hazmat.primitives.asymmetric.padding import PKCS1v15
+
+
+class MpesaResponse(Response):
+	request_id = ''
+	response_code = ''
+	response_description = ''
+	customer_message = ''
+	conversation_id = ''
+	originator_conversation_id = ''
+	error_code = ''
+	error_message = ''
+	merchant_request_id = ''
+	checkout_request_id = ''
+
+
+def mpesa_response(r):
+	"""
+	Create MpesaResponse object from requests.Response object
+	
+	Arguments:
+		r (requests.Response) -- The response to convert
+	"""
+
+	r.__class__ = MpesaResponse
+	json_response = r.json()
+	r.request_id = json_response.get('requestId', '')
+	r.response_code = json_response.get('ResponseCode', '')
+	r.response_description = json_response.get('ResponseDescription', '')
+	r.customer_message = json_response.get('CustomerMessage', '')
+	r.conversation_id = json_response.get('ConversationID', '')
+	r.originator_conversation_id = json_response.get('OriginatorConversationID', '')
+	r.error_code = json_response.get('errorCode')
+	r.error_message = json_response.get('errorMessage', '')
+	r.merchant_request_id = json_response.get('MerchantRequestID', '')
+	r.checkout_request_id = json_response.get('CheckoutRequestID', '')
+	return r
+
+
+def mpesa_config(key):
+	"""
+	Get Mpesa configuration variable with the matching key
+	
+	Arguments:
+		key (str) -- The configuration key
+
+	Returns:
+		str: Mpesa configuration variable with the matching key
+
+	Raises:
+		MpesaConfigurationException: Key not found
+	"""
+
+	value = getattr(settings, key, None)
+	if value is None:
+		try:
+			value = config(key)
+		except UndefinedValueError:
+			# Check key in settings file
+			raise MpesaConfigurationException('Mpesa environment not configured properly - ' + key + ' not found')
+
+	return value
+
+
+def api_base_url():
+	"""
+	Gets the base URL for making API calls
+
+	Returns:
+		The base URL depending on development environment (sandbox or production)
+
+	Raises:
+		MpesaConfigurationException: Environment not sandbox or production
+	"""
+
+	mpesa_environment = mpesa_config('MPESA_ENVIRONMENT')
+
+	if mpesa_environment == 'development':
+		return 'https://darajasimulator.azurewebsites.net/'
+	elif mpesa_environment == 'sandbox':
+		return 'https://sandbox.safaricom.co.ke/'
+	elif mpesa_environment == 'production':
+		return 'https://api.safaricom.co.ke/'
+	else:
+		raise MpesaConfigurationException('Mpesa environment not configured properly - MPESA_ENVIRONMENT should be sandbox or production')
+
+def generate_access_token_request(consumer_key = None, consumer_secret = None):
+	"""
+	Make a call to OAuth API to generate access token
+	
+	Arguments:
+		consumer_key (str) -- (Optional) The Consumer Key to use
+		consumer_secret (str) -- (Optional) The Consumer Secret to use
+
+	Returns:
+		requests.Response: Response object with the response details
+
+	Raises:
+		MpesaConnectionError: Connection error
+	"""
+
+	url = api_base_url() + 'oauth/v1/generate?grant_type=client_credentials'
+	consumer_key = consumer_key if consumer_key is not None else mpesa_config('MPESA_CONSUMER_KEY') 
+	consumer_secret = consumer_secret if consumer_secret is not None else mpesa_config('MPESA_CONSUMER_SECRET')
+
+	try:
+		r = requests.get(url, auth=(consumer_key, consumer_secret))
+	except requests.exceptions.ConnectionError:
+		raise MpesaConnectionError('Connection failed')
+	except Exception as ex:
+		return ex.message
+	
+	return r
+
+def generate_access_token():
+	"""
+	Parse generated OAuth access token, then updates database access token value
+
+	Returns:
+		AccessToken: The AccessToken object from the database
+
+	Raises:
+		MpesaError: Error generating access token
+	"""
+
+	r = generate_access_token_request()
+	if r.status_code != 200:
+		# Retry to generate access token
+		r = generate_access_token_request()
+		if r.status_code != 200:
+			raise MpesaError('Unable to generate access token')
+
+	token = r.json()['access_token']
+
+	AccessToken.objects.all().delete()
+	access_token = AccessToken.objects.create(token=token)
+
+	return access_token
+
+def mpesa_access_token():
+	"""
+	Generate access token if the current one has expired or if token is non-existent
+	Otherwise return existing access token
+
+	Returns:
+		str: A valid access token
+	"""
+
+	access_token = AccessToken.objects.first()
+	if access_token == None:
+		# No access token found
+		access_token = generate_access_token()
+	else:
+		delta = timezone.now() - access_token.created_at
+		minutes = (delta.total_seconds()//60)
+		if minutes > 50:
+			# Access token expired
+			access_token = generate_access_token()	
+	
+	return access_token.token
+
+def format_phone_number(phone_number):
+	"""
+	Format phone number into the format 2547XXXXXXXX
+	
+	Arguments:
+		phone_number (str) -- The phone number to format
+	"""
+
+	if len(phone_number) < 9:
+		raise IllegalPhoneNumberException('Phone number too short')
+	else:
+		return '254' + phone_number[-9:]
+
+def encrypt_security_credential(credential):
+	"""
+	Generate an encrypted security credential from a plaintext value
+	
+	Arguments:
+		credential (str) -- The plaintext credential display
+	"""
+
+	mpesa_environment = mpesa_config('MPESA_ENVIRONMENT')
+
+	if mpesa_environment in ('development', 'sandbox', 'production'):
+		certificate_name = mpesa_environment + '.cer'
+	else:
+		raise MpesaConfigurationException('Mpesa environment not configured properly - MPESA_ENVIRONMENT should be sandbox or production')
+
+	certificate_path = os.path.join(settings.BASE_DIR, 'certs', certificate_name)
+	return encrypt_rsa(certificate_path, credential)
+
+def encrypt_rsa(certificate_path, input):
+	message = input.encode('ascii')
+	with open(certificate_path, "rb") as cert_file:
+		cert = x509.load_pem_x509_certificate(cert_file.read())
+		encrypted = cert.public_key().encrypt(message, PKCS1v15())
+		output = base64.b64encode(encrypted).decode('ascii')
+
+	return output
```

### Comparing `django-daraja-1.2.0/django_daraja/urls.py` & `django-daraja-1.3.0/django_daraja/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from django.conf.urls import url, include
-from . import views
-
-test_patterns = [
-	url(r'^$', views.index, name='django_daraja_index'),
-	url(r'^oauth/success', views.oauth_success, name='test_oauth_success'),
-	url(r'^stk-push/success', views.stk_push_success, name='test_stk_push_success'),
-	url(r'^business-payment/success', views.business_payment_success, name='test_business_payment_success'),
-	url(r'^salary-payment/success', views.salary_payment_success, name='test_salary_payment_success'),
-	url(r'^promotion-payment/success', views.promotion_payment_success, name='test_promotion_payment_success'),
-]
-
-urlpatterns = [
-	url(r'^$', views.index, name='index'),
-	url(r'^tests/', include(test_patterns)),
-]
-
+from django.urls import re_path as url, include
+from . import views
+
+test_patterns = [
+	url(r'^$', views.index, name='django_daraja_index'),
+	url(r'^oauth/success', views.oauth_success, name='test_oauth_success'),
+	url(r'^stk-push/success', views.stk_push_success, name='test_stk_push_success'),
+	url(r'^business-payment/success', views.business_payment_success, name='test_business_payment_success'),
+	url(r'^salary-payment/success', views.salary_payment_success, name='test_salary_payment_success'),
+	url(r'^promotion-payment/success', views.promotion_payment_success, name='test_promotion_payment_success'),
+]
+
+urlpatterns = [
+	url(r'^$', views.index, name='index'),
+	url(r'^tests/', include(test_patterns)),
+]
+
```

### Comparing `django-daraja-1.2.0/django_daraja/views.py` & `django-daraja-1.3.0/django_daraja/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from django.http import HttpResponse, JsonResponse
 from django.views.generic import View
 from django_daraja.mpesa.core import MpesaClient
 from decouple import config
 from datetime import datetime
 
 cl = MpesaClient()
-stk_push_callback_url = 'https://darajambili.herokuapp.com/express-payment'
-b2c_callback_url = 'https://darajambili.herokuapp.com/b2c/result'
+stk_push_callback_url = 'https://api.darajambili.com/express-payment'
+b2c_callback_url = 'https://api.darajambili.com/b2c/result'
 
 def index(request):
 
 	return HttpResponse('Welcome to the home of daraja APIs')
 
 def oauth_success(request):
 	r = cl.access_token()
```

### Comparing `django-daraja-1.2.0/django_daraja.egg-info/PKG-INFO` & `django-daraja-1.3.0/django_daraja.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-daraja
-Version: 1.2.0
+Version: 1.3.0
 Summary: A python django library for interacting with the Safaricom MPESA Daraja API.
 Home-page: https://github.com/martinmogusu/django-daraja
+Download-URL: https://github.com/martinmogusu/django-daraja.git
 Author: Martin Mogusu
 Author-email: martinmogusu@gmail.com
 License: MIT License
-Download-URL: https://github.com/martinmogusu/django-daraja.git
 Project-URL: Documentation, https://django-daraja.readthedocs.io/
 Project-URL: Source, https://github.com/martinmogusu/django-daraja
-Description: 
-        This is a django library based on the Safaricom MPESA daraja API. Use it for a simplified experience, spend less time setting up...
-        
-        Read the full documentation at https://django-daraja.readthedocs.io
-        
-        MPESA Daraja API documentation can be found at https://developer.safaricom.co.ke
 Keywords: mpesa django daraja finance mobile-money safaricom api
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENCE.txt
+
+
+This is a django library based on the Safaricom MPESA daraja API. Use it for a simplified experience, spend less time setting up...
+
+Read the full documentation at https://django-daraja.readthedocs.io
+
+MPESA Daraja API documentation can be found at https://developer.safaricom.co.ke
```

### Comparing `django-daraja-1.2.0/django_daraja.egg-info/SOURCES.txt` & `django-daraja-1.3.0/django_daraja.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENCE.txt
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 tox.ini
 django_daraja/__init__.py
 django_daraja/admin.py
```

### Comparing `django-daraja-1.2.0/docs/Makefile` & `django-daraja-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-daraja-1.2.0/docs/conf.py` & `django-daraja-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-daraja-1.2.0/docs/index.rst` & `django-daraja-1.3.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
    sphinx-quickstart on Wed Oct 31 17:02:06 2018.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to django-daraja's documentation!
 =========================================
 
-This is a django library that interacts with the MPESA Daraja API. Source code can be found https://github.com/martinmogusu/django-daraja.git MPESA Daraja documentattion can be found at https://developer.safaricom.co.ke
+This is a django library that interacts with the MPESA Daraja API. Source code can be found https://github.com/martinmogusu/django-daraja.git MPESA Daraja documentation can be found at https://developer.safaricom.co.ke
 
 Installation
 ============
 To install the library, run:
 
 	..	code-block:: none
```

### Comparing `django-daraja-1.2.0/docs/make.bat` & `django-daraja-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-daraja-1.2.0/docs/pages/apis/b2c_payment.rst` & `django-daraja-1.3.0/docs/pages/apis/b2c_payment.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-B2C Payment APIs
-================
-
-The B2C Payment APIs are used to make Business to Customer payments. Currently 3 transactions are supported in this model:
-
-Business Payment
-  This is a normal business to customer payment,  supports only M-Pesa registered customers.
-
-Salary Payment
-  This supports sending money to both registere and unregistered M-Pesa customers.
-
-Promotion Payment
-  This is a promotional payment to customers. The M-Pesa notification message is a congratulatory message. Supports only M-Pesa registered customers.
-
-Examples:
-
-Business Payment
-----------------
-
-	..	code-block:: python
-
-		from django_daraja.mpesa.core import MpesaClient
-
-		phone_number = '07xxxxxxxx'
-		amount = 1
-		transaction_desc = 'Description'
-		occassion = 'Occassion'
-		callback_url = request.build_absolute_uri(reverse('mpesa_business_payment_callback'))
-		response = self.cl.business_payment(phone_number, amount, transaction_desc, self.callback_url, occassion)
-
-Salary Payment
-----------------
-
-	..	code-block:: python
-
-		from django_daraja.mpesa.core import MpesaClient
-
-		phone_number = '07xxxxxxxx'
-		amount = 1
-		transaction_desc = 'Description'
-		occassion = 'Occassion'
-		callback_url = request.build_absolute_uri(reverse('mpesa_salary_payment_callback'))
-		response = self.cl.business_payment(phone_number, amount, transaction_desc, self.callback_url, occassion)
-
-Promotion Payment
-----------------
-
-	..	code-block:: python
-
-		from django_daraja.mpesa.core import MpesaClient
-
-		phone_number = '07xxxxxxxx'
-		amount = 1
-		transaction_desc = 'Description'
-		occassion = 'Occassion'
-		callback_url = request.build_absolute_uri(reverse('mpesa_promotion_payment_callback'))
-		response = self.cl.promotion_payment(phone_number, amount, transaction_desc, self.callback_url, occassion)
-
-
-This will assign the ``response`` variable with an ``MpesaResponse`` object containing the response returned from the Business Payment B2C API Call 
-
-.. note::
-	- Test credentials to use for this scenario can be found at the developer portal (https://developer.safaricom.co.ke/test_credentials)
-	- Use `shortcode 1` as the shortcode, and the test MSISDN as the B2C phone number
-	- This example will work if your site is already hosted, since the callback URL needs to be accessible via internet. For local testing purposes, you can use an endpoint hosted outside your site to check the notification received on the callback URL. There is a test listener hosted at https://darajambili.herokuapp.com, which you can use to view logs of notifications received. You can head over there to pick a callback URL to use for B2C Payments.
+B2C Payment APIs
+================
+
+The B2C Payment APIs are used to make Business to Customer payments. Currently 3 transactions are supported in this model:
+
+Business Payment
+  This is a normal business to customer payment,  supports only M-Pesa registered customers.
+
+Salary Payment
+  This supports sending money to both registere and unregistered M-Pesa customers.
+
+Promotion Payment
+  This is a promotional payment to customers. The M-Pesa notification message is a congratulatory message. Supports only M-Pesa registered customers.
+
+Examples:
+
+Business Payment
+----------------
+
+	..	code-block:: python
+
+		from django_daraja.mpesa.core import MpesaClient
+
+		phone_number = '07xxxxxxxx'
+		amount = 1
+		transaction_desc = 'Description'
+		occassion = 'Occassion'
+		callback_url = 'https://api.darajambili.com/b2c/result'
+		response = self.cl.business_payment(phone_number, amount, transaction_desc, self.callback_url, occassion)
+
+Salary Payment
+----------------
+
+	..	code-block:: python
+
+		from django_daraja.mpesa.core import MpesaClient
+
+		phone_number = '07xxxxxxxx'
+		amount = 1
+		transaction_desc = 'Description'
+		occassion = 'Occassion'
+		callback_url = 'https://api.darajambili.com/b2c/result'
+		response = self.cl.business_payment(phone_number, amount, transaction_desc, self.callback_url, occassion)
+
+Promotion Payment
+----------------
+
+	..	code-block:: python
+
+		from django_daraja.mpesa.core import MpesaClient
+
+		phone_number = '07xxxxxxxx'
+		amount = 1
+		transaction_desc = 'Description'
+		occassion = 'Occassion'
+		callback_url = 'https://api.darajambili.com/b2c/result'
+		response = self.cl.promotion_payment(phone_number, amount, transaction_desc, self.callback_url, occassion)
+
+
+This will assign the ``response`` variable with an ``MpesaResponse`` object containing the response returned from the Business Payment B2C API Call 
+
+.. note::
+	- Test credentials to use for this scenario can be found at the developer portal (https://developer.safaricom.co.ke/test_credentials)
+	- Use `shortcode 1` as the shortcode, and the test MSISDN as the B2C phone number
+	- Once the transaction is complete, you will receive a notification on the callback URL you provided. If you used the exact callback URL in the example above (i.e. https://api.darajambili.com/b2c/result), you can head over to https://darajambili.com to view the notification received
```

### Comparing `django-daraja-1.2.0/docs/pages/apis/oauth.rst` & `django-daraja-1.3.0/docs/pages/apis/oauth.rst`

 * *Files identical despite different names*

### Comparing `django-daraja-1.2.0/tests/__init__.py` & `django-daraja-1.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-daraja-1.2.0/tests/runtests.py` & `django-daraja-1.3.0/tests/runtests.py`

 * *Files identical despite different names*

### Comparing `django-daraja-1.2.0/tests/settings.py` & `django-daraja-1.3.0/tests/settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,122 +1,120 @@
-"""
-Django settings for tests project.
-
-Generated by 'django-admin startproject' using Django 1.11.
-
-For more information on this file, see
-https://docs.djangoproject.com/en/1.11/topics/settings/
-
-For the full list of settings and their values, see
-https://docs.djangoproject.com/en/1.11/ref/settings/
-"""
-
-import os
-from decouple import config
-
-# Build paths inside the project like this: os.path.join(BASE_DIR, ...)
-BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-
-
-# Quick-start development settings - unsuitable for production
-# See https://docs.djangoproject.com/en/1.11/howto/deployment/checklist/
-
-# SECURITY WARNING: keep the secret key used in production secret!
-SECRET_KEY = 'lkk8@h!zhe4lxwf1!t=#5@bm(iuep+t+e6xik=4*lo(yy3u=f!'
-
-# SECURITY WARNING: don't run with debug turned on in production!
-DEBUG = True
-
-ALLOWED_HOSTS = []
-
-
-# Application definition
-
-INSTALLED_APPS = [
-    'django.contrib.admin',
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.messages',
-    'django.contrib.staticfiles',
-    'django_daraja',
-]
-
-MIDDLEWARE = [
-    'django.middleware.security.SecurityMiddleware',
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.middleware.common.CommonMiddleware',
-    'django.middleware.csrf.CsrfViewMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
-    'django.middleware.clickjacking.XFrameOptionsMiddleware',
-]
-
-ROOT_URLCONF = 'tests.urls'
-
-TEMPLATES = [
-    {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'DIRS': [],
-        'APP_DIRS': True,
-        'OPTIONS': {
-            'context_processors': [
-                'django.template.context_processors.debug',
-                'django.template.context_processors.request',
-                'django.contrib.auth.context_processors.auth',
-                'django.contrib.messages.context_processors.messages',
-            ],
-        },
-    },
-]
-
-WSGI_APPLICATION = 'tests.wsgi.application'
-
-
-# Database
-# https://docs.djangoproject.com/en/1.11/ref/settings/#databases
-
-DATABASES = {
-    'default': {
-        'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
-    }
-}
-
-
-# Password validation
-# https://docs.djangoproject.com/en/1.11/ref/settings/#auth-password-validators
-
-AUTH_PASSWORD_VALIDATORS = [
-    {
-        'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',
-    },
-    {
-        'NAME': 'django.contrib.auth.password_validation.MinimumLengthValidator',
-    },
-    {
-        'NAME': 'django.contrib.auth.password_validation.CommonPasswordValidator',
-    },
-    {
-        'NAME': 'django.contrib.auth.password_validation.NumericPasswordValidator',
-    },
-]
-
-
-# Internationalization
-# https://docs.djangoproject.com/en/1.11/topics/i18n/
-
-LANGUAGE_CODE = 'en-us'
-
-TIME_ZONE = 'UTC'
-
-USE_I18N = True
-
-USE_L10N = True
-
-USE_TZ = True
-
-
-# Static files (CSS, JavaScript, Images)
-# https://docs.djangoproject.com/en/1.11/howto/static-files/
-
+"""
+Django settings for tests project.
+
+Generated by 'django-admin startproject' using Django 1.11.
+
+For more information on this file, see
+https://docs.djangoproject.com/en/1.11/topics/settings/
+
+For the full list of settings and their values, see
+https://docs.djangoproject.com/en/1.11/ref/settings/
+"""
+
+import os
+from decouple import config
+
+# Build paths inside the project like this: os.path.join(BASE_DIR, ...)
+BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+
+
+# Quick-start development settings - unsuitable for production
+# See https://docs.djangoproject.com/en/1.11/howto/deployment/checklist/
+
+# SECURITY WARNING: keep the secret key used in production secret!
+SECRET_KEY = 'lkk8@h!zhe4lxwf1!t=#5@bm(iuep+t+e6xik=4*lo(yy3u=f!'
+
+# SECURITY WARNING: don't run with debug turned on in production!
+DEBUG = True
+
+ALLOWED_HOSTS = ['testserver']
+
+
+# Application definition
+
+INSTALLED_APPS = [
+    'django.contrib.admin',
+    'django.contrib.auth',
+    'django.contrib.contenttypes',
+    'django.contrib.sessions',
+    'django.contrib.messages',
+    'django.contrib.staticfiles',
+    'django_daraja',
+]
+
+MIDDLEWARE = [
+    'django.middleware.security.SecurityMiddleware',
+    'django.contrib.sessions.middleware.SessionMiddleware',
+    'django.middleware.common.CommonMiddleware',
+    'django.middleware.csrf.CsrfViewMiddleware',
+    'django.contrib.auth.middleware.AuthenticationMiddleware',
+    'django.contrib.messages.middleware.MessageMiddleware',
+    'django.middleware.clickjacking.XFrameOptionsMiddleware',
+]
+
+ROOT_URLCONF = 'tests.urls'
+
+TEMPLATES = [
+    {
+        'BACKEND': 'django.template.backends.django.DjangoTemplates',
+        'DIRS': [],
+        'APP_DIRS': True,
+        'OPTIONS': {
+            'context_processors': [
+                'django.template.context_processors.debug',
+                'django.template.context_processors.request',
+                'django.contrib.auth.context_processors.auth',
+                'django.contrib.messages.context_processors.messages',
+            ],
+        },
+    },
+]
+
+WSGI_APPLICATION = 'tests.wsgi.application'
+
+
+# Database
+# https://docs.djangoproject.com/en/1.11/ref/settings/#databases
+
+DATABASES = {
+    'default': {
+        'ENGINE': 'django.db.backends.sqlite3',
+        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
+    }
+}
+
+
+# Password validation
+# https://docs.djangoproject.com/en/1.11/ref/settings/#auth-password-validators
+
+AUTH_PASSWORD_VALIDATORS = [
+    {
+        'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',
+    },
+    {
+        'NAME': 'django.contrib.auth.password_validation.MinimumLengthValidator',
+    },
+    {
+        'NAME': 'django.contrib.auth.password_validation.CommonPasswordValidator',
+    },
+    {
+        'NAME': 'django.contrib.auth.password_validation.NumericPasswordValidator',
+    },
+]
+
+
+# Internationalization
+# https://docs.djangoproject.com/en/1.11/topics/i18n/
+
+LANGUAGE_CODE = 'en-us'
+
+TIME_ZONE = 'UTC'
+
+USE_I18N = True
+
+USE_TZ = True
+
+
+# Static files (CSS, JavaScript, Images)
+# https://docs.djangoproject.com/en/1.11/howto/static-files/
+
 STATIC_URL = '/static/'
```

### Comparing `django-daraja-1.2.0/tests/test_oauth.py` & `django-daraja-1.3.0/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `django-daraja-1.2.0/tests/test_parse_result.py` & `django-daraja-1.3.0/tests/test_parse_result.py`

 * *Files identical despite different names*

### Comparing `django-daraja-1.2.0/tests/test_stk_push.py` & `django-daraja-1.3.0/tests/test_stk_push.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# -*- coding: utf-8 -*-
-'''
-Test STK Push
-'''
-
-from django.test import TestCase
-from django_daraja.mpesa.core import MpesaClient
-from decouple import config
-from django_daraja.mpesa.exceptions import MpesaInvalidParameterException
-from django_daraja.mpesa.utils import sleep
-
-class MpesaStkPushTestCase(TestCase):
-
-	cl = MpesaClient()
-	callback_url = 'https://darajambili.herokuapp.com/express-payment'
-
-	def test_stk_push_success(self):
-		'''
-		Test successful STK push
-		'''
-		
-		# Wait for a short while (to avoid SpikeArrest)
-		sleep(150, 'Test STK push success')
-
-		phone_number = config('LNM_PHONE_NUMBER')
-		amount = 1
-		account_reference = 'reference'
-		transaction_desc = 'Description'
-		response = self.cl.stk_push(phone_number, amount, account_reference, transaction_desc, self.callback_url)
-		self.assertEqual(response.response_description, 'Success. Request accepted for processing')
-
-	def test_stk_push_empty_reference(self):
-		'''
-		Test that STK push with empty account reference raises MpesaInvalidParameterException
-		'''
-
-		with self.assertRaises(MpesaInvalidParameterException):
-			phone_number = config('LNM_PHONE_NUMBER')
-			amount = 1
-			account_reference = ''
-			transaction_desc = 'Description'
-			self.cl.stk_push(phone_number, amount, account_reference, transaction_desc, self.callback_url)
-
-		
-	def test_stk_push_empty_description(self):
-		'''
-		Test that STK push with empty description raises MpesaInvalidParameterException
-		'''
-
-		with self.assertRaises(MpesaInvalidParameterException):
-			phone_number = config('LNM_PHONE_NUMBER')
-			amount = 1000000
-			account_reference = 'reference'
-			transaction_desc = ''
-			self.cl.stk_push(phone_number, amount, account_reference, transaction_desc, self.callback_url)
-
-	def test_stk_push_invalid_amount(self):
-		'''
-		Test that STK push with invalid amount raises MpesaInvalidParameterException
-		'''
-
-		with self.assertRaises(MpesaInvalidParameterException):
-			phone_number = config('LNM_PHONE_NUMBER')
-			amount = 1.5
-			account_reference = 'reference'
-			transaction_desc = 'Description'
-			self.cl.stk_push(phone_number, amount, account_reference, transaction_desc, self.callback_url)
+# -*- coding: utf-8 -*-
+'''
+Test STK Push
+'''
+
+from django.test import TestCase
+from django_daraja.mpesa.core import MpesaClient
+from decouple import config
+from django_daraja.mpesa.exceptions import MpesaInvalidParameterException
+
+class MpesaStkPushTestCase(TestCase):
+
+	cl = MpesaClient()
+	callback_url = 'https://api.darajambili.com/express-payment'
+
+	def test_stk_push_success(self):
+		'''
+		Test successful STK push
+		'''
+
+		phone_number = config('LNM_PHONE_NUMBER')
+		amount = 1
+		account_reference = 'reference'
+		transaction_desc = 'Description'
+		response = self.cl.stk_push(phone_number, amount, account_reference, transaction_desc, self.callback_url)
+		self.assertEqual(response.response_code, '0')
+		self.assertEqual(response.response_description, 'Success. Request accepted for processing')
+		self.assertTrue(len(response.merchant_request_id) > 0)
+		self.assertTrue(len(response.checkout_request_id) > 0)
+		self.assertTrue(len(response.customer_message) > 0)
+
+	def test_stk_push_empty_reference(self):
+		'''
+		Test that STK push with empty account reference raises MpesaInvalidParameterException
+		'''
+
+		with self.assertRaises(MpesaInvalidParameterException):
+			phone_number = config('LNM_PHONE_NUMBER')
+			amount = 1
+			account_reference = ''
+			transaction_desc = 'Description'
+			self.cl.stk_push(phone_number, amount, account_reference, transaction_desc, self.callback_url)
+
+		
+	def test_stk_push_empty_description(self):
+		'''
+		Test that STK push with empty description raises MpesaInvalidParameterException
+		'''
+
+		with self.assertRaises(MpesaInvalidParameterException):
+			phone_number = config('LNM_PHONE_NUMBER')
+			amount = 1000000
+			account_reference = 'reference'
+			transaction_desc = ''
+			self.cl.stk_push(phone_number, amount, account_reference, transaction_desc, self.callback_url)
+
+	def test_stk_push_invalid_amount(self):
+		'''
+		Test that STK push with invalid amount raises MpesaInvalidParameterException
+		'''
+
+		with self.assertRaises(MpesaInvalidParameterException):
+			phone_number = config('LNM_PHONE_NUMBER')
+			amount = 1.5
+			account_reference = 'reference'
+			transaction_desc = 'Description'
+			self.cl.stk_push(phone_number, amount, account_reference, transaction_desc, self.callback_url)
```

### Comparing `django-daraja-1.2.0/tests/urls.py` & `django-daraja-1.3.0/tests/urls.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""tests URL Configuration
-
-The `urlpatterns` list routes URLs to views. For more information please see:
-    https://docs.djangoproject.com/en/1.11/topics/http/urls/
-Examples:
-Function views
-    1. Add an import:  from my_app import views
-    2. Add a URL to urlpatterns:  url(r'^$', views.home, name='home')
-Class-based views
-    1. Add an import:  from other_app.views import Home
-    2. Add a URL to urlpatterns:  url(r'^$', Home.as_view(), name='home')
-Including another URLconf
-    1. Import the include() function: from django.conf.urls import url, include
-    2. Add a URL to urlpatterns:  url(r'^blog/', include('blog.urls'))
-"""
-from django.conf.urls import url, include
-from django.contrib import admin
-
-urlpatterns = [
-    url(r'^admin/', admin.site.urls),
-    url(r'^daraja/', include('django_daraja.urls')),
-]
+"""tests URL Configuration
+
+The `urlpatterns` list routes URLs to views. For more information please see:
+    https://docs.djangoproject.com/en/1.11/topics/http/urls/
+Examples:
+Function views
+    1. Add an import:  from my_app import views
+    2. Add a URL to urlpatterns:  url(r'^$', views.home, name='home')
+Class-based views
+    1. Add an import:  from other_app.views import Home
+    2. Add a URL to urlpatterns:  url(r'^$', Home.as_view(), name='home')
+Including another URLconf
+    1. Import the include() function: from django.urls import re_path as url, include
+    2. Add a URL to urlpatterns:  url(r'^blog/', include('blog.urls'))
+"""
+from django.urls import re_path as url, include
+from django.contrib import admin
+
+urlpatterns = [
+    url(r'^admin/', admin.site.urls),
+    url(r'^daraja/', include('django_daraja.urls')),
+]
```

