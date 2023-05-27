# Comparing `tmp/athletes_unlimited_py-0.0.6a1.tar.gz` & `tmp/athletes_unlimited_py-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athletes_unlimited_py-0.0.6a1.tar", last modified: Sat May 27 04:12:36 2023, max compression
+gzip compressed data, was "athletes_unlimited_py-0.0.7.tar", last modified: Sat May 27 04:44:51 2023, max compression
```

## Comparing `athletes_unlimited_py-0.0.6a1.tar` & `athletes_unlimited_py-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:12:36.342243 athletes_unlimited_py-0.0.6a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-27 04:12:12.000000 athletes_unlimited_py-0.0.6a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-27 04:12:36.342243 athletes_unlimited_py-0.0.6a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-27 04:12:12.000000 athletes_unlimited_py-0.0.6a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:12:36.338243 athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-27 04:12:12.000000 athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27349 2023-05-27 04:12:12.000000 athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/aux_softball.py
--rw-r--r--   0 runner    (1001) docker     (123)    31493 2023-05-27 04:12:12.000000 athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/basketball.py
--rw-r--r--   0 runner    (1001) docker     (123)    31526 2023-05-27 04:12:12.000000 athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/lacrosse.py
--rw-r--r--   0 runner    (1001) docker     (123)    48904 2023-05-27 04:12:12.000000 athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/softball.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-27 04:12:12.000000 athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30686 2023-05-27 04:12:12.000000 athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/volleyball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:12:36.342243 athletes_unlimited_py-0.0.6a1/athletes_unlimited_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-27 04:12:36.000000 athletes_unlimited_py-0.0.6a1/athletes_unlimited_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-27 04:12:36.000000 athletes_unlimited_py-0.0.6a1/athletes_unlimited_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 04:12:36.000000 athletes_unlimited_py-0.0.6a1/athletes_unlimited_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-27 04:12:36.000000 athletes_unlimited_py-0.0.6a1/athletes_unlimited_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 04:12:36.000000 athletes_unlimited_py-0.0.6a1/athletes_unlimited_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-27 04:12:12.000000 athletes_unlimited_py-0.0.6a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 04:12:36.342243 athletes_unlimited_py-0.0.6a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:44:51.013225 athletes_unlimited_py-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-27 04:44:28.000000 athletes_unlimited_py-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-27 04:44:51.013225 athletes_unlimited_py-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-27 04:44:28.000000 athletes_unlimited_py-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:44:51.013225 athletes_unlimited_py-0.0.7/athetes_unlimited_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-27 04:44:28.000000 athletes_unlimited_py-0.0.7/athetes_unlimited_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27349 2023-05-27 04:44:28.000000 athletes_unlimited_py-0.0.7/athetes_unlimited_py/aux_softball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31493 2023-05-27 04:44:28.000000 athletes_unlimited_py-0.0.7/athetes_unlimited_py/basketball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31526 2023-05-27 04:44:28.000000 athletes_unlimited_py-0.0.7/athetes_unlimited_py/lacrosse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49923 2023-05-27 04:44:28.000000 athletes_unlimited_py-0.0.7/athetes_unlimited_py/softball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-27 04:44:28.000000 athletes_unlimited_py-0.0.7/athetes_unlimited_py/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31348 2023-05-27 04:44:28.000000 athletes_unlimited_py-0.0.7/athetes_unlimited_py/volleyball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:44:51.013225 athletes_unlimited_py-0.0.7/athletes_unlimited_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-27 04:44:51.000000 athletes_unlimited_py-0.0.7/athletes_unlimited_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-27 04:44:51.000000 athletes_unlimited_py-0.0.7/athletes_unlimited_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 04:44:51.000000 athletes_unlimited_py-0.0.7/athletes_unlimited_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-27 04:44:51.000000 athletes_unlimited_py-0.0.7/athletes_unlimited_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 04:44:51.000000 athletes_unlimited_py-0.0.7/athletes_unlimited_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-27 04:44:28.000000 athletes_unlimited_py-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 04:44:51.013225 athletes_unlimited_py-0.0.7/setup.cfg
```

### Comparing `athletes_unlimited_py-0.0.6a1/LICENSE` & `athletes_unlimited_py-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.6a1/PKG-INFO` & `athletes_unlimited_py-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athletes_unlimited_py
-Version: 0.0.6a1
+Version: 0.0.7
 Summary: Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/athletes-unlimited-py
 Project-URL: documentation, https://github.com/armstjc/athletes-unlimited-py/wiki
 Project-URL: repository, https://github.com/armstjc/athletes-unlimited-py.git
```

### Comparing `athletes_unlimited_py-0.0.6a1/README.md` & `athletes_unlimited_py-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/aux_softball.py` & `athletes_unlimited_py-0.0.7/athetes_unlimited_py/aux_softball.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/basketball.py` & `athletes_unlimited_py-0.0.7/athetes_unlimited_py/basketball.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/lacrosse.py` & `athletes_unlimited_py-0.0.7/athetes_unlimited_py/lacrosse.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/softball.py` & `athletes_unlimited_py-0.0.7/athetes_unlimited_py/softball.py`

 * *Files 1% similar despite different names*

```diff
@@ -705,132 +705,136 @@
     #    'pitching_HR9', 'pitching_BB9', 'pitching_SO9', 'pitching_SO/BB',
     #    'pitching_RA9', 'pitching_PI', 'pitching_PI_balls',
     #    'pitching_PI_strikes', 'fielding_position', 'fielding_IP_str',
     #    'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
     #    'fielding_FLD%', 'fielding_CS', 'fielding_CS%', 'fielding_TC',
     #    'fielding_CH', 'fielding_RF/9']
 
