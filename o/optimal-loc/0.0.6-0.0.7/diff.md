# Comparing `tmp/optimal_loc-0.0.6.tar.gz` & `tmp/optimal_loc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.0.6.tar", max compression
+gzip compressed data, was "optimal_loc-0.0.7.tar", max compression
```

## Comparing `optimal_loc-0.0.6.tar` & `optimal_loc-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.0.6/LICENSE
--rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.0.6/README.md
--rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.0.6/optimal_loc/Modelling Algorithm.png
--rw-r--r--   0        0        0       95 2023-05-07 15:11:13.940841 optimal_loc-0.0.6/optimal_loc/__init__.py
--rw-r--r--   0        0        0      399 2023-05-07 14:57:38.361508 optimal_loc-0.0.6/optimal_loc/bash_command.py
--rw-r--r--   0        0        0     9523 2023-05-07 15:00:25.950207 optimal_loc-0.0.6/optimal_loc/optimal_loc.py
--rw-r--r--   0        0        0     2740 2023-05-07 15:10:45.385177 optimal_loc-0.0.6/optimal_loc/st_app.py
--rw-r--r--   0        0        0      857 2023-05-07 15:11:06.844992 optimal_loc-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.0.7/LICENSE
+-rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.0.7/README.md
+-rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.0.7/optimal_loc/Modelling Algorithm.png
+-rw-r--r--   0        0        0       95 2023-05-27 13:34:30.584293 optimal_loc-0.0.7/optimal_loc/__init__.py
+-rw-r--r--   0        0        0      394 2023-05-26 01:21:37.073056 optimal_loc-0.0.7/optimal_loc/bash_command.py
+-rw-r--r--   0        0        0      731 2023-05-26 02:09:22.791228 optimal_loc-0.0.7/optimal_loc/constants.py
+-rw-r--r--   0        0        0    17723 2023-05-27 13:32:38.515388 optimal_loc-0.0.7/optimal_loc/optimal_loc.py
+-rw-r--r--   0        0        0     2676 2023-05-26 02:04:57.726729 optimal_loc-0.0.7/optimal_loc/st_app.py
+-rw-r--r--   0        0        0      857 2023-05-27 13:34:49.613069 optimal_loc-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.0.7/PKG-INFO
```

### Comparing `optimal_loc-0.0.6/LICENSE` & `optimal_loc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.6/README.md` & `optimal_loc-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.6/optimal_loc/Modelling Algorithm.png` & `optimal_loc-0.0.7/optimal_loc/Modelling Algorithm.png`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.6/optimal_loc/st_app.py` & `optimal_loc-0.0.7/optimal_loc/st_app.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,32 +2,22 @@
 import streamlit as st
 from pandas import DataFrame
 from streamlit_folium import folium_static
 from pickle import load as pickle_load
 from folium import plugins, Map, CircleMarker, Marker, Icon
 from PIL import Image
 
+from constants import COLOURS_LIST, FILENAME, OPTIMAL_DATA_COLUMN, SUPPLY_DATA_COLUMN, HEX_LAT, HEX_LON
+
 
 PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
 my_algorithm = Image.open(os.path.join(PACKAGE_DIR, 'Modelling Algorithm.png'))
 
 st.set_page_config(layout="wide")
 
-my_colours = [
-    'darkred',
-    'orange',
-    'darkgreen',
-    'darkblue',
-    'purple',
-    'lightgreen',
-    'pink',
-    'lightblue',
-    'black'
-]
-
 
 @st.cache_data
 def read_data(my_json):
     with open(my_json, 'rb') as handle:
         output_distances = pickle_load(handle)
     return output_distances
 
@@ -35,21 +25,21 @@
 st.sidebar.text('')
 st.sidebar.text('')
 st.sidebar.text('')
 
 ### SEASON RANGE ###
 st.sidebar.markdown("**First select the station number you want to analyze:** 👇")
 
-analysis_result = read_data("optimal_locations.pickle")
+analysis_result = read_data(FILENAME)
 
-optimal_data = DataFrame(analysis_result["optimal_data"])
-supply_data = DataFrame(analysis_result["supply_data"])
+optimal_data = DataFrame(analysis_result[OPTIMAL_DATA_COLUMN])
+supply_data = DataFrame(analysis_result[SUPPLY_DATA_COLUMN])
 
 optimal_data["supply_group"] = optimal_data.groupby(['supply_hexagon_id']).ngroup()
-optimal_data["my_colours"] = optimal_data["supply_group"].apply(lambda x: my_colours[x % (len(my_colours))])
+optimal_data["my_colours"] = optimal_data["supply_group"].apply(lambda x: COLOURS_LIST[x % (len(COLOURS_LIST))])
 
 st.sidebar.text('')
 agree = st.sidebar.checkbox('Show Model Algorithm')
 st.sidebar.text('')
 st.sidebar.text('')
 st.sidebar.write("[MODELLING CODE](https://sinan-demirhan.github.io/ALL-PROJECTS/Projects/BOSTON%20OPTIMIZATION.html)")
 st.sidebar.text('')
@@ -64,24 +54,24 @@
 #  )
 
 
 def plotting_main_map(optimization_data: DataFrame,
                       optimal_loc_data: DataFrame
                       ):
 
-    plot_center = [optimization_data["hex_lat"].median(), optimization_data["hex_lon"].median()]
+    plot_center = [optimization_data[HEX_LAT].median(), optimization_data[HEX_LON].median()]
     my_map = Map(location=plot_center, zoom_start=12)
 
     for j, i in optimal_data.iterrows():
-        CircleMarker([i["hex_lat"], i["hex_lon"]],
+        CircleMarker([i[HEX_LAT], i[HEX_LON]],
                      radius=5,
                      color=i["my_colours"]).add_to(my_map)
 
     for j, i in optimal_loc_data.iterrows():
-        Marker([i["hex_lat"], i["hex_lon"]], radius=5,
+        Marker([i[HEX_LAT], i[HEX_LON]], radius=5,
                icon=Icon(color='red', icon='info-sign')).add_to(my_map)
 
     plugins.Fullscreen(position='topleft').add_to(my_map)
 
     return my_map
```

### Comparing `optimal_loc-0.0.6/pyproject.toml` & `optimal_loc-0.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.0.6"
+version = "0.0.7"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
```

### Comparing `optimal_loc-0.0.6/PKG-INFO` & `optimal_loc-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimal-loc
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs.
 Home-page: https://github.com/sinan-demirhan/optimal-loc
 License: MIT
 Keywords: optimalLoc,optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
 Author: Sinan Demirhan
 Author-email: sdemirhan1320@gmail.com
 Requires-Python: >=3.7,<4.0
```

