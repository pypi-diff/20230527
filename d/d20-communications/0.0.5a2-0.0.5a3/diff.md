# Comparing `tmp/d20-communications-0.0.5a2.tar.gz` & `tmp/d20-communications-0.0.5a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\python_arango_communications_module\dist\.tmp-13e_vgcn\d20-communications-0.0.5a2.tar", last modified: Wed Mar  1 00:04:48 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\python_arango_communications_module\dist\.tmp-ejg90pnv\d20-communications-0.0.5a3.tar", last modified: Fri May 26 23:37:12 2023, max compression
```

## Comparing `d20-communications-0.0.5a2.tar` & `d20-communications-0.0.5a3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 00:04:48.803305 d20-communications-0.0.5a2/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-communications-0.0.5a2/LICENSE
--rw-rw-rw-   0        0        0      657 2023-03-01 00:04:48.802328 d20-communications-0.0.5a2/PKG-INFO
--rw-rw-rw-   0        0        0       67 2021-09-24 00:12:42.000000 d20-communications-0.0.5a2/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-communications-0.0.5a2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-01 00:04:48.803305 d20-communications-0.0.5a2/setup.cfg
--rw-rw-rw-   0        0        0     1013 2023-03-01 00:04:23.000000 d20-communications-0.0.5a2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-01 00:04:48.772769 d20-communications-0.0.5a2/src/
-drwxrwxrwx   0        0        0        0 2023-03-01 00:04:48.793814 d20-communications-0.0.5a2/src/d20_communications.egg-info/
--rw-rw-rw-   0        0        0      657 2023-03-01 00:04:48.000000 d20-communications-0.0.5a2/src/d20_communications.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-03-01 00:04:48.000000 d20-communications-0.0.5a2/src/d20_communications.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 00:04:48.000000 d20-communications-0.0.5a2/src/d20_communications.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-03-01 00:04:48.000000 d20-communications-0.0.5a2/src/d20_communications.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-03-01 00:04:48.000000 d20-communications-0.0.5a2/src/d20_communications.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-01 00:04:48.801276 d20-communications-0.0.5a2/src/dtwentyCommunications/
--rw-rw-rw-   0        0        0    15794 2023-03-01 00:04:04.000000 d20-communications-0.0.5a2/src/dtwentyCommunications/Communications.py
--rw-rw-rw-   0        0        0     1677 2021-09-24 00:11:26.000000 d20-communications-0.0.5a2/src/dtwentyCommunications/Exceptions.py
--rw-rw-rw-   0        0        0       29 2021-09-24 00:32:35.000000 d20-communications-0.0.5a2/src/dtwentyCommunications/__init__.py
--rw-rw-rw-   0        0        0      159 2023-02-28 23:58:15.000000 d20-communications-0.0.5a2/src/dtwentyCommunications/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 23:37:12.637464 d20-communications-0.0.5a3/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-communications-0.0.5a3/LICENSE
+-rw-rw-rw-   0        0        0      657 2023-05-26 23:37:12.635464 d20-communications-0.0.5a3/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2021-09-24 00:12:42.000000 d20-communications-0.0.5a3/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-communications-0.0.5a3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 23:37:12.638464 d20-communications-0.0.5a3/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-05-26 23:36:35.000000 d20-communications-0.0.5a3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 23:37:12.419487 d20-communications-0.0.5a3/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 23:37:12.566303 d20-communications-0.0.5a3/src/d20_communications.egg-info/
+-rw-rw-rw-   0        0        0      657 2023-05-26 23:37:12.000000 d20-communications-0.0.5a3/src/d20_communications.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-05-26 23:37:12.000000 d20-communications-0.0.5a3/src/d20_communications.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 23:37:12.000000 d20-communications-0.0.5a3/src/d20_communications.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-05-26 23:37:12.000000 d20-communications-0.0.5a3/src/d20_communications.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-26 23:37:12.000000 d20-communications-0.0.5a3/src/d20_communications.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 23:37:12.631528 d20-communications-0.0.5a3/src/dtwentyCommunications/
+-rw-rw-rw-   0        0        0    14757 2023-05-26 23:32:17.000000 d20-communications-0.0.5a3/src/dtwentyCommunications/Communications.py
+-rw-rw-rw-   0        0        0     1677 2021-09-24 00:11:26.000000 d20-communications-0.0.5a3/src/dtwentyCommunications/Exceptions.py
+-rw-rw-rw-   0        0        0       29 2021-09-24 00:32:35.000000 d20-communications-0.0.5a3/src/dtwentyCommunications/__init__.py
+-rw-rw-rw-   0        0        0      159 2023-02-28 23:58:15.000000 d20-communications-0.0.5a3/src/dtwentyCommunications/__version__.py
```

### Comparing `d20-communications-0.0.5a2/LICENSE` & `d20-communications-0.0.5a3/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-communications-0.0.5a2/PKG-INFO` & `d20-communications-0.0.5a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-communications
-Version: 0.0.5a2
+Version: 0.0.5a3
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/python_arango_communications_module
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/python_arango_communications_module/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-communications-0.0.5a2/setup.py` & `d20-communications-0.0.5a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-communications",
-    version="0.0.5a2",
+    version="0.0.5a3",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A small ORM for multimodel DBs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/python_arango_communications_module",
     project_urls={
@@ -19,9 +19,9 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.8",
-    install_requires=['pyArango', 'datetime', 'd20-orm', 'requests', 'sendgrid', 'exponent_server_sdk', 'Twilio'],
+    install_requires=['pyArango', 'datetime', 'd20-orm>=2.0', 'requests', 'sendgrid', 'exponent_server_sdk', 'Twilio'],
 )