-    finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'playerId',
-                                         'first_name', 'last_name', 'full_name'], as_index=False)[[
-                                             'G', 'GS', 'AU_POINTS',
-                                             'batting_PA', 'batting_AB', 'batting_R',
-                                             'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI',
-                                             'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA',
-                                             'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH',
-                                             'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS',
-                                             'pitching_SV', 'pitching_IP',
-                                             'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB',
-                                             'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls',
-                                             'pitching_PI_strikes',
-                                             'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
-                                             'fielding_CS', 'fielding_TC'
-                                         ]].sum()
-
-    finished_df[['G', 'GS', 'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']] = finished_df[[
-        'G', 'GS', 'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']].astype('int')
-    finished_df['pitching_IP'] = finished_df['pitching_IP'].astype('float')
-    # Batting
-    finished_df.loc[finished_df['batting_AB'] >= 1,
-                    'batting_BA'] = finished_df['batting_H'] / finished_df['batting_AB']
-    finished_df['batting_BA'] = finished_df['batting_BA'].round(3)
-
-    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_OBP'] = (finished_df['batting_H'] + finished_df['batting_BB'] + finished_df['batting_HBP']) / (
-        finished_df['batting_AB'] + finished_df['batting_BB'] + finished_df['batting_HBP'] + finished_df['batting_SF'])
-    finished_df['batting_OBP'] = finished_df['batting_OBP'].round(3)
-
-    finished_df.loc[finished_df['batting_AB'] > 0,
-                    'batting_SLG'] = finished_df['batting_TB'] / finished_df['batting_AB']
-    finished_df['batting_SLG'] = finished_df['batting_SLG'].round(3)
-
-    finished_df.loc[finished_df['batting_AB'] > 0,
-                    'batting_OPS'] = finished_df['batting_OBP'] + finished_df['batting_SLG']
-    finished_df['batting_OPS'] = finished_df['batting_OPS'].round(3)
-
-    finished_df['batting_OPS+'] = None
-
-    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_SecA'] = (finished_df['batting_BB'] + (
-        finished_df['batting_TB'] - finished_df['batting_H']) + (finished_df['batting_SB'] - finished_df['batting_CS'])) / finished_df['batting_AB']
-    finished_df['batting_SecA'] = finished_df['batting_SecA'].round(3)
-
-    finished_df.loc[finished_df['batting_PA'] > 0,
-                    'batting_BB%'] = finished_df['batting_BB'] / finished_df['batting_PA']
-    finished_df['batting_BB%'] = finished_df['batting_BB%'].round(3)
-
-    finished_df.loc[finished_df['batting_PA'] > 0,
-                    'batting_K%'] = finished_df['batting_K'] / finished_df['batting_PA']
-    finished_df['batting_K%'] = finished_df['batting_K%'].round(3)
-
-    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_ISO'] = (
-        finished_df['batting_TB'] - finished_df['batting_H']) / finished_df['batting_AB']
-    finished_df['batting_ISO'] = finished_df['batting_ISO'].round(3)
-
-    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_BABIP'] = (finished_df['batting_H'] + finished_df['batting_HR']) / (
-        finished_df['batting_AB'] - finished_df['batting_K'] - finished_df['batting_HR'] + finished_df['batting_SF'])
-    finished_df['batting_BABIP'] = finished_df['batting_BABIP'].round(3)
-
-    finished_df.loc[(finished_df['batting_SB'] > 0) | (finished_df['batting_HR'] > 0), 'batting_PSN'] = (
-        2 * finished_df['batting_HR'] * finished_df['batting_SB']) / (finished_df['batting_HR'] * finished_df['batting_SB'])
-    finished_df['batting_PSN'] = finished_df['batting_PSN'].round(3)
-
-    # Pitching
-    finished_df['pitching_ERA'] = 9 * \
-        (finished_df['pitching_ER'] / finished_df['pitching_IP'])
-    finished_df['pitching_ERA'] = finished_df['pitching_ERA'].round(3)
-
-    finished_df['pitching_ERA+'] = None
-    finished_df['pitching_FIP'] = None
-    finished_df['pitching_FIP-'] = None
-    finished_df['pitching_WHIP'] = (
-        finished_df['pitching_BB'] + finished_df['pitching_H']) / finished_df['pitching_IP']
-    finished_df['pitching_WHIP'] = finished_df['pitching_WHIP'].round(3)
-
-    finished_df['pitching_H9'] = (
-        9 * finished_df['pitching_H']) / finished_df['pitching_IP']
-    finished_df['pitching_H9'] = finished_df['pitching_H9'].round(3)
-
-    finished_df['pitching_HR9'] = (
-        9 * finished_df['pitching_HR']) / finished_df['pitching_IP']
-    finished_df['pitching_HR9'] = finished_df['pitching_HR9'].round(3)
-
-    finished_df['pitching_BB9'] = (
-        9 * finished_df['pitching_BB']) / finished_df['pitching_IP']
-    finished_df['pitching_BB9'] = finished_df['pitching_BB9'].round(3)
-
-    finished_df['pitching_SO9'] = (
-        9 * finished_df['pitching_SO']) / finished_df['pitching_IP']
-    finished_df['pitching_SO9'] = finished_df['pitching_SO9'].round(3)
-
-    finished_df['pitching_SO/BB'] = finished_df['pitching_SO'] / \
-        finished_df['pitching_BB']
-    finished_df['pitching_SO/BB'] = finished_df['pitching_SO/BB'].round(3)
-
-    finished_df['pitching_RA9'] = 9 * \
-        (finished_df['pitching_R'] / finished_df['pitching_IP'])
-    finished_df['pitching_RA9'] = finished_df['pitching_RA9'].round(3)
-
-    # Fielding
-    finished_df['fielding_FLD%'] = (finished_df['fielding_PO'] + finished_df['fielding_A']) / (
-        finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E'])
-    finished_df['fielding_FLD%'] = finished_df['fielding_FLD%'].round(3)
-
-    finished_df['fielding_CH'] = finished_df['fielding_PO'] + \
-        finished_df['fielding_A'] + finished_df['fielding_E']
-    finished_df['fielding_CH'] = finished_df['fielding_CH'].round(3)
-
-    # finished_df['fielding_CS%'] = 0
-    # finished_df['fielding_CS%'] = finished_df['fielding_CS%'].round(3)
-
-    finished_df['fielding_RF/9'] = (9 * (finished_df['fielding_PO'] +
-                                    finished_df['fielding_A'])) / finished_df['fielding_IP']
-    finished_df['fielding_RF/9'] = finished_df['fielding_RF/9'].round(3)
-
-    # finished_df.to_csv('test.csv')
-    # print(finished_df)
-    # print(game_stats_df.columns)
-    return finished_df
+    if len(game_stats_df) > 0:
+        finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'playerId',
+                                             'first_name', 'last_name', 'full_name'], as_index=False)[[
+                                                 'G', 'GS', 'AU_POINTS',
+                                                 'batting_PA', 'batting_AB', 'batting_R',
+                                                 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI',
+                                                 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA',
+                                                 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH',
+                                                 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS',
+                                                 'pitching_SV', 'pitching_IP',
+                                                 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB',
+                                                 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls',
+                                                 'pitching_PI_strikes',
+                                                 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
+                                                 'fielding_CS', 'fielding_TC'
+                                             ]].sum()
+
+        finished_df[['G', 'GS', 'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']] = finished_df[[
+            'G', 'GS', 'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']].astype('int')
+        finished_df['pitching_IP'] = finished_df['pitching_IP'].astype('float')
+        # Batting
+        finished_df.loc[finished_df['batting_AB'] >= 1,
+                        'batting_BA'] = finished_df['batting_H'] / finished_df['batting_AB']
+        finished_df['batting_BA'] = finished_df['batting_BA'].round(3)
+
+        finished_df.loc[finished_df['batting_AB'] > 0, 'batting_OBP'] = (finished_df['batting_H'] + finished_df['batting_BB'] + finished_df['batting_HBP']) / (
+            finished_df['batting_AB'] + finished_df['batting_BB'] + finished_df['batting_HBP'] + finished_df['batting_SF'])
+        finished_df['batting_OBP'] = finished_df['batting_OBP'].round(3)
+
+        finished_df.loc[finished_df['batting_AB'] > 0,
+                        'batting_SLG'] = finished_df['batting_TB'] / finished_df['batting_AB']
+        finished_df['batting_SLG'] = finished_df['batting_SLG'].round(3)
+
+        finished_df.loc[finished_df['batting_AB'] > 0,
+                        'batting_OPS'] = finished_df['batting_OBP'] + finished_df['batting_SLG']
+        finished_df['batting_OPS'] = finished_df['batting_OPS'].round(3)
+
+        finished_df['batting_OPS+'] = None
+
+        finished_df.loc[finished_df['batting_AB'] > 0, 'batting_SecA'] = (finished_df['batting_BB'] + (
+            finished_df['batting_TB'] - finished_df['batting_H']) + (finished_df['batting_SB'] - finished_df['batting_CS'])) / finished_df['batting_AB']
+        finished_df['batting_SecA'] = finished_df['batting_SecA'].round(3)
+
+        finished_df.loc[finished_df['batting_PA'] > 0,
+                        'batting_BB%'] = finished_df['batting_BB'] / finished_df['batting_PA']
+        finished_df['batting_BB%'] = finished_df['batting_BB%'].round(3)
+
+        finished_df.loc[finished_df['batting_PA'] > 0,
+                        'batting_K%'] = finished_df['batting_K'] / finished_df['batting_PA']
+        finished_df['batting_K%'] = finished_df['batting_K%'].round(3)
+
+        finished_df.loc[finished_df['batting_AB'] > 0, 'batting_ISO'] = (
+            finished_df['batting_TB'] - finished_df['batting_H']) / finished_df['batting_AB']
+        finished_df['batting_ISO'] = finished_df['batting_ISO'].round(3)
+
+        finished_df.loc[finished_df['batting_AB'] > 0, 'batting_BABIP'] = (finished_df['batting_H'] + finished_df['batting_HR']) / (
+            finished_df['batting_AB'] - finished_df['batting_K'] - finished_df['batting_HR'] + finished_df['batting_SF'])
+        finished_df['batting_BABIP'] = finished_df['batting_BABIP'].round(3)
+
+        finished_df.loc[(finished_df['batting_SB'] > 0) | (finished_df['batting_HR'] > 0), 'batting_PSN'] = (
+            2 * finished_df['batting_HR'] * finished_df['batting_SB']) / (finished_df['batting_HR'] * finished_df['batting_SB'])
+        finished_df['batting_PSN'] = finished_df['batting_PSN'].round(3)
+
+        # Pitching
+        finished_df['pitching_ERA'] = 9 * \
+            (finished_df['pitching_ER'] / finished_df['pitching_IP'])
+        finished_df['pitching_ERA'] = finished_df['pitching_ERA'].round(3)
+
+        finished_df['pitching_ERA+'] = None
+        finished_df['pitching_FIP'] = None
+        finished_df['pitching_FIP-'] = None
+        finished_df['pitching_WHIP'] = (
+            finished_df['pitching_BB'] + finished_df['pitching_H']) / finished_df['pitching_IP']
+        finished_df['pitching_WHIP'] = finished_df['pitching_WHIP'].round(3)
+
+        finished_df['pitching_H9'] = (
+            9 * finished_df['pitching_H']) / finished_df['pitching_IP']
+        finished_df['pitching_H9'] = finished_df['pitching_H9'].round(3)
+
+        finished_df['pitching_HR9'] = (
+            9 * finished_df['pitching_HR']) / finished_df['pitching_IP']
+        finished_df['pitching_HR9'] = finished_df['pitching_HR9'].round(3)
+
+        finished_df['pitching_BB9'] = (
+            9 * finished_df['pitching_BB']) / finished_df['pitching_IP']
+        finished_df['pitching_BB9'] = finished_df['pitching_BB9'].round(3)
+
+        finished_df['pitching_SO9'] = (
+            9 * finished_df['pitching_SO']) / finished_df['pitching_IP']
+        finished_df['pitching_SO9'] = finished_df['pitching_SO9'].round(3)
+
+        finished_df['pitching_SO/BB'] = finished_df['pitching_SO'] / \
+            finished_df['pitching_BB']
+        finished_df['pitching_SO/BB'] = finished_df['pitching_SO/BB'].round(3)
+
+        finished_df['pitching_RA9'] = 9 * \
+            (finished_df['pitching_R'] / finished_df['pitching_IP'])
+        finished_df['pitching_RA9'] = finished_df['pitching_RA9'].round(3)
+
+        # Fielding
+        finished_df['fielding_FLD%'] = (finished_df['fielding_PO'] + finished_df['fielding_A']) / (
+            finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E'])
+        finished_df['fielding_FLD%'] = finished_df['fielding_FLD%'].round(3)
+
+        finished_df['fielding_CH'] = finished_df['fielding_PO'] + \
+            finished_df['fielding_A'] + finished_df['fielding_E']
+        finished_df['fielding_CH'] = finished_df['fielding_CH'].round(3)
+
+        # finished_df['fielding_CS%'] = 0
+        # finished_df['fielding_CS%'] = finished_df['fielding_CS%'].round(3)
+
+        finished_df['fielding_RF/9'] = (9 * (finished_df['fielding_PO'] +
+                                        finished_df['fielding_A'])) / finished_df['fielding_IP']
+        finished_df['fielding_RF/9'] = finished_df['fielding_RF/9'].round(3)
+
+        # finished_df.to_csv('test.csv')
+        # print(finished_df)
+        # print(game_stats_df.columns)
+        return finished_df
+    else:
+        print(f'No AU softball stats found so far in {season}')
+        return pd.DataFrame()
 
 
 def get_au_softball_season_team_stats(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) softball season, get all season team stats for an AU softball season.
 
     Parameters
@@ -860,124 +864,129 @@
     #    'pitching_HR9', 'pitching_BB9', 'pitching_SO9', 'pitching_SO/BB',
     #    'pitching_RA9', 'pitching_PI', 'pitching_PI_balls',
     #    'pitching_PI_strikes', 'fielding_position', 'fielding_IP_str',
     #    'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
     #    'fielding_FLD%', 'fielding_CS', 'fielding_CS%', 'fielding_TC',
     #    'fielding_CH', 'fielding_RF/9']
 
-    finished_df = game_stats_df.groupby(['sport', 'api_version', 'season', 'seasonId', 'teamId'], as_index=False)[[
-        'G', 'AU_POINTS',
-        'batting_PA', 'batting_AB', 'batting_R',
-        'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI',
-        'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA',
-        'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH',
-        'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS',
-        'pitching_SV', 'pitching_IP',
-        'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB',
-        'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls',
-        'pitching_PI_strikes',
-        'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
-        'fielding_CS', 'fielding_TC'
-    ]].sum()
-
-    finished_df[['G',  'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']] = finished_df[[
-        'G', 'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']].astype('int')
-    finished_df['pitching_IP'] = finished_df['pitching_IP'].astype('float')
-    # Batting
-    finished_df.loc[finished_df['batting_AB'] >= 1,
-                    'batting_BA'] = finished_df['batting_H'] / finished_df['batting_AB']
-    finished_df['batting_BA'] = finished_df['batting_BA'].round(3)
-
-    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_OBP'] = (finished_df['batting_H'] + finished_df['batting_BB'] + finished_df['batting_HBP']) / (
-        finished_df['batting_AB'] + finished_df['batting_BB'] + finished_df['batting_HBP'] + finished_df['batting_SF'])
-    finished_df['batting_OBP'] = finished_df['batting_OBP'].round(3)
-
-    finished_df.loc[finished_df['batting_AB'] > 0,
-                    'batting_SLG'] = finished_df['batting_TB'] / finished_df['batting_AB']
-    finished_df['batting_SLG'] = finished_df['batting_SLG'].round(3)
-
-    finished_df.loc[finished_df['batting_AB'] > 0,
-                    'batting_OPS'] = finished_df['batting_OBP'] + finished_df['batting_SLG']
-    finished_df['batting_OPS'] = finished_df['batting_OPS'].round(3)
-
-    finished_df['batting_OPS+'] = None
-
-    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_SecA'] = (finished_df['batting_BB'] + (
-        finished_df['batting_TB'] - finished_df['batting_H']) + (finished_df['batting_SB'] - finished_df['batting_CS'])) / finished_df['batting_AB']
-    finished_df['batting_SecA'] = finished_df['batting_SecA'].round(3)
-
-    finished_df.loc[finished_df['batting_PA'] > 0,
-                    'batting_BB%'] = finished_df['batting_BB'] / finished_df['batting_PA']
-    finished_df['batting_BB%'] = finished_df['batting_BB%'].round(3)
-
-    finished_df.loc[finished_df['batting_PA'] > 0,
-                    'batting_K%'] = finished_df['batting_K'] / finished_df['batting_PA']
-    finished_df['batting_K%'] = finished_df['batting_K%'].round(3)
-
-    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_ISO'] = (
-        finished_df['batting_TB'] - finished_df['batting_H']) / finished_df['batting_AB']
-    finished_df['batting_ISO'] = finished_df['batting_ISO'].round(3)
-
-    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_BABIP'] = (finished_df['batting_H'] + finished_df['batting_HR']) / (
-        finished_df['batting_AB'] - finished_df['batting_K'] - finished_df['batting_HR'] + finished_df['batting_SF'])
-    finished_df['batting_BABIP'] = finished_df['batting_BABIP'].round(3)
-
-    finished_df.loc[(finished_df['batting_SB'] > 0) | (finished_df['batting_HR'] > 0), 'batting_PSN'] = (
-        2 * finished_df['batting_HR'] * finished_df['batting_SB']) / (finished_df['batting_HR'] * finished_df['batting_SB'])
-    finished_df['batting_PSN'] = finished_df['batting_PSN'].round(3)
-
-    # Pitching
-    finished_df['pitching_ERA'] = 9 * \
-        (finished_df['pitching_ER'] / finished_df['pitching_IP'])
-    finished_df['pitching_ERA'] = finished_df['pitching_ERA'].round(3)
-
-    finished_df['pitching_ERA+'] = None
-    finished_df['pitching_FIP'] = None
-    finished_df['pitching_FIP-'] = None
-    finished_df['pitching_WHIP'] = (
-        finished_df['pitching_BB'] + finished_df['pitching_H']) / finished_df['pitching_IP']
-    finished_df['pitching_WHIP'] = finished_df['pitching_WHIP'].round(3)
-
-    finished_df['pitching_H9'] = (
-        9 * finished_df['pitching_H']) / finished_df['pitching_IP']
-    finished_df['pitching_H9'] = finished_df['pitching_H9'].round(3)
-
-    finished_df['pitching_HR9'] = (
-        9 * finished_df['pitching_HR']) / finished_df['pitching_IP']
-    finished_df['pitching_HR9'] = finished_df['pitching_HR9'].round(3)
-
-    finished_df['pitching_BB9'] = (
-        9 * finished_df['pitching_BB']) / finished_df['pitching_IP']
-    finished_df['pitching_BB9'] = finished_df['pitching_BB9'].round(3)
-
-    finished_df['pitching_SO9'] = (
-        9 * finished_df['pitching_SO']) / finished_df['pitching_IP']
-    finished_df['pitching_SO9'] = finished_df['pitching_SO9'].round(3)
-
-    finished_df['pitching_SO/BB'] = finished_df['pitching_SO'] / \
-        finished_df['pitching_BB']
-    finished_df['pitching_SO/BB'] = finished_df['pitching_SO/BB'].round(3)
-
-    finished_df['pitching_RA9'] = 9 * \
-        (finished_df['pitching_R'] / finished_df['pitching_IP'])
-    finished_df['pitching_RA9'] = finished_df['pitching_RA9'].round(3)
-
-    # Fielding
-    finished_df['fielding_FLD%'] = (finished_df['fielding_PO'] + finished_df['fielding_A']) / (
-        finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E'])
-    finished_df['fielding_FLD%'] = finished_df['fielding_FLD%'].round(3)
-
-    finished_df['fielding_CH'] = finished_df['fielding_PO'] + \
-        finished_df['fielding_A'] + finished_df['fielding_E']
-    finished_df['fielding_CH'] = finished_df['fielding_CH'].round(3)
-
-    # finished_df['fielding_CS%'] = 0
-    # finished_df['fielding_CS%'] = finished_df['fielding_CS%'].round(3)
-
-    finished_df['fielding_RF/9'] = (9 * (finished_df['fielding_PO'] +
-                                    finished_df['fielding_A'])) / finished_df['fielding_IP']
-    finished_df['fielding_RF/9'] = finished_df['fielding_RF/9'].round(3)
-
-    # finished_df.to_csv('test.csv')
-    # print(finished_df)
-    # print(game_stats_df.columns)
-    return finished_df
+    if len(game_stats_df) > 0:
+        finished_df = game_stats_df.groupby(['sport', 'api_version', 'season', 'seasonId', 'teamId'], as_index=False)[[
+            'G', 'AU_POINTS',
+            'batting_PA', 'batting_AB', 'batting_R',
+            'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI',
+            'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA',
+            'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH',
+            'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS',
+            'pitching_SV', 'pitching_IP',
+            'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB',
+            'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls',
+            'pitching_PI_strikes',
+            'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
+            'fielding_CS', 'fielding_TC'
+        ]].sum()
+
+        finished_df[['G',  'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']] = finished_df[[
+            'G', 'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']].astype('int')
+        finished_df['pitching_IP'] = finished_df['pitching_IP'].astype('float')
+        # Batting
+        finished_df.loc[finished_df['batting_AB'] >= 1,
+                        'batting_BA'] = finished_df['batting_H'] / finished_df['batting_AB']
+        finished_df['batting_BA'] = finished_df['batting_BA'].round(3)
+
+        finished_df.loc[finished_df['batting_AB'] > 0, 'batting_OBP'] = (finished_df['batting_H'] + finished_df['batting_BB'] + finished_df['batting_HBP']) / (
+            finished_df['batting_AB'] + finished_df['batting_BB'] + finished_df['batting_HBP'] + finished_df['batting_SF'])
+        finished_df['batting_OBP'] = finished_df['batting_OBP'].round(3)
+
+        finished_df.loc[finished_df['batting_AB'] > 0,
+                        'batting_SLG'] = finished_df['batting_TB'] / finished_df['batting_AB']
+        finished_df['batting_SLG'] = finished_df['batting_SLG'].round(3)
+
+        finished_df.loc[finished_df['batting_AB'] > 0,
+                        'batting_OPS'] = finished_df['batting_OBP'] + finished_df['batting_SLG']
+        finished_df['batting_OPS'] = finished_df['batting_OPS'].round(3)
+
+        finished_df['batting_OPS+'] = None
+
+        finished_df.loc[finished_df['batting_AB'] > 0, 'batting_SecA'] = (finished_df['batting_BB'] + (
+            finished_df['batting_TB'] - finished_df['batting_H']) + (finished_df['batting_SB'] - finished_df['batting_CS'])) / finished_df['batting_AB']
+        finished_df['batting_SecA'] = finished_df['batting_SecA'].round(3)
+
+        finished_df.loc[finished_df['batting_PA'] > 0,
+                        'batting_BB%'] = finished_df['batting_BB'] / finished_df['batting_PA']
+        finished_df['batting_BB%'] = finished_df['batting_BB%'].round(3)
+
+        finished_df.loc[finished_df['batting_PA'] > 0,
+                        'batting_K%'] = finished_df['batting_K'] / finished_df['batting_PA']
+        finished_df['batting_K%'] = finished_df['batting_K%'].round(3)
+
+        finished_df.loc[finished_df['batting_AB'] > 0, 'batting_ISO'] = (
+            finished_df['batting_TB'] - finished_df['batting_H']) / finished_df['batting_AB']
+        finished_df['batting_ISO'] = finished_df['batting_ISO'].round(3)
+
+        finished_df.loc[finished_df['batting_AB'] > 0, 'batting_BABIP'] = (finished_df['batting_H'] + finished_df['batting_HR']) / (
+            finished_df['batting_AB'] - finished_df['batting_K'] - finished_df['batting_HR'] + finished_df['batting_SF'])
+        finished_df['batting_BABIP'] = finished_df['batting_BABIP'].round(3)
+
+        finished_df.loc[(finished_df['batting_SB'] > 0) | (finished_df['batting_HR'] > 0), 'batting_PSN'] = (
+            2 * finished_df['batting_HR'] * finished_df['batting_SB']) / (finished_df['batting_HR'] * finished_df['batting_SB'])
+        finished_df['batting_PSN'] = finished_df['batting_PSN'].round(3)
+
+        # Pitching
+        finished_df['pitching_ERA'] = 9 * \
+            (finished_df['pitching_ER'] / finished_df['pitching_IP'])
+        finished_df['pitching_ERA'] = finished_df['pitching_ERA'].round(3)
+
+        finished_df['pitching_ERA+'] = None
+        finished_df['pitching_FIP'] = None
+        finished_df['pitching_FIP-'] = None
+        finished_df['pitching_WHIP'] = (
+            finished_df['pitching_BB'] + finished_df['pitching_H']) / finished_df['pitching_IP']
+        finished_df['pitching_WHIP'] = finished_df['pitching_WHIP'].round(3)
+
+        finished_df['pitching_H9'] = (
+            9 * finished_df['pitching_H']) / finished_df['pitching_IP']
+        finished_df['pitching_H9'] = finished_df['pitching_H9'].round(3)
+
+        finished_df['pitching_HR9'] = (
+            9 * finished_df['pitching_HR']) / finished_df['pitching_IP']
+        finished_df['pitching_HR9'] = finished_df['pitching_HR9'].round(3)
+
+        finished_df['pitching_BB9'] = (
+            9 * finished_df['pitching_BB']) / finished_df['pitching_IP']
+        finished_df['pitching_BB9'] = finished_df['pitching_BB9'].round(3)
+
+        finished_df['pitching_SO9'] = (
+            9 * finished_df['pitching_SO']) / finished_df['pitching_IP']
+        finished_df['pitching_SO9'] = finished_df['pitching_SO9'].round(3)
+
+        finished_df['pitching_SO/BB'] = finished_df['pitching_SO'] / \
+            finished_df['pitching_BB']
+        finished_df['pitching_SO/BB'] = finished_df['pitching_SO/BB'].round(3)
+
+        finished_df['pitching_RA9'] = 9 * \
+            (finished_df['pitching_R'] / finished_df['pitching_IP'])
+        finished_df['pitching_RA9'] = finished_df['pitching_RA9'].round(3)
+
+        # Fielding
+        finished_df['fielding_FLD%'] = (finished_df['fielding_PO'] + finished_df['fielding_A']) / (
+            finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E'])
+        finished_df['fielding_FLD%'] = finished_df['fielding_FLD%'].round(3)
+
+        finished_df['fielding_CH'] = finished_df['fielding_PO'] + \
+            finished_df['fielding_A'] + finished_df['fielding_E']
+        finished_df['fielding_CH'] = finished_df['fielding_CH'].round(3)
+
+        # finished_df['fielding_CS%'] = 0
+        # finished_df['fielding_CS%'] = finished_df['fielding_CS%'].round(3)
+
+        finished_df['fielding_RF/9'] = (9 * (finished_df['fielding_PO'] +
+                                        finished_df['fielding_A'])) / finished_df['fielding_IP']
+        finished_df['fielding_RF/9'] = finished_df['fielding_RF/9'].round(3)
+
+        # finished_df.to_csv('test.csv')
+        # print(finished_df)
+        # print(game_stats_df.columns)
+        return finished_df
+
+    else:
+        print(f'No AU softball stats found so far in {season}')
+        return pd.DataFrame()
```

### Comparing `athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/utils.py` & `athletes_unlimited_py-0.0.7/athetes_unlimited_py/utils.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.6a1/athetes_unlimited_py/volleyball.py` & `athletes_unlimited_py-0.0.7/athetes_unlimited_py/volleyball.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,72 +541,77 @@
     #    'secondary_position_lk', 'team_id', 'sets_played', 'kills',
     #    'kills_per_set', 'attack_errors', 'attack_attempts',
     #    'attack_percentage', 'assists', 'assists_per_set', 'setting_errors',
     #    'service_errors', 'service_aces', 'service_aces_per_set',
     #    'total_reception_attempts', 'reception_errors',
     #    'positive_reception_pct', 'digs', 'digs_per_set', 'blocks',
     #    'blocks_per_set', 'au_total_points']
+    if len(game_stats_df) > 0:
 
-    game_stats_df.loc[game_stats_df['sets_played'] > 0, 'G'] = 1
+        game_stats_df.loc[game_stats_df['sets_played'] > 0, 'G'] = 1
 
-    finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'playerId',
-                                         'first_name', 'last_name', 'full_name'], as_index=False)[[
-                                             'G', 'sets_played', 'kills',
-                                             'attack_errors', 'attack_attempts',
-                                             'assists', 'setting_errors',
-                                             'service_errors', 'service_aces',
-                                             'total_reception_attempts', 'reception_errors',
-                                             'digs', 'blocks',
-                                             'au_total_points']].sum()
-
-    finished_df[['G', 'sets_played', 'kills',
-                 'attack_errors', 'attack_attempts',
-                 'assists', 'setting_errors',
-                 'service_errors', 'service_aces',
-                 'total_reception_attempts', 'reception_errors',
-                 'digs', 'blocks',
-                 'au_total_points']] = finished_df[['G', 'sets_played', 'kills',
-                                                    'attack_errors', 'attack_attempts',
-                                                    'assists', 'setting_errors',
-                                                    'service_errors', 'service_aces',
-                                                    'total_reception_attempts', 'reception_errors',
-                                                    'digs', 'blocks',
-                                                    'au_total_points']].astype('int')
-
-    finished_df.loc[finished_df['sets_played'] > 0, 'kills_per_set'] = (
-        finished_df['kills']) / finished_df['sets_played']
-    finished_df['kills_per_set'] = finished_df['kills_per_set'].round(3)
-
-    finished_df.loc[finished_df['attack_attempts'] > 0, 'attack_percentage'] = (
-        finished_df['kills'] - finished_df['attack_errors']) / finished_df['attack_attempts']
-    finished_df['attack_percentage'] = finished_df['attack_percentage'].round(
-        3)
-
-    finished_df.loc[finished_df['sets_played'] > 0, 'assists_per_set'] = (
-        finished_df['assists']) / finished_df['sets_played']
-    finished_df['assists_per_set'] = finished_df['assists_per_set'].round(3)
-
-    finished_df.loc[finished_df['sets_played'] > 0, 'service_aces_per_set'] = (
-        finished_df['service_aces']) / finished_df['sets_played']
-    finished_df['service_aces_per_set'] = finished_df['service_aces_per_set'].round(
-        3)
-
-    # finished_df['positive_reception_pct'] = 0
-    # finished_df['positive_reception_pct'] = finished_df['positive_reception_pct'].round(
-    #     3)
-
-    finished_df.loc[finished_df['sets_played'] > 0, 'digs_per_set'] = (
-        finished_df['digs']) / finished_df['sets_played']
-    finished_df['digs_per_set'] = finished_df['digs_per_set'].round(3)
-
-    finished_df.loc[finished_df['sets_played'] > 0, 'blocks_per_set'] = (
-        finished_df['blocks']) / finished_df['sets_played']
-    finished_df['blocks_per_set'] = finished_df['blocks_per_set'].round(3)
-
-    return finished_df
+        finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'playerId',
+                                            'first_name', 'last_name', 'full_name'], as_index=False)[[
+                                                'G', 'sets_played', 'kills',
+                                                'attack_errors', 'attack_attempts',
+                                                'assists', 'setting_errors',
+                                                'service_errors', 'service_aces',
+                                                'total_reception_attempts', 'reception_errors',
+                                                'digs', 'blocks',
+                                                'au_total_points']].sum()
+
+        finished_df[['G', 'sets_played', 'kills',
+                    'attack_errors', 'attack_attempts',
+                     'assists', 'setting_errors',
+                     'service_errors', 'service_aces',
+                     'total_reception_attempts', 'reception_errors',
+                     'digs', 'blocks',
+                     'au_total_points']] = finished_df[['G', 'sets_played', 'kills',
+                                                       'attack_errors', 'attack_attempts',
+                                                        'assists', 'setting_errors',
+                                                        'service_errors', 'service_aces',
+                                                        'total_reception_attempts', 'reception_errors',
+                                                        'digs', 'blocks',
+                                                        'au_total_points']].astype('int')
+
+        finished_df.loc[finished_df['sets_played'] > 0, 'kills_per_set'] = (
+            finished_df['kills']) / finished_df['sets_played']
+        finished_df['kills_per_set'] = finished_df['kills_per_set'].round(3)
+
+        finished_df.loc[finished_df['attack_attempts'] > 0, 'attack_percentage'] = (
+            finished_df['kills'] - finished_df['attack_errors']) / finished_df['attack_attempts']
+        finished_df['attack_percentage'] = finished_df['attack_percentage'].round(
+            3)
+
+        finished_df.loc[finished_df['sets_played'] > 0, 'assists_per_set'] = (
+            finished_df['assists']) / finished_df['sets_played']
+        finished_df['assists_per_set'] = finished_df['assists_per_set'].round(
+            3)
+
+        finished_df.loc[finished_df['sets_played'] > 0, 'service_aces_per_set'] = (
+            finished_df['service_aces']) / finished_df['sets_played']
+        finished_df['service_aces_per_set'] = finished_df['service_aces_per_set'].round(
+            3)
+
+        # finished_df['positive_reception_pct'] = 0
+        # finished_df['positive_reception_pct'] = finished_df['positive_reception_pct'].round(
+        #     3)
+
+        finished_df.loc[finished_df['sets_played'] > 0, 'digs_per_set'] = (
+            finished_df['digs']) / finished_df['sets_played']
+        finished_df['digs_per_set'] = finished_df['digs_per_set'].round(3)
+
+        finished_df.loc[finished_df['sets_played'] > 0, 'blocks_per_set'] = (
+            finished_df['blocks']) / finished_df['sets_played']
+        finished_df['blocks_per_set'] = finished_df['blocks_per_set'].round(3)
+
+        return finished_df
+    else:
+        print(f'No AU volleyball stats found so far in {season}')
+        return pd.DataFrame()
 
 
 def get_au_volleyball_season_team_stats(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) volleyball season, get all season team stats for an AU volleyball season.
 
     Parameters
