# Comparing `tmp/PyOTRS-0.9.0.tar.gz` & `tmp/PyOTRS-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyOTRS-0.9.0.tar", last modified: Thu Apr 23 21:35:13 2020, max compression
+gzip compressed data, was "PyOTRS-1.0.1.tar", last modified: Sat May 27 11:07:49 2023, max compression
```

## Comparing `PyOTRS-0.9.0.tar` & `PyOTRS-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/
--rw-rw-r--   0 robbie    (1000) robbie    (1000)      131 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/setup.cfg
--rw-rw-r--   0 robbie    (1000) robbie    (1000)      235 2017-07-12 19:07:34.000000 PyOTRS-0.9.0/MANIFEST.in
-drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/webservices_templates/
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     2154 2017-03-04 20:30:10.000000 PyOTRS-0.9.0/webservices_templates/GenericLinkConnectorREST.yml
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     1745 2020-04-23 20:54:54.000000 PyOTRS-0.9.0/webservices_templates/GenericTicketConnectorREST.yml
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     1338 2017-03-04 21:03:17.000000 PyOTRS-0.9.0/webservices_templates/GenericFAQConnectorREST.yml
--rw-rw-r--   0 robbie    (1000) robbie    (1000)    17191 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/PKG-INFO
-drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/pyotrs/
--rw-rw-r--   0 robbie    (1000) robbie    (1000)      273 2020-04-23 21:07:39.000000 PyOTRS-0.9.0/pyotrs/version.py
--rw-rw-r--   0 robbie    (1000) robbie    (1000)    71254 2020-04-23 20:54:54.000000 PyOTRS-0.9.0/pyotrs/lib.py
--rw-rw-r--   0 robbie    (1000) robbie    (1000)      690 2020-03-12 20:20:18.000000 PyOTRS-0.9.0/pyotrs/__init__.py
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     2052 2020-04-17 15:35:36.000000 PyOTRS-0.9.0/setup.py
--rw-rw-r--   0 robbie    (1000) robbie    (1000)    11787 2020-04-23 21:21:51.000000 PyOTRS-0.9.0/README.rst
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     1088 2020-04-06 11:16:28.000000 PyOTRS-0.9.0/LICENSE
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     3633 2020-04-23 21:07:39.000000 PyOTRS-0.9.0/CHANGELOG.rst
-drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/PyOTRS.egg-info/
--rw-rw-r--   0 robbie    (1000) robbie    (1000)    17191 2020-04-23 21:35:12.000000 PyOTRS-0.9.0/PyOTRS.egg-info/PKG-INFO
--rw-rw-r--   0 robbie    (1000) robbie    (1000)        1 2020-04-23 21:35:12.000000 PyOTRS-0.9.0/PyOTRS.egg-info/dependency_links.txt
--rw-rw-r--   0 robbie    (1000) robbie    (1000)       11 2020-04-23 21:35:12.000000 PyOTRS-0.9.0/PyOTRS.egg-info/top_level.txt
--rw-rw-r--   0 robbie    (1000) robbie    (1000)      509 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/PyOTRS.egg-info/SOURCES.txt
--rw-rw-r--   0 robbie    (1000) robbie    (1000)        1 2020-04-23 19:25:53.000000 PyOTRS-0.9.0/PyOTRS.egg-info/not-zip-safe
--rw-rw-r--   0 robbie    (1000) robbie    (1000)       43 2020-04-23 21:35:12.000000 PyOTRS-0.9.0/PyOTRS.egg-info/requires.txt
--rw-rw-r--   0 robbie    (1000) robbie    (1000)       61 2020-04-23 21:35:12.000000 PyOTRS-0.9.0/PyOTRS.egg-info/entry_points.txt
-drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/cli/
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     5331 2020-04-17 15:35:36.000000 PyOTRS-0.9.0/cli/PyOTRS.py
--rw-rw-r--   0 robbie    (1000) robbie    (1000)        0 2016-04-16 20:46:18.000000 PyOTRS-0.9.0/cli/__init__.py
+drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2023-05-27 11:07:49.386984 PyOTRS-1.0.1/
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)     5174 2023-05-27 11:06:02.000000 PyOTRS-1.0.1/CHANGELOG.rst
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)     1088 2020-04-06 11:16:28.000000 PyOTRS-1.0.1/LICENSE
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)      235 2017-07-12 19:07:34.000000 PyOTRS-1.0.1/MANIFEST.in
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)    17480 2023-05-27 11:07:49.386984 PyOTRS-1.0.1/PKG-INFO
+drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2023-05-27 11:07:49.374984 PyOTRS-1.0.1/PyOTRS.egg-info/
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)    17480 2023-05-27 11:07:49.000000 PyOTRS-1.0.1/PyOTRS.egg-info/PKG-INFO
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)      459 2023-05-27 11:07:49.000000 PyOTRS-1.0.1/PyOTRS.egg-info/SOURCES.txt
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)        1 2023-05-27 11:07:49.000000 PyOTRS-1.0.1/PyOTRS.egg-info/dependency_links.txt
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)       61 2023-05-27 11:07:49.000000 PyOTRS-1.0.1/PyOTRS.egg-info/entry_points.txt
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)        1 2020-04-23 19:25:53.000000 PyOTRS-1.0.1/PyOTRS.egg-info/not-zip-safe
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)       43 2023-05-27 11:07:49.000000 PyOTRS-1.0.1/PyOTRS.egg-info/requires.txt
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)       11 2023-05-27 11:07:49.000000 PyOTRS-1.0.1/PyOTRS.egg-info/top_level.txt
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)    12164 2023-05-27 10:59:19.000000 PyOTRS-1.0.1/README.rst
+drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2023-05-27 11:07:49.374984 PyOTRS-1.0.1/cli/
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)     5527 2021-07-21 17:52:19.000000 PyOTRS-1.0.1/cli/PyOTRS.py
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)        0 2016-04-16 20:46:18.000000 PyOTRS-1.0.1/cli/__init__.py
+drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2023-05-27 11:07:49.374984 PyOTRS-1.0.1/pyotrs/
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)      678 2021-12-11 21:36:09.000000 PyOTRS-1.0.1/pyotrs/__init__.py
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)    72661 2023-05-27 10:58:38.000000 PyOTRS-1.0.1/pyotrs/lib.py
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)      273 2023-05-27 11:06:09.000000 PyOTRS-1.0.1/pyotrs/version.py
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)      131 2023-05-27 11:07:49.386984 PyOTRS-1.0.1/setup.cfg
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)     1846 2023-05-27 10:58:38.000000 PyOTRS-1.0.1/setup.py
+drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2023-05-27 11:07:49.386984 PyOTRS-1.0.1/webservices_templates/
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)     2154 2017-03-04 20:30:10.000000 PyOTRS-1.0.1/webservices_templates/GenericLinkConnectorREST.yml
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)     2046 2023-05-27 10:58:38.000000 PyOTRS-1.0.1/webservices_templates/GenericTicketConnectorREST.yml
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyOTRS-0.9.0/webservices_templates/GenericLinkConnectorREST.yml` & `PyOTRS-1.0.1/webservices_templates/GenericLinkConnectorREST.yml`

 * *Files identical despite different names*

### Comparing `PyOTRS-0.9.0/webservices_templates/GenericTicketConnectorREST.yml` & `PyOTRS-1.0.1/webservices_templates/GenericTicketConnectorREST.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 ---
 Debugger:
   DebugThreshold: info
   TestMode: '0'
-Description: Ticket Connector REST Sample
-FrameworkVersion: 5.0.13
+Description: Ticket Connector REST
+FrameworkVersion: 6.0.13
 Provider:
   Operation:
     SessionCreate:
-      Description: Creates a Session
+      Description: Creates a new Session by providing UserLogin or CustomerUserLogin and Password
       MappingInbound: {}
       MappingOutbound: {}
       Type: Session::SessionCreate
+    SessionGet:
+      Description: Check and validate a Session ID
+      MappingInbound: {}
+      MappingOutbound: {}
+      Type: Session::SessionGet
     TicketCreate:
       Description: Creates a Ticket
       MappingInbound: {}
       MappingOutbound: {}
       Type: Ticket::TicketCreate
     TicketGet:
       Description: Retrieves Ticket data
@@ -41,29 +46,33 @@
       KeepAlive: ''
       MaxLength: '100000000'
       RouteOperationMapping:
         SessionCreate:
           RequestMethod:
           - POST
           Route: /Session
+        SessionGet:
+          RequestMethod:
+          - GET
+          Route: /Session/:SessionID
         TicketCreate:
           RequestMethod:
           - POST
           Route: /Ticket
         TicketGet:
           RequestMethod:
           - GET
           Route: /Ticket/:TicketID
         TicketGetList:
           RequestMethod:
           - GET
           Route: /TicketList
         TicketSearch:
           RequestMethod:
-          - POST
+          - GET
           Route: /TicketSearch
         TicketUpdate:
           RequestMethod:
           - PATCH
           Route: /Ticket/:TicketID
     Type: HTTP::REST
 RemoteSystem: ''
```

### Comparing `PyOTRS-0.9.0/PKG-INFO` & `PyOTRS-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOTRS
-Version: 0.9.0
+Version: 1.0.1
 Summary: Python wrapper for OTRS (using REST API)
 Home-page: https://gitlab.com/rhab/PyOTRS
 Author: Robert Habermann
 Author-email: mail@rhab.de
 Maintainer: Robert Habermann
 License: The MIT License (MIT)
 
@@ -34,48 +34,47 @@
         |VersionBadge| |BuildStatus| |CoverageReport| |DocsBuildStatus| |LicenseBadge| |PythonVersions|
         
         
         .. |VersionBadge| image:: https://badge.fury.io/py/PyOTRS.svg
             :target: https://badge.fury.io/py/PyOTRS
             :alt: |version|
         
-        .. |BuildStatus| image:: https://gitlab.com/rhab/PyOTRS/badges/master/pipeline.svg
-            :target: https://gitlab.com/rhab/PyOTRS/commits/master
+        .. |BuildStatus| image:: https://gitlab.com/rhab/PyOTRS/badges/main/pipeline.svg
+            :target: https://gitlab.com/rhab/PyOTRS/commits/main
             :alt: Build Status
         
-        .. |CoverageReport| image:: https://gitlab.com/rhab/PyOTRS/badges/master/coverage.svg
-            :target: https://gitlab.com/rhab/PyOTRS/commits/master
+        .. |CoverageReport| image:: https://gitlab.com/rhab/PyOTRS/badges/main/coverage.svg
+            :target: https://gitlab.com/rhab/PyOTRS/commits/main
             :alt: Coverage Report
         
         .. |DocsBuildStatus| image:: https://readthedocs.org/projects/pyotrs/badge/?version=stable
             :target: https://pyotrs.readthedocs.org/en/stable/index.html
             :alt: Docs Build Status
         
         .. |LicenseBadge| image:: https://img.shields.io/badge/license-MIT-blue.svg
-            :target: https://gitlab.com/rhab/PyOTRS/-/blob/master/LICENSE
+            :target: https://gitlab.com/rhab/PyOTRS/-/blob/main/LICENSE
             :alt: MIT licensed
         
-        .. |PythonVersions| image:: https://img.shields.io/badge/python-2.7%2C%203.4%2C%203.5%2C%203.6%2C%203.7%2C%203.8-blue.svg
-            :alt: python: 2.7, 3.4, 3.5, 3.6, 3.7, 3.8
+        .. |PythonVersions| image:: https://img.shields.io/badge/python-3.7%2C%203.8%2C%203.9%2C%203.10%2C%203.11-blue.svg
+            :alt: python: 3.7, 3.8, 3.9, 3.10, 3.11
         
         
-        PyOTRS is a Python wrapper for accessing `OTRS <https://www.otrs.com/>`_ (Version 5, 6, 7) using the
+        PyOTRS is a Python wrapper for accessing `OTRS <https://www.otrs.com/>`_ (Version 5, 6, 7, 8) using the
         (GenericInterface) REST API.
         
         Warning
         =======
         
-            Please upgrade PyOTRS to at least version 0.7.1 if you are using OTRS 6.0.27, 7.0.16 or
-            newer. See `issue 27 <https://gitlab.com/rhab/PyOTRS/-/issues/27>`_ and
-            `issue 29 <https://gitlab.com/rhab/PyOTRS/-/issues/29>`_ for more details.
+            Please upgrade PyOTRS to at least version 0.10.0 (recommended version is at least 1.0.0) if you
+            are using OTRS 6.0.27, 7.0.16 or newer. See `issue 27 <https://gitlab.com/rhab/PyOTRS/-/issues/27>`_
+            and `issue 29 <https://gitlab.com/rhab/PyOTRS/-/issues/29>`_ for more details.
         
             OTRS has introduced a new API in version 8 and with this also changed the API endpoint from
-            "Session::SessionCreate" to "AccessToken::Create". At the moment PyOTRS does not support
-            OTRS v8. See `issue 28 <https://gitlab.com/rhab/PyOTRS/-/issues/28>`_ for progress and
-            discussions.
+            "Session::SessionCreate" to "AccessToken::Create". PyOTRS attempts to use the new API and will
+            fallback to the old way ("legacy") if the attempt fails.
         
         
         Features
         ========
         
         Access an OTRS instance to::
         
@@ -99,17 +98,16 @@
         Installation
         ============
         
         OTRS Prerequisite
         -----------------
         
         You have to enable the **webservices** in your OTRS instance.  It is recommended to use the
-        provided `template <https://gitlab.com/rhab/PyOTRS/raw/master/webservices_templates/GenericTicketConnectorREST.yml>`_.
-        This YAML configuration template includes the **Route: /TicketList** endpoint that is **required for PyOTRS** but which
-        is not included in the default OTRS webservice setup.
+        provided `template <https://gitlab.com/rhab/PyOTRS/raw/main/webservices_templates/GenericTicketConnectorREST.yml>`_.
+        This YAML configuration template includes the **Route: /TicketList** and **SessionGet: /Session/:SessionID** endpoint which both are **required for PyOTRS** but which are not included in the default OTRS webservice setup.
         
         Dependencies
         ------------
         
         *Dependencies are installed automatically*
         
         pip::
@@ -143,14 +141,25 @@
         
             from pyotrs import Client
             client = Client("https://otrs.example.com", "root@localhost", "password")
             client.session_create()
             client.ticket_get_by_id(1)
         
         
+        The usage of ``Client.session_restore_or_create`` is **recommended**. It uses a temporary file
+        on the hard drive to store the Session ID (just like cookies in a browser) and avoids sending
+        the username+password (and therefore creating a new session) on every API call::
+        
+            from pyotrs import Client
+            client = Client("https://otrs.example.com", "root@localhost", "password")
+            client.session_restore_or_create()
+            client.ticket_get_by_id(1)
+        
+        Method ``Client.session_restore_or_set_up_new`` is **deprecated** as of v0.10.
+        
         More Examples
         -------------
         
         - instantiate a ``Client`` object called **client**
         - create a session ("login") on **client**
         - get the ``Ticket`` with ID 1
         
@@ -307,22 +316,14 @@
         [u'2']
         
         
         
         Tips
         ----
         
-        When using **ipython** you could run into UTF8 encoding issues on Python2. This is a workaround
-        that can help::
-        
-            import sys
-            reload(sys)
-            sys.setdefaultencoding('utf-8')
-        
-        
         **If needed** the *insecure plattform warnings* can be disabled::
         
             # turn off platform insecurity warnings from urllib3
             from requests.packages.urllib3 import disable_warnings
             disable_warnings()  # TODO 2016-04-23 (RH) verify this
         
         PyOTRS Shell CLI
@@ -436,17 +437,15 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Pytest
 Classifier: Framework :: Sphinx
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
 Provides-Extra: cli
```

### Comparing `PyOTRS-0.9.0/pyotrs/lib.py` & `PyOTRS-1.0.1/pyotrs/lib.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
 TICKET_CONNECTOR_CONFIG_DEFAULT = {
     'Name': 'GenericTicketConnectorREST',
     'Config': {
         'SessionCreate': {'RequestMethod': 'POST',
                           'Route': '/Session',
                           'Result': 'SessionID'},
+        'AccessTokenCreate': {'RequestMethod': 'POST',
+                              'Route': '/Session',
+                              'Result': 'AccessToken'},
+        'SessionGet': {'RequestMethod': 'GET',
+                       'Route': '/Session/:SessionID',
+                       'Result': 'SessionData'},
         'TicketCreate': {'RequestMethod': 'POST',
                          'Route': '/Ticket',
                          'Result': 'TicketID'},
         'TicketGet': {'RequestMethod': 'GET',
                       'Route': '/Ticket/:TicketID',
                       'Result': 'Ticket'},
         'TicketGetList': {'RequestMethod': 'GET',
@@ -42,32 +48,14 @@
                          'Result': 'TicketID'},
         'TicketUpdate': {'RequestMethod': 'PATCH',
                          'Route': '/Ticket/:TicketID',
                          'Result': 'TicketID'},
     }
 }
 
