# Comparing `tmp/SecuriPy-1.0.2.tar.gz` & `tmp/SecuriPy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecuriPy-1.0.2.tar", last modified: Sat May 20 12:11:08 2023, max compression
+gzip compressed data, was "SecuriPy-1.0.3.tar", last modified: Sat May 27 06:05:00 2023, max compression
```

## Comparing `SecuriPy-1.0.2.tar` & `SecuriPy-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 12:11:08.627121 SecuriPy-1.0.2/
--rw-rw-rw-   0        0        0     3521 2023-05-20 12:11:08.626126 SecuriPy-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2925 2023-05-18 11:39:07.000000 SecuriPy-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 12:11:08.624123 SecuriPy-1.0.2/SecuriPy.egg-info/
--rw-rw-rw-   0        0        0     3521 2023-05-20 12:11:08.000000 SecuriPy-1.0.2/SecuriPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-05-20 12:11:08.000000 SecuriPy-1.0.2/SecuriPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 12:11:08.000000 SecuriPy-1.0.2/SecuriPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 12:11:08.000000 SecuriPy-1.0.2/SecuriPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1531 2023-05-17 17:44:10.000000 SecuriPy-1.0.2/SecuriPy.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 12:11:08.627121 SecuriPy-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      879 2023-05-20 12:10:52.000000 SecuriPy-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 06:05:00.495556 SecuriPy-1.0.3/
+-rw-rw-rw-   0        0        0     3594 2023-05-27 06:05:00.494486 SecuriPy-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2998 2023-05-27 06:04:44.000000 SecuriPy-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 06:05:00.492177 SecuriPy-1.0.3/SecuriPy.egg-info/
+-rw-rw-rw-   0        0        0     3594 2023-05-27 06:05:00.000000 SecuriPy-1.0.3/SecuriPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-05-27 06:05:00.000000 SecuriPy-1.0.3/SecuriPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 06:05:00.000000 SecuriPy-1.0.3/SecuriPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 06:05:00.000000 SecuriPy-1.0.3/SecuriPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1663 2023-05-27 06:02:51.000000 SecuriPy-1.0.3/SecuriPy.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 06:05:00.496064 SecuriPy-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-05-27 06:03:32.000000 SecuriPy-1.0.3/setup.py
```

### Comparing `SecuriPy-1.0.2/PKG-INFO` & `SecuriPy-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
@@ -27,15 +27,15 @@
 ```
 
 ## Usage
 
 Import the `SecuriPy` module in your Python script to access the functions:
 
 ```python
-from SecuriPy import encrypt, decrypt, key
+from SecuriPy import encrypt, decrypt, pwd
 ```
 OR
 ```python
 from SecuriPy import *
 
 ### `encrypt(message, secret_key)`
 
@@ -51,34 +51,35 @@
 ```
 
 Output:
 ```
 ե֎Չ֏քԿՂլ֓ՏևչՊԽĵŁõĻĭīĺĭļõĳĭŁĵ
 ```
 
-### `decrypt(encrypted_message)`
+### `decrypt(encrypted_message, password)`
 
-The `decrypt` function takes one parameter: `encrypted_message`. It decrypts the provided `encrypted_message` using the given `secret_key` that is embeded in the `encrypted_message` and returns the original human-readable message.
+The `decrypt` function takes two parameters: `encrypted_message`and `password`. It decrypts the provided `encrypted_message` using the given `secret_key` that is embeded in the `encrypted_message` and returns the original human-readable message.
 
 Example:
 ```python
 encrypted_message = "ե֎Չ֏քԿՂլ֓ՏևչՊԽĵŁõĻĭīĺĭļõĳĭŁĵ'"
+secret_key = "my-secret-key"
 
-decrypted_message = decrypt(encrypted_message)
+decrypted_message = decrypt(encrypted_message, secret_key)
 print(decrypted_message)
 ```
 
 Output:
 ```
 Hello, World!
 ```
 
-### `key()`
+### `pwd()`
 
-The `key` function generates a secret key that can be used for encryption and decryption. It takes two parameters `message` and `password`. With respect to the message it generateda a secret key. It returns the secret key as a string.
+The `pwd` function generates a secret password that can be used for encryption and decryption. It takes two parameters `message` and `password`. With respect to the message it generates a a secret key. It returns the secret key as a string.
 
 ## Security Considerations
 
 - Once the encryption is done you won't be able to access the secret key.
 - Use a strong and unique `secret_key` for each encryption operation to enhance security. Avoid using easily guessable or common phrases.
 - Always encrypt sensitive information before storing or transmitting it. SecuriPy is a tool for obfuscating the data but does not provide additional security measures for data storage or transmission.
```

### Comparing `SecuriPy-1.0.2/README.md` & `SecuriPy-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```
 
 ## Usage
 
 Import the `SecuriPy` module in your Python script to access the functions:
 
 ```python
-from SecuriPy import encrypt, decrypt, key
+from SecuriPy import encrypt, decrypt, pwd
 ```
 OR
 ```python
 from SecuriPy import *
 
 ### `encrypt(message, secret_key)`
 
@@ -35,34 +35,35 @@
 ```
 
 Output:
 ```
 ե֎Չ֏քԿՂլ֓ՏևչՊԽĵŁõĻĭīĺĭļõĳĭŁĵ
 ```
 
-### `decrypt(encrypted_message)`
+### `decrypt(encrypted_message, password)`
 
