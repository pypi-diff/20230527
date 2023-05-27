# Comparing `tmp/permaswap-0.1.2.tar.gz` & `tmp/permaswap-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permaswap-0.1.2.tar", last modified: Mon Nov 14 16:05:57 2022, max compression
+gzip compressed data, was "permaswap-0.1.3.tar", last modified: Sat May 27 03:44:08 2023, max compression
```

## Comparing `permaswap-0.1.2.tar` & `permaswap-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-11-14 16:05:57.054854 permaswap-0.1.2/
--rw-r--r--   0 jay        (501) staff       (20)     1066 2022-11-13 04:21:00.000000 permaswap-0.1.2/LICENSE
--rw-r--r--   0 jay        (501) staff       (20)     1313 2022-11-14 16:05:57.054754 permaswap-0.1.2/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      732 2022-11-14 11:18:20.000000 permaswap-0.1.2/README.md
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-11-14 16:05:57.054149 permaswap-0.1.2/permaswap/
--rw-r--r--   0 jay        (501) staff       (20)     2441 2022-11-14 15:54:24.000000 permaswap-0.1.2/permaswap/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-11-14 16:05:57.054620 permaswap-0.1.2/permaswap.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)     1313 2022-11-14 16:05:57.000000 permaswap-0.1.2/permaswap.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      212 2022-11-14 16:05:57.000000 permaswap-0.1.2/permaswap.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2022-11-14 16:05:57.000000 permaswap-0.1.2/permaswap.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)       25 2022-11-14 16:05:57.000000 permaswap-0.1.2/permaswap.egg-info/requires.txt
--rw-r--r--   0 jay        (501) staff       (20)       10 2022-11-14 16:05:57.000000 permaswap-0.1.2/permaswap.egg-info/top_level.txt
--rw-r--r--   0 jay        (501) staff       (20)       38 2022-11-14 16:05:57.054885 permaswap-0.1.2/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)      773 2022-11-14 16:03:29.000000 permaswap-0.1.2/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-27 03:44:08.911804 permaswap-0.1.3/
+-rw-r--r--   0 jay        (501) staff       (20)     1066 2022-11-13 04:21:00.000000 permaswap-0.1.3/LICENSE
+-rw-r--r--   0 jay        (501) staff       (20)     1320 2023-05-27 03:44:08.911710 permaswap-0.1.3/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      759 2023-02-28 05:14:17.000000 permaswap-0.1.3/README.md
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-27 03:44:08.911125 permaswap-0.1.3/permaswap/
+-rw-r--r--   0 jay        (501) staff       (20)       58 2023-05-27 03:26:43.000000 permaswap-0.1.3/permaswap/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      630 2023-02-28 04:59:13.000000 permaswap-0.1.3/permaswap/lp.py
+-rw-r--r--   0 jay        (501) staff       (20)     3753 2023-05-27 03:26:35.000000 permaswap-0.1.3/permaswap/swap.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-27 03:44:08.911583 permaswap-0.1.3/permaswap.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)     1320 2023-05-27 03:44:08.000000 permaswap-0.1.3/permaswap.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      246 2023-05-27 03:44:08.000000 permaswap-0.1.3/permaswap.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2023-05-27 03:44:08.000000 permaswap-0.1.3/permaswap.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)       25 2023-05-27 03:44:08.000000 permaswap-0.1.3/permaswap.egg-info/requires.txt
+-rw-r--r--   0 jay        (501) staff       (20)       10 2023-05-27 03:44:08.000000 permaswap-0.1.3/permaswap.egg-info/top_level.txt
+-rw-r--r--   0 jay        (501) staff       (20)       38 2023-05-27 03:44:08.911835 permaswap-0.1.3/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)      773 2023-05-27 03:43:49.000000 permaswap-0.1.3/setup.py
```

### Comparing `permaswap-0.1.2/LICENSE` & `permaswap-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `permaswap-0.1.2/PKG-INFO` & `permaswap-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: permaswap
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python wrappers for permaswap
 Home-page: https://github.com/permaswap/permaswap.py
+Download-URL: https://github.com/permaswap/permaswap.py/archive/refs/tags/v0.1.3.tar.gz
 Author: haroldfinch2022
 Author-email: e2d8nnhp8@gmail.com
 License: MIT
-Download-URL: https://github.com/permaswap/permaswap.py/archive/refs/tags/v0.1.2.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -25,14 +24,15 @@
 ```
 
 # usage
 
 1. perpare everpay account
 
 ```python
+import everpay
 api_server = 'https://api-dev.everpay.io'
 
 # eth account
 pk = ''
 signer = everpay.ETHSigner(pk)
 
 # or ar account
@@ -40,27 +40,26 @@
 account = everpay.Account(api_server, signer)
 ```
 
 2. init permaswap
 
 ```python
 router_host = 'wss://router0-dev.permaswap.network/'
-swap = permaswap.Permaswap(router_host, account)
+swap = permaswap.Swap(router_host, account)
 ```
 
 3. query order
 
 ```python
+import permaswap
 # get_order('token_in', 'token_out', 'amount_in')
 # sell 1 tar for tusdc
 order = swap.get_order('tAR', 'tUSDC', 10**12)
 print(order)
 ```
 
 4. place order
 
 ```python
 result = swap.place_order(order)
 print(result)
 ```