```

### Comparing `d20-communications-0.0.5a2/src/d20_communications.egg-info/PKG-INFO` & `d20-communications-0.0.5a3/src/d20_communications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-communications
-Version: 0.0.5a2
+Version: 0.0.5a3
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/python_arango_communications_module
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/python_arango_communications_module/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-communications-0.0.5a2/src/dtwentyCommunications/Communications.py` & `d20-communications-0.0.5a3/src/dtwentyCommunications/Communications.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,73 +3,47 @@
 # Company: d20
 # Version: 1.0
 
 
 from pyArango.connection import *
 from pyArango.collection import *
 from pyArango.graph import *
-from dtwentyORM import BasicElement, Metadata
+from dtwentyORM import BasicElement, Metadata, GraphClassFactory, Error as ORM_Error
 import json
 import requests
 import os
 import sendgrid
 from .Exceptions import *
 from exponent_server_sdk import (
     DeviceNotRegisteredError,
     PushClient,
     PushMessage,
     PushServerError,
     PushTicketError,
 )
 from requests.exceptions import ConnectionError, HTTPError
 
-class Communications():
-    if os.environ.get('D20_COMM_CONF') != None:
-        conf = json.loads(os.environ.get('D20_COMM_CONF'))
-        arangoURL=conf.get('D20_COMM_DBURL')
-        username=conf.get('D20_COMM_DBUSERNAME')
-        password=conf.get('D20_COMM_DBPASSWORD')    
-        prefix=conf.get('D20_COMM_DBPREFIX', '')   
-    else:
-        print("No configuration given, cannot start.")
-        raise Exception
-
-    db_client = Connection(arangoURL=arangoURL, username=username, password=password, verify=True, verbose=True, statsdClient=None, reportFileName=None, loadBalancing='round-robin', use_grequests=False, use_jwt_authentication=False, use_lock_for_reseting_jwt=True, max_retries=10)
-    db_name = F'{prefix}communications'
-
-    def __init__(self):
-        if not self.db_client.hasDatabase(self.db_name):
-            self.db = self.db_client.createDatabase(self.db_name)
-            self.db.createCollection(className='Collection', name='Messages')
-            self.db.createCollection(className='Collection', name='Status')
-            self.db.createCollection(className='Collection', name='Optative')
-        else:
-            self.db = self.db_client[self.db_name]
+def comm_dbname():
+    return f'{os.environ.get("DBPREFIX", "")}communications'
 
