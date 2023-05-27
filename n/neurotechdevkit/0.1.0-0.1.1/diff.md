# Comparing `tmp/neurotechdevkit-0.1.0.tar.gz` & `tmp/neurotechdevkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurotechdevkit-0.1.0.tar", max compression
+gzip compressed data, was "neurotechdevkit-0.1.1.tar", max compression
```

## Comparing `neurotechdevkit-0.1.0.tar` & `neurotechdevkit-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11339 2023-05-25 15:57:42.896499 neurotechdevkit-0.1.0/LICENSE
--rw-r--r--   0        0        0     6043 2023-05-25 15:57:43.024500 neurotechdevkit-0.1.0/docs/index.md
--rw-r--r--   0        0        0     2146 2023-05-25 15:58:00.520779 neurotechdevkit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2404 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/__init__.py
--rw-r--r--   0        0        0     1162 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/__init__.py
--rw-r--r--   0        0        0     4747 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/_animations.py
--rw-r--r--   0        0        0     2304 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/_formatting.py
--rw-r--r--   0        0        0     8996 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/_source.py
--rw-r--r--   0        0        0     3485 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/_target.py
--rw-r--r--   0        0        0    49858 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/colormaps.py
--rw-r--r--   0        0        0     2307 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=10°.png
--rw-r--r--   0        0        0    30101 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=120°.png
--rw-r--r--   0        0        0    50607 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=150°.png
--rw-r--r--   0        0        0    61496 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=180°.png
--rw-r--r--   0        0        0     4467 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=20°.png
--rw-r--r--   0        0        0      715 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=2°.png
--rw-r--r--   0        0        0     8691 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=40°.png
--rw-r--r--   0        0        0     1147 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=5°.png
--rw-r--r--   0        0        0    12673 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=60°.png
--rw-r--r--   0        0        0    20015 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=90°.png
--rw-r--r--   0        0        0     2753 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=Flat.png
--rw-r--r--   0        0        0     3377 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/target-dark.png
--rw-r--r--   0        0        0     3598 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/target-light.png
--rw-r--r--   0        0        0      722 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/font.py
--rw-r--r--   0        0        0    96364 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf
--rw-r--r--   0        0        0    97116 2023-05-25 15:57:43.028499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf
--rw-r--r--   0        0        0    96304 2023-05-25 15:57:43.032499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf
--rw-r--r--   0        0        0    96312 2023-05-25 15:57:43.032499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf
--rw-r--r--   0        0        0    96492 2023-05-25 15:57:43.032499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf
--rw-r--r--   0        0        0    96412 2023-05-25 15:57:43.032499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf
--rw-r--r--   0        0        0    96528 2023-05-25 15:57:43.032499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf
--rw-r--r--   0        0        0     4314 2023-05-25 15:57:43.032499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/layers.py
--rw-r--r--   0        0        0     5561 2023-05-25 15:57:43.032499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/layout.py
--rw-r--r--   0        0        0     6290 2023-05-25 15:57:43.032499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/legends.py
--rw-r--r--   0        0        0     7499 2023-05-25 15:57:43.032499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/napari.py
--rw-r--r--   0        0        0     8880 2023-05-25 15:57:43.032499 neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/simulations.py
--rw-r--r--   0        0        0      593 2023-05-25 15:57:43.032499 neurotechdevkit-0.1.0/src/neurotechdevkit/results/__init__.py
--rw-r--r--   0        0        0    53394 2023-05-25 15:57:43.036500 neurotechdevkit-0.1.0/src/neurotechdevkit/results/_results.py
--rw-r--r--   0        0        0      420 2023-05-25 15:57:43.036500 neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/__init__.py
--rw-r--r--   0        0        0    44996 2023-05-25 15:57:43.036500 neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_base.py
--rw-r--r--   0        0        0    13024 2023-05-25 15:57:43.036500 neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_metrics.py
--rw-r--r--   0        0        0     6053 2023-05-25 15:57:43.036500 neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_resources.py
--rw-r--r--   0        0        0     4766 2023-05-25 15:57:43.036500 neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_scenario_0.py
--rw-r--r--   0        0        0     8932 2023-05-25 15:57:43.036500 neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_scenario_1.py
--rw-r--r--   0        0        0    11891 2023-05-25 15:57:43.036500 neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_scenario_2.py
--rw-r--r--   0        0        0     7378 2023-05-25 15:57:43.036500 neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_shots.py
--rw-r--r--   0        0        0     4559 2023-05-25 15:57:43.036500 neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_time.py
--rw-r--r--   0        0        0    11381 2023-05-25 15:57:43.036500 neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_utils.py
--rw-r--r--   0        0        0  2195183 2023-05-25 15:57:43.048500 neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat
--rw-r--r--   0        0        0      936 2023-05-25 15:57:43.048500 neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/materials.py
--rw-r--r--   0        0        0    55819 2023-05-25 15:57:43.048500 neurotechdevkit-0.1.0/src/neurotechdevkit/sources.py
--rw-r--r--   0        0        0     7465 1970-01-01 00:00:00.000000 neurotechdevkit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-05-27 00:58:36.941683 neurotechdevkit-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3304 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/docs/index.md
+-rw-r--r--   0        0        0     2146 2023-05-27 00:58:56.145862 neurotechdevkit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2404 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/src/neurotechdevkit/__init__.py
+-rw-r--r--   0        0        0     1162 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/__init__.py
+-rw-r--r--   0        0        0     4747 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_animations.py
+-rw-r--r--   0        0        0     2304 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_formatting.py
+-rw-r--r--   0        0        0     8996 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_source.py
+-rw-r--r--   0        0        0     3485 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_target.py
+-rw-r--r--   0        0        0    49858 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/colormaps.py
+-rw-r--r--   0        0        0     2307 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=10°.png
+-rw-r--r--   0        0        0    30101 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=120°.png
+-rw-r--r--   0        0        0    50607 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=150°.png
+-rw-r--r--   0        0        0    61496 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=180°.png
+-rw-r--r--   0        0        0     4467 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=20°.png
+-rw-r--r--   0        0        0      715 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=2°.png
+-rw-r--r--   0        0        0     8691 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=40°.png
+-rw-r--r--   0        0        0     1147 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=5°.png
+-rw-r--r--   0        0        0    12673 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=60°.png
+-rw-r--r--   0        0        0    20015 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=90°.png
+-rw-r--r--   0        0        0     2753 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=Flat.png
+-rw-r--r--   0        0        0     3377 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/target-dark.png
+-rw-r--r--   0        0        0     3598 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/target-light.png
+-rw-r--r--   0        0        0      722 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/font.py
+-rw-r--r--   0        0        0    96364 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf
+-rw-r--r--   0        0        0    97116 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf
+-rw-r--r--   0        0        0    96304 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf
+-rw-r--r--   0        0        0    96312 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf
+-rw-r--r--   0        0        0    96492 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf
+-rw-r--r--   0        0        0    96412 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf
+-rw-r--r--   0        0        0    96528 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf
+-rw-r--r--   0        0        0     4314 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/layers.py
+-rw-r--r--   0        0        0     5561 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/layout.py
+-rw-r--r--   0        0        0     6290 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/legends.py
+-rw-r--r--   0        0        0     7499 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/napari.py
+-rw-r--r--   0        0        0     8880 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/simulations.py
+-rw-r--r--   0        0        0      593 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/results/__init__.py
+-rw-r--r--   0        0        0    53394 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/results/_results.py
+-rw-r--r--   0        0        0      619 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/__init__.py
+-rw-r--r--   0        0        0    44605 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_base.py
+-rw-r--r--   0        0        0    13024 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_metrics.py
+-rw-r--r--   0        0        0     6053 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_resources.py
+-rw-r--r--   0        0        0     4549 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_scenario_0.py
+-rw-r--r--   0        0        0     8500 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_scenario_1.py
+-rw-r--r--   0        0        0    11457 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_scenario_2.py
+-rw-r--r--   0        0        0     7378 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_shots.py
+-rw-r--r--   0        0        0     4559 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_time.py
+-rw-r--r--   0        0        0    11913 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_utils.py
+-rw-r--r--   0        0        0  2195183 2023-05-27 00:58:37.077684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat
+-rw-r--r--   0        0        0      936 2023-05-27 00:58:37.077684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/materials.py
+-rw-r--r--   0        0        0    55819 2023-05-27 00:58:37.077684 neurotechdevkit-0.1.1/src/neurotechdevkit/sources.py
+-rw-r--r--   0        0        0     4726 1970-01-01 00:00:00.000000 neurotechdevkit-0.1.1/PKG-INFO
```

### Comparing `neurotechdevkit-0.1.0/LICENSE` & `neurotechdevkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/pyproject.toml` & `neurotechdevkit-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neurotechdevkit"
-version = "v0.1.0"
+version = "v0.1.1"
 description = "Neurotech Development Kit: an open-source software library designed to enhance accessibility to cutting-edge neurotechnology"
 authors = ["AE Studio <bci@ae.studio>"]
 maintainers = ["AE Studio <bci@ae.studio>"]
 packages = [{include = "neurotechdevkit", from = "src" }]
 
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/__init__.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/__init__.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/_animations.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_animations.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/_formatting.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_formatting.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/_source.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_source.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/_target.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_target.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/colormaps.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/colormaps.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=10°.png` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=10°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=120°.png` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=120°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=150°.png` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=150°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=180°.png` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=180°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=20°.png` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=20°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=2°.png` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=2°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=40°.png` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=40°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=5°.png` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=5°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=60°.png` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=60°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=90°.png` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=90°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/Angle=Flat.png` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=Flat.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/target-dark.png` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/target-dark.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/components/target-light.png` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/target-light.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/font.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/font.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/layers.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/layers.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/layout.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/layout.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/legends.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/legends.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/napari.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/napari.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/rendering/simulations.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/simulations.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/results/__init__.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/results/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/results/_results.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/results/_results.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_base.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -870,27 +870,14 @@
                 save_bounds=save_bounds,
                 save_undersampling=save_undersampling,
                 wavefield_slice=wavefield_slice,
                 devito_args=devito_args,
             )
         )
 
-    @abc.abstractmethod
-    def render_material_property(
-        self,
-        name,
-        show_orientation: bool = True,
-        show_sources: bool = True,
-        show_target: bool = True,
-    ) -> None:
-        """Render a material property for the scenario."""
-        # speed of sound, density, and absorption
-        # maybe split these out into 3 separate functions?
-        pass
-
 
 class Scenario2D(Scenario):
     """A 2D scenario."""
 
     def get_target_mask(self) -> npt.NDArray[np.bool_]:
         """Return the mask for the target region."""
         target_mask = create_grid_circular_mask(
```

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_metrics.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_metrics.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_resources.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_resources.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_scenario_0.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_scenario_0.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,20 +31,14 @@
         self._target_id = "target_1"
 
         super().__init__(
             origin=np.array([0.0, -0.02]),
             complexity=complexity,
         )
 
