# Comparing `tmp/inema-0.8.7.tar.gz` & `tmp/inema-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inema-0.8.7.tar", last modified: Sun Jan  1 18:05:48 2023, max compression
+gzip compressed data, was "inema-0.8.8.tar", last modified: Sat May 27 11:21:10 2023, max compression
```

## Comparing `inema-0.8.7.tar` & `inema-0.8.8.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-01-01 18:05:48.018472 inema-0.8.7/
--rw-r--r--   0 gms       (1000) gms       (1000)    34520 2020-12-05 11:52:42.000000 inema-0.8.7/LICENSE
--rw-r--r--   0 gms       (1000) gms       (1000)     2551 2023-01-01 18:05:48.018472 inema-0.8.7/PKG-INFO
--rw-r--r--   0 gms       (1000) gms       (1000)     1962 2021-03-13 09:37:23.000000 inema-0.8.7/README.rst
-drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-01-01 18:05:48.018472 inema-0.8.7/inema/
--rw-r--r--   0 gms       (1000) gms       (1000)      158 2021-03-13 09:37:23.000000 inema-0.8.7/inema/__init__.py
-drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-01-01 18:05:48.018472 inema-0.8.7/inema/data/
--rw-r--r--   0 gms       (1000) gms       (1000)    60237 2020-12-05 11:52:42.000000 inema-0.8.7/inema/data/formats.json
--rw-r--r--   0 gms       (1000) gms       (1000)     8113 2023-01-01 17:57:14.000000 inema-0.8.7/inema/data/products.json
--rwxr-xr-x   0 gms       (1000) gms       (1000)    13717 2021-03-13 09:39:38.000000 inema-0.8.7/inema/frank.py
--rw-r--r--   0 gms       (1000) gms       (1000)    10881 2021-02-02 20:14:54.000000 inema-0.8.7/inema/inema.py
--rw-r--r--   0 gms       (1000) gms       (1000)    13970 2021-03-13 09:37:23.000000 inema-0.8.7/inema/wpint.py
-drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-01-01 18:05:48.018472 inema-0.8.7/inema.egg-info/
--rw-r--r--   0 gms       (1000) gms       (1000)     2551 2023-01-01 18:05:47.000000 inema-0.8.7/inema.egg-info/PKG-INFO
--rw-r--r--   0 gms       (1000) gms       (1000)      325 2023-01-01 18:05:48.000000 inema-0.8.7/inema.egg-info/SOURCES.txt
--rw-r--r--   0 gms       (1000) gms       (1000)        1 2023-01-01 18:05:47.000000 inema-0.8.7/inema.egg-info/dependency_links.txt
--rw-r--r--   0 gms       (1000) gms       (1000)       43 2023-01-01 18:05:47.000000 inema-0.8.7/inema.egg-info/entry_points.txt
--rw-r--r--   0 gms       (1000) gms       (1000)       29 2023-01-01 18:05:47.000000 inema-0.8.7/inema.egg-info/requires.txt
--rw-r--r--   0 gms       (1000) gms       (1000)        6 2023-01-01 18:05:47.000000 inema-0.8.7/inema.egg-info/top_level.txt
--rw-r--r--   0 gms       (1000) gms       (1000)       92 2023-01-01 18:05:48.018472 inema-0.8.7/setup.cfg
--rw-r--r--   0 gms       (1000) gms       (1000)     1159 2023-01-01 17:57:56.000000 inema-0.8.7/setup.py
+drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-05-27 11:21:10.667201 inema-0.8.8/
+-rw-r--r--   0 gms       (1000) gms       (1000)     7651 2023-05-19 17:49:22.000000 inema-0.8.8/LICENSE
+-rw-r--r--   0 gms       (1000) gms       (1000)     2551 2023-05-27 11:21:10.667201 inema-0.8.8/PKG-INFO
+-rw-r--r--   0 gms       (1000) gms       (1000)     1962 2021-03-13 09:37:23.000000 inema-0.8.8/README.rst
+drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-05-27 11:21:10.666201 inema-0.8.8/inema/
+-rw-r--r--   0 gms       (1000) gms       (1000)      158 2021-03-13 09:37:23.000000 inema-0.8.8/inema/__init__.py
+drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-05-27 11:21:10.667201 inema-0.8.8/inema/data/
+-rw-r--r--   0 gms       (1000) gms       (1000)    60237 2020-12-05 11:52:42.000000 inema-0.8.8/inema/data/formats.json
+-rw-r--r--   0 gms       (1000) gms       (1000)    10382 2023-05-19 17:51:32.000000 inema-0.8.8/inema/data/products-2023-07-01.json
+-rw-r--r--   0 gms       (1000) gms       (1000)     8113 2023-01-01 17:57:14.000000 inema-0.8.8/inema/data/products.json
+-rwxr-xr-x   0 gms       (1000) gms       (1000)    13755 2023-05-19 17:49:22.000000 inema-0.8.8/inema/frank.py
+-rw-r--r--   0 gms       (1000) gms       (1000)    10070 2023-05-19 17:49:22.000000 inema-0.8.8/inema/inema.py
+-rw-r--r--   0 gms       (1000) gms       (1000)      901 2023-05-19 17:49:22.000000 inema-0.8.8/inema/utils.py
+-rw-r--r--   0 gms       (1000) gms       (1000)    13183 2023-05-19 17:49:22.000000 inema-0.8.8/inema/wpint.py
+drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-05-27 11:21:10.666201 inema-0.8.8/inema.egg-info/
+-rw-r--r--   0 gms       (1000) gms       (1000)     2551 2023-05-27 11:21:10.000000 inema-0.8.8/inema.egg-info/PKG-INFO
+-rw-r--r--   0 gms       (1000) gms       (1000)      376 2023-05-27 11:21:10.000000 inema-0.8.8/inema.egg-info/SOURCES.txt
+-rw-r--r--   0 gms       (1000) gms       (1000)        1 2023-05-27 11:21:10.000000 inema-0.8.8/inema.egg-info/dependency_links.txt
+-rw-r--r--   0 gms       (1000) gms       (1000)       43 2023-05-27 11:21:10.000000 inema-0.8.8/inema.egg-info/entry_points.txt
+-rw-r--r--   0 gms       (1000) gms       (1000)       29 2023-05-27 11:21:10.000000 inema-0.8.8/inema.egg-info/requires.txt
+-rw-r--r--   0 gms       (1000) gms       (1000)        6 2023-05-27 11:21:10.000000 inema-0.8.8/inema.egg-info/top_level.txt
+-rw-r--r--   0 gms       (1000) gms       (1000)       92 2023-05-27 11:21:10.667201 inema-0.8.8/setup.cfg
+-rw-r--r--   0 gms       (1000) gms       (1000)     1224 2023-05-19 17:55:56.000000 inema-0.8.8/setup.py
```

### Comparing `inema-0.8.7/PKG-INFO` & `inema-0.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: inema
-Version: 0.8.7
+Version: 0.8.8
 Summary: A Python interface to the Deutsche Post Internetmarke and Warenpost International Online Franking
 Home-page: https://git.sysmocom.de/odoo/python-inema/
 Author: Harald Welte
 Author-email: hwelte@sysmocom.de