-FAQ_CONNECTOR_CONFIG_DEFAULT = {
-    'Name': 'GenericFAQConnectorREST',
-    'Config': {
-        'LanguageList': {'RequestMethod': 'GET',
-                         'Route': '/LanguageList',
-                         'Result': 'Language'},
-        'PublicCategoryList': {'RequestMethod': 'GET',
-                               'Route': '/PublicCategoryList',
-                               'Result': 'Category'},
-        'PublicFAQGet': {'RequestMethod': 'GET',
-                         'Route': '/PublicFAQGet',
-                         'Result': 'FAQItem'},
-        'PublicFAQSearch': {'RequestMethod': 'POST',
-                            'Route': '/PublicFAQSearch',
-                            'Result': 'ID'},
-    }
-}
-
 LINK_CONNECTOR_CONFIG_DEFAULT = {
     'Name': 'GenericLinkConnectorREST',
     'Config': {
         'LinkAdd': {'RequestMethod': 'POST',
                     'Route': '/LinkAdd',
                     'Result': 'LinkAdd'},
         'LinkDelete': {'RequestMethod': 'DELETE',
@@ -87,14 +75,26 @@
                                 'Result': 'PossibleObject'},
         'PossibleTypesList': {'RequestMethod': 'GET',
                               'Route': '/PossibleTypesList',
                               'Result': 'PossibleType'},
     }
 }
 
+# Check if OS is Linux or Windows (#47):
+OS_TYPE_WINDOWS = False
+try:
+    from platform import system
+    if 'Windows' in system():
+        OS_TYPE_WINDOWS = True
+        log.debug("OS Type: Windows")
+    else:
+        log.debug("OS Type: Linux")
+except:  # noqa: E722
+    log.warning("Could not determine OS-Type (Linux/Windows). Using default: 'Linux'.")
+
 
 class PyOTRSError(Exception):
     def __init__(self, message):
         super(PyOTRSError, self).__init__(message)
         self.message = message
 
 
@@ -147,21 +147,19 @@
         self.dynamic_fields = self._parse_dynamic_fields()
         self.fields.pop("DynamicField", None)
 
     def __repr__(self):
         if self.aid != 0:
             _len = len(self.attachments)
             if _len == 0:
-                return "<ArticleID: {1}>".format(self.__class__.__name__, self.aid)
+                return "<ArticleID: {0}>".format(self.aid)
             elif _len == 1:
-                return "<ArticleID: {1} (1 Attachment)>".format(self.__class__.__name__,
-                                                                self.aid)
+                return "<ArticleID: {0} (1 Attachment)>".format(self.aid)
             else:
-                return "<ArticleID: {1} ({2} Attachments)>".format(self.__class__.__name__,
-                                                                   self.aid, _len)
+                return "<ArticleID: {0} ({1} Attachments)>".format(self.aid, _len)
         else:
             return "<{0}>".format(self.__class__.__name__)
 
     def to_dct(self, attachments=True, attachment_cont=True, dynamic_fields=True):
         """represent as nested dict compatible for OTRS
 
         Args:
@@ -724,33 +722,35 @@
 
     Args:
         file_path (str): Path on disc
         session_timeout (int): OTRS Session Timeout Value (to avoid reusing outdated session id
         value (str): A Session ID as str
         created (int): seconds as epoch when a session_id record was created
         expires (int): seconds as epoch when a session_id record expires
+        is_legacy (bool): whether the Session ID is for an older OTRS Version (<=7)
 
     Raises:
         ArgumentMissingError
 
     """
 
     def __init__(self, file_path=None, session_timeout=None,
-                 value=None, created=None, expires=None):
+                 value=None, created=None, expires=None, is_legacy=False):
         if not file_path:
             raise ArgumentMissingError("Argument file_path is required!")
 
         if not session_timeout:
             raise ArgumentMissingError("Argument session_timeout is required!")
 
         self.file_path = file_path
         self.timeout = session_timeout
         self.value = value
         self.created = created
         self.expires = expires
+        self.is_legacy = is_legacy
 
     def __repr__(self):
         return "<{0}: {1}>".format(self.__class__.__name__, self.file_path)
 
     def read(self):
         """Retrieve a stored Session ID from file
 
@@ -765,17 +765,18 @@
             return None
 
         with open(self.file_path, "r") as f:
             content = f.read()
         try:
             data = json.loads(content)
             self.value = data['session_id']
+            self.is_legacy = data.get('is_legacy', False)
 
             self.created = datetime.datetime.utcfromtimestamp(int(data['created']))
-            self.expires = (self.created + datetime.timedelta(minutes=self.timeout))
+            self.expires = (self.created + datetime.timedelta(seconds=self.timeout))
 
             if self.expires > datetime.datetime.utcnow():
                 return self.value  # still valid
         except ValueError:
             return None
         except KeyError:
             return None
@@ -795,15 +796,16 @@
 
         if os.path.isfile(self.file_path):
             if not SessionStore._validate_file_owner_and_permissions(self.file_path):
                 raise IOError("File exists but is not ok (wrong owner/permissions)!")
 
         with open(self.file_path, 'w') as f:
             f.write(json.dumps({'created': str(int(time.time())),
-                                'session_id': self.value}))
+                                'session_id': self.value,
+                                'is_legacy': self.is_legacy}))
         os.chmod(self.file_path, 384)  # 384 is '0600'
 
         # TODO 2016-04-23 (RH): check this
         if not SessionStore._validate_file_owner_and_permissions(self.file_path):
             raise IOError("Race condition: Something happened to file during the run!")
 
         return True
@@ -826,20 +828,23 @@
     def _validate_file_owner_and_permissions(full_file_path):
         """validate SessionStore file ownership and permissions
 
         Args:
             full_file_path (str): full path to file on disc
 
         Returns:
-            **bool**: **True** if valid and correct, otherwise **False**...
+            **bool**: **True** if valid and correct (or running on Windows), otherwise **False**...
 
         """
         if not os.path.isfile(full_file_path):
             raise IOError("Does not exist or not a file: {0}".format(full_file_path))
 
+        if OS_TYPE_WINDOWS:  # We have to do this, as os.getuid() is not defined if run on Windows
+            return True
+
         file_lstat = os.lstat(full_file_path)
         if not file_lstat.st_uid == os.getuid():
             return False
 
         if not file_lstat.st_mode & 0o777 == 384:
             """ check for unix permission User R+W only (0600)
             >>> oct(384)
@@ -859,29 +864,31 @@
         username (str): Username
         password (str): Password
         session_id_file (str): Session ID path on disc, used to persistently store Session ID
         session_timeout (int): Session Timeout configured in OTRS (usually 28800 seconds = 8h)
         session_validation_ticket_id (int): Ticket ID of an existing ticket - used to perform
             several check - e.g. validate log in (defaults to 1)
         webservice_config_ticket (dict): OTRS REST Web Service Name - Ticket Connector
-        webservice_config_faq (dict): OTRS REST Web Service Name - FAQ Connector
+        webservice_config_faq (dict): OTRS REST Web Service Name - FAQ Connector (FAQ code was
+            deprecated in 0.4.0 and removed in 1.0.0 - parameter stays for compatibility)
         webservice_config_link (dict): OTRS REST Web Service Name - Link Connector
         proxies (dict): Proxy settings - refer to requests docs for
             more information - default to no proxies
         https_verify (bool): Should HTTPS certificates be verified (defaults to True)
         ca_cert_bundle (str): file path - if specified overrides python/system default for
             Root CA bundle that will be used.
         auth (tuple): e.g. ("user", "pass") - see requests documentation ("auth") for details
         client_auth_cert (str): file path containing both certificate and key (unencrypted) in
             PEM format to use for TLS client authentication (passed to requests as "cert")
         customer_user (bool): flag to indicate that the username is for a "CustomerUser"
            (defaults to False)
         user_agent (str): optional HTTP UserAgent string
         webservice_path (str): OTRS REST Web Service Path part - defaults to
             "/otrs/nph-genericinterface.pl/Webservice/"