-    def render_material_property(
-        self, name, show_orientation=True, show_sources=True, show_target=True
-    ):
-        """Render the material property of the scenario."""
-        raise NotImplementedError()
-
     @property
     def _material_layers(self) -> list[tuple[str, Struct]]:
         return [
             ("water", materials.water),
             ("skull", materials.cortical_bone),
             ("brain", materials.brain),
             ("tumor", materials.tumor),
```

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_scenario_1.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_scenario_1.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,20 +122,14 @@
         self._target_id = "target_1"
 
         super().__init__(
             origin=np.array([0.0, -0.035]),
             complexity=complexity,
         )
 
-    def render_material_property(
-        self, name, show_orientation=True, show_sources=True, show_target=True
-    ):
-        """Render a material property for the scenario."""
-        raise NotImplementedError()
-
     def _compile_problem(self) -> stride.Problem:
         extent = np.array([0.12, 0.07])  # m
         return self._compile_scenario_1_problem(extent)
 
     def get_default_source(self) -> sources.Source:
         """Return the default source for the scenario."""
         return sources.FocusedSource2D(
@@ -214,20 +208,14 @@
         return 1
 
     def get_default_slice_position(self, axis: int) -> float:
         """Return the default slice position for the scenario."""
         default_positions = np.array([0.064, 0.0, 0.0])
         return default_positions[axis]
 
-    def render_material_property(
-        self, name, show_orientation=True, show_sources=True, show_target=True
-    ):
-        """Render a material property for the scenario."""
-        raise NotImplementedError()
-
     def _compile_problem(self) -> stride.Problem:
         extent = np.array([0.12, 0.07, 0.07])  # m
         return self._compile_scenario_1_problem(extent)
 
     def get_default_source(self) -> sources.Source:
         """Return the default source for the scenario."""
         return sources.FocusedSource3D(
```

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_scenario_2.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_scenario_2.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,20 +144,14 @@
         self._target_id = "primary-visual-cortex"
 
         super().__init__(
             origin=np.array([0.0, -0.085]),
             complexity=complexity,
         )
 
-    def render_material_property(
-        self, name, show_orientation=True, show_sources=True, show_target=True
-    ):
-        """Render the material property of the scenario."""
-        raise NotImplementedError()
-
     def _compile_problem(self) -> stride.Problem:
         extent = np.array([0.225, 0.170])  # m
         return self._compile_scenario_2_problem(extent)
 
     def _get_material_masks(self) -> Mapping[str, npt.NDArray[np.bool_]]:
         return {
             name: _create_scenario_2_mask(name, convert_2d=True)
@@ -281,20 +275,14 @@
         return 2
 
     def get_default_slice_position(self, axis: int) -> float:
         """Get the default slice position for the scenario."""
         default_positions = np.array([0.1, 0.0, 0.0])
         return default_positions[axis]
 
-    def render_material_property(
-        self, name, show_orientation=True, show_sources=True, show_target=True
-    ):
-        """Render the material property of the scenario."""
-        raise NotImplementedError()
-
     def _compile_problem(self) -> stride.Problem:
         extent = np.array([0.225, 0.170, 0.190])  # m
         return self._compile_scenario_2_problem(extent)
 
     def _get_material_masks(self):
         return {
             name: _create_scenario_2_mask(name, convert_2d=False)
```

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_shots.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_shots.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_time.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_time.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/_utils.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,17 +63,28 @@
     materials: Mapping[str, Struct],
     layer_ids: Mapping[str, int],
     masks: Mapping[str, npt.NDArray[np.bool_]],
 ) -> stride.Problem:
     """Add material fields as media to the problem.
 
     Included fields are:
-    * the speed of sound (in m/s)
-    * density (in kg/m^3)
-    * absorption (in dB/cm)
+
+    - the speed of sound (in m/s)
+    - density (in kg/m^3)
+    - absorption (in dB/cm)
+
+    Args:
+        problem (stride.Problem): the stride Problem object to which the
+            media should be added.
+        materials (Mapping[str, Struct]): a mapping from material names
+            to Structs containing the material properties.
+        layer_ids (Mapping[str, int]): a mapping from material names to
+            integers representing the layer number for each material.
+        masks (Mapping[str, npt.NDArray[np.bool_]]): a mapping from material
+            names to boolean masks indicating the gridpoints.
     """
     grid = problem.grid
 
     vp = stride.ScalarField(name="vp", grid=grid)  # [m/s]
     rho = stride.ScalarField(name="rho", grid=grid)  # [kg/m^3]
     alpha = stride.ScalarField(name="alpha", grid=grid)  # [dB/cm]
     layer = stride.ScalarField(name="layer", grid=grid)  # integers
```

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat` & `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/scenarios/materials.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/materials.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.0/src/neurotechdevkit/sources.py` & `neurotechdevkit-0.1.1/src/neurotechdevkit/sources.py`

 * *Files identical despite different names*

