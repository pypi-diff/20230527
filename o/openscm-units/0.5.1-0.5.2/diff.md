# Comparing `tmp/openscm-units-0.5.1.tar.gz` & `tmp/openscm-units-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openscm-units-0.5.1.tar", last modified: Fri Apr 28 07:48:13 2023, max compression
+gzip compressed data, was "openscm-units-0.5.2.tar", last modified: Sat May 27 03:04:06 2023, max compression
```

## Comparing `openscm-units-0.5.1.tar` & `openscm-units-0.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 znicholls (1461210280) 2094513965        0 2023-04-28 07:48:13.898023 openscm-units-0.5.1/
--rw-r--r--   0 znicholls (1461210280) 2094513965     3805 2023-04-28 07:36:36.000000 openscm-units-0.5.1/CHANGELOG.rst
--rw-r--r--   0 znicholls (1461210280) 2094513965     1552 2021-07-27 07:27:26.000000 openscm-units-0.5.1/LICENSE
--rw-r--r--   0 znicholls (1461210280) 2094513965      118 2021-09-07 00:01:10.000000 openscm-units-0.5.1/MANIFEST.in
--rw-r--r--   0 znicholls (1461210280) 2094513965     1382 2023-04-28 07:48:13.898436 openscm-units-0.5.1/PKG-INFO
--rw-r--r--   0 znicholls (1461210280) 2094513965     3872 2021-07-27 07:27:26.000000 openscm-units-0.5.1/README.rst
--rw-r--r--   0 znicholls (1461210280) 2094513965      925 2023-04-28 07:48:13.900656 openscm-units-0.5.1/setup.cfg
--rw-r--r--   0 znicholls (1461210280) 2094513965     3501 2022-05-24 17:23:48.000000 openscm-units-0.5.1/setup.py
-drwxr-xr-x   0 znicholls (1461210280) 2094513965        0 2023-04-28 07:48:13.877330 openscm-units-0.5.1/src/
-drwxr-xr-x   0 znicholls (1461210280) 2094513965        0 2023-04-28 07:48:13.901697 openscm-units-0.5.1/src/openscm_units/
--rw-r--r--   0 znicholls (1461210280) 2094513965      233 2021-07-27 07:27:26.000000 openscm-units-0.5.1/src/openscm_units/__init__.py
--rw-r--r--   0 znicholls (1461210280) 2094513965    20654 2023-04-28 07:36:20.000000 openscm-units-0.5.1/src/openscm_units/_unit_registry.py
--rw-r--r--   0 znicholls (1461210280) 2094513965      497 2023-04-28 07:48:13.901999 openscm-units-0.5.1/src/openscm_units/_version.py
-drwxr-xr-x   0 znicholls (1461210280) 2094513965        0 2023-04-28 07:48:13.896098 openscm-units-0.5.1/src/openscm_units/data/
--rw-r--r--   0 znicholls (1461210280) 2094513965      135 2021-07-27 07:27:26.000000 openscm-units-0.5.1/src/openscm_units/data/__init__.py
--rw-r--r--   0 znicholls (1461210280) 2094513965    14607 2021-07-27 07:27:26.000000 openscm-units-0.5.1/src/openscm_units/data/mixtures.py
-drwxr-xr-x   0 znicholls (1461210280) 2094513965        0 2023-04-28 07:48:13.893654 openscm-units-0.5.1/src/openscm_units.egg-info/
--rw-r--r--   0 znicholls (1461210280) 2094513965     1382 2023-04-28 07:48:13.000000 openscm-units-0.5.1/src/openscm_units.egg-info/PKG-INFO
--rw-r--r--   0 znicholls (1461210280) 2094513965      447 2023-04-28 07:48:13.000000 openscm-units-0.5.1/src/openscm_units.egg-info/SOURCES.txt
--rw-r--r--   0 znicholls (1461210280) 2094513965        1 2023-04-28 07:48:13.000000 openscm-units-0.5.1/src/openscm_units.egg-info/dependency_links.txt
--rw-r--r--   0 znicholls (1461210280) 2094513965      505 2023-04-28 07:48:13.000000 openscm-units-0.5.1/src/openscm_units.egg-info/requires.txt
--rw-r--r--   0 znicholls (1461210280) 2094513965       14 2023-04-28 07:48:13.000000 openscm-units-0.5.1/src/openscm_units.egg-info/top_level.txt
--rw-r--r--   0 znicholls (1461210280) 2094513965    68611 2021-07-27 07:27:26.000000 openscm-units-0.5.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:04:06.238557 openscm-units-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-27 03:02:43.000000 openscm-units-0.5.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-27 03:02:43.000000 openscm-units-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-27 03:02:43.000000 openscm-units-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-27 03:04:06.238557 openscm-units-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-27 03:02:43.000000 openscm-units-0.5.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-27 03:04:06.242557 openscm-units-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-27 03:02:43.000000 openscm-units-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:04:06.238557 openscm-units-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:04:06.242557 openscm-units-0.5.2/src/openscm_units/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-27 03:02:43.000000 openscm-units-0.5.2/src/openscm_units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20946 2023-05-27 03:02:43.000000 openscm-units-0.5.2/src/openscm_units/_unit_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-27 03:04:06.242557 openscm-units-0.5.2/src/openscm_units/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:04:06.238557 openscm-units-0.5.2/src/openscm_units/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-27 03:02:43.000000 openscm-units-0.5.2/src/openscm_units/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-05-27 03:02:43.000000 openscm-units-0.5.2/src/openscm_units/data/mixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:04:06.238557 openscm-units-0.5.2/src/openscm_units.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-27 03:04:05.000000 openscm-units-0.5.2/src/openscm_units.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-27 03:04:05.000000 openscm-units-0.5.2/src/openscm_units.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 03:04:05.000000 openscm-units-0.5.2/src/openscm_units.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-27 03:04:05.000000 openscm-units-0.5.2/src/openscm_units.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-27 03:04:05.000000 openscm-units-0.5.2/src/openscm_units.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-27 03:02:43.000000 openscm-units-0.5.2/versioneer.py
```

### Comparing `openscm-units-0.5.1/CHANGELOG.rst` & `openscm-units-0.5.2/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+v0.5.2
+------
+
+- (`#40 <https://github.com/openscm/openscm-units/pull/40>`_) Fixed broken definition of ppm, caused by regression in Pint where `'ppm' was added to Pint <https://github.com/hgrecco/pint/pull/1661>`_
+
 v0.5.1
 ------
 
 - (`#33 <https://github.com/openscm/openscm-units/pull/33>`_) Generate static usage documentation from the introduction notebook
 - (`#34 <https://github.com/openscm/openscm-units/pull/34>`_) Update documentation regarding NOx conversions.
 - (`#38 <https://github.com/openscm/openscm-units/pull/38>`_) Fixed Series.iteritems() removal in pandas, see e.g. `#150 in primap2 <https://github.com/pik-primap/primap2/issues/150>`_