+        use_legacy_sessions (bool): if True, use sessions compatibility for OTRS < V8
 
     """
 
     def __init__(self,
                  baseurl=None,
                  username=None,
                  password=None,
@@ -894,57 +901,62 @@
                  proxies=None,
                  https_verify=True,
                  ca_cert_bundle=None,
                  auth=None,
                  client_auth_cert=None,
                  customer_user=False,
                  user_agent=None,
-                 webservice_path="/otrs/nph-genericinterface.pl/Webservice/"):
+                 webservice_path="/otrs/nph-genericinterface.pl/Webservice/",
+                 use_legacy_sessions=False
+                 ):
 
         if not baseurl:
             raise ArgumentMissingError("baseurl")
         self.baseurl = baseurl.rstrip("/")
         self.webservice_path = webservice_path
 
         if not session_timeout:
             self.session_timeout = 28800  # 8 hours is OTRS default
         else:
             self.session_timeout = session_timeout
 
         if not session_id_file:
-            self.session_id_store = SessionStore(file_path="/tmp/.pyotrs_session_id",
-                                                 session_timeout=self.session_timeout)
+            if OS_TYPE_WINDOWS:
+                # No '/tmp/...' available on Windows OS, so using in Windows Temp folder instead
+                p = os.path.expanduser('~\\AppData\\Local\\Temp\\.pyotrs_session_id')
+                SESSION_ID_PATH = p
+            else:
+                SESSION_ID_PATH = "/tmp/.pyotrs_session_id"  # Default for Linux
+
+            self.session_id_store = SessionStore(file_path=SESSION_ID_PATH,
+                                                 session_timeout=self.session_timeout,
+                                                 is_legacy=use_legacy_sessions)
         else:
             self.session_id_store = SessionStore(file_path=session_id_file,
-                                                 session_timeout=self.session_timeout)
+                                                 session_timeout=self.session_timeout,
+                                                 is_legacy=use_legacy_sessions)
 
         self.session_validation_ticket_id = session_validation_ticket_id
 
         # A dictionary for mapping OTRS WebService operations to HTTP Method, Route and
         # Result string.
         if not webservice_config_ticket:
             webservice_config_ticket = TICKET_CONNECTOR_CONFIG_DEFAULT
 
-        if not webservice_config_faq:
-            webservice_config_faq = FAQ_CONNECTOR_CONFIG_DEFAULT
-
         if not webservice_config_link:
             webservice_config_link = LINK_CONNECTOR_CONFIG_DEFAULT
 
         self.ws_ticket = webservice_config_ticket['Name']
-        self.ws_faq = webservice_config_faq['Name']
         self.ws_link = webservice_config_link['Name']
 
         self.routes_ticket = [x[1]["Route"] for x in webservice_config_ticket['Config'].items()]
-        self.routes_faq = [x[1]["Route"] for x in webservice_config_faq['Config'].items()]
         self.routes_link = [x[1]["Route"] for x in webservice_config_link['Config'].items()]
 
         webservice_config = {}
         webservice_config.update(webservice_config_ticket['Config'])
-        webservice_config.update(webservice_config_faq['Config'])
         webservice_config.update(webservice_config_link['Config'])
         self.ws_config = webservice_config
 
         if not proxies:
             self.proxies = {"http": "", "https": "", "no": ""}
         else:
             if not isinstance(proxies, dict):
@@ -965,30 +977,53 @@
         self.auth = auth
         self.client_auth_cert = client_auth_cert
 
         self.customer_user = customer_user
 
         self.user_agent = user_agent
 
+        self.use_legacy_sessions = use_legacy_sessions
+
         # credentials
         self.username = username
         self.password = password
 
         # dummy initialization
         self.operation = None
         self.result_json = None
         self.result = []
 
     """
+    Returns the correct session key to look for/send based
+    on the current session compatibility level
+    for legacy sessions (< OTRS V8) this returns 'SessionID'
+    from V8 onwards this returns 'AccessToken'
+    """
+
+    @property
+    def _session_key(self):
+        if self.use_legacy_sessions:
+            return 'SessionID'
+        else:
+            return 'AccessToken'
+
+    """
     GenericInterface::Operation::Session::SessionCreate
         * session_check_is_valid
         * session_create
+        * session_get
         * session_restore_or_set_up_new  # try to get session_id from a (json) file on disc
     """
 
+    @deprecation.deprecated(deprecated_in="0.10.0", removed_in="2.0", current_version=__version__,
+                            details="This method was implemented with a \"dirty\" workaround and "
+                                    "should not be called anymore. Use Client.session_get() "
+                                    "instead. ATTENTION: Using session_get() requires the OTRS "
+                                    "route for HTTP GET /Session to be configured  (which is/was "
+                                    "not the default).")
     def session_check_is_valid(self, session_id=None):
         """check whether session_id is currently valid
 
         Args:
             session_id (str): optional if set overrides the self.session_id
 
         Raises:
@@ -1002,17 +1037,17 @@
         """
         self.operation = "TicketGet"
 
         if not session_id:
             raise ArgumentMissingError("session_id")
 
         # TODO 2016-04-13 (RH): Is there a nicer way to check whether session is valid?!
-        payload = {"SessionID": session_id}
+        payload = {self._session_key: session_id}
 
-        response = self._send_request(payload, ticket_id=self.session_validation_ticket_id)
+        response = self._send_request(payload, data_id=self.session_validation_ticket_id)
         return self._parse_and_validate_response(response)
 
     def session_create(self):
         """create new (temporary) session (and Session ID)
 
         Returns:
             **bool**: **True** if successful, otherwise **False**.
@@ -1020,33 +1055,115 @@
         .. note::
             Session ID is recorded in self.session_id_store.value (**non persistently**)
 
         .. note::
             Uses HTTP Method: POST
 
         """
-        self.operation = "SessionCreate"
+        if self.use_legacy_sessions:
+            self.operation = "SessionCreate"
+        else:
+            self.operation = "AccessTokenCreate"
 
         if self.customer_user:
             payload = {
                 "CustomerUserLogin": self.username,
                 "Password": self.password
             }
         else:
             payload = {
                 "UserLogin": self.username,
                 "Password": self.password
             }
 
-        if not self._parse_and_validate_response(self._send_request(payload)):
+        response = self._send_request(payload)
+        try:
+            if not self._parse_and_validate_response(response):
+                return False
+        except ResponseParseError:
+            if not self.use_legacy_sessions:
+                log.warning("AccessTokenCreate failed, retrying using legacy session")
+                self.use_legacy_sessions = True
+                self.session_id_store.is_legacy = True
+                return self.session_create()
             return False
 
-        self.session_id_store.value = self.result_json['SessionID']
+        self.session_id_store.value = self.result_json[self._session_key]
         return True
 
+    def session_get(self, session_id=None):
+        """get/check/validate a Session ID
+
+        Returns:
+            **bool**: **True** if successful, otherwise **False**.
+
+        .. note::
+            Uses HTTP Method: GET
+
+        """
+        self.operation = "SessionGet"
+
+        if not session_id:
+            raise ArgumentMissingError("session_id")
+
+        payload = {self._session_key: session_id}
+
+        response = self._send_request(payload, data_id=session_id)
+        return self._parse_and_validate_response(response)
+
+    def session_restore_or_create(self):
+        """Try to restore Session ID from file otherwise create new one and save to file
+
+        Raises:
+            SessionCreateError
+            SessionIDFileError
+
+        .. note::
+            Session ID is recorded in self.session_id_store.value (**non persistently**)
+
+        .. note::
+            Session ID is **saved persistently** to file: *self.session_id_store.file_path*
+
+        Returns:
+            **bool**: **True** if successful, otherwise **False**.
+        """
+        # try to read session_id from file
+        self.session_id_store.value = self.session_id_store.read()
+
+        if self.session_id_store.value:
+            # got one.. use stored is_legacy status info
+            self.use_legacy_sessions = self.session_id_store.is_legacy
+            # and the check whether it's still valid
+            if self.session_get(self.session_id_store.value):
+                log.info("Using valid Session ID "
+                         "from ({0})".format(self.session_id_store.file_path))
+                return True
+
+        # got no (valid) session_id; clean store
+        self.session_id_store.write("")
+
+        # and try to create new one
+        if not self.session_create():
+            raise SessionCreateError("Failed to create a Session ID!")
+
+        # save new created session_id to file
+        if not self.session_id_store.write(self.result_json[self._session_key]):
+            raise IOError("Failed to save Session ID to file!")
+        else:
+            log.info("Saved new Session ID to file: "
+                     "{0}".format(self.session_id_store.file_path))
+            return True
+
+    @deprecation.deprecated(deprecated_in="0.10.0", removed_in="2.0", current_version=__version__,
+                            details="This method uses session_check_is_valid which was "
+                                    "implemented with a \"dirty\" workaround and should not be "
+                                    "called anymore. Use Client.session_restore_or_create() "
+                                    "instead. ATTENTION: Using that also switches to "
+                                    "session_get() which requires the OTRS route for HTTP GET "
+                                    "/Session to be configured  (which is/was not the default).")
     def session_restore_or_set_up_new(self):
         """Try to restore Session ID from file otherwise create new one and save to file
 
         Raises:
             SessionCreateError
             SessionIDFileError
 
@@ -1077,15 +1194,15 @@
         self.session_id_store.write("")
 
         # and try to create new one
         if not self.session_create():
             raise SessionCreateError("Failed to create a Session ID!")
 
         # save new created session_id to file
-        if not self.session_id_store.write(self.result_json['SessionID']):
+        if not self.session_id_store.write(self.result_json[self._session_key]):
             raise IOError("Failed to save Session ID to file!")
         else:
             log.info("Saved new Session ID to file: "
                      "{0}".format(self.session_id_store.file_path))
             return True
 
     """
@@ -1109,18 +1226,18 @@
             **kwargs: any regular OTRS Fields (not for Dynamic Fields!)
 
         Returns:
             **dict** or **False**: dict if successful, otherwise **False**.
         """
         if not self.session_id_store.value:
             raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