-
-
```

### Comparing `permaswap-0.1.2/README.md` & `permaswap-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 ```
 
 # usage
 
 1. perpare everpay account
 
 ```python
+import everpay
 api_server = 'https://api-dev.everpay.io'
 
 # eth account
 pk = ''
 signer = everpay.ETHSigner(pk)
 
 # or ar account
@@ -23,20 +24,21 @@
 account = everpay.Account(api_server, signer)
 ```
 
 2. init permaswap
 
 ```python
 router_host = 'wss://router0-dev.permaswap.network/'
-swap = permaswap.Permaswap(router_host, account)
+swap = permaswap.Swap(router_host, account)
 ```
 
 3. query order
 
 ```python
+import permaswap
 # get_order('token_in', 'token_out', 'amount_in')
 # sell 1 tar for tusdc
 order = swap.get_order('tAR', 'tUSDC', 10**12)
 print(order)
 ```
 
 4. place order
```

### Comparing `permaswap-0.1.2/permaswap/__init__.py` & `permaswap-0.1.3/permaswap/swap.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,16 +5,46 @@
 
 def get_amount_out(user, order, token_out_tag):
     amount_out = 0
     for path in order['paths']:
         if path['to'].lower() == user.lower() and path['tokenTag'] == token_out_tag:
             amount_out += int(path['amount'])
     return str(amount_out)
-    
-class Permaswap:
+
+def get_order(pay_host, ps_router_host, address, token_in, token_out, amount_in):
+    ps_router_url= urllib.parse.urljoin(ps_router_host, '/wsuser')
+    client = everpay.Client(pay_host)
+    token_in_tag = client.get_token_tag(token_in)
+    token_out_tag = client.get_token_tag(token_out)
+    token_in_decimals = client.get_token(token_in).decimals
+    token_out_decimals = client.get_token(token_out).decimals
+
+    query = {
+        'event': 'query',
+        'address': address,
+        'tokenIn': token_in_tag,
+        'tokenOut': token_out_tag,
+        'amountIn': str(amount_in)
+    }
+    ws = create_connection(ps_router_url)
+    ws.send(json.dumps(query))
+    data = json.loads(ws.recv())
+    if data['event'] == 'order':
+        order = data
+        order['tokenIn'] = token_in_tag
+        order['tokenOut'] = token_out_tag
+        order['amount_in'] = str(amount_in)
+        order['amount_out'] = get_amount_out(address, order, token_out_tag)
+        order['amount_in2'] = str(Decimal(int(order['amount_in']))/Decimal(10**token_in_decimals))
+        order['amount_out2'] = str(Decimal(int(order['amount_out']))/Decimal(10**token_out_decimals))
+        order['rate'] = float(order['amount_out2'])/float(order['amount_in2'])
+        return order
+    return data
+
+class Swap:
     def __init__(self, router_host, account):
         self.router_url = urllib.parse.urljoin(router_host, '/wsuser')
         self.account = account
     
     def get_order(self, token_in, token_out, amount_in):
         token_in_tag = self.account.get_token_tag(token_in)
         token_out_tag = self.account.get_token_tag(token_out)