-License: AGPLv3
+License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business
 License-File: LICENSE
 
 python-inema
 ============
```

### Comparing `inema-0.8.7/README.rst` & `inema-0.8.8/README.rst`

 * *Files identical despite different names*

### Comparing `inema-0.8.7/inema/data/formats.json` & `inema-0.8.8/inema/data/formats.json`

 * *Files identical despite different names*

### Comparing `inema-0.8.7/inema/data/products.json` & `inema-0.8.8/inema/data/products.json`

 * *Files identical despite different names*

### Comparing `inema-0.8.7/inema/frank.py` & `inema-0.8.8/inema/frank.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 
-# 2016, Georg Sauthoff <mail@georg.so>, GPLv3+
+# 2016, Georg Sauthoff <mail@georg.so>, LGPLv3+
+# SPDX-Identifier: LGPL-3.0-or-later
 
 import argparse
 import configparser
 import csv
 import datetime
 import json
 import logging
```

### Comparing `inema-0.8.7/inema/inema.py` & `inema-0.8.8/inema/inema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
+# SPDX-Identifier: LGPL-3.0-or-later
 
-from datetime import datetime, date
-from pytz import timezone
-import hashlib
+from datetime import date
 import json
 from lxml import etree
 from zeep import Client
 from zeep.wsse.username import UsernameToken
 from pkg_resources import resource_stream, resource_listdir
 import pkg_resources
 import requests, zipfile
 import io
 import logging
 import decimal
 
