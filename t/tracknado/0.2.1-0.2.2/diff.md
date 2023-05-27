# Comparing `tmp/tracknado-0.2.1.tar.gz` & `tmp/tracknado-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracknado-0.2.1.tar", last modified: Fri May 12 14:46:09 2023, max compression
+gzip compressed data, was "tracknado-0.2.2.tar", last modified: Sat May 27 19:24:33 2023, max compression
```

## Comparing `tracknado-0.2.1.tar` & `tracknado-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:46:09.280572 tracknado-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:46:09.280572 tracknado-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:46:09.280572 tracknado-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-12 14:45:57.000000 tracknado-0.2.1/.github/workflows/python-publish.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-05-12 14:45:57.000000 tracknado-0.2.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-12 14:45:57.000000 tracknado-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-12 14:46:09.280572 tracknado-0.2.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2422 2023-05-12 14:45:57.000000 tracknado-0.2.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-05-12 14:45:57.000000 tracknado-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 14:46:09.280572 tracknado-0.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-12 14:45:57.000000 tracknado-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:46:09.280572 tracknado-0.2.1/tracknado/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    28022 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:46:09.280572 tracknado-0.2.1/tracknado/old/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3967 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/old/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6644 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/old/grouping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/old/hub_setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6442 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/old/make_hub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2356 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/old/track.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:46:09.280572 tracknado-0.2.1/tracknado.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:24:33.143016 tracknado-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:24:33.139016 tracknado-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:24:33.139016 tracknado-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-27 19:24:18.000000 tracknado-0.2.2/.github/workflows/python-publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-05-27 19:24:18.000000 tracknado-0.2.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-27 19:24:18.000000 tracknado-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-27 19:24:33.143016 tracknado-0.2.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2422 2023-05-27 19:24:18.000000 tracknado-0.2.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-05-27 19:24:18.000000 tracknado-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 19:24:33.143016 tracknado-0.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-27 19:24:18.000000 tracknado-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:24:33.143016 tracknado-0.2.2/tracknado/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-27 19:24:32.000000 tracknado-0.2.2/tracknado/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:24:33.143016 tracknado-0.2.2/tracknado/old/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3967 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/old/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6644 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/old/grouping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/old/hub_setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6442 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/old/make_hub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2356 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/old/track.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:24:33.143016 tracknado-0.2.2/tracknado.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-27 19:24:33.000000 tracknado-0.2.2/tracknado.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-27 19:24:33.000000 tracknado-0.2.2/tracknado.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 19:24:33.000000 tracknado-0.2.2/tracknado.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 19:24:33.000000 tracknado-0.2.2/tracknado.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-27 19:24:33.000000 tracknado-0.2.2/tracknado.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 19:24:33.000000 tracknado-0.2.2/tracknado.egg-info/top_level.txt
```

### Comparing `tracknado-0.2.1/.github/workflows/python-publish.yml` & `tracknado-0.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.1/LICENSE` & `tracknado-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.1/PKG-INFO` & `tracknado-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracknado
-Version: 0.2.1
+Version: 0.2.2
 Summary: CLI library to generate UCSC trackhubs from sequencing data
 Author-email: Alastair Smith <alastair.smith@ndcls.ox.ac.uk>
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tracknado-0.2.1/README.md` & `tracknado-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.1/pyproject.toml` & `tracknado-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.1/tracknado/api.py` & `tracknado-0.2.2/tracknado/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -403,23 +403,24 @@
 
             self.details["supertrack"] = get_hash_for_df(self.details, self._supertrack_columns)
     
     def _get_composite_tracks(self) -> Dict[str, trackhub.CompositeTrack]:
         """Generate a dictionary of CompositeTracks from the details dataframe"""
 
         composite_tracks = dict()