@@ -628,63 +633,70 @@
     #    'secondary_position_lk', 'team_id', 'sets_played', 'kills',
     #    'kills_per_set', 'attack_errors', 'attack_attempts',
     #    'attack_percentage', 'assists', 'assists_per_set', 'setting_errors',
     #    'service_errors', 'service_aces', 'service_aces_per_set',
     #    'total_reception_attempts', 'reception_errors',
     #    'positive_reception_pct', 'digs', 'digs_per_set', 'blocks',
     #    'blocks_per_set', 'au_total_points']
-    game_stats_df['G'] = 1
 
-    finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'team_id'], as_index=False)[[
-        'G', 'sets_played', 'kills',
-        'attack_errors', 'attack_attempts',
-        'assists', 'setting_errors',
-        'service_errors', 'service_aces',
-        'total_reception_attempts', 'reception_errors',
-        'digs', 'blocks',
-        'au_total_points']].sum()
-
-    finished_df[['G', 'sets_played', 'kills',
-                 'attack_errors', 'attack_attempts',
-                 'assists', 'setting_errors',
-                 'service_errors', 'service_aces',
-                 'total_reception_attempts', 'reception_errors',
-                 'digs', 'blocks',
-                 'au_total_points']] = finished_df[['G', 'sets_played', 'kills',
-                                                    'attack_errors', 'attack_attempts',
-                                                    'assists', 'setting_errors',
-                                                    'service_errors', 'service_aces',
-                                                    'total_reception_attempts', 'reception_errors',
-                                                    'digs', 'blocks',
-                                                    'au_total_points']].astype('int')
-
-    finished_df.loc[finished_df['sets_played'] > 0, 'kills_per_set'] = (
-        finished_df['kills']) / finished_df['sets_played']
-    finished_df['kills_per_set'] = finished_df['kills_per_set'].round(3)
-
-    finished_df.loc[finished_df['attack_attempts'] > 0, 'attack_percentage'] = (
-        finished_df['kills'] - finished_df['attack_errors']) / finished_df['attack_attempts']
-    finished_df['attack_percentage'] = finished_df['attack_percentage'].round(
-        3)
-
-    finished_df.loc[finished_df['sets_played'] > 0, 'assists_per_set'] = (
-        finished_df['assists']) / finished_df['sets_played']
-    finished_df['assists_per_set'] = finished_df['assists_per_set'].round(3)
-
-    finished_df.loc[finished_df['sets_played'] > 0, 'service_aces_per_set'] = (
-        finished_df['service_aces']) / finished_df['sets_played']
-    finished_df['service_aces_per_set'] = finished_df['service_aces_per_set'].round(
-        3)
-
-    # finished_df['positive_reception_pct'] = 0
-    # finished_df['positive_reception_pct'] = finished_df['positive_reception_pct'].round(
-    #     3)
-
-    finished_df.loc[finished_df['sets_played'] > 0, 'digs_per_set'] = (
-        finished_df['digs']) / finished_df['sets_played']
-    finished_df['digs_per_set'] = finished_df['digs_per_set'].round(3)
-
-    finished_df.loc[finished_df['sets_played'] > 0, 'blocks_per_set'] = (
-        finished_df['blocks']) / finished_df['sets_played']
-    finished_df['blocks_per_set'] = finished_df['blocks_per_set'].round(3)
+    if len(game_stats_df) > 0:
+
+        game_stats_df['G'] = 1
 