```

### Comparing `openscm-units-0.5.1/LICENSE` & `openscm-units-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openscm-units-0.5.1/PKG-INFO` & `openscm-units-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openscm-units
-Version: 0.5.1
+Version: 0.5.2
 Summary: OpenSCM-Units is a repository for handling of units related to simple climate modelling.
 Home-page: https://github.com/openscm/openscm-units
 Author: Zeb Nicholls, Sven Willner, Jared Lewis, Robert Gieseke
 Author-email: zebedee.nicholls@climate-energy-college.org, sven.willner@pik-potsdam.de, jared.lewis@climate-energy-college.org, rob.g@web.de
 License: 3-Clause BSD License
 Keywords: openscm,units,python,repo,simple,climate,model
 Platform: UNKNOWN
```

### Comparing `openscm-units-0.5.1/README.rst` & `openscm-units-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `openscm-units-0.5.1/setup.cfg` & `openscm-units-0.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `openscm-units-0.5.1/setup.py` & `openscm-units-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `openscm-units-0.5.1/src/openscm_units/_unit_registry.py` & `openscm-units-0.5.2/src/openscm_units/_unit_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,15 +298,15 @@
     "SF6": "SF6",
     "SO2F2": "SO2F2",
     "NF3": "NF3",
     "HCO1130": "HCO1130",
 }
 
 
-class ScmUnitRegistry(pint.UnitRegistry):
+class ScmUnitRegistry(pint.UnitRegistry):  # pylint: disable=too-many-ancestors
     """
     Unit registry class.
 
     Provides some convenience methods to add standard units and contexts.
     """
 
     _contexts_added = False
@@ -328,14 +328,16 @@
         *args
             Passed to the ``__init__`` method of the super class
 
         **kwargs
             Passed to the ``__init__`` method of the super class
         """
         self._metric_conversions = metric_conversions
+        # If we didn't call init here, we wouldn't need to rebuild the cache
+        # below but that also feels like a bad pattern
         super().__init__(*args, **kwargs)
 
     def add_standards(self):
         """
         Add standard units.
 
         Has to be done separately because of pint's weird initializing.
@@ -350,17 +352,20 @@
         self.define("degreeC = degC")
         self.define("degreeF = degF")
         self.define("kt = 1000 * t")  # since kt is used for "knot" in the defaults
         self.define(
             "Tt = 1000000000000 * t"
         )  # since Tt is used for "tex" in the defaults
 
-        self.define("ppt = [concentrations]")
-        self.define("ppb = 1000 * ppt")
-        self.define("ppm = 1000 * ppb")
+        self.define("ppm = [concentrations]")
+        self.define("ppb = ppm / 1000")
+        self.define("ppt = ppb / 1000")
+        # Have to rebuild cache to get right units for ppm as it is defined in
+        # pint
+        self._build_cache()
 
     def enable_contexts(self, *names_or_contexts, **kwargs):
         """
         Overload pint's :func:`enable_contexts` to add contexts once (the first time
         they are used) to avoid (unnecessary) operations.
         """
         if not self._contexts_added:
```

### Comparing `openscm-units-0.5.1/src/openscm_units/data/mixtures.py` & `openscm-units-0.5.2/src/openscm_units/data/mixtures.py`

 * *Files identical despite different names*

### Comparing `openscm-units-0.5.1/src/openscm_units.egg-info/PKG-INFO` & `openscm-units-0.5.2/src/openscm_units.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openscm-units
-Version: 0.5.1
+Version: 0.5.2
 Summary: OpenSCM-Units is a repository for handling of units related to simple climate modelling.
 Home-page: https://github.com/openscm/openscm-units
 Author: Zeb Nicholls, Sven Willner, Jared Lewis, Robert Gieseke
 Author-email: zebedee.nicholls@climate-energy-college.org, sven.willner@pik-potsdam.de, jared.lewis@climate-energy-college.org, rob.g@web.de
 License: 3-Clause BSD License
 Keywords: openscm,units,python,repo,simple,climate,model
 Platform: UNKNOWN
```

### Comparing `openscm-units-0.5.1/versioneer.py` & `openscm-units-0.5.2/versioneer.py`

 * *Files identical despite different names*