-        if "supertrack" in self.details.columns:
-            for (supertrack, ext) , df in self.details.groupby(["supertrack", "ext"]):
-                
-                dimensions = dict(
+        dimensions = dict(
                     zip(
                         [f"dim{d}" for d in ["X", "Y", "A", "B", "C", "D"]],
                         self._subgroup_columns,
                     )
                 )
+        
+        if "supertrack" in self.details.columns:
+            for (supertrack, ext) , df in self.details.groupby(["supertrack", "ext"]):
+                
 
                 supertrack_name = self.super_tracks[supertrack].name
                 composite_name = "_".join([supertrack_name, ext])
 
 
                 composite = trackhub.CompositeTrack(
                     name=composite_name,
@@ -442,16 +443,21 @@
             for ext, df in self.details.groupby("ext"):
                 composite = trackhub.CompositeTrack(
                     name=ext,
                     tracktype=ext,
                     visibility="hide",
                     dragAndDrop="subTracks",
                     allButtonPair="off",
+                    dimensions=" ".join([f"{k}={v}" for k, v in dimensions.items()])
+                    if dimensions
+                    else None,
+                    sortOrder=" ".join([f"{k}=+" for k in self._subgroup_columns]),
                 )
 
+                composite.add_subgroups(self.subgroup_definitions)
                 composite_tracks[get_hash((ext,))] = composite
         
         else:
             composite_tracks = dict()
 
         return composite_tracks
 
@@ -611,35 +617,40 @@
         self._add_tracks_to_hub()
 
     def _add_tracks_to_hub(self) -> None:
         # Loop through each entry in the details dataframe
         
         for row in self.track_design.details.itertuples():
 
+            has_composite = False
+            has_overlay = False
+
             # If the row has a "composite" attribute
             if hasattr(row, "composite"):
+                has_composite = True
                 composite_track = self.track_design.composite_tracks[row.composite]
                 # Create a new track and add it as a subtrack to the composite track
                 track = self._get_track(row, suffix=f"_{composite_track.name}")
                 composite_track.add_subtrack(track)
 
             # If the row has an "overlay" attribute
             if hasattr(row, "overlay"):
+                has_overlay = True
                 overlay_track = self.track_design.overlay_tracks[row.overlay]
                 # Create a new track and add it to the overlay track
                 track = self._get_track(row, suffix=f"_{overlay_track.name}")
 
                 # Ignore the track if it is not a signal track e.g. bigWig
                 if track.tracktype not in ["bigWig", ]:
                     logger.warning(f"Track {track.name} is not a signal track and will be ignored for the overlay track {overlay_track.name}")
                 else:
                     overlay_track.add_subtrack(track)
 
             # If the row doesn't have a "supertrack" attribute
-            if not hasattr(row, "supertrack"):
+            if not hasattr(row, "supertrack") and not has_composite and not has_overlay:
                 # Create a new track and add it to the trackdb
                 track = self._get_track(row)
                 self.trackdb.add_tracks(track)
 
         # Add the supertracks or composite/overlay tracks to the trackdb
         if self.track_design.super_tracks:
             tracks = self.track_design.super_tracks.values()
@@ -649,15 +660,15 @@
                 for t in [*self.track_design.composite_tracks.values(), *self.track_design.overlay_tracks.values()]:
                     t.add_params(group=self._hub.hub)
 
         else:
             tracks = [*self.track_design.composite_tracks.values(), *self.track_design.overlay_tracks.values()]
 
         # Add the composite/overlay and supertracks to the trackdb
-        for track in tracks:
+        for ii, track in enumerate(tracks):
             # Add group if custom genome
             if self.custom_genome:
                 track.add_params(group=self._hub.hub)
             self.trackdb.add_tracks(track)
```

### Comparing `tracknado-0.2.1/tracknado/cli.py` & `tracknado-0.2.2/tracknado/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 @click.option(
     "--overlay-by",
     help="Column(s) defining overlay tracks",
     multiple=True,
     default=None,
 )
 @click.option(
-    "--convert",
+    "--convert-files",
     help="Convert files to UCSC compatible format",
     is_flag=True,
     default=False,
 )
 @click.option(
     "--chrom-sizes",
     help="Path to chrom.sizes file",
@@ -188,15 +188,15 @@
 
     --supergroup-by sample --subgroup-by antibody --composite-by replicate
 
     The --color-by option can be used to specify a column in the design file that will be used to
     assign colors to the tracks. The colors will be assigned in the order that the values appear in
     the column unless colors are specified in the design file using the 'color' column.
 
-    The --convert option can be used to convert the input files to UCSC compatible format. This
+    The --convert-files option can be used to convert the input files to UCSC compatible format. This
     option is only available for bed files at this time. The files will be converted in the current
     working directory and the converted files will be used to generate the hub. The original files
     will be left in place.
 
     A custom genome can be specified using the --custom-genome option. This option requires that
     the --genome-twobit and --genome-organism options are also provided.
```

### Comparing `tracknado-0.2.1/tracknado/old/cli.py` & `tracknado-0.2.2/tracknado/old/cli.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.1/tracknado/old/grouping.py` & `tracknado-0.2.2/tracknado/old/grouping.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.1/tracknado/old/hub_setup.py` & `tracknado-0.2.2/tracknado/old/hub_setup.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.1/tracknado/old/make_hub.py` & `tracknado-0.2.2/tracknado/old/make_hub.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.1/tracknado/old/track.py` & `tracknado-0.2.2/tracknado/old/track.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.1/tracknado/utils.py` & `tracknado-0.2.2/tracknado/utils.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.1/tracknado.egg-info/PKG-INFO` & `tracknado-0.2.2/tracknado.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracknado
-Version: 0.2.1
+Version: 0.2.2
 Summary: CLI library to generate UCSC trackhubs from sequencing data
 Author-email: Alastair Smith <alastair.smith@ndcls.ox.ac.uk>
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