+from .utils import compute_1c4a_hash, gen_timestamp
+
 __version__ = pkg_resources.get_distribution(__package__).version
 
 _logger = logging.getLogger(__name__)
 
 
 # Read the most recent inema/data/products-YYYY-MM-DD.json where YYYY-MM-DD is
 # not more recent than today. Fall back to inema/data/products.json.
@@ -57,33 +58,14 @@
 
 
 class Internetmarke(object):
     wsdl_url = 'https://internetmarke.deutschepost.de/OneClickForAppV3/OneClickForAppServiceV3?wsdl'
 
     # generate a 1C4A SOAP header
     def gen_1c4a_hdr(self, partner_id, key_phase, key):
-        # Compute 1C4A request hash accordig to Section 4 of service description
-        def compute_1c4a_hash(partner_id, req_ts, key_phase, key):
-            # trim leading and trailing spaces of each argument
-            partner_id = partner_id.strip()
-            req_ts = req_ts.strip()
-            key_phase = key_phase.strip()
-            key = key.strip()
-            # concatenate with "::" separator
-            inp = "%s::%s::%s::%s" % (partner_id, req_ts, key_phase, key)
-            # compute MD5 hash as 32 hex nibbles
-            md5_hex = hashlib.md5(inp.encode('utf8')).hexdigest()
-            # return the first 8 characters
-            return md5_hex[:8]
-
-        def gen_timestamp():
-            de_zone = timezone("Europe/Berlin")
-            de_time = datetime.now(de_zone)
-            return de_time.strftime("%d%m%Y-%H%M%S")
-
         nsmap={'soapenv': 'http://schemas.xmlsoap.org/soap/envelope/',
                'v3':'http://oneclickforpartner.dpag.de'}
         r = etree.Element("{http://schemas.xmlsoap.org/soap/envelope/}Header", nsmap = nsmap)
         p = etree.SubElement(r, "{http://oneclickforpartner.dpag.de}PARTNER_ID")
         p.text = partner_id
         t = etree.SubElement(r, "{http://oneclickforpartner.dpag.de}REQUEST_TIMESTAMP")
         t.text = gen_timestamp()
```

### Comparing `inema-0.8.7/inema/wpint.py` & `inema-0.8.8/inema/wpint.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 # This is a completely different interface that Deutsche Post came up many years
 # after the "1C4A" Internetmarke API.  For some strange reason they didn't
 # extend the old Internetmarke API to add support for the harmonized label and
 # the electronic customs declaration.  Instead, they decided to implement a
 # completely different API with different standards (REST vs. SOAP) with
 # literally nothing in common to the old Internetmarke API
 
+# SPDX-Identifier: LGPL-3.0-or-later
+
 import json
 import logging
-import hashlib
-from datetime import datetime
 
 import requests
 from lxml import etree
-from pytz import timezone
+
+from .utils import compute_1c4a_hash, gen_timestamp
 
 _logger = logging.getLogger(__name__)
 
 class WarenpostInt(object):
     """Represents the Warenpost Internatoinal ReST interface."""
     def __init__(self, partner_id, key, ekp, pk_email, pk_passwd, key_phase="1", sandbox = False):
         self.sandbox = sandbox
@@ -35,51 +36,27 @@
             self.url = 'https://api-qa.deutschepost.com/dpi/shipping/v1'
         else:
             self.auth_url = 'https://api.deutschepost.com/v1'
             self.url = 'https://api.deutschepost.com/dpi/shipping/v1'
         self.user_token = None
         self.wallet_balance = None
 
-    # FIXME: merge with inema?
-    @staticmethod
-    def compute_1c4a_hash(partner_id, req_ts, key_phase, key):
-        """ Compute 1C4A request hash accordig to Section 4 of service description. """
-        # trim leading and trailing spaces of each argument
-        partner_id = partner_id.strip()
-        req_ts = req_ts.strip()
-        key_phase = key_phase.strip()
-        key = key.strip()
-        # concatenate with "::" separator
-        inp = "%s::%s::%s::%s" % (partner_id, req_ts, key_phase, key)
-        # compute MD5 hash as 32 hex nibbles
-        md5_hex = hashlib.md5(inp.encode('utf8')).hexdigest()
-        # return the first 8 characters
-        return md5_hex[:8]
-
-    # FIXME: merge with inema?
-    @staticmethod
-    def gen_timestamp():
-        """Generate a timestamp as used in the Warenpsost International API."""
-        de_zone = timezone("Europe/Berlin")
-        de_time = datetime.now(de_zone)
-        return de_time.strftime("%d%m%Y-%H%M%S")
-
     def gen_headers(self):
         """Generate the HTTP headers required for the API."""
         ret = {
             'KEY_PHASE': self.key_phase,
             'PARTNER_ID': self.partner_id,
             'Authorization': 'Bearer %s' % self.user_token
             }
         if self.sandbox:
             ret['REQUEST_TIMESTAMP'] = '16082018-122210'
             ret['PARTNER_SIGNATURE'] = '9d7c35be'
         else:
-            timestamp = self.gen_timestamp()
-            sig = self.compute_1c4a_hash(self.partner_id, timestamp, self.key_phase, self.key)
+            timestamp = gen_timestamp()
+            sig = compute_1c4a_hash(self.partner_id, timestamp, self.key_phase, self.key)
             ret['REQUEST_TIMESTAMP'] = timestamp
             ret['PARTNER_SIGNATURE'] = sig
         return ret
 
     def get_token(self):
         """Get an Access Token for further API requests."""
         url = "%s/%s" % (self.auth_url, 'auth/accesstoken')
@@ -292,23 +269,28 @@
         return ret
 
     def api_create_order(self, items, contact_name, order_status='FINALIZE'):
         """Issue an API request to create an order consisting of items."""
         order = self.build_order(items, contact_name=contact_name, order_status=order_status)
         _logger.info("Order Request: %s", order)
         r = self.request('POST', 'orders', json = order)
+        if r.ok:
         # TODO: figure out the AWB and the (item, barcode, voucherId, ...) for the items
-        json_resp = r.json()
-        #print(json.dumps(json_resp, indent=4))
-        _logger.info("Order Response: %s", json_resp)
-        # TODO: download the PDF for each AWB
-        return json_resp
+            json_resp = r.json()
+            #print(json.dumps(json_resp, indent=4))
+            _logger.info("Order Response: %s", json_resp)
+            # TODO: download the PDF for each AWB
+            return json_resp
+        else:
+            raise ValueError('%s: %s' % (r.status_code, r.text))
 
     def api_get_item_label(self, item_id, accept='application/pdf'):
         """Download the label for a given item.  Returns PDF as 'bytes'"""
         r = self.request('GET', 'items/%s/label' % item_id, headers={'Accept': accept})
+        r.raise_for_status()
         return r.content
 
     def api_get_item_labels(self, awb, accept='application/pdf'):
         """Download the labels for all items in a given AWB. Returns PDF as 'bytes'"""
         r = self.request('GET', 'shipments/%s/itemlabels' % awb, headers={'Accept': accept})
+        r.raise_for_status()
         return r.content
```

### Comparing `inema-0.8.7/inema.egg-info/PKG-INFO` & `inema-0.8.8/inema.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: inema
-Version: 0.8.7
+Version: 0.8.8
 Summary: A Python interface to the Deutsche Post Internetmarke and Warenpost International Online Franking
 Home-page: https://git.sysmocom.de/odoo/python-inema/
 Author: Harald Welte
 Author-email: hwelte@sysmocom.de
-License: AGPLv3
+License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business
 License-File: LICENSE
 
 python-inema
 ============
```

### Comparing `inema-0.8.7/setup.py` & `inema-0.8.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,29 @@
         'zeep >= 0.12.0',
         'pytz',
         'setuptools' # i.e. provides pkg_resources
 ]
 
 setup(
         name='inema',
-        version='0.8.7',
+        version='0.8.8',
         description='A Python interface to the Deutsche Post Internetmarke and Warenpost International Online Franking',
         long_description=open('README.rst').read(),
         author='Harald Welte',
         author_email='hwelte@sysmocom.de',
         url='https://git.sysmocom.de/odoo/python-inema/',
         packages=['inema'],
         install_requires=install_requires,
         package_data={'inema': ['data/products.json',
+                                'data/products-2023-07-01.json',
                                 'data/formats.json']},
-        license='AGPLv3',
+        license='LGPLv3',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
-            'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
+            'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
             'Programming Language :: Python :: 2.7',
             'Programming Language :: Python :: 3',
             'Topic :: Office/Business',
         ],
         entry_points={
             'console_scripts': [ 'frank = inema.frank:main' ]
         },
```