-    class Messages(Collection):
-        _fields = {
-        }
 
-    class Status(Collection):
-        _fields = {
-        }
+class Communications():
+    graphname = ''
+    collections = ['Messages', 'Status', 'Optative']
+    edgeDefinitions={}
+    db_name = comm_dbname()
+    factory = GraphClassFactory.ClassFactory(graphname, db_name, collections = collections, edgeDefinitions=edgeDefinitions, conf=conf)
 
-    class Optative(Collection):
-        _fields = {
-        }
+    print(factory, " - OK")
 
+ 
     class Email(BasicElement):
-        db_name = 'communications'
-
-        @classmethod
-        def get_collection(cls):
-            return 'Messages'
-
-        def get_class(self):
-            return 'Email'
+        def __init__(self, data=None):
+            self.collection = 'Messages'
+            super().__init__(db_name = comm_dbname(), data=data)
 
         def make(self):
             self.attributes = ['sender', 'receiver', 'type', 'params', 'channel', 'status_code']
             for key in self.attributes:
                 setattr(self, key, None)
             self.channel = 'email'
 
@@ -79,15 +53,15 @@
                 if False in [a in contact_data for a in requirement]:
                     if ignore_errors:
                         return
                     else:
                         raise MissingRequiredParametersException
             url = "https://api.sendgrid.com/v3/marketing/contacts"
 
-            lists_ids = [Metadata.Parameter('find', {'_key' : list_id}).get('value') for list_id in lists  if Metadata.Parameter('find', {'_key' : list_id}).get('value') != None and Metadata.Parameter('find', {'_key' : list_id}).get('value') != '']
+            lists_ids = [Metadata.Parameter().find(list_id).get('value') for list_id in lists  if Metadata.Parameter('find', {'_key' : list_id}).get('value') != None and Metadata.Parameter('find', {'_key' : list_id}).get('value') != '']
 
             contacts = []
             
             for contact_data in contacts_data:
                 if '_key' in contact_data:
                     contact_data['uid'] = contact_data['_key']
                 if "gender" in contact_data and contact_data["gender"] == 'Femenino':
@@ -113,27 +87,27 @@
 
             payload = {
                 "list_ids": lists_ids,
                 "contacts": contacts
             }
 
 
-            p = Metadata.Parameter('find', {'_key' : 'sg_conf'})
+            p = Metadata.Parameter().find('sg_conf')
 
             sg = p.get('value')['api_key']     
 
             headers = {
                 'authorization': f"Bearer {sg}",
                 'content-type': "application/json"
                 }
 
-            print("PUT", url, json.dumps(payload), headers)
+            # print("PUT", url, json.dumps(payload), headers)
             response = requests.request("PUT", url, data=json.dumps(payload), headers=headers)
 
-            print(response.text)
+            # print(response.text)
             if response.status_code == "200":
                 return {'res': True}
             return {'res': False}
 
         
         def personalize(self):
             if "gender" in self.get('params') and self.get('params')["gender"] == 'Femenino':
@@ -159,25 +133,25 @@
                     }
                 ]
             }
             return data
 
 
         def send(self):
-            p = Metadata.Parameter('find', {'_key' : self.get('type')})
+            p = Metadata.Parameter().find(self.get('type'))
             template_id = p.get('value')
             return self.sg_send(template_id)
 
         def send_by_id(self, template_id):
             return self.sg_send(template_id)
 
         def sg_send(self, template_id):
             if self.get('receiver', None) == None or self.get('receiver', None) == '':
                 raise MissingRequiredParametersException 
-            p = Metadata.Parameter('find', {'_key' : 'sg_conf'})
+            p = Metadata.Parameter().find('sg_conf')
 
             sg = sendgrid.SendGridAPIClient(api_key=p.get('value')['api_key'])            
             email_from_name = p.get('value')['email_from_name']
             email_from_inbox = p.get('value')['email_from_inbox']
 
             data = self.personalize()
             data['template_id'] = template_id
