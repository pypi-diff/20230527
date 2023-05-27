# Comparing `tmp/optimal_loc-0.0.8.tar.gz` & `tmp/optimal_loc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.0.8.tar", max compression
+gzip compressed data, was "optimal_loc-0.0.9.tar", max compression
```

## Comparing `optimal_loc-0.0.8.tar` & `optimal_loc-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.0.8/LICENSE
--rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.0.8/README.md
--rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.0.8/optimal_loc/Modelling Algorithm.png
--rw-r--r--   0        0        0       95 2023-05-27 14:12:04.391034 optimal_loc-0.0.8/optimal_loc/__init__.py
--rw-r--r--   0        0        0      406 2023-05-27 13:51:08.122984 optimal_loc-0.0.8/optimal_loc/bash_command.py
--rw-r--r--   0        0        0      731 2023-05-26 02:09:22.791228 optimal_loc-0.0.8/optimal_loc/constants.py
--rw-r--r--   0        0        0    18081 2023-05-27 14:11:40.389076 optimal_loc-0.0.8/optimal_loc/optimal_loc.py
--rw-r--r--   0        0        0     2688 2023-05-27 13:51:08.119920 optimal_loc-0.0.8/optimal_loc/st_app.py
--rw-r--r--   0        0        0      857 2023-05-27 14:12:12.882456 optimal_loc-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.0.9/LICENSE
+-rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.0.9/README.md
+-rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.0.9/optimal_loc/Modelling Algorithm.png
+-rw-r--r--   0        0        0       95 2023-05-27 15:08:53.367902 optimal_loc-0.0.9/optimal_loc/__init__.py
+-rw-r--r--   0        0        0      406 2023-05-27 13:51:08.122984 optimal_loc-0.0.9/optimal_loc/bash_command.py
+-rw-r--r--   0        0        0      731 2023-05-26 02:09:22.791228 optimal_loc-0.0.9/optimal_loc/constants.py
+-rw-r--r--   0        0        0    18111 2023-05-27 14:15:21.582817 optimal_loc-0.0.9/optimal_loc/optimal_loc.py
+-rw-r--r--   0        0        0     2688 2023-05-27 13:51:08.119920 optimal_loc-0.0.9/optimal_loc/st_app.py
+-rw-r--r--   0        0        0      857 2023-05-27 15:08:53.370265 optimal_loc-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.0.9/PKG-INFO
```

### Comparing `optimal_loc-0.0.8/LICENSE` & `optimal_loc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.8/README.md` & `optimal_loc-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.8/optimal_loc/Modelling Algorithm.png` & `optimal_loc-0.0.9/optimal_loc/Modelling Algorithm.png`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.8/optimal_loc/constants.py` & `optimal_loc-0.0.9/optimal_loc/constants.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.8/optimal_loc/optimal_loc.py` & `optimal_loc-0.0.9/optimal_loc/optimal_loc.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             hexagon_ids[[HEXAGON, HEX_LAT, HEX_LON]],
             left_on=TOHEX,
             right_on=HEXAGON,
             how="left").drop(columns=[HEXAGON]).rename(columns={HEX_LON: "tohex_lon", HEX_LAT: 'tohex_lat'})
 
         # Average distance between two random points within a circle according to its diameter = (2 * radius) / 3
         eq_hex_distance = int((edge_length(self.resolution, "m") * 2) / 3)
-        hex_distance_data.apply(lambda x: eq_hex_distance if x[FROMHEX] == x[TOHEX] else nan, 1)
+        hex_distance_data[DISTANCE] = hex_distance_data.apply(lambda x: eq_hex_distance if x[FROMHEX] == x[TOHEX] else nan, 1)
 
         self.hex_distance_data = hex_distance_data
 
         print("Distance data for each hexagons was created. You can read it by object_name.hex_distance_data")
 
     def read_distances_from_mongodb(self, mongo_client: MongoClient,
                                     mongo_database_name: str,
```

### Comparing `optimal_loc-0.0.8/optimal_loc/st_app.py` & `optimal_loc-0.0.9/optimal_loc/st_app.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.8/pyproject.toml` & `optimal_loc-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.0.8"
+version = "0.0.9"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
```

### Comparing `optimal_loc-0.0.8/PKG-INFO` & `optimal_loc-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimal-loc
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs.
 Home-page: https://github.com/sinan-demirhan/optimal-loc
 License: MIT
 Keywords: optimalLoc,optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
 Author: Sinan Demirhan
 Author-email: sdemirhan1320@gmail.com
 Requires-Python: >=3.7,<4.0
```