+                                    "session_restore_or_create() first")
         self.operation = "TicketCreate"
 
-        payload = {"SessionID": self.session_id_store.value}
+        payload = {self._session_key: self.session_id_store.value}
 
         if not ticket:
             raise ArgumentMissingError("Ticket")
 
         if not article:
             raise ArgumentMissingError("Article")
 
@@ -1171,19 +1288,19 @@
 
         Returns:
             **Ticket** or **False**: Ticket object if successful, otherwise **False**.
 
         """
         if not self.session_id_store.value:
             raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
+                                    "session_restore_or_create() first")
         self.operation = "TicketGet"
 
         payload = {
-            "SessionID": self.session_id_store.value,
+            self._session_key: self.session_id_store.value,
             "TicketID": "{0}".format(ticket_id),
             "AllArticles": int(articles),
             "Attachments": int(attachments),
             "DynamicFields": int(dynamic_fields),
             "HTMLBodyAsAttachment": int(html_body_as_attachment),
         }
 
@@ -1213,26 +1330,26 @@
 
         Returns:
             **list**: Ticket objects (as list) if successful, otherwise **False**.
 
         """
         if not self.session_id_store.value:
             raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
+                                    "session_restore_or_create() first")
         self.operation = "TicketGetList"
 
         if not isinstance(ticket_id_list, list):
             raise ArgumentInvalidError("Please provide list of IDs!")
 
         # When you ask with an empty ticket_id_list, you get an empty response
         if not ticket_id_list:
             return []
 
         payload = {
-            "SessionID": self.session_id_store.value,
+            self._session_key: self.session_id_store.value,
             "TicketID": ','.join([str(item) for item in ticket_id_list]),
             "AllArticles": int(articles),
             "Attachments": int(attachments),
             "DynamicFields": int(dynamic_fields),
             "HTMLBodyAsAttachment": int(html_body_as_attachment),
         }
 
@@ -1310,18 +1427,18 @@
         .. note::
             If value of kwargs is a datetime object then this object will be
             converted to the appropriate string format for OTRS API.
 
         """
         if not self.session_id_store.value:
             raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
+                                    "session_restore_or_create() first")
         self.operation = "TicketSearch"
         payload = {
-            "SessionID": self.session_id_store.value,
+            self._session_key: self.session_id_store.value,
         }
 
         if dynamic_fields:
             if isinstance(dynamic_fields, DynamicField):
                 payload.update(dynamic_fields.to_dct_search())
             else:
                 for df in dynamic_fields:
@@ -1381,18 +1498,18 @@
             **kwargs: any regular Ticket Fields (not for Dynamic Fields!)
 
         Returns:
             **dict** or **False**: A dict if successful, otherwise **False**.
         """
         if not self.session_id_store.value:
             raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
+                                    "session_restore_or_create() first")
         self.operation = "TicketUpdate"
 
-        payload = {"SessionID": self.session_id_store.value, "TicketID": ticket_id}
+        payload = {self._session_key: self.session_id_store.value, "TicketID": ticket_id}
 
         if article:
             article.validate()
             payload.update({"Article": article.to_dct()})
 
         if attachments:
             if not article:
@@ -1438,151 +1555,14 @@
         pending_till = datetime_now + datetime.timedelta(days=pending_days, hours=pending_hours)
 
         pt = Ticket.datetime_to_pending_time_text(datetime_object=pending_till)
 
         return self.ticket_update(ticket_id, State=new_state, PendingTime=pt)
 
     """
-    GenericInterface::Operation::FAQ::LanguageList
-        * faq_language_list
-
-    """
-
-    @deprecation.deprecated(deprecated_in="0.4", removed_in="1.0", current_version=__version__,
-                            details="FAQ API is out-of-scope and there is no replacement")
-    def faq_language_list(self):
-        """faq_language_list"""
-        if not self.session_id_store.value:
-            raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
-        self.operation = "LanguageList"
-
-        payload = {
-            "SessionID": self.session_id_store.value
-        }
-
-        result = self._parse_and_validate_response(self._send_request(payload))
-        if result:
-            return self.result
-
-    @deprecation.deprecated(deprecated_in="0.4", removed_in="1.0", current_version=__version__,
-                            details="FAQ API is out-of-scope and there is no replacement")
-    def faq_category_list(self):
-        """faq_public_category_list"""
-        if not self.session_id_store.value:
-            raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
-        self.operation = "PublicCategoryList"
-
-        payload = {
-            "SessionID": self.session_id_store.value
-        }
-
-        result = self._parse_and_validate_response(self._send_request(payload))
-        if result:
-            return self.result
-
-    @deprecation.deprecated(deprecated_in="0.4", removed_in="1.0", current_version=__version__,
-                            details="FAQ API is out-of-scope and there is no replacement")
-    def faq_public_faq_get(self, item_ids=None, attachment_contents=True):
-        """faq_public_category_list
-
-        Args:
-            item_ids (list): list of item IDs
-            attachment_contents (bool): whether to retrieve content of FAQ attachments
-
-        Returns:
-            **list**: of **dict** containing FAQ data
-
-        """
-
-        if not self.session_id_store.value:
-            raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
-        self.operation = "PublicFAQGet"
-
-        payload = {
-            "SessionID": self.session_id_store.value
-        }
-
-        if not item_ids:
-            raise ArgumentMissingError("item_ids is required")
-
-        if isinstance(item_ids, list):
-            _ids = ",".join([str(x) for x in item_ids])
-        else:
-            _ids = item_ids
-
-        payload.update({"ItemID": _ids})
-        if not attachment_contents:
-            payload.update({"GetAttachmentContents": 0})
-
-        if self._parse_and_validate_response(self._send_request(payload)):
-            return self.result
-
-    @deprecation.deprecated(deprecated_in="0.4", removed_in="1.0", current_version=__version__,
-                            details="FAQ API is out-of-scope and there is no replacement")
-    def faq_public_faq_search(self, what=None, number=None, title=None, search_dict=None):
-        """faq_public_category_list
-
-        Args:
-            what (str):
-            number (str):
-            title (str):
-            search_dict (dict):
-
-        Returns:
-            **list**: of found FAQ item IDs
-
-        # Original documentation:
-        # perform PublicFAQSearch Operation. This will return a list of public FAQ entries.
-        #       Number = > '*134*',              # (optional)
-        #       Title = > '*some title*',        # (optional)
-        #
-        #       # is searching in Number, Title, Keyword and Field1-6
-        #       What = > '*some text*',          # (optional)
-        #
-        #       Keyword = > '*webserver*',       # (optional)
-        #       LanguageIDs = > [4, 5, 6],       # (optional)
-        #       CategoryIDs = > [7, 8, 9],       # (optional)
-
-        """
-
-        if not self.session_id_store.value:
-            raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
-        self.operation = "PublicFAQSearch"
-
-        payload = {
-            "SessionID": self.session_id_store.value,
-        }
-
-        if what:
-            payload.update({"What": what})
-
-        if number:
-            payload.update({"Number": number})
-
-        if title:
-            payload.update({"Title": title})
-
-        if search_dict:
-            if not isinstance(search_dict, dict):
-                raise ArgumentInvalidError("Expecting dict for search_dict!")
-            payload.update(search_dict)
-
-        if self._parse_and_validate_response(self._send_request(payload)):
-            if not self.result:
-                return []
-            elif len(self.result) == 1:
-                return [self.result]
-            else:
-                return self.result
-
-    """
     GenericInterface::Operation::Link::LinkAdd
         * link_add
     """
 
     def link_add(self,
                  src_object_id,
                  dst_object_id,
@@ -1604,19 +1584,19 @@
 
         Returns:
             **True** or **False**: True if successful, otherwise **False**.
 
         """
         if not self.session_id_store.value:
             raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
+                                    "session_restore_or_create() first")
         self.operation = "LinkAdd"
 
         payload = {
-            "SessionID": self.session_id_store.value,
+            self._session_key: self.session_id_store.value,
             "SourceObject": src_object_type,
             "SourceKey": int(src_object_id),
             "TargetObject": dst_object_type,
             "TargetKey": int(dst_object_id),
             "Type": link_type,
             "State": state
         }
@@ -1647,19 +1627,19 @@
 
         Returns:
             **True** or **False**: True if successful, otherwise **False**.
 
         """
         if not self.session_id_store.value:
             raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
+                                    "session_restore_or_create() first")
         self.operation = "LinkDelete"
 
         payload = {
-            "SessionID": self.session_id_store.value,
+            self._session_key: self.session_id_store.value,
             "Object1": src_object_type,
             "Key1": int(src_object_id),
             "Object2": dst_object_type,
             "Key2": int(dst_object_id),
             "Type": link_type
         }
 
