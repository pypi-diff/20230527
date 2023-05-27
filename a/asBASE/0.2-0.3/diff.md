# Comparing `tmp/asBASE-0.2.tar.gz` & `tmp/asBASE-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asBASE-0.2.tar", last modified: Sat May 27 12:28:13 2023, max compression
+gzip compressed data, was "asBASE-0.3.tar", last modified: Sat May 27 12:56:47 2023, max compression
```

## Comparing `asBASE-0.2.tar` & `asBASE-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 12:28:13.090643 asBASE-0.2/
--rw-rw----   0 root         (0) everybody  (9997)       20 2023-05-26 23:55:19.000000 asBASE-0.2/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)      320 2023-05-27 12:28:13.066643 asBASE-0.2/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      818 2023-05-27 00:54:02.000000 asBASE-0.2/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 12:28:12.926643 asBASE-0.2/asBASE/
--rw-rw----   0 root         (0) everybody  (9997)     2175 2023-05-27 12:27:19.000000 asBASE-0.2/asBASE/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 12:28:13.042643 asBASE-0.2/asBASE.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      320 2023-05-27 12:28:12.000000 asBASE-0.2/asBASE.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      169 2023-05-27 12:28:12.000000 asBASE-0.2/asBASE.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-27 12:28:12.000000 asBASE-0.2/asBASE.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        7 2023-05-27 12:28:12.000000 asBASE-0.2/asBASE.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-27 12:28:13.090643 asBASE-0.2/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      361 2023-05-27 12:28:01.000000 asBASE-0.2/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 12:56:47.759232 asBASE-0.3/
+-rw-rw----   0 root         (0) everybody  (9997)       20 2023-05-26 23:55:19.000000 asBASE-0.3/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)      320 2023-05-27 12:56:47.735232 asBASE-0.3/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      818 2023-05-27 00:54:02.000000 asBASE-0.3/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 12:56:47.595232 asBASE-0.3/asBASE/
+-rw-rw----   0 root         (0) everybody  (9997)     2183 2023-05-27 12:55:57.000000 asBASE-0.3/asBASE/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 12:56:47.711232 asBASE-0.3/asBASE.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      320 2023-05-27 12:56:47.000000 asBASE-0.3/asBASE.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      169 2023-05-27 12:56:47.000000 asBASE-0.3/asBASE.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-27 12:56:47.000000 asBASE-0.3/asBASE.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        7 2023-05-27 12:56:47.000000 asBASE-0.3/asBASE.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-27 12:56:47.763232 asBASE-0.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      361 2023-05-27 12:56:33.000000 asBASE-0.3/setup.py
```

### Comparing `asBASE-0.2/README.md` & `asBASE-0.3/README.md`

 * *Files identical despite different names*

### Comparing `asBASE-0.2/asBASE/__init__.py` & `asBASE-0.3/asBASE/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 		if key in json_dict:
 			if "time" not in json_dict:
 				json_dict["time"] = {"expire": {}}
 			json_dict["time"]["expire"][key] = time.time() + ttl
 			self.write_json(json_dict)
 			return True
 		return False
-	def sadd(self, key, value):
+	def sadd(self, key, *values):
 		json_dict = self.read_json()
 		if "set" in json_dict.get(key, {}):
-			json_dict[key]["set"].append(value)
+			json_dict[key]["set"].extend(values)
 		else:
-			json_dict[key] = {"set": [value]}
+			json_dict[key] = {"set": list(values)}
 		self.write_json(json_dict)
 	def smembers(self, key):
 		json_dict = self.read_json()
 		return json_dict.get(key, {}).get("set", [])
 	def srem(self, key, value):
 		json_dict = self.read_json()
 		if "set" in json_dict.get(key, {}):
```

