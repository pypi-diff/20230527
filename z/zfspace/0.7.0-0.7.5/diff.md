# Comparing `tmp/zfspace-0.7.0-py3-none-any.whl.zip` & `tmp/zfspace-0.7.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 13230 bytes, number of entries: 8
+Zip file size: 13360 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      149 b- defN 20-Feb-02 00:00 zfspace/__init__.py
 -rwxr-xr-x  2.0 unx       57 b- defN 20-Feb-02 00:00 zfspace/__main__.py
--rwxr-xr-x  2.0 unx    22778 b- defN 20-Feb-02 00:00 zfspace/zfspace.py
-?rw-r--r--  2.0 unx     3170 b- defN 20-Feb-02 00:00 zfspace-0.7.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       83 b- defN 20-Feb-02 00:00 zfspace-0.7.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx       41 b- defN 20-Feb-02 00:00 zfspace-0.7.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     7048 b- defN 20-Feb-02 00:00 zfspace-0.7.0.dist-info/license_files/LICENSE
-?rw-r--r--  2.0 unx      628 b- defN 20-Feb-02 00:00 zfspace-0.7.0.dist-info/RECORD
-8 files, 33954 bytes uncompressed, 12136 bytes compressed:  64.3%
+-rwxr-xr-x  2.0 unx    23089 b- defN 20-Feb-02 00:00 zfspace/zfspace.py
+?rw-r--r--  2.0 unx     3238 b- defN 20-Feb-02 00:00 zfspace-0.7.5.dist-info/METADATA
+?rw-r--r--  2.0 unx       83 b- defN 20-Feb-02 00:00 zfspace-0.7.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx       41 b- defN 20-Feb-02 00:00 zfspace-0.7.5.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     7048 b- defN 20-Feb-02 00:00 zfspace-0.7.5.dist-info/license_files/LICENSE
+?rw-r--r--  2.0 unx      628 b- defN 20-Feb-02 00:00 zfspace-0.7.5.dist-info/RECORD
+8 files, 34333 bytes uncompressed, 12266 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: zfspace/__main__.py
 Comment: 
 
 Filename: zfspace/zfspace.py
 Comment: 
 
-Filename: zfspace-0.7.0.dist-info/METADATA
+Filename: zfspace-0.7.5.dist-info/METADATA
 Comment: 
 
-Filename: zfspace-0.7.0.dist-info/WHEEL
+Filename: zfspace-0.7.5.dist-info/WHEEL
 Comment: 
 
-Filename: zfspace-0.7.0.dist-info/entry_points.txt
+Filename: zfspace-0.7.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: zfspace-0.7.0.dist-info/license_files/LICENSE
+Filename: zfspace-0.7.5.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: zfspace-0.7.0.dist-info/RECORD
+Filename: zfspace-0.7.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zfspace/__init__.py

```diff
@@ -1,4 +1,4 @@
 from .zfspace import main  # noqa
 
 # Version is updated with bump2version helper. Do not update manually or you will lose sync
-__version__ = '0.7.0'
+__version__ = '0.7.5'
```

## zfspace/zfspace.py

```diff
@@ -13,15 +13,15 @@
 import os
 import math
 import difflib
 import argparse
 import copy
 
 # Version is updated with bump2version helper. Do not update manually or you will lose sync
-__version__ = '0.7.0'
+__version__ = '0.7.5'
 filter_level = 0.368  # This value will be overwritten by default argparse filter value
 
 term_format = dict(PURPLE='\033[95m', CYAN='\033[96m', DARKCYAN='\033[36m', BLUE='\033[94m',
                    GREEN='\033[92m', YELLOW='\033[93m', RED='\033[91m', BOLD='\033[1m',
                    UNDERLINE='\033[4m', WHITEBOLD='\033[1;37m', END='\033[0m')
 
 
@@ -53,16 +53,18 @@
             s = int(round(size_bytes / p))
             return '{} {}'.format(s, size_name[order])
         else:  # Limit accuracy to 1 or 2 fractional decimals to get representations 1.23 and 12.3 and not 12.34
             s = round(size_bytes / p, 2 - digits)
             return '{:.4} {}'.format(s, size_name[order])
 
 
-def split_terminal_line(term_columns, slices=0, fractions_list=list(), padding=0):
+def split_terminal_line(term_columns, slices=0, fractions_list=None, padding=0):
     # Convert slices into fractions_list
+    if fractions_list is None:
+        fractions_list = []
     if len(fractions_list) == 0:
         if slices == 0:
             raise TypeError('At least one parameter must be set. '
                             'Either slices > 0 or fractions_list must be a not empty list.')
         else:
             fractions_list = [1/slices] * slices
     else:
@@ -205,14 +207,24 @@
                 suggest_str = '\nDid you mean using ' + \
                               term_format['WHITEBOLD'] + '"{}"'.format(candidate_list[0]) + term_format['END'] + \
                               ' instead?'
             else:
                 suggest_str = ''
             raise ValueError('There is no dataset "{}" in the system.{}'.format(dataset_name, suggest_str))
 
+    @staticmethod
+    def _zfs_output_convert(line: str):
+        """
+        Takes a line of ZFS output and convert it to a list with name and integer values
+        :param line: ZFS console output
+        :return: list starting with a string and followed by integers with data from input line
+        """
+        lst = list(filter(None, line.split(' ')))
+        return [lst[0], *list(map(int, lst[1:]))]  # Convert to integers all but name of the dataset
+
     def get_filesystem_mountpoint(self, dataset_name):
         self._check_dataset_name(dataset_name)
         command = '{} get -Hp mountpoint {}'.format(self.zfs_path, dataset_name)
         stream = os.popen(command)
         output = stream.read().split('\t')[2]
         return output
 
@@ -227,18 +239,17 @@
         self._check_dataset_name(dataset_name)
         command = '{} list -d 1 -p -S used -o space {}'.format(self.zfs_path, dataset_name)
         stream = os.popen(command)
         output = stream.read().split('\n')[:-1]  # Get all lines except the last one, that is empty
         names = list(filter(None, output[0].split(' ')))
         children = list()
         for child in output[1:]:
-            item = list(filter(None, child.split(' ')))
-            if item[0] == dataset_name:  # Filter out the parent
+            data = self._zfs_output_convert(child)
+            if data[0] == dataset_name:  # Filter out the parent
                 continue
-            data = [item[0]] + list(map(int, item[1:]))  # Convert to integers all but name of the dataset
             children.append(list(zip(names, data)))
         return children
 
     def get_snapshot_names(self, dataset_name):
         self._check_dataset_name(dataset_name)
         command = '{} list -H -d 1 -t snapshot -s creation -o name {}'.format(self.zfs_path, dataset_name)
         stream = os.popen(command)
@@ -281,17 +292,16 @@
 
     def get_dataset_summary(self, dataset_name):
         self._check_dataset_name(dataset_name)
         command = '{} list -p -o space {}'.format(self.zfs_path, dataset_name)
         stream = os.popen(command)
         string_list = stream.read().split('\n')[0:2]  # Get names and data strings
         # Split it by spaces and remove empty strings.
-        data = list(filter(None, string_list[1].split(' ')))
         names = list(filter(None, string_list[0].split(' ')))
-        data = [data[0]] + list(map(int, data[1:]))  # Convert to integers all but name
+        data = self._zfs_output_convert(string_list[1])
         return list(zip(names, data))
 
 
 class SnapshotSpace:
     zfs_max_snapshots = 30
 
     def __init__(self, dataset_name):
```

