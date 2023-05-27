# Comparing `tmp/jsbgym-0.1.8.tar.gz` & `tmp/jsbgym-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsbgym-0.1.8.tar", last modified: Sun Apr 23 06:28:06 2023, max compression
+gzip compressed data, was "jsbgym-0.1.9.tar", last modified: Sat May 27 04:13:12 2023, max compression
```

## Comparing `jsbgym-0.1.8.tar` & `jsbgym-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:28:06.816856 jsbgym-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-23 06:27:52.000000 jsbgym-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 06:27:52.000000 jsbgym-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-04-23 06:28:06.816856 jsbgym-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-04-23 06:27:52.000000 jsbgym-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:28:06.816856 jsbgym-0.1.8/jsbgym/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:28:06.816856 jsbgym-0.1.8/jsbgym/agents/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/aircraft.py
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/assessors.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/basic_ic.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/flightgear.xml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/minimal_ic.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19494 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:28:06.816856 jsbgym-0.1.8/jsbgym/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/manual_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/stubs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_assessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_geodetic_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    17121 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25499 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_visualiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/visualiser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:28:06.816856 jsbgym-0.1.8/jsbgym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-04-23 06:28:06.000000 jsbgym-0.1.8/jsbgym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-23 06:28:06.000000 jsbgym-0.1.8/jsbgym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:28:06.000000 jsbgym-0.1.8/jsbgym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:28:06.000000 jsbgym-0.1.8/jsbgym.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 06:28:06.000000 jsbgym-0.1.8/jsbgym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 06:28:06.000000 jsbgym-0.1.8/jsbgym.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-23 06:27:52.000000 jsbgym-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 06:28:06.816856 jsbgym-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:13:12.954995 jsbgym-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-27 04:12:57.000000 jsbgym-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 04:12:57.000000 jsbgym-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-27 04:13:12.954995 jsbgym-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-27 04:12:57.000000 jsbgym-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:13:12.950995 jsbgym-0.1.9/jsbgym/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:13:12.954995 jsbgym-0.1.9/jsbgym/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/aircraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/assessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/basic_ic.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/flightgear.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/minimal_ic.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19494 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:13:12.954995 jsbgym-0.1.9/jsbgym/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/manual_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_assessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_geodetic_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17121 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25499 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_visualiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/visualiser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:13:12.954995 jsbgym-0.1.9/jsbgym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-27 04:13:12.000000 jsbgym-0.1.9/jsbgym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-27 04:13:12.000000 jsbgym-0.1.9/jsbgym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 04:13:12.000000 jsbgym-0.1.9/jsbgym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 04:13:12.000000 jsbgym-0.1.9/jsbgym.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 04:13:12.000000 jsbgym-0.1.9/jsbgym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 04:13:12.000000 jsbgym-0.1.9/jsbgym.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-27 04:12:57.000000 jsbgym-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 04:13:12.954995 jsbgym-0.1.9/setup.cfg
```

### Comparing `jsbgym-0.1.8/LICENSE` & `jsbgym-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/PKG-INFO` & `jsbgym-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsbgym
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model.
 Author: sryu1
 License: MIT
 Project-URL: Homepage, https://github.com/sryu1/jsbgym
 Project-URL: Bug Tracker, https://github.com/sryu1/jsbgym/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -66,21 +66,20 @@
 
 ### Aircraft
 
 The environment can be configured to use one of Six aircraft:
 
 * **Cessna172P** Cessna 172P Skyhawk (Default FlightGear Aircraft)
 * **PA28** Piper PA-28-161 Warrior II
+* **J3** Piper J-3 Cub
 * **F15** McDonnell Douglas F-15C Eagle (F-15C in FlightGear)
 * **F16** General Dynamics F-16CJ Block 52
 * **A320** Airbus A320 (A320 Familiy in Flightgear)
 * **B747** Boeing 747-400
 
-Some aircraft will not work until the next update of JSBSim.
-
 All aircraft except the Cessna 172P requires the aircraft to be downloaded via the launcher using the default FlightGear Hangar.
 
 ### Task
 
 JSBGym implements two tasks for controlling the altitude and heading of aircraft:
 
 * **HeadingControlTask**: aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
@@ -116,15 +115,15 @@
 env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0", render_mode="human")
 env.reset()
 env.render()
 ```
 
 ### 3D
 
-Visualising with FlightGear requires the Gymnasium environment to be created with a FlightGear-enabled environment ID by specifying the render_mode in `gym.make()` and changing the value after `shaping` to `FG`. Using this render mode while training is strongly discouraged due to an error occuring midway through the training (`Could not connect to socket for output!`).
+Visualising with FlightGear requires the Gymnasium environment to be created with a FlightGear-enabled environment ID by specifying the render_mode in `gym.make()` and changing the value after `{shaping}` to `FG`. Using this render mode while training is strongly discouraged due to an error occuring midway through the training (`Could not connect to socket for output!`).
 
 ```python
 env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-FG-v0", render_mode="flightgear")
 env.reset()
 env.render()
 ```
```