@@ -203,15 +177,17 @@
             if self.status_code in [200,202,'200','202']:
                 return {'res': True}
             return {'res': False, 'err_code': self.status_code, 'err_desc': 'Cannot send email', 'err_params': '?error=invalid_request'}
 
 
 
     class PushNotification(BasicElement):
-        db_name = 'communications'
+        def __init__(self, data=None):
+            self.collection = 'Messages'
+            super().__init__(db_name = comm_dbname(), data=data)
 
         type_buttons = {
             "intake" : [
                     {
                         "id": "intake-confirm-button",
                         "text": "Registrar toma",
                         "icon": "https://icons.getbootstrap.com/icons/check2-circle.svg",
@@ -236,21 +212,14 @@
                         "text": "Ver tomas",
                         "icon": "https://icons.getbootstrap.com/icons/eye-fill.svg",
                         "url": "https://webapp.vitiacare.com/Reminders"
                     }
             ],
         }
 
-        @classmethod
-        def get_collection(cls):
-            return 'Messages'
-
-        def get_class(self):
-            return 'PushNotification'
-
 
 
         def make(self):
             self.attributes = ['heading', 'content', 'type', 'receivers', 'channel', 'status', 'additional_data']
             for key in self.attributes:
                 setattr(self, key, None)
             self.channel = 'push'
@@ -316,15 +285,15 @@
                     pass
                 except PushTicketError as exc:
                     raise self.retry(exc=exc)
             return sent
 
         def send_desktop(self):
 
-            p = Metadata.Parameter('find', {'_key' : 'os_conf'})
+            p = Metadata.Parameter().find('os_conf')
             api_key=p.get('value')['api_key']
             app_id=p.get('value')['app_id']
 
 
 
             header = {"Content-Type": "application/json; charset=utf-8",
                     "Authorization": f"Basic {api_key}"}
@@ -376,30 +345,30 @@
                 self.create()
             except Exception:
                 return {'res': False, 'err_code': 500, 'err_desc': 'Cannot send', 'err_params': '?error=invalid_request'}
             if req.status_code == "200" or req.status_code == 200:
                 return {'res': True}
             return {'res': False, 'err_code': 500, 'err_desc': 'Cannot send', 'err_params': '?error=invalid_request'}
 
-    class Whatsapp(BasicElement):
-        db_name = 'communications'
-
-        @classmethod
-        def get_collection(cls):
-            return 'Messages'
-
-        def get_class(self):
-            return 'Whatsapp'
-
-        def make(self):
-            self.attributes = ['sender', 'receiver', 'type', 'params', 'channel', 'status_code']
-            for key in self.attributes:
-                setattr(self, key, None)
-            self.channel = 'whatsapp'
-
-        def send_oneway(self):
+    # class Whatsapp(BasicElement):
+    #     db_name = 'communications'
 
-            p = Metadata.Parameter('find', {'_key' : 'twilio_conf'})
-            api_key=p.get('value')['TWILIO_ACCOUNT_SID']
-            app_id=p.get('value')['TWILIO_AUTH_TOKEN']
+    #     @classmethod
+    #     def get_collection(cls):
+    #         return 'Messages'
+
+    #     def get_class(self):
+    #         return 'Whatsapp'
+
+    #     def make(self):
+    #         self.attributes = ['sender', 'receiver', 'type', 'params', 'channel', 'status_code']
+    #         for key in self.attributes:
+    #             setattr(self, key, None)
+    #         self.channel = 'whatsapp'
+
+    #     def send_oneway(self):
+
+    #         p = Metadata.Parameter('find', {'_key' : 'twilio_conf'})
+    #         api_key=p.get('value')['TWILIO_ACCOUNT_SID']
+    #         app_id=p.get('value')['TWILIO_AUTH_TOKEN']
```

### Comparing `d20-communications-0.0.5a2/src/dtwentyCommunications/Exceptions.py` & `d20-communications-0.0.5a3/src/dtwentyCommunications/Exceptions.py`

 * *Files identical despite different names*

