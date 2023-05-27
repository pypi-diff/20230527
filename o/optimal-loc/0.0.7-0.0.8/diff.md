# Comparing `tmp/optimal_loc-0.0.7.tar.gz` & `tmp/optimal_loc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.0.7.tar", max compression
+gzip compressed data, was "optimal_loc-0.0.8.tar", max compression
```

## Comparing `optimal_loc-0.0.7.tar` & `optimal_loc-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.0.7/LICENSE
--rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.0.7/README.md
--rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.0.7/optimal_loc/Modelling Algorithm.png
--rw-r--r--   0        0        0       95 2023-05-27 13:34:30.584293 optimal_loc-0.0.7/optimal_loc/__init__.py
--rw-r--r--   0        0        0      394 2023-05-26 01:21:37.073056 optimal_loc-0.0.7/optimal_loc/bash_command.py
--rw-r--r--   0        0        0      731 2023-05-26 02:09:22.791228 optimal_loc-0.0.7/optimal_loc/constants.py
--rw-r--r--   0        0        0    17723 2023-05-27 13:32:38.515388 optimal_loc-0.0.7/optimal_loc/optimal_loc.py
--rw-r--r--   0        0        0     2676 2023-05-26 02:04:57.726729 optimal_loc-0.0.7/optimal_loc/st_app.py
--rw-r--r--   0        0        0      857 2023-05-27 13:34:49.613069 optimal_loc-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.0.8/LICENSE
+-rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.0.8/README.md
+-rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.0.8/optimal_loc/Modelling Algorithm.png
+-rw-r--r--   0        0        0       95 2023-05-27 14:12:04.391034 optimal_loc-0.0.8/optimal_loc/__init__.py
+-rw-r--r--   0        0        0      406 2023-05-27 13:51:08.122984 optimal_loc-0.0.8/optimal_loc/bash_command.py
+-rw-r--r--   0        0        0      731 2023-05-26 02:09:22.791228 optimal_loc-0.0.8/optimal_loc/constants.py
+-rw-r--r--   0        0        0    18081 2023-05-27 14:11:40.389076 optimal_loc-0.0.8/optimal_loc/optimal_loc.py
+-rw-r--r--   0        0        0     2688 2023-05-27 13:51:08.119920 optimal_loc-0.0.8/optimal_loc/st_app.py
+-rw-r--r--   0        0        0      857 2023-05-27 14:12:12.882456 optimal_loc-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.0.8/PKG-INFO
```

### Comparing `optimal_loc-0.0.7/LICENSE` & `optimal_loc-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.7/README.md` & `optimal_loc-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.7/optimal_loc/Modelling Algorithm.png` & `optimal_loc-0.0.8/optimal_loc/Modelling Algorithm.png`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.7/optimal_loc/constants.py` & `optimal_loc-0.0.8/optimal_loc/constants.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.7/optimal_loc/optimal_loc.py` & `optimal_loc-0.0.8/optimal_loc/optimal_loc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from numpy import array, meshgrid
+from numpy import array, meshgrid, nan
 from pandas import DataFrame, pivot_table
 from pymongo.mongo_client import MongoClient
-from h3 import geo_to_h3, h3_to_geo
+from h3 import geo_to_h3, h3_to_geo, edge_length
 import pickle
 from pulp import LpProblem, LpMinimize, LpVariable, lpSum, PULP_CBC_CMD
 
-from constants import (
+from optimal_loc.constants import (
     HEX_LAT, FROMHEX, TOHEX, HEX_LOCATION, SUPPLY_HEXAGON_ID, TOTAL_EVENT, HEX_ID, HEX_LON, HEXAGON_ID, LATITUDE,
     LONGITUDE, FROMHEX_LAT, FROMHEX_LON, HEXAGON, FILENAME, DISTANCE, SUPPLY_DATA_COLUMN, OPTIMAL_DATA_COLUMN, INDEX
 )
 
 
 def set_resolution(raw_data: DataFrame, hex_size: str):
     if hex_size == 'medium':
@@ -31,14 +31,15 @@
 
 class OptimalLoc:
     def __init__(self):
         self.supply_data = None
         self.optimal_data = None
         self.hex_distance_data = None
         self.event_frequency_data = None
+        self.resolution = None
 
     def event_frequency(self, raw_data: DataFrame, hex_size: str = 'auto') -> None:
         """
         Calculate the frequency of events in each hexagonal region.
 
         Parameters:
         raw_data (DataFrame): pandas DataFrame containing event data, with columns "latitude" and "longitude".
@@ -59,17 +60,17 @@
         Example:
         raw_event_data = pd.DataFrame({'latitude': [42.123, 42.456, 42.789], 'longitude': [-71.123, -71.456, -71.789]})
         object_name = OptimalLoc()
         object_name.event_frequency(raw_event_data)
         event_freq_data = object_name.event_frequency_data
         print(event_freq_data)
         """
-        resolution = set_resolution(raw_data, hex_size)
+        self.resolution = set_resolution(raw_data, hex_size)
 
-        raw_data[HEX_ID] = raw_data.apply(lambda x: geo_to_h3(x[LATITUDE], x[LONGITUDE], resolution), 1)
+        raw_data[HEX_ID] = raw_data.apply(lambda x: geo_to_h3(x[LATITUDE], x[LONGITUDE], self.resolution), 1)
 
         raw_data = raw_data[HEX_ID].value_counts().reset_index().rename(columns={INDEX: HEXAGON_ID,
                                                                                  HEX_ID: TOTAL_EVENT})
         raw_data[HEX_LOCATION] = raw_data.apply(lambda x: h3_to_geo(h=x[HEXAGON_ID]), 1)
         raw_data[HEX_LAT] = raw_data.apply(lambda x: x[HEX_LOCATION][0], 1)
         raw_data[HEX_LON] = raw_data.apply(lambda x: x[HEX_LOCATION][1], 1)
         raw_data = raw_data.drop(columns=HEX_LOCATION)
@@ -121,14 +122,18 @@
 
         hex_distance_data = hex_distance_data.merge(
             hexagon_ids[[HEXAGON, HEX_LAT, HEX_LON]],
             left_on=TOHEX,
             right_on=HEXAGON,
             how="left").drop(columns=[HEXAGON]).rename(columns={HEX_LON: "tohex_lon", HEX_LAT: 'tohex_lat'})
 
+        # Average distance between two random points within a circle according to its diameter = (2 * radius) / 3
+        eq_hex_distance = int((edge_length(self.resolution, "m") * 2) / 3)
+        hex_distance_data.apply(lambda x: eq_hex_distance if x[FROMHEX] == x[TOHEX] else nan, 1)
+
         self.hex_distance_data = hex_distance_data
 
         print("Distance data for each hexagons was created. You can read it by object_name.hex_distance_data")
 
     def read_distances_from_mongodb(self, mongo_client: MongoClient,
                                     mongo_database_name: str,
                                     mongo_collection_name: str):
```