-    return finished_df
+        finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'team_id'], as_index=False)[[
+            'G', 'sets_played', 'kills',
+            'attack_errors', 'attack_attempts',
+            'assists', 'setting_errors',
+            'service_errors', 'service_aces',
+            'total_reception_attempts', 'reception_errors',
+            'digs', 'blocks',
+            'au_total_points']].sum()
+
+        finished_df[['G', 'sets_played', 'kills',
+                    'attack_errors', 'attack_attempts',
+                     'assists', 'setting_errors',
+                     'service_errors', 'service_aces',
+                     'total_reception_attempts', 'reception_errors',
+                     'digs', 'blocks',
+                     'au_total_points']] = finished_df[['G', 'sets_played', 'kills',
+                                                       'attack_errors', 'attack_attempts',
+                                                        'assists', 'setting_errors',
+                                                        'service_errors', 'service_aces',
+                                                        'total_reception_attempts', 'reception_errors',
+                                                        'digs', 'blocks',
+                                                        'au_total_points']].astype('int')
+
+        finished_df.loc[finished_df['sets_played'] > 0, 'kills_per_set'] = (
+            finished_df['kills']) / finished_df['sets_played']
+        finished_df['kills_per_set'] = finished_df['kills_per_set'].round(3)
+
+        finished_df.loc[finished_df['attack_attempts'] > 0, 'attack_percentage'] = (
+            finished_df['kills'] - finished_df['attack_errors']) / finished_df['attack_attempts']
+        finished_df['attack_percentage'] = finished_df['attack_percentage'].round(
+            3)
+
+        finished_df.loc[finished_df['sets_played'] > 0, 'assists_per_set'] = (
+            finished_df['assists']) / finished_df['sets_played']
+        finished_df['assists_per_set'] = finished_df['assists_per_set'].round(
+            3)
+
+        finished_df.loc[finished_df['sets_played'] > 0, 'service_aces_per_set'] = (
+            finished_df['service_aces']) / finished_df['sets_played']
+        finished_df['service_aces_per_set'] = finished_df['service_aces_per_set'].round(
+            3)
+
+        # finished_df['positive_reception_pct'] = 0
+        # finished_df['positive_reception_pct'] = finished_df['positive_reception_pct'].round(
+        #     3)
+
+        finished_df.loc[finished_df['sets_played'] > 0, 'digs_per_set'] = (
+            finished_df['digs']) / finished_df['sets_played']
+        finished_df['digs_per_set'] = finished_df['digs_per_set'].round(3)
+
+        finished_df.loc[finished_df['sets_played'] > 0, 'blocks_per_set'] = (
+            finished_df['blocks']) / finished_df['sets_played']
+        finished_df['blocks_per_set'] = finished_df['blocks_per_set'].round(3)
+
+        return finished_df
+    else:
+        print(f'No AU volleyball stats found so far in {season}')
+        return pd.DataFrame()
```

### Comparing `athletes_unlimited_py-0.0.6a1/athletes_unlimited_py.egg-info/PKG-INFO` & `athletes_unlimited_py-0.0.7/athletes_unlimited_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athletes-unlimited-py
-Version: 0.0.6a1
+Version: 0.0.7
 Summary: Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/athletes-unlimited-py
 Project-URL: documentation, https://github.com/armstjc/athletes-unlimited-py/wiki
 Project-URL: repository, https://github.com/armstjc/athletes-unlimited-py.git
```

### Comparing `athletes_unlimited_py-0.0.6a1/pyproject.toml` & `athletes_unlimited_py-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools","wheel","pyarrow","pandas","tqdm","requests","lxml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "athletes_unlimited_py"
-version = "0.0.6a1"
+version = "0.0.7"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
 
 authors = [
     {name = "Joseph Armstrong", email="armstrongjoseph08@gmail.com"}
 ]
```