@@ -1682,19 +1662,19 @@
 
         Returns:
             **True** or **False**: True if successful, otherwise **False**.
 
         """
         if not self.session_id_store.value:
             raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
+                                    "session_restore_or_create() first")
         self.operation = "LinkDeleteAll"
 
         payload = {
-            "SessionID": self.session_id_store.value,
+            self._session_key: self.session_id_store.value,
             "Object": object_type,
             "Key": int(object_id)
         }
 
         return self._parse_and_validate_response(self._send_request(payload))
 
     """
@@ -1708,50 +1688,52 @@
                   dst_object_type=None,
                   state="Valid",
                   link_type=None,
                   direction=None):
         """link_list
 
         Args:
-            src_object_id (int): Object type of source; e.g. "Ticket", "FAQ"...
-                (*default: Ticket*)
-            src_object_type (str): Object type of destination; e.g. "Ticket", "FAQ"...
+            src_object_id (int): Integer value of source object ID
+            src_object_type (str): Object type of source; e.g. "Ticket", "FAQ"...
                 (*default: Ticket*)
             dst_object_type (str): Object type of destination; e.g. "Ticket", "FAQ"...
                 Optional restriction of the object where the links point to. (*default: Ticket*)
             state (str): State of the link (*default: Valid*)
             link_type (str): Type of the link: "Normal" or "ParentChild" (*default: Normal*)
             direction (str): Optional restriction of the link direction ('Source' or 'Target').
 
         Returns:
-            **Dict** or **None**: Dict if successful, if empty **None**.
+            **list** or **None**: List of found dict links if successful, if empty **None**.
 
         """
         if not self.session_id_store.value:
             raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
+                                    "session_restore_or_create() first")
         self.operation = "LinkList"
 
         payload = {
-            "SessionID": self.session_id_store.value,
+            self._session_key: self.session_id_store.value,
             "Object": src_object_type,
             "Key": int(src_object_id),
             "State": state
         }
 
         if dst_object_type:
             payload.update({"Object2": dst_object_type})
 
         if link_type:
             payload.update({"Type": link_type})
 
         if direction:
             payload.update({"Direction": direction})
 
-        return self._parse_and_validate_response(self._send_request(payload))
+        result = None
+        if self._parse_and_validate_response(self._send_request(payload)):
+            result = self.result
+        return result
 
     """
     GenericInterface::Operation::Link::PossibleLinkList
         * link_possible_link_list
     """
 
     def link_possible_link_list(self):
@@ -1759,19 +1741,19 @@
 
         Returns:
             **List** or **False**: List if successful, otherwise **False**.
 
         """
         if not self.session_id_store.value:
             raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
+                                    "session_restore_or_create() first")
         self.operation = "PossibleLinkList"
 
         payload = {
-            "SessionID": self.session_id_store.value,
+            self._session_key: self.session_id_store.value,
         }
 
         if self._parse_and_validate_response(self._send_request(payload)):
             return self.result
         else:
             return False
 
@@ -1790,19 +1772,19 @@
 
         Returns:
             **List** or **False**: List if successful, otherwise **False**.
 
         """
         if not self.session_id_store.value:
             raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
+                                    "session_restore_or_create() first")
         self.operation = "PossibleObjectsList"
 
         payload = {
-            "SessionID": self.session_id_store.value,
+            self._session_key: self.session_id_store.value,
             "Object": object_type,
         }
 
         if self._parse_and_validate_response(self._send_request(payload)):
             return self.result
         else:
             return False
@@ -1825,70 +1807,73 @@
 
         Returns:
             **List** or **False**: List if successful, otherwise **False**.
 
         """
         if not self.session_id_store.value:
             raise SessionNotCreated("Call session_create() or "
-                                    "session_restore_or_set_up_new() first")
+                                    "session_restore_or_create() first")
         self.operation = "PossibleTypesList"
 
         payload = {
-            "SessionID": self.session_id_store.value,
+            self._session_key: self.session_id_store.value,
             "Object1": src_object_type,
             "Object2": dst_object_type,
         }
 
         if self._parse_and_validate_response(self._send_request(payload)):
             return self.result
         else:
             return False
 
-    def _build_url(self, ticket_id=None):
+    def _build_url(self, data_id=None):
         """build url for request
 
         Args:
-            ticket_id (optional[int])
+            data_id (optional[int])
 
         Returns:
             **str**: The complete URL where the request will be send to.
 
         """
         route = self.ws_config[self.operation]["Route"]
 
         if ":" in route:
             route_split = route.split(":")
             route = route_split[0]
             route_arg = route_split[1]
 
             if route_arg == "TicketID":
-                if not ticket_id:
+                if not data_id:
                     raise ValueError("TicketID is None but Route requires "
                                      "TicketID: {0}".format(route))
                 self._url = ("{0}{1}{2}{3}{4}".format(
-                    self.baseurl, self.webservice_path, self.ws_ticket, route, ticket_id))
+                    self.baseurl, self.webservice_path, self.ws_ticket, route, data_id))
+            elif route_arg == "SessionID":
+                if not data_id:
+                    raise ValueError("SessionID is None but Route requires "
+                                     "SessionID: {0}".format(route))
+                self._url = ("{0}{1}{2}{3}{4}".format(
+                    self.baseurl, self.webservice_path, self.ws_ticket, route, data_id))
         else:
             if route in self.routes_ticket:
                 self._url = ("{0}{1}{2}{3}".format(
                     self.baseurl, self.webservice_path, self.ws_ticket, route))
-            elif route in self.routes_faq:
-                self._url = ("{0}{1}{2}{3}".format(
-                    self.baseurl, self.webservice_path, self.ws_faq, route))
             elif route in self.routes_link:
                 self._url = ("{0}{1}{2}{3}".format(
                     self.baseurl, self.webservice_path, self.ws_link, route))
 
         return self._url
 
-    def _send_request(self, payload=None, ticket_id=None):
+    def _send_request(self, payload=None, data_id=None):
         """send the API request using the *requests.request* method
 
         Args:
             payload (dict)
-            ticket_id (optional[dict])
+            data_id (optional[dict])
 
         Raises:
             OTRSHTTPError:
 
         Returns:
             **requests.Response**: Response received after sending the request.
 
@@ -1896,15 +1881,15 @@
             Supported HTTP Methods: DELETE, GET, HEAD, PATCH, POST, PUT
         """
         if not payload:
             raise ArgumentMissingError("payload")
 
         self._result_type = self.ws_config[self.operation]["Result"]
 
-        url = self._build_url(ticket_id)
+        url = self._build_url(data_id)
 
         http_method = self.ws_config[self.operation]["RequestMethod"]
 
         if http_method not in ["DELETE", "GET", "HEAD", "PATCH", "POST", "PUT"]:
             raise ValueError("invalid http_method")
 
         headers = {}
@@ -1962,15 +1947,15 @@
 
         if not response.status_code == 200:
             raise HTTPError("Received HTTP Error. Check Hostname and WebServiceName.\n"
                             "HTTP Status Code: {0.status_code}\n"
                             "HTTP Message: {0.content}".format(response))
         return response
 
-    def _parse_and_validate_response(self, response):
+    def _parse_and_validate_response(self, response): # noqa: max-complexity: 25
         """_parse_and_validate_response
 
         Args:
             response (requests.Response): result of _send_request
 
         Raises:
             OTRSAPIError
@@ -2002,14 +1987,42 @@
             if not self.result_json:
                 self.result = []
                 return True
             if self.result_json.get(self._result_type, None):
                 self.result = self.result_json['TicketID']
                 return True
 
+        # now handle SessionGet operation
+        if self.operation in ["SessionGet"]:
+            # For SessionGet the "Result" that is returned is different when legacy session
+            # are used.
+            # SessionData was default in OTRS <= 7 / PyOTRS used it as default from v0.1.
+            # AccessTokenData was introduced in OTRS 8 - for CustomerUser already in 7 (?!).
+            # Unless the dict was modified - use the hardcoded defaults accordingly.
+            if self._result_type not in ["AccessTokenData", "SessionData"]:
+                session_result_type = self._result_type
+            else:
+                if self.use_legacy_sessions:
+                    session_result_type = "SessionData"
+                else:
+                    session_result_type = "AccessTokenData"
+
+            _session_data = self.result_json.get(session_result_type, None)
+            if _session_data:  # received SessionData -> Session ID is valid
+                self._result_error = False
+                self.result = self.result_json[session_result_type]
+                return True
+            elif self.result_json["Error"]["ErrorCode"] == "SessionGet.SessionInvalid":
+                return False
+            else:
+                raise APIError("Failed to access OTRS API.\n"
+                               "OTRS Error Code: {0}\nOTRS Error Message: {1}"
+                               "".format(self.result_json["Error"]["ErrorCode"],
+                                         self.result_json["Error"]["ErrorMessage"]))
+
         # handle Link operations; Add, Delete, DeleteAll return: {"Success":1}
         if self.operation in ["LinkAdd", "LinkDelete", "LinkDeleteAll"]:
             if self.result_json.get("Success", None) == 1:
                 return True
 
         # LinkList result can be empty
         if self.operation in "LinkList":
