# Comparing `tmp/whatsapp-python-2.4.3.tar.gz` & `tmp/whatsapp-python-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-python-2.4.3.tar", last modified: Fri May 26 16:32:05 2023, max compression
+gzip compressed data, was "whatsapp-python-2.9.3.tar", last modified: Sat May 27 10:35:58 2023, max compression
```

## Comparing `whatsapp-python-2.4.3.tar` & `whatsapp-python-2.9.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:32:05.630838 whatsapp-python-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 16:32:04.000000 whatsapp-python-2.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-26 16:32:05.630838 whatsapp-python-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-26 16:32:04.000000 whatsapp-python-2.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:32:05.630838 whatsapp-python-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-26 16:32:04.000000 whatsapp-python-2.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:32:05.630838 whatsapp-python-2.4.3/whatsapp/
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-05-26 16:32:04.000000 whatsapp-python-2.4.3/whatsapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:32:05.630838 whatsapp-python-2.4.3/whatsapp_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-26 16:32:05.000000 whatsapp-python-2.4.3/whatsapp_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-26 16:32:05.000000 whatsapp-python-2.4.3/whatsapp_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:32:05.000000 whatsapp-python-2.4.3/whatsapp_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 16:32:05.000000 whatsapp-python-2.4.3/whatsapp_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 16:32:05.000000 whatsapp-python-2.4.3/whatsapp_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:35:58.667622 whatsapp-python-2.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-27 10:35:57.000000 whatsapp-python-2.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-27 10:35:58.667622 whatsapp-python-2.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-27 10:35:57.000000 whatsapp-python-2.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 10:35:58.667622 whatsapp-python-2.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-27 10:35:57.000000 whatsapp-python-2.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:35:58.667622 whatsapp-python-2.9.3/whatsapp/
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-27 10:35:57.000000 whatsapp-python-2.9.3/whatsapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:35:58.667622 whatsapp-python-2.9.3/whatsapp_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-27 10:35:58.000000 whatsapp-python-2.9.3/whatsapp_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-27 10:35:58.000000 whatsapp-python-2.9.3/whatsapp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:35:58.000000 whatsapp-python-2.9.3/whatsapp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 10:35:58.000000 whatsapp-python-2.9.3/whatsapp_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-27 10:35:58.000000 whatsapp-python-2.9.3/whatsapp_python.egg-info/top_level.txt
```

### Comparing `whatsapp-python-2.4.3/LICENSE` & `whatsapp-python-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-python-2.4.3/PKG-INFO` & `whatsapp-python-2.9.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-python
-Version: 2.4.3
+Version: 2.9.3
 Summary: Opensource Python wrapper to WhatsApp Cloud API
 Home-page: https://github.com/filipporomani/whatsapp
 Author: Filippo Romani
 Author-email: mail@filipporomani.it
 License: MIT
 Keywords: whatsapp,whatsapp-libary,WhatsApp Cloud API Wrapper,PyWhatsApp,WhatsApp API in Python
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [whatsapp-python](https://pypi.org/project/whatsapp-python/)
 
 ![Made in Italy](https://img.shields.io/badge/made%20in-italy-008751.svg?style=flat-square)
-[![Downloads](https://pepy.tech/badge/whatsapp-python)](https://pepy.tech/project/whatsapp-python)
+[![Downloads](https://static.pepy.tech/personalized-badge/whatsapp-python?period=total&units=none&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/month)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/week)](https://pepy.tech/project/whatsapp-python)
 
 Free, open-source Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api).
 
 Forked from [Neurotech-HQ/heyoo](https://github.com/Neurotech-HQ/heyoo)
 
@@ -36,18 +36,41 @@
 1. Sending messages
 2. Marking messages as read
 3. Sending Media (images, audio, video and documents)
 4. Sending location
 5. Sending interactive buttons
 6. Sending template messages
 7. Parsing messages and media received
+8. Receiving and parsing messages - [hook object](https://github.com/filipporomani/whatsapp/wiki/Hook()-object)
+
+## App events
+
+App events are now available! 
+
+The docs are available in the [wiki](https://github.com/filipporomani/whatsapp/wiki/App-events)
+
+Please test this feature out and leave feedbacks/report issues on GitHub!
+
+## Installation
+
+To install the library you can either use pip:
+
+``pip install whatsapp-python``
+
+or git:
+
+```bash
+git clone https://github.com/filipporomani/whatsapp.git
+cd whatsapp
+python3 setup.py install
+```
 
 ## Documentation
 
-The documentation for the is available in the [**wiki**](https://github.com/filipporomani/whatsapp/wiki)
+The documentation for the library is available in the [**wiki**](https://github.com/filipporomani/whatsapp/wiki)
 
 ## Costs of the API
 
 While using third-party API providers of the WhatsApp API may have some monthly fees, using the WhatsApp API provided directly by Facebook is way cheaper. 
 The first 1000 chats created are free, then there is a pay-as-you-go fee that is paid for each conversation started.
 
 All the prices are available in the [**WhatsApp API docs**](https://developers.facebook.com/docs/whatsapp/pricing)
```

### Comparing `whatsapp-python-2.4.3/README.md` & `whatsapp-python-2.9.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # [whatsapp-python](https://pypi.org/project/whatsapp-python/)
 
 ![Made in Italy](https://img.shields.io/badge/made%20in-italy-008751.svg?style=flat-square)
-[![Downloads](https://pepy.tech/badge/whatsapp-python)](https://pepy.tech/project/whatsapp-python)
+[![Downloads](https://static.pepy.tech/personalized-badge/whatsapp-python?period=total&units=none&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/month)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/week)](https://pepy.tech/project/whatsapp-python)
 
 Free, open-source Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api).
 
 Forked from [Neurotech-HQ/heyoo](https://github.com/Neurotech-HQ/heyoo)
 
@@ -14,18 +14,41 @@
 1. Sending messages
 2. Marking messages as read
 3. Sending Media (images, audio, video and documents)
 4. Sending location
 5. Sending interactive buttons
 6. Sending template messages
 7. Parsing messages and media received
+8. Receiving and parsing messages - [hook object](https://github.com/filipporomani/whatsapp/wiki/Hook()-object)
+
+## App events
+
+App events are now available! 
+
+The docs are available in the [wiki](https://github.com/filipporomani/whatsapp/wiki/App-events)
+
+Please test this feature out and leave feedbacks/report issues on GitHub!
+
+## Installation
+
+To install the library you can either use pip:
+
+``pip install whatsapp-python``
+
+or git:
+
+```bash
+git clone https://github.com/filipporomani/whatsapp.git
+cd whatsapp
+python3 setup.py install
+```
 
 ## Documentation
 
-The documentation for the is available in the [**wiki**](https://github.com/filipporomani/whatsapp/wiki)
+The documentation for the library is available in the [**wiki**](https://github.com/filipporomani/whatsapp/wiki)
 
 ## Costs of the API
 
 While using third-party API providers of the WhatsApp API may have some monthly fees, using the WhatsApp API provided directly by Facebook is way cheaper. 
 The first 1000 chats created are free, then there is a pay-as-you-go fee that is paid for each conversation started.
 
 All the prices are available in the [**WhatsApp API docs**](https://developers.facebook.com/docs/whatsapp/pricing)
```

### Comparing `whatsapp-python-2.4.3/setup.py` & `whatsapp-python-2.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from os import path
 from setuptools import setup
 
 # read the contents of your description file
+# the version in this file should be updated ONLY on a new PYPI release
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="whatsapp-python",
-    version="2.4.3",
+    version="2.9.3",
     description="Opensource Python wrapper to WhatsApp Cloud API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/filipporomani/whatsapp",
     author="Filippo Romani",
     author_email="mail@filipporomani.it",
     license="MIT",
```

### Comparing `whatsapp-python-2.4.3/whatsapp/__init__.py` & `whatsapp-python-2.9.3/whatsapp/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,30 +10,29 @@
 
 
 # Setup logging
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 
 class WhatsApp(object):
-    """ "
-    WhatsApp Object
-    """
-
     def __init__(self, token: str = "", phone_number_id: str = "", logger: bool = True):
         """
         Initialize the WhatsApp Object
 
         Args:
             token[str]: Token for the WhatsApp cloud API obtained from the Facebook developer portal
             phone_number_id[str]: Phone number id for the WhatsApp cloud API obtained from the developer portal
             logger[bool]: Whether to enable logging or not (default: True)
         """
 
+        # version here MUST be changed manually after every change to deferentiate between PYPI and GitHub versions
         # Check if the version is up to date
-        self.VERSION = "2.4.3"
+
+        self.VERSION = "2.9.3"
+
         latest = str(requests.get(
             "https://pypi.org/pypi/whatsapp-python/json").json()["info"]["version"])
         if self.VERSION != latest:
             version_int = int(self.VERSION.replace(".", ""))
             latest_int = int(latest.replace(".", ""))
             # this is to avoid the case where the version is 1.0.10 and the latest is 1.0.2 (possible if user is using the github version)
             if version_int < latest_int:
@@ -48,24 +47,63 @@
             raise ValueError(
                 "Token or phone number ID not provided but is required")
         self.token = token
         self.phone_number_id = phone_number_id
         self.base_url = "https://graph.facebook.com/v15.0"
         self.url = f"{self.base_url}/{phone_number_id}/messages"
 
+        def base():
+            pass
+        self.message_handler = base
+        self.other_handler = base
+        self.verification_handler = base
         self.headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.token}"
         }
         if logger is False:
             logging.disable(logging.INFO)
             logging.disable(logging.ERROR)
 
+        self.app = Flask(__name__)
+
+        # Verification handler has 1 argument: challenge (str | bool): str if verification is successful, False if not
+
+        @self.app.get("/")
+        def verify_token():
+            if request.args.get("hub.verify_token") == self.token:
+                logging.info("Verified webhook")
+                challenge = request.args.get("hub.challenge")
+                self.verification_handler(challenge)
+                self.other_handler(challenge)
+                return str(challenge)
+            logging.error("Webhook Verification failed")
+            self.verification_handler(False)
+            self.other_handler(False)
+            return "Invalid verification token"
+
+        @self.app.post("/")
+        def hook():
+            # Handle Webhook Subscriptions
+            data = request.get_json()
+            if data is None:
+                return Response(status=200)
+            logging.info("Received webhook data: %s", data)
+            changed_field = self.instance.changed_field(data)
+            if changed_field == "messages":
+                new_message = self.instance.is_message(data)
+                if new_message:
+                    msg = Message(instance=self.instance, data=data)
+                    self.message_handler(msg)
+                    self.other_handler(msg)
+            return "OK", 200
+
     # all the files starting with _ are imported here, and should not be imported directly.
 
+
     from ext._property import authorized
     from ext._send_others import send_custom_json, send_contacts
     from ext._message import send_template
     from ext._send_media import send_image, send_video, send_audio, send_location, send_sticker, send_document
     from ext._media import upload_media, query_media_url, download_media, delete_media
     from ext._buttons import send_button, create_button, send_reply_button
     from ext._static import is_message, get_mobile, get_author, get_name, get_message, get_message_id, get_message_type, get_message_timestamp, get_audio, get_delivery, get_document, get_image, get_interactive_response, get_location, get_video, changed_field
@@ -83,27 +121,56 @@
     get_interactive_response = staticmethod(get_interactive_response)
     get_location = staticmethod(get_location)
     get_video = staticmethod(get_video)
     changed_field = staticmethod(changed_field)
     get_author = staticmethod(get_author)
 
     authorized = property(authorized)
-    
+
     def create_message(self, **kwargs) -> Message:
         """
         Create a message object
 
         Args:
             data[dict]: The message data
             content[str]: The message content
             to[str]: The recipient
             rec_type[str]: The recipient type (individual/group)
         """
         return Message(**kwargs, instance=self)
-    
+
+    def on_message(self, handler: function):
+        """
+        Set the handler for incoming messages
+
+        Args:
+            handler[function]: The handler function
+        """
+        self.message_handler = handler
+
+    def on_event(self, handler: function):
+        """
+        Set the handler for other events
+
+        Args:
+            handler[function]: The handler function
+        """
+        self.other_handler = handler
+
+    def on_verification(self, handler: function):
+        """
+        Set the handler for verification
+
+        Args:
+            handler[function]: The handler function
+        """
+        self.verification_handler = handler
+
+    def run(self, host: str = "localhost", port: int = 5000, debug: bool = False, **options):
+        self.app.run(host=host, port=port, debug=debug, **options)
 
 
 class Message(object):
     def __init__(self, data: dict = {}, instance: WhatsApp = None, content: str = "", to: str = "", rec_type: str = "individual"):  # type: ignore
         try:
             self.id = instance.get_message_id(data)
         except:
@@ -161,48 +228,7 @@
                 pass
 
         self.instance = instance
         self.url = self.instance.url
         self.headers = self.instance.headers
 
     from ext._message import send, reply, mark_as_read
-
-
-
-
-class Hook(object):
-
-    def __init__(self, instance: WhatsApp = None, host: str = "localhost", port: int = 8080, verify_token: str = "", handler: function = None):
-        self.instance = instance
-        self.host = host
-        self.port = port
-        self.token = verify_token
-        self.app = Flask(__name__)
-        self.handler = handler
-    
-        @self.app.get("/")
-        def verify_token():
-            if request.args.get("hub.verify_token") == self.token:
-                logging.info("Verified webhook")
-                challenge = request.args.get("hub.challenge")
-                return str(challenge)
-            logging.error("Webhook Verification failed")
-            return "Invalid verification token"
-
-
-        @self.app.post("/")
-        def hook():
-            # Handle Webhook Subscriptions
-            data = request.get_json()
-            if data is None:
-                return Response(status=200)
-            logging.info("Received webhook data: %s", data)
-            changed_field = self.instance.changed_field(data)
-            if changed_field == "messages":
-                new_message = self.instance.is_message(data)
-                if new_message:
-                    msg = Message(instance=self.instance, data=data)
-                    self.handler(msg)
-            return "OK", 200
-
-    def run(self):
-        self.app.run(host=self.host, port=self.port)
```

### Comparing `whatsapp-python-2.4.3/whatsapp_python.egg-info/PKG-INFO` & `whatsapp-python-2.9.3/whatsapp_python.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-python
-Version: 2.4.3
+Version: 2.9.3
 Summary: Opensource Python wrapper to WhatsApp Cloud API
 Home-page: https://github.com/filipporomani/whatsapp
 Author: Filippo Romani
 Author-email: mail@filipporomani.it
 License: MIT
 Keywords: whatsapp,whatsapp-libary,WhatsApp Cloud API Wrapper,PyWhatsApp,WhatsApp API in Python
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [whatsapp-python](https://pypi.org/project/whatsapp-python/)
 
 ![Made in Italy](https://img.shields.io/badge/made%20in-italy-008751.svg?style=flat-square)
-[![Downloads](https://pepy.tech/badge/whatsapp-python)](https://pepy.tech/project/whatsapp-python)
+[![Downloads](https://static.pepy.tech/personalized-badge/whatsapp-python?period=total&units=none&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/month)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/week)](https://pepy.tech/project/whatsapp-python)
 
 Free, open-source Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api).
 
 Forked from [Neurotech-HQ/heyoo](https://github.com/Neurotech-HQ/heyoo)
 
@@ -36,18 +36,41 @@
 1. Sending messages
 2. Marking messages as read
 3. Sending Media (images, audio, video and documents)
 4. Sending location
 5. Sending interactive buttons
 6. Sending template messages
 7. Parsing messages and media received
+8. Receiving and parsing messages - [hook object](https://github.com/filipporomani/whatsapp/wiki/Hook()-object)
+
+## App events
+
+App events are now available! 
+
+The docs are available in the [wiki](https://github.com/filipporomani/whatsapp/wiki/App-events)
+
+Please test this feature out and leave feedbacks/report issues on GitHub!
+
+## Installation
+
+To install the library you can either use pip:
+
+``pip install whatsapp-python``
+
+or git:
+
+```bash
+git clone https://github.com/filipporomani/whatsapp.git
+cd whatsapp
+python3 setup.py install
+```
 
 ## Documentation
 
-The documentation for the is available in the [**wiki**](https://github.com/filipporomani/whatsapp/wiki)
+The documentation for the library is available in the [**wiki**](https://github.com/filipporomani/whatsapp/wiki)
 
 ## Costs of the API
 
 While using third-party API providers of the WhatsApp API may have some monthly fees, using the WhatsApp API provided directly by Facebook is way cheaper. 
 The first 1000 chats created are free, then there is a pay-as-you-go fee that is paid for each conversation started.
 
 All the prices are available in the [**WhatsApp API docs**](https://developers.facebook.com/docs/whatsapp/pricing)
```