## Comparing `zfspace-0.7.0.dist-info/METADATA` & `zfspace-0.7.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: zfspace
-Version: 0.7.0
+Version: 0.7.5
 Summary: zfspace tool helps to analyze how zfs disk space is used
 Project-URL: Bug Tracker, https://github.com/Zapunidi/zfspace/issues
 Project-URL: Homepage, https://github.com/Zapunidi/zfspace
 Author-email: Sergey Zapunidi <zapunidy@gmail.com>
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Filesystems
-Requires-Python: >=3.4
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # zfspace
 Console tool to find occupied pool space in ZFS on Linux.
 The tool uses pure python3 with shell commands to collect useful information from ZFS 
 and show it in convenient way wit recommendations how to free some space.
+![An example of zfspace console output](./docs/zfspace_example.png)
 
 ## Introduction
 
 ZFS is a non-trivial LVS filesystem with snapshots, reservations, deduplication, filesystems hierarchy and so on. 
 Common tools, such as `df` or `ls` can't provide relevant information when you **need to free some space**.
 There is an [explanatory article](https://zedfs.com/all-you-have-to-know-about-reading-zfs-disk-usage/) about this.
```

## Comparing `zfspace-0.7.0.dist-info/license_files/LICENSE` & `zfspace-0.7.5.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `zfspace-0.7.0.dist-info/RECORD` & `zfspace-0.7.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-zfspace/__init__.py,sha256=6lBB0Ix4KW_ZQbOzxtAWx0T4q4GFFyS4Vbf8hUYeiBk,149
+zfspace/__init__.py,sha256=a32y8TAe86OkuvjeC1gdTQy6tKVf_3QaJCKj-QKZT-M,149
 zfspace/__main__.py,sha256=pizqcondngclefYVhunu7FLoZkPYRwJQukZrn9cK3NM,57
-zfspace/zfspace.py,sha256=q-ZsRy0EkIQpBNK-B3b1n85xGchW0gA4egSGgzEzkmQ,22778
-zfspace-0.7.0.dist-info/METADATA,sha256=DJlJsmWklHdrgvAxWHp-VGu6w3QkaVP9f7io4_ZhspY,3170
-zfspace-0.7.0.dist-info/WHEEL,sha256=sb4ZHsmozXdkdXRvpMHZmhxsxQvL8DERDUEGA9tAfc8,83
-zfspace-0.7.0.dist-info/entry_points.txt,sha256=ldVd8NxpptS21EvnYrC8Xy2VTHvwjFiz74fTtJdjKog,41
-zfspace-0.7.0.dist-info/license_files/LICENSE,sha256=ogEPNDSH0_dhiv_lT3ifVIdgIzHAqNA_SemnxUfPBJk,7048
-zfspace-0.7.0.dist-info/RECORD,,
+zfspace/zfspace.py,sha256=vsxeWe7UyJxkooUTdUaVpS6tBnCvR9Qw8CrNbaQJDsk,23089
+zfspace-0.7.5.dist-info/METADATA,sha256=dcE0CVKGNlfNVk_NefSkpGFoR1HixZpubMVWsmbo5HQ,3238
+zfspace-0.7.5.dist-info/WHEEL,sha256=sb4ZHsmozXdkdXRvpMHZmhxsxQvL8DERDUEGA9tAfc8,83
+zfspace-0.7.5.dist-info/entry_points.txt,sha256=ldVd8NxpptS21EvnYrC8Xy2VTHvwjFiz74fTtJdjKog,41
+zfspace-0.7.5.dist-info/license_files/LICENSE,sha256=ogEPNDSH0_dhiv_lT3ifVIdgIzHAqNA_SemnxUfPBJk,7048
+zfspace-0.7.5.dist-info/RECORD,,
```