@@ -2017,25 +2030,14 @@
             if not _link_list:
                 self.result = None
                 return True
             else:
                 self.result = _link_list
                 return True
 
-        # PublicFAQSearch result can be empty
-        if self.operation in "PublicFAQSearch":
-            _public_faq_search_result_list = self.result_json.get(self._result_type, None)
-            if not _public_faq_search_result_list:
-                if self.result_json["Error"]["ErrorCode"] == "PublicFAQSearch.NotFAQData":
-                    self.result = []
-                    return True
-            else:
-                self.result = _public_faq_search_result_list
-                return True
-
         # now handle other operations
         if self.result_json.get(self._result_type, None):
             self._result_error = False
             self.result = self.result_json[self._result_type]
         elif self.result_json.get("Error", None):
             self._result_error = True
         else:
```

### Comparing `PyOTRS-0.9.0/pyotrs/__init__.py` & `PyOTRS-1.0.1/pyotrs/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ This is PyOTRS provide python access to OTRS
 
 .. note::
 
-   Implements: https://otrs.github.io/doc/api/otrs/6.0/Perl/index.html
+   Implements: https://doc.otrs.com/doc/api/otrs/8.0/Perl/
 
 """
 
 from .lib import Article  # noqa
 from .lib import Attachment  # noqa
 from .lib import Client  # noqa
 from .lib import DynamicField  # noqa
```

### Comparing `PyOTRS-0.9.0/setup.py` & `PyOTRS-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,14 @@
     extras_require={
         "cli": ['click', 'colorama'],
     },
     entry_points='''
         [console_scripts]
         pyotrs=cli.PyOTRS:cli
     ''',
-    test_suite='unittest2.collector',
-    tests_require=['tox', 'coverage', 'unittest2', 'mock', 'responses'],
     classifiers=[
         'Development Status :: 4 - Beta',
 
         'Environment :: Console',
         'Environment :: Web Environment',
 
         'Framework :: Pytest',
@@ -51,20 +49,17 @@
 
         'License :: OSI Approved :: MIT License',
 
         'Operating System :: POSIX :: Linux',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 
         'Topic :: Documentation :: Sphinx',
     ],
 )
```

### Comparing `PyOTRS-0.9.0/README.rst` & `PyOTRS-1.0.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,48 +4,47 @@
 |VersionBadge| |BuildStatus| |CoverageReport| |DocsBuildStatus| |LicenseBadge| |PythonVersions|
 
 
 .. |VersionBadge| image:: https://badge.fury.io/py/PyOTRS.svg
     :target: https://badge.fury.io/py/PyOTRS
     :alt: |version|
 
-.. |BuildStatus| image:: https://gitlab.com/rhab/PyOTRS/badges/master/pipeline.svg
-    :target: https://gitlab.com/rhab/PyOTRS/commits/master
+.. |BuildStatus| image:: https://gitlab.com/rhab/PyOTRS/badges/main/pipeline.svg
+    :target: https://gitlab.com/rhab/PyOTRS/commits/main
     :alt: Build Status
 
-.. |CoverageReport| image:: https://gitlab.com/rhab/PyOTRS/badges/master/coverage.svg
-    :target: https://gitlab.com/rhab/PyOTRS/commits/master
+.. |CoverageReport| image:: https://gitlab.com/rhab/PyOTRS/badges/main/coverage.svg
+    :target: https://gitlab.com/rhab/PyOTRS/commits/main
     :alt: Coverage Report
 
 .. |DocsBuildStatus| image:: https://readthedocs.org/projects/pyotrs/badge/?version=stable
     :target: https://pyotrs.readthedocs.org/en/stable/index.html
     :alt: Docs Build Status
 
 .. |LicenseBadge| image:: https://img.shields.io/badge/license-MIT-blue.svg
-    :target: https://gitlab.com/rhab/PyOTRS/-/blob/master/LICENSE
+    :target: https://gitlab.com/rhab/PyOTRS/-/blob/main/LICENSE
     :alt: MIT licensed
 
-.. |PythonVersions| image:: https://img.shields.io/badge/python-2.7%2C%203.4%2C%203.5%2C%203.6%2C%203.7%2C%203.8-blue.svg
-    :alt: python: 2.7, 3.4, 3.5, 3.6, 3.7, 3.8
+.. |PythonVersions| image:: https://img.shields.io/badge/python-3.7%2C%203.8%2C%203.9%2C%203.10%2C%203.11-blue.svg
+    :alt: python: 3.7, 3.8, 3.9, 3.10, 3.11
 
 
-PyOTRS is a Python wrapper for accessing `OTRS <https://www.otrs.com/>`_ (Version 5, 6, 7) using the
+PyOTRS is a Python wrapper for accessing `OTRS <https://www.otrs.com/>`_ (Version 5, 6, 7, 8) using the
 (GenericInterface) REST API.
 
 Warning
 =======
 
-    Please upgrade PyOTRS to at least version 0.7.1 if you are using OTRS 6.0.27, 7.0.16 or
-    newer. See `issue 27 <https://gitlab.com/rhab/PyOTRS/-/issues/27>`_ and
-    `issue 29 <https://gitlab.com/rhab/PyOTRS/-/issues/29>`_ for more details.
+    Please upgrade PyOTRS to at least version 0.10.0 (recommended version is at least 1.0.0) if you
+    are using OTRS 6.0.27, 7.0.16 or newer. See `issue 27 <https://gitlab.com/rhab/PyOTRS/-/issues/27>`_
+    and `issue 29 <https://gitlab.com/rhab/PyOTRS/-/issues/29>`_ for more details.
 
     OTRS has introduced a new API in version 8 and with this also changed the API endpoint from
-    "Session::SessionCreate" to "AccessToken::Create". At the moment PyOTRS does not support
-    OTRS v8. See `issue 28 <https://gitlab.com/rhab/PyOTRS/-/issues/28>`_ for progress and
-    discussions.
+    "Session::SessionCreate" to "AccessToken::Create". PyOTRS attempts to use the new API and will
+    fallback to the old way ("legacy") if the attempt fails.
 
 
 Features
 ========
 
 Access an OTRS instance to::
 
@@ -69,17 +68,16 @@
 Installation
 ============
 
 OTRS Prerequisite
 -----------------
 
 You have to enable the **webservices** in your OTRS instance.  It is recommended to use the
-provided `template <https://gitlab.com/rhab/PyOTRS/raw/master/webservices_templates/GenericTicketConnectorREST.yml>`_.
-This YAML configuration template includes the **Route: /TicketList** endpoint that is **required for PyOTRS** but which
-is not included in the default OTRS webservice setup.
+provided `template <https://gitlab.com/rhab/PyOTRS/raw/main/webservices_templates/GenericTicketConnectorREST.yml>`_.
+This YAML configuration template includes the **Route: /TicketList** and **SessionGet: /Session/:SessionID** endpoint which both are **required for PyOTRS** but which are not included in the default OTRS webservice setup.
 
 Dependencies
 ------------
 
 *Dependencies are installed automatically*
 
 pip::
@@ -113,14 +111,25 @@
 
     from pyotrs import Client
     client = Client("https://otrs.example.com", "root@localhost", "password")
     client.session_create()
     client.ticket_get_by_id(1)
 
 
+The usage of ``Client.session_restore_or_create`` is **recommended**. It uses a temporary file
+on the hard drive to store the Session ID (just like cookies in a browser) and avoids sending
+the username+password (and therefore creating a new session) on every API call::
+
+    from pyotrs import Client
+    client = Client("https://otrs.example.com", "root@localhost", "password")
+    client.session_restore_or_create()
+    client.ticket_get_by_id(1)
+
+Method ``Client.session_restore_or_set_up_new`` is **deprecated** as of v0.10.
+
 More Examples
 -------------
 
 - instantiate a ``Client`` object called **client**
 - create a session ("login") on **client**
 - get the ``Ticket`` with ID 1
 
@@ -277,22 +286,14 @@
 [u'2']
 
 
 
 Tips
 ----
 
-When using **ipython** you could run into UTF8 encoding issues on Python2. This is a workaround
-that can help::
-
-    import sys
-    reload(sys)
-    sys.setdefaultencoding('utf-8')
-
-
 **If needed** the *insecure plattform warnings* can be disabled::
 
     # turn off platform insecurity warnings from urllib3
     from requests.packages.urllib3 import disable_warnings
     disable_warnings()  # TODO 2016-04-23 (RH) verify this
 
 PyOTRS Shell CLI
```

### Comparing `PyOTRS-0.9.0/LICENSE` & `PyOTRS-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOTRS-0.9.0/PyOTRS.egg-info/PKG-INFO` & `PyOTRS-1.0.1/PyOTRS.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOTRS
-Version: 0.9.0
+Version: 1.0.1
 Summary: Python wrapper for OTRS (using REST API)
 Home-page: https://gitlab.com/rhab/PyOTRS
 Author: Robert Habermann
 Author-email: mail@rhab.de
 Maintainer: Robert Habermann
 License: The MIT License (MIT)
 
@@ -34,48 +34,47 @@
         |VersionBadge| |BuildStatus| |CoverageReport| |DocsBuildStatus| |LicenseBadge| |PythonVersions|
         
         
         .. |VersionBadge| image:: https://badge.fury.io/py/PyOTRS.svg
             :target: https://badge.fury.io/py/PyOTRS
             :alt: |version|
         
-        .. |BuildStatus| image:: https://gitlab.com/rhab/PyOTRS/badges/master/pipeline.svg
-            :target: https://gitlab.com/rhab/PyOTRS/commits/master
+        .. |BuildStatus| image:: https://gitlab.com/rhab/PyOTRS/badges/main/pipeline.svg
+            :target: https://gitlab.com/rhab/PyOTRS/commits/main
             :alt: Build Status
         
-        .. |CoverageReport| image:: https://gitlab.com/rhab/PyOTRS/badges/master/coverage.svg
-            :target: https://gitlab.com/rhab/PyOTRS/commits/master
+        .. |CoverageReport| image:: https://gitlab.com/rhab/PyOTRS/badges/main/coverage.svg
+            :target: https://gitlab.com/rhab/PyOTRS/commits/main
             :alt: Coverage Report
         
         .. |DocsBuildStatus| image:: https://readthedocs.org/projects/pyotrs/badge/?version=stable
             :target: https://pyotrs.readthedocs.org/en/stable/index.html
             :alt: Docs Build Status
         
         .. |LicenseBadge| image:: https://img.shields.io/badge/license-MIT-blue.svg
-            :target: https://gitlab.com/rhab/PyOTRS/-/blob/master/LICENSE
+            :target: https://gitlab.com/rhab/PyOTRS/-/blob/main/LICENSE
             :alt: MIT licensed
         
-        .. |PythonVersions| image:: https://img.shields.io/badge/python-2.7%2C%203.4%2C%203.5%2C%203.6%2C%203.7%2C%203.8-blue.svg
-            :alt: python: 2.7, 3.4, 3.5, 3.6, 3.7, 3.8
+        .. |PythonVersions| image:: https://img.shields.io/badge/python-3.7%2C%203.8%2C%203.9%2C%203.10%2C%203.11-blue.svg
+            :alt: python: 3.7, 3.8, 3.9, 3.10, 3.11
         
         
-        PyOTRS is a Python wrapper for accessing `OTRS <https://www.otrs.com/>`_ (Version 5, 6, 7) using the
+        PyOTRS is a Python wrapper for accessing `OTRS <https://www.otrs.com/>`_ (Version 5, 6, 7, 8) using the
         (GenericInterface) REST API.
         
         Warning
         =======
         
-            Please upgrade PyOTRS to at least version 0.7.1 if you are using OTRS 6.0.27, 7.0.16 or
-            newer. See `issue 27 <https://gitlab.com/rhab/PyOTRS/-/issues/27>`_ and
-            `issue 29 <https://gitlab.com/rhab/PyOTRS/-/issues/29>`_ for more details.
+            Please upgrade PyOTRS to at least version 0.10.0 (recommended version is at least 1.0.0) if you
+            are using OTRS 6.0.27, 7.0.16 or newer. See `issue 27 <https://gitlab.com/rhab/PyOTRS/-/issues/27>`_
+            and `issue 29 <https://gitlab.com/rhab/PyOTRS/-/issues/29>`_ for more details.
         
             OTRS has introduced a new API in version 8 and with this also changed the API endpoint from
-            "Session::SessionCreate" to "AccessToken::Create". At the moment PyOTRS does not support
-            OTRS v8. See `issue 28 <https://gitlab.com/rhab/PyOTRS/-/issues/28>`_ for progress and
-            discussions.
+            "Session::SessionCreate" to "AccessToken::Create". PyOTRS attempts to use the new API and will
+            fallback to the old way ("legacy") if the attempt fails.
         
         
         Features
         ========
         
         Access an OTRS instance to::
         
@@ -99,17 +98,16 @@
         Installation
         ============
         
         OTRS Prerequisite
         -----------------
         
         You have to enable the **webservices** in your OTRS instance.  It is recommended to use the
-        provided `template <https://gitlab.com/rhab/PyOTRS/raw/master/webservices_templates/GenericTicketConnectorREST.yml>`_.
-        This YAML configuration template includes the **Route: /TicketList** endpoint that is **required for PyOTRS** but which
-        is not included in the default OTRS webservice setup.
+        provided `template <https://gitlab.com/rhab/PyOTRS/raw/main/webservices_templates/GenericTicketConnectorREST.yml>`_.
+        This YAML configuration template includes the **Route: /TicketList** and **SessionGet: /Session/:SessionID** endpoint which both are **required for PyOTRS** but which are not included in the default OTRS webservice setup.
         
         Dependencies
         ------------
         
         *Dependencies are installed automatically*
         
         pip::
@@ -143,14 +141,25 @@
         
             from pyotrs import Client
             client = Client("https://otrs.example.com", "root@localhost", "password")
             client.session_create()
             client.ticket_get_by_id(1)
         
         
+        The usage of ``Client.session_restore_or_create`` is **recommended**. It uses a temporary file
+        on the hard drive to store the Session ID (just like cookies in a browser) and avoids sending
+        the username+password (and therefore creating a new session) on every API call::
+        
+            from pyotrs import Client
+            client = Client("https://otrs.example.com", "root@localhost", "password")
+            client.session_restore_or_create()
+            client.ticket_get_by_id(1)
+        
+        Method ``Client.session_restore_or_set_up_new`` is **deprecated** as of v0.10.
+        
         More Examples
         -------------
         
         - instantiate a ``Client`` object called **client**
         - create a session ("login") on **client**
         - get the ``Ticket`` with ID 1
         
@@ -307,22 +316,14 @@
         [u'2']
         
         
         
         Tips
         ----
         
-        When using **ipython** you could run into UTF8 encoding issues on Python2. This is a workaround
-        that can help::
-        
-            import sys
-            reload(sys)
-            sys.setdefaultencoding('utf-8')
-        
-        
         **If needed** the *insecure plattform warnings* can be disabled::
         
             # turn off platform insecurity warnings from urllib3
             from requests.packages.urllib3 import disable_warnings
             disable_warnings()  # TODO 2016-04-23 (RH) verify this
         
         PyOTRS Shell CLI
@@ -436,17 +437,15 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Pytest
 Classifier: Framework :: Sphinx
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
 Provides-Extra: cli
```

### Comparing `PyOTRS-0.9.0/cli/PyOTRS.py` & `PyOTRS-1.0.1/cli/PyOTRS.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,23 +90,26 @@
               help='Password')
 @click.option('-u', '--username', type=click.STRING, prompt=True,
               envvar="PYOTRS_USERNAME",
               help='Username')
 @click.option('-b', '--baseurl', type=click.STRING, prompt=True,
               envvar="PYOTRS_BASEURL",
               help='Base URL')
+@click.option('--use-legacy-sessions', is_flag=True,
+              help='use legacy sessions for OTRS < 8')
 @cli.command(name="get")
 def get(baseurl=None, username=None, password=None, ticket_id=None,
         articles=False,
         attachments=False, store_attachments=False, store_path=None,
-        https_verify=True, ca_cert_bundle=None):
+        https_verify=True, ca_cert_bundle=None, use_legacy_sessions=False):
     """PyOTRS get command"""
     click.secho("Connecting to %s as %s.." % (baseurl, username))
     client = Client(baseurl, username, password,
-                    https_verify=https_verify, ca_cert_bundle=ca_cert_bundle)
+                    https_verify=https_verify, ca_cert_bundle=ca_cert_bundle,
+                    use_legacy_sessions=use_legacy_sessions)
     client.session_create()
 
     ticket = client.ticket_get_by_id(ticket_id, articles=articles, attachments=attachments)
 
     if ticket:
         click.secho("Ticket: \t%s" % ticket.field_get("Title"))
         click.secho("Queue: \t\t%s" % ticket.field_get("Queue"))
```

