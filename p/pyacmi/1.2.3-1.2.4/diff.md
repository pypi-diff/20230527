# Comparing `tmp/pyacmi-1.2.3.tar.gz` & `tmp/pyacmi-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacmi-1.2.3.tar", last modified: Tue May  9 20:15:18 2023, max compression
+gzip compressed data, was "pyacmi-1.2.4.tar", last modified: Sat May 27 12:39:31 2023, max compression
```

## Comparing `pyacmi-1.2.3.tar` & `pyacmi-1.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:15:18.780234 pyacmi-1.2.3/
--rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 16:16:44.000000 pyacmi-1.2.3/LICENSE
--rw-r--r--   0 wangtong   (501) staff       (20)     2104 2023-05-09 20:15:18.780085 pyacmi-1.2.3/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)     1426 2023-05-09 20:14:47.000000 pyacmi-1.2.3/README.md
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:15:18.779183 pyacmi-1.2.3/pyacmi/
--rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 16:19:56.000000 pyacmi-1.2.3/pyacmi/__init__.py
--rw-r--r--   0 wangtong   (501) staff       (20)    36480 2023-05-09 20:13:50.000000 pyacmi-1.2.3/pyacmi/acmi.py
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:15:18.779895 pyacmi-1.2.3/pyacmi.egg-info/
--rw-r--r--   0 wangtong   (501) staff       (20)     2104 2023-05-09 20:15:18.000000 pyacmi-1.2.3/pyacmi.egg-info/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-09 20:15:18.000000 pyacmi-1.2.3/pyacmi.egg-info/SOURCES.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-09 20:15:18.000000 pyacmi-1.2.3/pyacmi.egg-info/dependency_links.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       22 2023-05-09 20:15:18.000000 pyacmi-1.2.3/pyacmi.egg-info/requires.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-09 20:15:18.000000 pyacmi-1.2.3/pyacmi.egg-info/top_level.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-09 20:15:18.780282 pyacmi-1.2.3/setup.cfg
--rw-r--r--   0 wangtong   (501) staff       (20)     1030 2023-05-09 20:15:17.000000 pyacmi-1.2.3/setup.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-27 12:39:31.726018 pyacmi-1.2.4/
+-rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 16:16:44.000000 pyacmi-1.2.4/LICENSE
+-rw-r--r--   0 wangtong   (501) staff       (20)     2130 2023-05-27 12:39:31.725900 pyacmi-1.2.4/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)     1452 2023-05-11 09:48:17.000000 pyacmi-1.2.4/README.md
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-27 12:39:31.725043 pyacmi-1.2.4/pyacmi/
+-rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 16:19:56.000000 pyacmi-1.2.4/pyacmi/__init__.py
+-rw-r--r--   0 wangtong   (501) staff       (20)    38064 2023-05-11 15:39:43.000000 pyacmi-1.2.4/pyacmi/acmi.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-27 12:39:31.725713 pyacmi-1.2.4/pyacmi.egg-info/
+-rw-r--r--   0 wangtong   (501) staff       (20)     2130 2023-05-27 12:39:31.000000 pyacmi-1.2.4/pyacmi.egg-info/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-27 12:39:31.000000 pyacmi-1.2.4/pyacmi.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-27 12:39:31.000000 pyacmi-1.2.4/pyacmi.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       22 2023-05-27 12:39:31.000000 pyacmi-1.2.4/pyacmi.egg-info/requires.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-27 12:39:31.000000 pyacmi-1.2.4/pyacmi.egg-info/top_level.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-27 12:39:31.726061 pyacmi-1.2.4/setup.cfg
+-rw-r--r--   0 wangtong   (501) staff       (20)     1030 2023-05-27 12:39:21.000000 pyacmi-1.2.4/setup.py
```

### Comparing `pyacmi-1.2.3/LICENSE` & `pyacmi-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacmi-1.2.3/PKG-INFO` & `pyacmi-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.2.3
+Version: 1.2.4
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
@@ -51,15 +51,16 @@
 
 ## Example
 
 ```python
 
 from pyacmi import Acmi
 
-acmi = Acmi('test.acmi')
+acmi = Acmi()
+acmi.load_acmi(filepath='test.acmi')
 print(acmi)
 
 print(acmi.reference_latitude, acmi.reference_longitude, acmi.reference_time)
 
 # 打印所有的object
 for obj_id in acmi.objects:
     obj = acmi.objects[obj_id]
```