### Comparing `jsbgym-0.1.8/README.md` & `jsbgym-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,21 +47,20 @@
 
 ### Aircraft
 
 The environment can be configured to use one of Six aircraft:
 
 * **Cessna172P** Cessna 172P Skyhawk (Default FlightGear Aircraft)
 * **PA28** Piper PA-28-161 Warrior II
+* **J3** Piper J-3 Cub
 * **F15** McDonnell Douglas F-15C Eagle (F-15C in FlightGear)
 * **F16** General Dynamics F-16CJ Block 52
 * **A320** Airbus A320 (A320 Familiy in Flightgear)
 * **B747** Boeing 747-400
 
-Some aircraft will not work until the next update of JSBSim.
-
 All aircraft except the Cessna 172P requires the aircraft to be downloaded via the launcher using the default FlightGear Hangar.
 
 ### Task
 
 JSBGym implements two tasks for controlling the altitude and heading of aircraft:
 
 * **HeadingControlTask**: aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
@@ -97,15 +96,15 @@
 env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0", render_mode="human")
 env.reset()
 env.render()
 ```
 
 ### 3D
 
-Visualising with FlightGear requires the Gymnasium environment to be created with a FlightGear-enabled environment ID by specifying the render_mode in `gym.make()` and changing the value after `shaping` to `FG`. Using this render mode while training is strongly discouraged due to an error occuring midway through the training (`Could not connect to socket for output!`).
+Visualising with FlightGear requires the Gymnasium environment to be created with a FlightGear-enabled environment ID by specifying the render_mode in `gym.make()` and changing the value after `{shaping}` to `FG`. Using this render mode while training is strongly discouraged due to an error occuring midway through the training (`Could not connect to socket for output!`).
 
 ```python
 env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-FG-v0", render_mode="flightgear")
 env.reset()
 env.render()
 ```
```

### Comparing `jsbgym-0.1.8/jsbgym/__init__.py` & `jsbgym-0.1.9/jsbgym/__init__.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/agents/agents.py` & `jsbgym-0.1.9/jsbgym/agents/agents.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/aircraft.py` & `jsbgym-0.1.9/jsbgym/aircraft.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,11 +18,12 @@
 
     def get_cruise_speed_fps(self) -> float:
         return self.cruise_speed_kts * self.KTS_TO_FT_PER_S
 
 
 cessna172P = Aircraft("c172p", "c172p", "Cessna172P", 120)
 pa28 = Aircraft("pa28", "PA28-161-180", "PA28", 130)
+j3 = Aircraft("J3Cub", "J3Cub", "J3", 70)
 f15 = Aircraft("f15", "f15c", "F15", 500)
 f16 = Aircraft("f16", "f16-block-52", "F16", 550)
 a320 = Aircraft("A320", "A320-200-CFM", "A320", 480)
 b747 = Aircraft("B747", "747-400", "B747", 490)
```

### Comparing `jsbgym-0.1.8/jsbgym/assessors.py` & `jsbgym-0.1.9/jsbgym/assessors.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/basic_ic.xml` & `jsbgym-0.1.9/jsbgym/basic_ic.xml`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/environment.py` & `jsbgym-0.1.9/jsbgym/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,10 +208,10 @@
             aircraft=aircraft,
             init_conditions=initial_conditions,
             allow_flightgear_output=False,
         )
 
     def render(self, flightgear_blocking=True):
         if self.render_mode == "flightgear" or self.render_mode == "human_fg":
-            raise ValueError("flightgear rendering is disabled for this class")
+            raise ValueError("FlightGear rendering is disabled for this class")
         else:
             super().render(flightgear_blocking)
```

### Comparing `jsbgym-0.1.8/jsbgym/flightgear.xml` & `jsbgym-0.1.9/jsbgym/flightgear.xml`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/properties.py` & `jsbgym-0.1.9/jsbgym/properties.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/rewards.py` & `jsbgym-0.1.9/jsbgym/rewards.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/simulation.py` & `jsbgym-0.1.9/jsbgym/simulation.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/tasks.py` & `jsbgym-0.1.9/jsbgym/tasks.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/tests/manual_tests.py` & `jsbgym-0.1.9/jsbgym/tests/manual_tests.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/tests/stubs.py` & `jsbgym-0.1.9/jsbgym/tests/stubs.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/tests/test_agents.py` & `jsbgym-0.1.9/jsbgym/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/tests/test_assessors.py` & `jsbgym-0.1.9/jsbgym/tests/test_assessors.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/tests/test_environment.py` & `jsbgym-0.1.9/jsbgym/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/tests/test_functional.py` & `jsbgym-0.1.9/jsbgym/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/tests/test_geodetic_position.py` & `jsbgym-0.1.9/jsbgym/tests/test_geodetic_position.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/tests/test_rewards.py` & `jsbgym-0.1.9/jsbgym/tests/test_rewards.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/tests/test_simulation.py` & `jsbgym-0.1.9/jsbgym/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/tests/test_tasks.py` & `jsbgym-0.1.9/jsbgym/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/tests/test_visualiser.py` & `jsbgym-0.1.9/jsbgym/tests/test_visualiser.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/jsbgym/utils.py` & `jsbgym-0.1.9/jsbgym/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools
 import operator
 from typing import Tuple