-The `decrypt` function takes one parameter: `encrypted_message`. It decrypts the provided `encrypted_message` using the given `secret_key` that is embeded in the `encrypted_message` and returns the original human-readable message.
+The `decrypt` function takes two parameters: `encrypted_message`and `password`. It decrypts the provided `encrypted_message` using the given `secret_key` that is embeded in the `encrypted_message` and returns the original human-readable message.
 
 Example:
 ```python
 encrypted_message = "ե֎Չ֏քԿՂլ֓ՏևչՊԽĵŁõĻĭīĺĭļõĳĭŁĵ'"
+secret_key = "my-secret-key"
 
-decrypted_message = decrypt(encrypted_message)
+decrypted_message = decrypt(encrypted_message, secret_key)
 print(decrypted_message)
 ```
 
 Output:
 ```
 Hello, World!
 ```
 
-### `key()`
+### `pwd()`
 
-The `key` function generates a secret key that can be used for encryption and decryption. It takes two parameters `message` and `password`. With respect to the message it generateda a secret key. It returns the secret key as a string.
+The `pwd` function generates a secret password that can be used for encryption and decryption. It takes two parameters `message` and `password`. With respect to the message it generates a a secret key. It returns the secret key as a string.
 
 ## Security Considerations
 
 - Once the encryption is done you won't be able to access the secret key.
 - Use a strong and unique `secret_key` for each encryption operation to enhance security. Avoid using easily guessable or common phrases.
 - Always encrypt sensitive information before storing or transmitting it. SecuriPy is a tool for obfuscating the data but does not provide additional security measures for data storage or transmission.
```

### Comparing `SecuriPy-1.0.2/SecuriPy.egg-info/PKG-INFO` & `SecuriPy-1.0.3/SecuriPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
@@ -27,15 +27,15 @@
 ```
 
 ## Usage
 
 Import the `SecuriPy` module in your Python script to access the functions:
 
 ```python
-from SecuriPy import encrypt, decrypt, key
+from SecuriPy import encrypt, decrypt, pwd
 ```
 OR
 ```python
 from SecuriPy import *
 
 ### `encrypt(message, secret_key)`
 
@@ -51,34 +51,35 @@
 ```
 
 Output:
 ```
 ե֎Չ֏քԿՂլ֓ՏևչՊԽĵŁõĻĭīĺĭļõĳĭŁĵ
 ```
 
-### `decrypt(encrypted_message)`
+### `decrypt(encrypted_message, password)`
 
-The `decrypt` function takes one parameter: `encrypted_message`. It decrypts the provided `encrypted_message` using the given `secret_key` that is embeded in the `encrypted_message` and returns the original human-readable message.
+The `decrypt` function takes two parameters: `encrypted_message`and `password`. It decrypts the provided `encrypted_message` using the given `secret_key` that is embeded in the `encrypted_message` and returns the original human-readable message.
 
 Example:
 ```python
 encrypted_message = "ե֎Չ֏քԿՂլ֓ՏևչՊԽĵŁõĻĭīĺĭļõĳĭŁĵ'"
+secret_key = "my-secret-key"
 
-decrypted_message = decrypt(encrypted_message)
+decrypted_message = decrypt(encrypted_message, secret_key)
 print(decrypted_message)
 ```
 
 Output:
 ```
 Hello, World!
 ```
 
-### `key()`
+### `pwd()`
 
-The `key` function generates a secret key that can be used for encryption and decryption. It takes two parameters `message` and `password`. With respect to the message it generateda a secret key. It returns the secret key as a string.
+The `pwd` function generates a secret password that can be used for encryption and decryption. It takes two parameters `message` and `password`. With respect to the message it generates a a secret key. It returns the secret key as a string.
 
 ## Security Considerations
 
 - Once the encryption is done you won't be able to access the secret key.
 - Use a strong and unique `secret_key` for each encryption operation to enhance security. Avoid using easily guessable or common phrases.
 - Always encrypt sensitive information before storing or transmitting it. SecuriPy is a tool for obfuscating the data but does not provide additional security measures for data storage or transmission.
```

### Comparing `SecuriPy-1.0.2/SecuriPy.py` & `SecuriPy-1.0.3/SecuriPy.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,20 +23,23 @@
     key = pwd(message, password)
     encrypted_text = []
     for i in range(len(message)):
         x = (ord(message[i]) +ord(key[i]) + 1000)
         encrypted_text.append(chr(x))
     encrypted_text = ("" . join(encrypted_text))
     key = ("".join(key))
-    return encrypted_text + key
+    return encrypted_text+key , key
 
-def decrypt(encrypted_text):
+def decrypt(encrypted_text, password):
     """Figures out the key from the encrypted text and decryptes it with respect to the key"""
     orig_text = []
     b = int(len(encrypted_text)/2)
     key = encrypted_text[b:]
     encrypted_text = encrypted_text[:b-1]
-    for i in range(len(encrypted_text)):
-        x = (ord(encrypted_text[i]) -ord(key[i]) - 1000)
-        orig_text.append(chr(x))
-    orig_text = ("" . join(orig_text))
-    return orig_text
+    if key == password:
+        for i in range(len(encrypted_text)):
+            x = (ord(encrypted_text[i]) -ord(key[i]) - 1000)
+            orig_text.append(chr(x))
+        orig_text = ("" . join(orig_text))
+        return orig_text
+    else:
+        return "Message is corrupt or Password is incorrect"
```

### Comparing `SecuriPy-1.0.2/setup.py` & `SecuriPy-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SecuriPy",
-    version="1.0.2",
+    version="1.0.3",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Encrypter and Decrypter of Readable messages Using Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/SecuriPy",
     project_urls={
```