### Comparing `pyacmi-1.2.3/README.md` & `pyacmi-1.2.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 
 ## Example
 
 ```python
 
 from pyacmi import Acmi
 
-acmi = Acmi('test.acmi')
+acmi = Acmi()
+acmi.load_acmi(filepath='test.acmi')
 print(acmi)
 
 print(acmi.reference_latitude, acmi.reference_longitude, acmi.reference_time)
 
 # 打印所有的object
 for obj_id in acmi.objects:
     obj = acmi.objects[obj_id]
```

### Comparing `pyacmi-1.2.3/pyacmi/acmi.py` & `pyacmi-1.2.4/pyacmi/acmi.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import bisect
 import json
 import io
 from constantly import ValueConstant
 import csv
 from typing import Union, Optional
 from tqdm import tqdm
+import shutil
 
 ACMI_FILE_ENCODING = 'utf-8-sig'
 
 ACMI_NUMERIC_PROPERTIES = {
     'Importance',
     'Slot',
     'Disabled', 'Visible',
@@ -593,16 +594,16 @@
             line = line.strip()[:-1] + '\n' + self.fh.readline()
 
         return line
 
 
 class Acmi:
 
-    def __init__(self, filepath: str):
-        self.filepath: Optional[str] = filepath
+    def __init__(self):
+        self.filepath: Optional[str] = None
         self.file_version: Optional[str] = None
         self.file_type: Optional[str] = None
 
         # global properties
         self.data_source: Optional[str] = None
         self.data_recorder: Optional[str] = None
         self.reference_time: Optional[str] = None
@@ -621,35 +622,35 @@
         self.category: Optional[str] = None
 
         self.briefing: Optional[str] = None
         self.debriefing: Optional[str] = None
         self.comments: Optional[str] = None
         self.reference_longitude = 0
         self.reference_latitude = 0
+        self.playback_delay = 0 # 回放文件的延迟时间
 
         self.objects: dict[str, AcmiObject] = { }
         self.timeframes: list[float] = []
+
         # 加载
         # 解析到的object_keys
         self.object_fields: set[str] = { 'ID', 'Name', 'Type', 'Tags' }
 
-        self._parse(filepath=filepath)
-
     @staticmethod
     def parse_obj_id(val: str) -> str:
         # return int(val, 16)
         return val
 
     @staticmethod
     def strptime(val: str):
         if len(val) < 22:
             return datetime.datetime.strptime(val, "%Y-%m-%dT%H:%M:%SZ")
         else:
             return datetime.datetime.strptime(val, "%Y-%m-%dT%H:%M:%S.%fZ")
-    
+
     @staticmethod
     def split_fields(line):
         fields = []
         i = 1
         lastfield = 0
         while i < len(line):
             if line[i - 1] != '\\' and line[i] == ',':
@@ -684,16 +685,29 @@
                 self.category = val
             elif prop == "Briefing":
                 self.briefing = val
             elif prop == "Debriefing":
                 self.debriefing = val
             elif prop == "Comments":
                 self.comments = val
+            elif prop == 'AuthenticationKey':
+                # TODO: 需要整明白这是个啥
+                return
+            elif prop == 'PlaybackDelay':
+                # 指定了回放文件的延迟时间。在这个例子中，PlaybackDelay的值为600.000000，这意味着回放文件将在600秒后开始播放。
+                self.playback_delay = float(val)
+                # TODO: 需要整明白这是个啥
+                return
+            elif prop == 'PlaybackKey':
+                # 回放文件的密钥
+                # TODO: 需要整明白这是个啥
+                return
             else:
-                raise RuntimeError("Unknown global property: " + prop)
+                print("Unknown global property: " + prop)
+                # raise RuntimeError("Unknown global property: " + prop)
 
     # 解析Object Property
     def _parse_object_property(self, obj_id: str, timeframe: float, fields):
         if obj_id not in self.objects:
             self.objects[obj_id] = AcmiObject(obj_id)
 
         obj = self.objects[obj_id]
@@ -760,19 +774,20 @@
                 obj.set_value(prop, timeframe, val)
             elif prop in ACMI_TEXT_PROPERTIES:
                 obj.set_value(prop, timeframe, val)
             elif prop in ACMI_NUMERIC_PROPERTIES:
                 obj.set_value(prop, timeframe, float(val))
             else:
                 obj.set_value(prop, timeframe, val)
-                print("Unknown property:", prop)
+                print("Unknown Object property:", prop)
 
             self.object_fields.add(prop)
 
-    def _parse(self, filepath: str):
+    def load_acmi(self, filepath: str):
+        self.filepath = filepath
 
         def do_parse(f):
             ar = AcmiFileReader(f)
             rawline = next(ar)
             if rawline.startswith('FileType='):
                 self.file_type = rawline[len('FileType='):].strip()
             else:
@@ -791,15 +806,18 @@
             for rawline in ar:
                 linenr += 1
                 line = rawline.strip()  # type: str
                 if not line or line.startswith('//'):
                     continue  # ignore comments
 
                 if line.startswith('#'):
-                    cur_reftime = float(line[1:])
+                    try:
+                        cur_reftime = float(line[1:])
+                    except Exception as e:
+                        continue
                     self.timeframes.append(cur_reftime)
                     continue
 
                 if line.startswith('-'):
                     obj_id = self.parse_obj_id(line[1:])
                     self.objects[obj_id].removed_at = cur_reftime
                 else:
@@ -913,7 +931,30 @@
                         else:
                             line.append(obj.get_value(field=field, time=t))
                     lines.append(line)
                     if len(lines) > 1000:
                         writer.writerows(lines)
                         lines = []
             writer.writerows(lines)
+
+    # 导出acmi
+    def export_acmi(self, filepath: str):
+        pass
+
+
+# 解压缩acmi到指定目录，如果该acmi不是压缩文件，则复制到指定目录里
+def extract_acmi(filepath: str, to_dir: str):
+    if zipfile.is_zipfile(filepath):
+        with zipfile.ZipFile(filepath, 'r') as zip_ref:
+            zip_ref.extractall(to_dir)
+    else:
+        shutil.copy(filepath, to_dir)
+
+
+# 解压缩文件夹
+def extract_acmi_dir(from_dir: str, to_dir: str):
+    for root, dirs, files in os.walk(from_dir):
+        for file in files:
+            if file.endswith('.acmi') or file.endswith('.zip'):
+                filepath = os.path.join(root, file)
+                print(f'Extract {filepath}')
+                extract_acmi(filepath, to_dir)
```

### Comparing `pyacmi-1.2.3/pyacmi.egg-info/PKG-INFO` & `pyacmi-1.2.4/pyacmi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.2.3
+Version: 1.2.4
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
@@ -51,15 +51,16 @@
 
 ## Example
 
 ```python
 
 from pyacmi import Acmi
 
-acmi = Acmi('test.acmi')
+acmi = Acmi()
+acmi.load_acmi(filepath='test.acmi')
 print(acmi)
 
 print(acmi.reference_latitude, acmi.reference_longitude, acmi.reference_time)
 
 # 打印所有的object
 for obj_id in acmi.objects:
     obj = acmi.objects[obj_id]
```

### Comparing `pyacmi-1.2.3/setup.py` & `pyacmi-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
         name="pyacmi",
-        version='1.2.3',
+        version='1.2.4',
         description="ACMI flight record file parser",
         long_description=long_description,
         long_description_content_type='text/markdown',
         url='https://github.com/wangtong2015/pyacmi',
         author="Wang Tong",
         author_email="astroboythu@gmail.com",
         license="MIT",
```