-from jsbgym.aircraft import cessna172P, a320, f15, pa28, b747, f16
+from jsbgym.aircraft import cessna172P, a320, f15, pa28, b747, f16, j3
 from typing import Dict, Iterable
 
 
 class AttributeFormatter(object):
     """
     Replaces characters that would be illegal in an attribute name
 
@@ -39,15 +39,15 @@
 def get_env_id_kwargs_map() -> Dict[str, Tuple]:
     """Returns all environment IDs mapped to tuple of (task, aircraft, shaping, flightgear)"""
     # lazy import to avoid circular dependencies
     from jsbgym.tasks import Shaping, HeadingControlTask, TurnHeadingControlTask
 
     map = {}
     for task_type in (HeadingControlTask, TurnHeadingControlTask):
-        for plane in (cessna172P, a320, f15, pa28, b747, f16):
+        for plane in (cessna172P, a320, f15, pa28, b747, f16, j3):
             for shaping in (Shaping.STANDARD, Shaping.EXTRA, Shaping.EXTRA_SEQUENTIAL):
                 for enable_flightgear in (True, False):
                     id = get_env_id(plane, task_type, shaping, enable_flightgear)
                     assert id not in map
                     map[id] = (plane, task_type, shaping, enable_flightgear)
     return map
```

### Comparing `jsbgym-0.1.8/jsbgym/visualiser.py` & `jsbgym-0.1.9/jsbgym/visualiser.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         if not self.figure:
             self.figure, self.axes = self._plot_configure()
 
         # delete old control surface data points
         for subplot in self.axes[1:]:
             # pop and translate all data points
             while subplot.lines:
-                data = subplot.lines.pop()
+                data = subplot.lines[0].remove()
                 del data
 
         self._print_state(sim)
         self._plot_control_states(sim, self.axes)
         self._plot_control_commands(sim, self.axes)
         plt.pause(self.PLOT_PAUSE_SECONDS)  # voodoo pause needed for figure to update
```

### Comparing `jsbgym-0.1.8/jsbgym.egg-info/PKG-INFO` & `jsbgym-0.1.9/jsbgym.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsbgym
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model.
 Author: sryu1
 License: MIT
 Project-URL: Homepage, https://github.com/sryu1/jsbgym
 Project-URL: Bug Tracker, https://github.com/sryu1/jsbgym/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -66,21 +66,20 @@
 
 ### Aircraft
 
 The environment can be configured to use one of Six aircraft:
 
 * **Cessna172P** Cessna 172P Skyhawk (Default FlightGear Aircraft)
 * **PA28** Piper PA-28-161 Warrior II
+* **J3** Piper J-3 Cub
 * **F15** McDonnell Douglas F-15C Eagle (F-15C in FlightGear)
 * **F16** General Dynamics F-16CJ Block 52
 * **A320** Airbus A320 (A320 Familiy in Flightgear)
 * **B747** Boeing 747-400
 
-Some aircraft will not work until the next update of JSBSim.
-
 All aircraft except the Cessna 172P requires the aircraft to be downloaded via the launcher using the default FlightGear Hangar.
 
 ### Task
 
 JSBGym implements two tasks for controlling the altitude and heading of aircraft:
 
 * **HeadingControlTask**: aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
@@ -116,15 +115,15 @@
 env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0", render_mode="human")
 env.reset()
 env.render()
 ```
 
 ### 3D
 
-Visualising with FlightGear requires the Gymnasium environment to be created with a FlightGear-enabled environment ID by specifying the render_mode in `gym.make()` and changing the value after `shaping` to `FG`. Using this render mode while training is strongly discouraged due to an error occuring midway through the training (`Could not connect to socket for output!`).
+Visualising with FlightGear requires the Gymnasium environment to be created with a FlightGear-enabled environment ID by specifying the render_mode in `gym.make()` and changing the value after `{shaping}` to `FG`. Using this render mode while training is strongly discouraged due to an error occuring midway through the training (`Could not connect to socket for output!`).
 
 ```python
 env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-FG-v0", render_mode="flightgear")
 env.reset()
 env.render()
 ```
```

### Comparing `jsbgym-0.1.8/jsbgym.egg-info/SOURCES.txt` & `jsbgym-0.1.9/jsbgym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.8/pyproject.toml` & `jsbgym-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsbgym"
-version = "0.1.8"
+version = "0.1.9"
 authors = [{ name = "sryu1" }]
 readme = "README.md"
 license = { text = "MIT" }
 description = "A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model."
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.7",
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 
 requires-python = ">=3.7"
-dependencies = ["numpy", "gymnasium", "jsbsim", "matplotlib<=3.6.3"]
+dependencies = ["numpy", "gymnasium", "jsbsim", "matplotlib"]
 
 [project.urls]
 Homepage = "https://github.com/sryu1/jsbgym"
 "Bug Tracker" = "https://github.com/sryu1/jsbgym/issues"
 
 
 [tool.setuptools]
```