### Comparing `optimal_loc-0.0.7/optimal_loc/st_app.py` & `optimal_loc-0.0.8/optimal_loc/st_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import streamlit as st
 from pandas import DataFrame
 from streamlit_folium import folium_static
 from pickle import load as pickle_load
 from folium import plugins, Map, CircleMarker, Marker, Icon
 from PIL import Image
 
-from constants import COLOURS_LIST, FILENAME, OPTIMAL_DATA_COLUMN, SUPPLY_DATA_COLUMN, HEX_LAT, HEX_LON
+from optimal_loc.constants import COLOURS_LIST, FILENAME, OPTIMAL_DATA_COLUMN, SUPPLY_DATA_COLUMN, HEX_LAT, HEX_LON
 
 
 PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
 my_algorithm = Image.open(os.path.join(PACKAGE_DIR, 'Modelling Algorithm.png'))
 
 st.set_page_config(layout="wide")
```

### Comparing `optimal_loc-0.0.7/pyproject.toml` & `optimal_loc-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.0.7"
+version = "0.0.8"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
```

### Comparing `optimal_loc-0.0.7/PKG-INFO` & `optimal_loc-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimal-loc
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs.
 Home-page: https://github.com/sinan-demirhan/optimal-loc
 License: MIT
 Keywords: optimalLoc,optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
 Author: Sinan Demirhan
 Author-email: sdemirhan1320@gmail.com
 Requires-Python: >=3.7,<4.0
```