@@ -25,24 +55,27 @@
             'address': self.account.address,
             'tokenIn': token_in_tag,
             'tokenOut': token_out_tag,
             'amountIn': str(amount_in)
         }
         ws = create_connection(self.router_url)
         ws.send(json.dumps(query))
-        order = json.loads(ws.recv())
-        if order['event'] == 'order':
+        data = json.loads(ws.recv())
+        if data['event'] == 'order':
+            order = data
             order['tokenIn'] = token_in_tag
             order['tokenOut'] = token_out_tag
             order['amount_in'] = str(amount_in)
             order['amount_out'] = get_amount_out(self.account.address, order, token_out_tag)
             order['amount_in2'] = str(Decimal(int(order['amount_in']))/Decimal(10**token_in_decimals))
             order['amount_out2'] = str(Decimal(int(order['amount_out']))/Decimal(10**token_out_decimals))
             order['rate'] = float(order['amount_out2'])/float(order['amount_in2'])
             return order
+        
+        return data
     
     def place_order(self, order):
         bundle = everpay.load_bundle(order)
         sig = self.account.sign_bundle(bundle.get_data_to_sign())
         bundle.add_sig(self.account.address, sig)
         submit_order = {
             'event': 'submit',
```

### Comparing `permaswap-0.1.2/permaswap.egg-info/PKG-INFO` & `permaswap-0.1.3/permaswap.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: permaswap
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python wrappers for permaswap
 Home-page: https://github.com/permaswap/permaswap.py
+Download-URL: https://github.com/permaswap/permaswap.py/archive/refs/tags/v0.1.3.tar.gz
 Author: haroldfinch2022
 Author-email: e2d8nnhp8@gmail.com
 License: MIT
-Download-URL: https://github.com/permaswap/permaswap.py/archive/refs/tags/v0.1.2.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -25,14 +24,15 @@
 ```
 
 # usage
 
 1. perpare everpay account
 
 ```python
+import everpay
 api_server = 'https://api-dev.everpay.io'
 
 # eth account
 pk = ''
 signer = everpay.ETHSigner(pk)
 
 # or ar account
@@ -40,27 +40,26 @@
 account = everpay.Account(api_server, signer)
 ```
 
 2. init permaswap
 
 ```python
 router_host = 'wss://router0-dev.permaswap.network/'
-swap = permaswap.Permaswap(router_host, account)
+swap = permaswap.Swap(router_host, account)
 ```
 
 3. query order
 
 ```python
+import permaswap
 # get_order('token_in', 'token_out', 'amount_in')
 # sell 1 tar for tusdc
 order = swap.get_order('tAR', 'tUSDC', 10**12)
 print(order)
 ```
 
 4. place order
 
 ```python
 result = swap.place_order(order)
 print(result)
 ```
-
-
```

### Comparing `permaswap-0.1.2/setup.py` & `permaswap-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 setuptools.setup(
     name='permaswap',
-    version='0.1.2',
+    version='0.1.3',
     packages=['permaswap',],
     license='MIT',
     description = 'Python wrappers for permaswap',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author = 'haroldfinch2022',
     author_email = 'e2d8nnhp8@gmail.com',
     install_requires=['everpay', 'websocket-client'],
     url = 'https://github.com/permaswap/permaswap.py',
-    download_url = 'https://github.com/permaswap/permaswap.py/archive/refs/tags/v0.1.2.tar.gz',
+    download_url = 'https://github.com/permaswap/permaswap.py/archive/refs/tags/v0.1.3.tar.gz',
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 2",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

