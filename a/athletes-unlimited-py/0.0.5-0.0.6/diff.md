# Comparing `tmp/athletes_unlimited_py-0.0.5.tar.gz` & `tmp/athletes_unlimited_py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athletes_unlimited_py-0.0.5.tar", last modified: Sun May 14 22:07:23 2023, max compression
+gzip compressed data, was "athletes_unlimited_py-0.0.6.tar", last modified: Sat May 27 04:00:34 2023, max compression
```

## Comparing `athletes_unlimited_py-0.0.5.tar` & `athletes_unlimited_py-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:07:23.595607 athletes_unlimited_py-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-14 22:07:23.595607 athletes_unlimited_py-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:07:23.595607 athletes_unlimited_py-0.0.5/athetes_unlimited_py/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26277 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/aux_softball.py
--rw-r--r--   0 runner    (1001) docker     (123)    31440 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/basketball.py
--rw-r--r--   0 runner    (1001) docker     (123)    30879 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/lacrosse.py
--rw-r--r--   0 runner    (1001) docker     (123)    47197 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/softball.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30686 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/volleyball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:07:23.595607 athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-14 22:07:23.000000 athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-14 22:07:23.000000 athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 22:07:23.000000 athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-14 22:07:23.000000 athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-14 22:07:23.000000 athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 22:07:23.595607 athletes_unlimited_py-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:00:34.922721 athletes_unlimited_py-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-27 04:00:09.000000 athletes_unlimited_py-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-27 04:00:34.922721 athletes_unlimited_py-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-27 04:00:09.000000 athletes_unlimited_py-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:00:34.922721 athletes_unlimited_py-0.0.6/athetes_unlimited_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-27 04:00:09.000000 athletes_unlimited_py-0.0.6/athetes_unlimited_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26330 2023-05-27 04:00:09.000000 athletes_unlimited_py-0.0.6/athetes_unlimited_py/aux_softball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31493 2023-05-27 04:00:09.000000 athletes_unlimited_py-0.0.6/athetes_unlimited_py/basketball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31526 2023-05-27 04:00:09.000000 athletes_unlimited_py-0.0.6/athetes_unlimited_py/lacrosse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48904 2023-05-27 04:00:09.000000 athletes_unlimited_py-0.0.6/athetes_unlimited_py/softball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-27 04:00:09.000000 athletes_unlimited_py-0.0.6/athetes_unlimited_py/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30686 2023-05-27 04:00:09.000000 athletes_unlimited_py-0.0.6/athetes_unlimited_py/volleyball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:00:34.922721 athletes_unlimited_py-0.0.6/athletes_unlimited_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-27 04:00:34.000000 athletes_unlimited_py-0.0.6/athletes_unlimited_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-27 04:00:34.000000 athletes_unlimited_py-0.0.6/athletes_unlimited_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 04:00:34.000000 athletes_unlimited_py-0.0.6/athletes_unlimited_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-27 04:00:34.000000 athletes_unlimited_py-0.0.6/athletes_unlimited_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 04:00:34.000000 athletes_unlimited_py-0.0.6/athletes_unlimited_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-27 04:00:09.000000 athletes_unlimited_py-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 04:00:34.922721 athletes_unlimited_py-0.0.6/setup.cfg
```

### Comparing `athletes_unlimited_py-0.0.5/LICENSE` & `athletes_unlimited_py-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.5/PKG-INFO` & `athletes_unlimited_py-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athletes_unlimited_py
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/athletes-unlimited-py
 Project-URL: documentation, https://github.com/armstjc/athletes-unlimited-py/wiki
 Project-URL: repository, https://github.com/armstjc/athletes-unlimited-py.git
```

### Comparing `athletes_unlimited_py-0.0.5/README.md` & `athletes_unlimited_py-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.5/athetes_unlimited_py/aux_softball.py` & `athletes_unlimited_py-0.0.6/athetes_unlimited_py/aux_softball.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,16 +67,18 @@
     sport_json_data = json.loads(response.text)
 
     for i in sport_json_data['data']:
         # print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
+            count = 0
             for j in tqdm(i['gameIds']):
-                print(f'\nOn game {j} of {len_game_ids} for {season}.')
+                count += 1
+                print(f'\nOn game {count} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_softball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
                 game_df = get_au_softball_pbp(seasonId, j)
```

### Comparing `athletes_unlimited_py-0.0.5/athetes_unlimited_py/basketball.py` & `athletes_unlimited_py-0.0.6/athetes_unlimited_py/basketball.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,16 +433,18 @@
     sport_json_data = json.loads(response.text)
 
     for i in tqdm(sport_json_data['data']):
         # print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
+            count = 0
             for j in tqdm(i['gameIds']):
-                print(f'\nOn game {j} of {len_game_ids} for {season}.')
+                count += 1
+                print(f'\nOn game {count} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_basketball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
                 game_df = get_au_basketball_pbp(season, j)
```

### Comparing `athletes_unlimited_py-0.0.5/athetes_unlimited_py/lacrosse.py` & `athletes_unlimited_py-0.0.6/athetes_unlimited_py/lacrosse.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,18 +415,19 @@
 
     response = requests.get(url, headers=headers)
     sport_json_data = json.loads(response.text)
 
     for i in sport_json_data['data']:
         # print(i)
         if i['seasonId'] == season_id:
-            # len_game_ids = len(i['gameIds'])
-
+            len_game_ids = len(i['gameIds'])
+            count = 0
             for j in tqdm(i['gameIds']):
-                print(f'\nOn game ID {j} in {season}.')
+                count += 1
+                print(f'\nOn game ID {count} of {len_game_ids} in {season}.')
                 # try:
                 #     game_df = get_lacrosse_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
                 game_df = get_au_lacrosse_pbp(season_id, j)
@@ -561,58 +562,63 @@
     #    'shotsSaved', 'shotsOnGoal', 'yellowCards', 'redCards',
     #    'shotClockViolationsCommitted', 'shotClockViolationsDrawn',
     #    'auTotalPoints', 'goalie_gamesPlayed', 'goalie_gamesStarted',
     #    'goalie_goalsAgainst', 'goalie_saves', 'goalie_savePct',
     #    'goalie_shotsFaced', 'goalie_shotClockViolationsCommitted',
     #    'goalie_shotClockViolationsDrawn']
     game_stats_df['G'] = 1
+    if len(game_stats_df) > 0:
+        finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'playerId',
+                                             'first_name', 'last_name', 'full_name'], as_index=False)[[
+                                                 'G', 'periodsPlayed',
+                                                 'goals', 'assists', 'points', 'shots', 'turnovers', 'causedTurnovers',
+                                                 'groundballs', 'twoPointGoals', 'drawControls',
+                                                 'shotsSaved', 'shotsOnGoal', 'yellowCards', 'redCards',
+                                                 'shotClockViolationsCommitted', 'shotClockViolationsDrawn',
+                                                 'auTotalPoints', 'goalie_gamesPlayed', 'goalie_gamesStarted',
+                                                 'goalie_goalsAgainst', 'goalie_saves',
+                                                 'goalie_shotsFaced', 'goalie_shotClockViolationsCommitted',
+                                                 'goalie_shotClockViolationsDrawn'
+                                             ]].sum()
 
-    finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'playerId',
-                                         'first_name', 'last_name', 'full_name'], as_index=False)[[
-                                             'G', 'periodsPlayed',
-                                             'goals', 'assists', 'points', 'shots', 'turnovers', 'causedTurnovers',
-                                             'groundballs', 'twoPointGoals', 'drawControls',
-                                             'shotsSaved', 'shotsOnGoal', 'yellowCards', 'redCards',
-                                             'shotClockViolationsCommitted', 'shotClockViolationsDrawn',
-                                             'auTotalPoints', 'goalie_gamesPlayed', 'goalie_gamesStarted',
-                                             'goalie_goalsAgainst', 'goalie_saves',
-                                             'goalie_shotsFaced', 'goalie_shotClockViolationsCommitted',
-                                             'goalie_shotClockViolationsDrawn'
-                                         ]].sum()
-
-    finished_df[['G', 'periodsPlayed',
-                 'goals', 'assists', 'points', 'shots', 'turnovers', 'causedTurnovers',
-                 'groundballs', 'twoPointGoals', 'drawControls',
-                 'shotsSaved', 'shotsOnGoal', 'yellowCards', 'redCards',
-                 'shotClockViolationsCommitted', 'shotClockViolationsDrawn',
-                 'auTotalPoints', 'goalie_gamesPlayed', 'goalie_gamesStarted',
-                 'goalie_goalsAgainst', 'goalie_saves',
-                 'goalie_shotsFaced', 'goalie_shotClockViolationsCommitted',
-                 'goalie_shotClockViolationsDrawn']] = finished_df[[
-                     'G', 'periodsPlayed',
+        finished_df[['G', 'periodsPlayed',
                      'goals', 'assists', 'points', 'shots', 'turnovers', 'causedTurnovers',
                      'groundballs', 'twoPointGoals', 'drawControls',
                      'shotsSaved', 'shotsOnGoal', 'yellowCards', 'redCards',
                      'shotClockViolationsCommitted', 'shotClockViolationsDrawn',
                      'auTotalPoints', 'goalie_gamesPlayed', 'goalie_gamesStarted',
                      'goalie_goalsAgainst', 'goalie_saves',
                      'goalie_shotsFaced', 'goalie_shotClockViolationsCommitted',
-                     'goalie_shotClockViolationsDrawn']].astype('int')
-
-    finished_df['shotPct'] = finished_df['goals'] / finished_df['shots']
-    finished_df['shotPct'] = finished_df['shotPct'].round(3)
-
-    finished_df['sogPct'] = finished_df['shotsOnGoal'] / finished_df['shots']
-    finished_df['sogPct'] = finished_df['sogPct'].round(3)
-
-    finished_df['goalie_savePct'] = finished_df['goalie_goalsAgainst'] / \
-        finished_df['goalie_shotsFaced']
-    finished_df['goalie_savePct'] = finished_df['goalie_savePct'].round(3)
-
-    return finished_df
+                     'goalie_shotClockViolationsDrawn']] = finished_df[[
+                         'G', 'periodsPlayed',
+                         'goals', 'assists', 'points', 'shots', 'turnovers', 'causedTurnovers',
+                         'groundballs', 'twoPointGoals', 'drawControls',
+                         'shotsSaved', 'shotsOnGoal', 'yellowCards', 'redCards',
+                         'shotClockViolationsCommitted', 'shotClockViolationsDrawn',
+                         'auTotalPoints', 'goalie_gamesPlayed', 'goalie_gamesStarted',
+                         'goalie_goalsAgainst', 'goalie_saves',
+                         'goalie_shotsFaced', 'goalie_shotClockViolationsCommitted',
+                         'goalie_shotClockViolationsDrawn']].astype('int')
+
+        finished_df['shotPct'] = finished_df['goals'] / finished_df['shots']
+        finished_df['shotPct'] = finished_df['shotPct'].round(3)
+
+        finished_df['sogPct'] = finished_df['shotsOnGoal'] / \
+            finished_df['shots']
+        finished_df['sogPct'] = finished_df['sogPct'].round(3)
+
+        finished_df['goalie_savePct'] = finished_df['goalie_goalsAgainst'] / \
+            finished_df['goalie_shotsFaced']
+        finished_df['goalie_savePct'] = finished_df['goalie_savePct'].round(3)
+
+        return finished_df
+
+    else:
+        print(f'No lacrosse stats found in {season}.')
+        return pd.DataFrame()
 
 
 def get_au_lacrosse_season_team_stats(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) lacrosse season, get all season team stats for an AU lacrosse season.
 
     Parameters
@@ -636,49 +642,54 @@
     #    'shotClockViolationsCommitted', 'shotClockViolationsDrawn',
     #    'auTotalPoints', 'goalie_gamesPlayed', 'goalie_gamesStarted',
     #    'goalie_goalsAgainst', 'goalie_saves', 'goalie_savePct',
     #    'goalie_shotsFaced', 'goalie_shotClockViolationsCommitted',
     #    'goalie_shotClockViolationsDrawn']
     game_stats_df['G'] = 1
 
-    finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'teamId'], as_index=False)[[
-        'G', 'periodsPlayed',
-        'goals', 'assists', 'points', 'shots', 'turnovers', 'causedTurnovers',
-        'groundballs', 'twoPointGoals', 'drawControls',
-        'shotsSaved', 'shotsOnGoal', 'yellowCards', 'redCards',
-        'shotClockViolationsCommitted', 'shotClockViolationsDrawn',
-        'auTotalPoints', 'goalie_gamesPlayed', 'goalie_gamesStarted',
-        'goalie_goalsAgainst', 'goalie_saves',
-        'goalie_shotsFaced', 'goalie_shotClockViolationsCommitted',
-        'goalie_shotClockViolationsDrawn'
-    ]].sum()
-
-    finished_df[['G', 'periodsPlayed',
-                 'goals', 'assists', 'points', 'shots', 'turnovers', 'causedTurnovers',
-                 'groundballs', 'twoPointGoals', 'drawControls',
-                 'shotsSaved', 'shotsOnGoal', 'yellowCards', 'redCards',
-                 'shotClockViolationsCommitted', 'shotClockViolationsDrawn',
-                 'auTotalPoints', 'goalie_gamesPlayed', 'goalie_gamesStarted',
-                 'goalie_goalsAgainst', 'goalie_saves',
-                 'goalie_shotsFaced', 'goalie_shotClockViolationsCommitted',
-                 'goalie_shotClockViolationsDrawn']] = finished_df[[
-                     'G', 'periodsPlayed',
-                     'goals', 'assists', 'points', 'shots', 'turnovers', 'causedTurnovers',
+    if len(game_stats_df) > 0:
+        finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'teamId'], as_index=False)[[
+            'G', 'periodsPlayed',
+            'goals', 'assists', 'points', 'shots', 'turnovers', 'causedTurnovers',
+            'groundballs', 'twoPointGoals', 'drawControls',
+            'shotsSaved', 'shotsOnGoal', 'yellowCards', 'redCards',
+            'shotClockViolationsCommitted', 'shotClockViolationsDrawn',
+            'auTotalPoints', 'goalie_gamesPlayed', 'goalie_gamesStarted',
+            'goalie_goalsAgainst', 'goalie_saves',
+            'goalie_shotsFaced', 'goalie_shotClockViolationsCommitted',
+            'goalie_shotClockViolationsDrawn'
+        ]].sum()
+
+        finished_df[['G', 'periodsPlayed',
+                    'goals', 'assists', 'points', 'shots', 'turnovers', 'causedTurnovers',
                      'groundballs', 'twoPointGoals', 'drawControls',
                      'shotsSaved', 'shotsOnGoal', 'yellowCards', 'redCards',
                      'shotClockViolationsCommitted', 'shotClockViolationsDrawn',
                      'auTotalPoints', 'goalie_gamesPlayed', 'goalie_gamesStarted',
                      'goalie_goalsAgainst', 'goalie_saves',
                      'goalie_shotsFaced', 'goalie_shotClockViolationsCommitted',
-                     'goalie_shotClockViolationsDrawn']].astype('int')
-
-    finished_df['shotPct'] = finished_df['goals'] / finished_df['shots']
-    finished_df['shotPct'] = finished_df['shotPct'].round(3)
-
-    finished_df['sogPct'] = finished_df['shotsOnGoal'] / finished_df['shots']
-    finished_df['sogPct'] = finished_df['sogPct'].round(3)
-
-    finished_df['goalie_savePct'] = finished_df['goalie_goalsAgainst'] / \
-        finished_df['goalie_shotsFaced']
-    finished_df['goalie_savePct'] = finished_df['goalie_savePct'].round(3)
-
-    return finished_df
+                     'goalie_shotClockViolationsDrawn']] = finished_df[[
+                         'G', 'periodsPlayed',
+                         'goals', 'assists', 'points', 'shots', 'turnovers', 'causedTurnovers',
+                         'groundballs', 'twoPointGoals', 'drawControls',
+                         'shotsSaved', 'shotsOnGoal', 'yellowCards', 'redCards',
+                         'shotClockViolationsCommitted', 'shotClockViolationsDrawn',
+                         'auTotalPoints', 'goalie_gamesPlayed', 'goalie_gamesStarted',
+                         'goalie_goalsAgainst', 'goalie_saves',
+                         'goalie_shotsFaced', 'goalie_shotClockViolationsCommitted',
+                         'goalie_shotClockViolationsDrawn']].astype('int')
+
+        finished_df['shotPct'] = finished_df['goals'] / finished_df['shots']
+        finished_df['shotPct'] = finished_df['shotPct'].round(3)
+
+        finished_df['sogPct'] = finished_df['shotsOnGoal'] / \
+            finished_df['shots']
+        finished_df['sogPct'] = finished_df['sogPct'].round(3)
+
+        finished_df['goalie_savePct'] = finished_df['goalie_goalsAgainst'] / \
+            finished_df['goalie_shotsFaced']
+        finished_df['goalie_savePct'] = finished_df['goalie_savePct'].round(3)
+
+        return finished_df
+    else:
+        print(f'No lacrosse stats found in {season}.')
+        return pd.DataFrame()
```

### Comparing `athletes_unlimited_py-0.0.5/athetes_unlimited_py/softball.py` & `athletes_unlimited_py-0.0.6/athetes_unlimited_py/softball.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,180 +1,190 @@
 import json
 import time
-#from urllib.request import urlopen
+# from urllib.request import urlopen
 
 import pandas as pd
 import requests
 from tqdm import tqdm
 
 from athetes_unlimited_py.utils import raise_html_status_code
 
 ############################################################################################################################################################################################################################################################
 ##
-## Softball-only utilities
+# Softball-only utilities
 ##
 ############################################################################################################################################################################################################################################################
 
-def get_au_softball_season(season_id:int) -> int:
+
+def get_au_softball_season(season_id: int) -> int:
     """
     Given a season ID, `get_au_softball_season()` returns the proper season for the corresponding Athletes Unlimited softball season.
 
     Parameters
     ----------
     `season_id` (int, mandatory):
         The season ID you want a season for in Athletes Unlimited softball. 
         If there isn't a season for the inputted `season_id`, a `ValueError()` exception will be raised.
-    
+
     Returns
     ----------
     The proper season corresponding to an Athletes Unlimited softball season ID.
     """
-    #season = 0
-    
+    # season = 0
+
     if season_id == 2:
-        season= 2020
+        season = 2020
         return season
     elif season_id == 4:
         season = 2021
-        return season 
-    elif season_id == 13: # AUX = 39, non-AUX = 13
+        return season
+    elif season_id == 13:  # AUX = 39, non-AUX = 13
         season = 2022
         return season
     elif season_id == 39:
         season = 2022
         return season
-    elif season_id == 14: # AUX = 106, non-AUX = 14
+    elif season_id == 14:  # AUX = 106, non-AUX = 14
         season = 2023
-        return season 
+        return season
     elif season_id == 106:
         season = 2023
-        return season 
+        return season
     else:
-        raise ValueError(f'[season] can only be 2022 or 2023 at this time for softball.\nYou entered :\n\t{season_id}')
+        raise ValueError(
+            f'[season] can only be 2022 or 2023 at this time for softball.\nYou entered :\n\t{season_id}')
+
 
-def get_au_softball_season_id(season:int) -> int:
+def get_au_softball_season_id(season: int) -> int:
     """
     Given a season, `get_au_softball_season_id()` returns the proper season ID for the Athletes Unlimited softball season.
 
     Parameters
     ----------
     `season` (int, mandatory):
         The season you want a season ID for softball. 
         If there isn't a season ID for the inputted `season`, a `ValueError()` exception will be raised.
-    
+
     Returns
     ----------
     The proper season ID corresponding to an Athletes Unlimited softball season.
     """
     seasonId = 0
-    
+
     if season == 2020:
         seasonId = 2
         return seasonId
     elif season == 2021:
         seasonId = 4
-        return seasonId 
+        return seasonId
     elif season == 2022:
         seasonId = 13
-        return seasonId 
+        return seasonId
     elif season == 2023:
         seasonId = 14
-        return seasonId 
+        return seasonId
     else:
-        raise ValueError(f'[season] can only be 2022 or 2023 at this time for softball.\nYou entered :\n\t{season}')
+        raise ValueError(
+            f'[season] can only be 2022 or 2023 at this time for softball.\nYou entered :\n\t{season}')
 
 ############################################################################################################################################################################################################################################################
 ##
-## Game Functions
+# Game Functions
 ##
 ############################################################################################################################################################################################################################################################
 
-def get_au_softball_game_stats(season_id:int,game_num:int,get_team_stats=False,get_player_and_team_stats=False,rename_cols=False) -> pd.DataFrame():
+
+def get_au_softball_game_stats(season_id: int, game_num: int, get_team_stats=False, get_player_and_team_stats=False, rename_cols=False) -> pd.DataFrame():
     """
     Retrieves the player and/or team game stats for an Atheltes Unlimited (AU) softball game.
 
     Parameters
     ----------
     `season_id` (int, mandatory):
         The AU softball season ID you want a game from.
-    
+
     `game_num` (int, mandatory):
         The game number you want player and/or team stats from.
         This is not the game ID!
         A `ValueError` will be raised if `game_num` is set to less than 1.
-    
+
     `get_team_stats` (bool, optional) = False:
         Optional boolean argument. 
         If set to `True`, the pandas DataFrame returned by `get_softball_game_stats()` will only return team stats for that game, 
         and will not return player stats, unless `get_player_and_team_stats` is set to `True` if `get_team_stats` is set to `True`.
-    
+
     `get_player_and_team_stats` (bool, optional) = False:
 
     `rename_cols` (bool, optional) = False:
         NOT IMPLEMENTED YET!
         `get_softball_game_stats()` will have no change in functionality at this time if `rename_cols` is set to `True`.
-        
+
 
     Returns
     ----------
     A pandas DataFrame containing player and/or team stats for a given AU game within a given AU season ID.
     """
 
-    headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
     player_stats_df = pd.DataFrame()
     team_stats_df = pd.DataFrame()
     row_df = pd.DataFrame()
-    
+
     # season_id = get_au_softball_season_id(season)
     # season = get_au_softball_season(season_id)
 
     if game_num < 1:
         raise ValueError('`game_num` cannot be less than 0.')
-    
-    key = int(time.time()) # Yes, the key is literaly the int of the Epoch time at the time of the GET request.
-    
+
+    # Yes, the key is literaly the int of the Epoch time at the time of the GET request.
+    key = int(time.time())
+
     url = f"https://auprosports.com/proxy.php?request=/api/stats/softball/v1/{season_id}/by-game/{game_num}?statType=batting%26statType=pitching%26statType=fielding%26k={key}"
-    
-    response = requests.get(url,headers=headers)
+
+    response = requests.get(url, headers=headers)
     raise_html_status_code(response.status_code)
-    
+
     json_data = json.loads(response.text)
 
     sport = json_data['metaSport']['sport']
     api_version = json_data['metaSport']['version']
 
     for i in tqdm(json_data['data']):
-        row_df = pd.DataFrame({'sport':sport,'api_version':api_version},index=[0])
-        
+        row_df = pd.DataFrame(
+            {'sport': sport, 'api_version': api_version}, index=[0])
+
         ##############################################################################################################################
-        ## Player/Team info
+        # Player/Team info
         ##############################################################################################################################
-        row_df['season'] = get_au_softball_season(i['seasonId'])
+        season = get_au_softball_season(i['seasonId'])
+        row_df['season'] = season
         row_df['seasonId'] = i['seasonId']
         row_df['weekNumber'] = 0
         row_df['gameNumber'] = 0
         row_df['seasonType'] = ""
 
         row_df['playerId'] = i['playerId']
         row_df['uniformNumber'] = i['uniformNumber']
         row_df['uniformNumberDisplay'] = str(i['uniformNumberDisplay'])
-        
+
         row_df['primaryPositionLk'] = i['primaryPositionLk']
         row_df['secondaryPositionLk'] = i['secondaryPositionLk']
-        row_df['first_name'] = str(i['firstName']).replace('\u2019','\'')
-        row_df['last_name'] = str(i['lastName']).replace('\u2019','\'')
-        row_df['full_name'] = f"{i['firstName']} {i['lastName']}".replace('\u2019','\'')
+        row_df['first_name'] = str(i['firstName']).replace('\u2019', '\'')
+        row_df['last_name'] = str(i['lastName']).replace('\u2019', '\'')
+        row_df['full_name'] = f"{i['firstName']} {i['lastName']}".replace(
+            '\u2019', '\'')
 
         ##############################################################################################################################
-        ## Catching Stats
-        ## An endpoint sugests that this is a thing in their API, but no data can be found here.
+        # Catching Stats
+        # An endpoint sugests that this is a thing in their API, but no data can be found here.
         ##############################################################################################################################
 
         ##############################################################################################################################
-        ## Batting Stats
+        # Batting Stats
         ##############################################################################################################################
         if len(i['battingStats']) > 0:
             row_df['week'] = i['battingStats'][0]['weekNumber']
             row_df['game_num'] = i['battingStats'][0]['gameNumber']
             row_df['season_type'] = i['battingStats'][0]['gamesStarted']
             row_df['G'] = i['battingStats'][0]['gamesPlayed']
             row_df['GS'] = i['battingStats'][0]['gamesStarted']
@@ -196,15 +206,17 @@
             row_df['batting_OBP'] = i['battingStats'][0]['onBasePercentage']
             row_df['batting_SLG'] = i['battingStats'][0]['sluggingPercentage']
             row_df['batting_TB'] = i['battingStats'][0]['totalBases']
             row_df['batting_SF'] = i['battingStats'][0]['sacrificeFly']
             row_df['batting_SH'] = i['battingStats'][0]['sacrificeHit']
             row_df['AU_POINTS'] = i['battingStats'][0]['auTotalPoints']
 
-            row_df['batting_PA'] = row_df['batting_AB'] + row_df['batting_BB'] + row_df['batting_HBP'] + row_df['batting_SF'] + row_df['batting_SH']
+            row_df['batting_PA'] = row_df['batting_AB'] + row_df['batting_BB'] + \
+                row_df['batting_HBP'] + \
+                row_df['batting_SF'] + row_df['batting_SH']
         else:
             row_df['batting_AB'] = None
             row_df['batting_R'] = None
             row_df['batting_H'] = None
             row_df['batting_2B'] = None
             row_df['batting_3B'] = None
             row_df['batting_HR'] = None
@@ -219,206 +231,226 @@
             row_df['batting_OBP'] = None
             row_df['batting_SLG'] = None
             row_df['batting_TB'] = None
             row_df['batting_SF'] = None
             row_df['batting_SH'] = None
 
         ##############################################################################################################################
-        ## Pitching Stats
+        # Pitching Stats
         ##############################################################################################################################
 
         if len(i['pitchingStats']) > 0:
             row_df['week'] = i['pitchingStats'][0]['weekNumber']
             row_df['game_num'] = i['pitchingStats'][0]['gameNumber']
 
             row_df['G'] = i['pitchingStats'][0]['appearances']
             row_df['GS'] = i['pitchingStats'][0]['gamesStarted']
             row_df['pitching_W'] = i['pitchingStats'][0]['wins']
             row_df['pitching_L'] = i['pitchingStats'][0]['losses']
             row_df['pitching_ERA'] = i['pitchingStats'][0]['earnedRunAverage']
             row_df['pitching_SHO'] = i['pitchingStats'][0]['shutout']
             row_df['pitching_CG'] = i['pitchingStats'][0]['completeGames']
             row_df['pitching_SV'] = i['pitchingStats'][0]['saves']
-            row_df['pitching_IP_str'] = str(i['pitchingStats'][0]['inningsPitched'])
-            row_df['pitching_IP_str'] = row_df['pitching_IP_str'].replace('None',None)
+            row_df['pitching_IP_str'] = str(
+                i['pitchingStats'][0]['inningsPitched'])
+            row_df['pitching_IP_str'] = row_df['pitching_IP_str'].replace(
+                'None', None)
 
             try:
-                row_df['pitching_IP'] = float(str(i['pitchingStats'][0]['inningsPitched']).replace('.1','.333').replace('.2','.667'))
+                row_df['pitching_IP'] = float(str(i['pitchingStats'][0]['inningsPitched']).replace(
+                    '.1', '.333').replace('.2', '.667'))
             except:
                 row_df['pitching_IP'] = None
 
             row_df['pitching_QS'] = 0
             row_df['pitching_H'] = i['pitchingStats'][0]['hits']
             row_df['pitching_R'] = i['pitchingStats'][0]['runs']
             row_df['pitching_ER'] = i['pitchingStats'][0]['earnedRuns']
             row_df['pitching_HR'] = i['pitchingStats'][0]['homeRuns']
             row_df['pitching_BB'] = i['pitchingStats'][0]['baseOnBalls']
             row_df['pitching_SO'] = i['pitchingStats'][0]['strikeOuts']
             row_df['pitching_HBP'] = i['pitchingStats'][0]['hitByPitch']
             row_df['pitching_WP'] = i['pitchingStats'][0]['wildPitch']
-            row_df['pitching_WHIP'] = (row_df['pitching_BB'] + row_df['pitching_H']) / row_df['pitching_IP']
-            row_df['pitching_H9'] = (9 * row_df['pitching_H']) / row_df['pitching_IP']
-            row_df['pitching_HR9'] = (9 * row_df['pitching_HR']) / row_df['pitching_IP']
-            row_df['pitching_BB9'] = (9 * row_df['pitching_BB']) / row_df['pitching_IP']
-            row_df['pitching_SO9'] = (9 * row_df['pitching_SO']) / row_df['pitching_IP']
-            row_df['pitching_SO/BB'] = row_df['pitching_SO'] / row_df['pitching_BB']
-            row_df['pitching_RA9'] = 9 * (row_df['pitching_R'] / row_df['pitching_IP'])
+            row_df['pitching_WHIP'] = (
+                row_df['pitching_BB'] + row_df['pitching_H']) / row_df['pitching_IP']
+            row_df['pitching_H9'] = (
+                9 * row_df['pitching_H']) / row_df['pitching_IP']
+            row_df['pitching_HR9'] = (
+                9 * row_df['pitching_HR']) / row_df['pitching_IP']
+            row_df['pitching_BB9'] = (
+                9 * row_df['pitching_BB']) / row_df['pitching_IP']
+            row_df['pitching_SO9'] = (
+                9 * row_df['pitching_SO']) / row_df['pitching_IP']
+            row_df['pitching_SO/BB'] = row_df['pitching_SO'] / \
+                row_df['pitching_BB']
+            row_df['pitching_RA9'] = 9 * \
+                (row_df['pitching_R'] / row_df['pitching_IP'])
             row_df['pitching_PI'] = i['pitchingStats'][0]['numberOfPitches']
             row_df['pitching_PI_balls'] = i['pitchingStats'][0]['balls']
             row_df['pitching_PI_strikes'] = i['pitchingStats'][0]['strikes']
-            row_df['pitcing_game_score'] = 50 + (row_df['pitching_IP'] * 3) + row_df['pitching_SO'] - (row_df['pitching_H'] * 2) - (row_df['pitching_ER'] * 4) - ((row_df['pitching_R'] - row_df['pitching_ER']) * 2) - row_df['pitching_BB']
+            row_df['pitcing_game_score'] = 50 + (row_df['pitching_IP'] * 3) + row_df['pitching_SO'] - (row_df['pitching_H'] * 2) - (
+                row_df['pitching_ER'] * 4) - ((row_df['pitching_R'] - row_df['pitching_ER']) * 2) - row_df['pitching_BB']
             row_df['AU_POINTS'] = i['pitchingStats'][0]['auTotalPoints']
         else:
             row_df['pitching_H'] = None
             row_df['pitching_R'] = None
             row_df['pitching_ER'] = None
             row_df['pitching_HR'] = None
             row_df['pitching_BB'] = None
             row_df['pitching_SO'] = None
             row_df['pitching_HBP'] = None
             row_df['pitching_WP'] = None
             row_df['pitching_WHIP'] = None
             row_df['pitching_H9'] = None
-            row_df['pitching_HR9']= None
+            row_df['pitching_HR9'] = None
             row_df['pitching_BB9'] = None
             row_df['pitching_SO9'] = None
             row_df['pitching_SO/BB'] = None
             row_df['pitching_RA9'] = None
             row_df['pitching_PI'] = None
             row_df['pitching_PI_balls'] = None
             row_df['pitching_PI_strikes'] = None
 
         ##############################################################################################################################
-        ## Fielding Stats
+        # Fielding Stats
         ##############################################################################################################################
         if len(i['fieldingStats']) > 0:
             row_df['week'] = i['fieldingStats'][0]['weekNumber']
             row_df['game_num'] = i['fieldingStats'][0]['gameNumber']
 
             row_df['G'] = i['fieldingStats'][0]['gamesPlayed']
             row_df['fielding_position'] = i['fieldingStats'][0]['position']
             row_df['fielding_IP_str'] = i['fieldingStats'][0]['inningsPlayed']
 
             try:
-                row_df['fielding_IP'] = float(str(i['fieldingStats'][0]['inningsPlayed']).replace('.1','.333').replace('.2','.667'))
+                row_df['fielding_IP'] = float(str(i['fieldingStats'][0]['inningsPlayed']).replace(
+                    '.1', '.333').replace('.2', '.667'))
             except:
                 row_df['fielding_IP'] = None
 
             row_df['fielding_PO'] = i['fieldingStats'][0]['putOuts']
             row_df['fielding_A'] = i['fieldingStats'][0]['assists']
             row_df['fielding_E'] = i['fieldingStats'][0]['errors']
             row_df['fielding_DP'] = i['fieldingStats'][0]['doublePlays']
             row_df['fielding_FLD%'] = i['fieldingStats'][0]['fieldingPercent']
             row_df['fielding_CS'] = i['fieldingStats'][0]['caughtStealing']
             row_df['fielding_CS%'] = i['fieldingStats'][0]['caughtStealingPercentage']
             row_df['fielding_TC'] = i['fieldingStats'][0]['totalChances']
-        
-            row_df['fielding_CH'] = row_df['fielding_PO'] + row_df['fielding_A'] + row_df['fielding_E']
-            row_df['fielding_RF/9'] = (9 * (row_df['fielding_PO'] + row_df['fielding_A'])) / row_df['fielding_IP']
+
+            row_df['fielding_CH'] = row_df['fielding_PO'] + \
+                row_df['fielding_A'] + row_df['fielding_E']
+            row_df['fielding_RF/9'] = (9 * (row_df['fielding_PO'] +
+                                       row_df['fielding_A'])) / row_df['fielding_IP']
         else:
             row_df['fielding_position'] = None
             row_df['fielding_IP_str'] = None
             row_df['fielding_IP'] = None
             row_df['fielding_PO'] = None
             row_df['fielding_A'] = None
             row_df['fielding_E'] = None
             row_df['fielding_DP'] = None
             row_df['fielding_FLD%'] = None
             row_df['fielding_CS'] = None
             row_df['fielding_CS%'] = None
             row_df['fielding_TC'] = None
-        
+
             row_df['fielding_CH'] = None
             row_df['fielding_RF/9'] = None
 
-
         ##############################################################################################################################
-        ## Save the data to the correct DataFrame
+        # Save the data to the correct DataFrame
         ##############################################################################################################################
 
-
         row_df['type'] = i['type']
         row_df['teamId'] = i['teamId']
 
         if i['homeTeamFlg'] == True:
             row_df['homeTeamFlg'] = 1
         else:
             row_df['homeTeamFlg'] = 0
 
         if i['type'] == "Team":
-            team_stats_df = pd.concat([team_stats_df,row_df],ignore_index=True)
+            team_stats_df = pd.concat(
+                [team_stats_df, row_df], ignore_index=True)
         else:
-            player_stats_df = pd.concat([player_stats_df,row_df],ignore_index=True)
+            player_stats_df = pd.concat(
+                [player_stats_df, row_df], ignore_index=True)
 
         del row_df
-
-    player_stats_df.loc[(player_stats_df['pitching_IP'] >= 6) & (player_stats_df['GS'] == 1) & (player_stats_df['pitching_ER'] <= 3),'pitching_QS'] = 1
-
+    try:
+        player_stats_df.loc[(player_stats_df['pitching_IP'] >= 6) & (
+            player_stats_df['GS'] == 1) & (player_stats_df['pitching_ER'] <= 3), 'pitching_QS'] = 1
+    except:
+        print('No pitching stats found in this game.')
     ##############################################################################################################################
-    ## Once we're done, return the correct dataframe.
+    # Once we're done, return the correct dataframe.
     ##############################################################################################################################
-    
+
     if get_player_and_team_stats == True:
-        stats_df = pd.concat([player_stats_df,team_stats_df],ignore_index=True)
-        del player_stats_df,team_stats_df
+        stats_df = pd.concat(
+            [player_stats_df, team_stats_df], ignore_index=True)
+        del player_stats_df, team_stats_df
         return stats_df
-    elif get_team_stats == True:        
+    elif get_team_stats == True:
         del player_stats_df
         return team_stats_df
     else:
         del team_stats_df
         return player_stats_df
 
-def get_au_softball_pbp(season_id:int,game_id:int,return_participation_data=False) -> pd.DataFrame():
+
+def get_au_softball_pbp(season_id: int, game_id: int, return_participation_data=False) -> pd.DataFrame():
     """
     Retrieves the play-by-play (PBP) data for an Atheltes Unlimited (AU) softball game.
 
     Parameters
     ----------
     `season_id` (int, mandatory):
         The AU softball season ID you want a game from.
-    
+
     `game_id` (int, mandatory):
         The AU softball game ID you want PBP data from.
-    
+
     `return_participation_data` (bool, optional) = `False`:
         Optional argument. 
         If set to `True`, `get_au_softball_pbp()` will return a secondary pandas DataFrame
         containing roster information for this AU softball game.
 
     Returns
     ----------
     A pandas DataFrame containing PBP data for a given AU game ID within a given AU season ID.
     If `return_participation_data` is set to `True`, an additional pandas DataFrame containing roster data for this game will be returned as well.
     """
 
     # season_id = get_au_softball_season_id(season)
     season = get_au_softball_season(season_id)
 
-    headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
     game_pbp_df = pd.DataFrame()
     roster_df = pd.DataFrame()
     row_df = pd.DataFrame()
-        
+
     if game_id < 1:
         raise ValueError('`game_id` cannot be less than 0.')
-    
-    key = int(time.time()) # Yes, the key is literaly the int of the Epoch time at the time of the GET request.
+
+    # Yes, the key is literaly the int of the Epoch time at the time of the GET request.
+    key = int(time.time())
     url = f"https://auprosports.com/proxy.php?request=/api/play-by-play/softball/v1/event/{season_id}/game/{game_id}?k={key}"
 
-    response = requests.get(url,headers=headers)
+    response = requests.get(url, headers=headers)
     raise_html_status_code(response.status_code)
-    
 
     json_data = json.loads(response.text)
 
     del headers, key
 
     for i in json_data['data'][0]['plays']:
-        row_df = pd.DataFrame({'season':season,'game_id':game_id},index=[0])
+        row_df = pd.DataFrame(
+            {'season': season, 'game_id': game_id}, index=[0])
 
         row_df['game_number'] = i['gameNumber']
         row_df['play_seq_num'] = i['playSeqno']
         row_df['narrative'] = i['narrative']
         row_df['home_team_id'] = i['homeTeamId']
         row_df['home_team_score'] = i['homeTeamScore']
         row_df['away_team_id'] = i['awayTeamId']
@@ -431,35 +463,35 @@
         row_df['top_bottom_flag'] = i['topBottomFlg']
         row_df['outs'] = i['outs']
         row_df['winning_team_id'] = i['winningTeamId']
         row_df['action'] = i['action']
         row_df['hit_location'] = i['hitLocation']
         row_df['hit_location_description'] = i['hitLocationDescription']
         row_df['batter_id'] = i['batterId']
-        row_df['pitcher_id'] = i['pitcherId']        
+        row_df['pitcher_id'] = i['pitcherId']
 
-        game_pbp_df = pd.concat([game_pbp_df,row_df])
+        game_pbp_df = pd.concat([game_pbp_df, row_df])
         del row_df
-    
+
     if return_participation_data == True:
-        
+
         for i in json_data['data'][0]['competitors']:
 
             competitor_id = i['competitorId']
             competitor_color = i['color']
             competitor_name = i['name']
-            
+
             for j in i['players']:
                 row_df = pd.DataFrame({
-                        'season':season,
-                        'game_id':game_id,
-                        'competitor_id':competitor_id,
-                        'competitor_color':competitor_color,
-                        'competitor_name':competitor_name
-                    },
+                    'season': season,
+                    'game_id': game_id,
+                    'competitor_id': competitor_id,
+                    'competitor_color': competitor_color,
+                    'competitor_name': competitor_name
+                },
                     index=[0]
                 )
 
                 row_df['competitor_id'] = j['competitorId']
                 row_df['player_id'] = j['playerId']
                 row_df['captain_flag'] = j['captainFlg']
                 row_df['display_name'] = j['displayName']
@@ -474,73 +506,79 @@
                 row_df['has_voted_flag'] = j['hasVotedFlg']
                 row_df['uniform_number'] = str(j['uniformNumber'])
                 row_df['is_nominated_flag'] = j['isNominatedFlg']
                 row_df['nominated_flag'] = j['nominatedFlg']
                 row_df['player_url'] = j['resourceUrl']
                 row_df['image_url'] = j['imageResource']['imageUrl']
 
-                roster_df = pd.concat([roster_df,row_df],ignore_index=True)
+                roster_df = pd.concat([roster_df, row_df], ignore_index=True)
             del row_df
 
         del json_data
-        return game_pbp_df,roster_df
-    
+        return game_pbp_df, roster_df
+
     else:
         del json_data, roster_df
         return game_pbp_df
 
 ############################################################################################################################################################################################################################################################
 ##
-## Season Functions
+# Season Functions
 ##
 ############################################################################################################################################################################################################################################################
 
-def get_au_softball_season_pbp(season:int) -> pd.DataFrame():
+
+def get_au_softball_season_pbp(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) softball season, get and parse all play-by-play (PBP) data for an AU softball season.
-    
+
     Parameters
     ----------
     `season` (int, mandatory):
         The AU softball season you want PBP data from.
 
     Returns
     ----------
     A pandas DataFrame containing PBP data from a AU season.
 
     """
     season_pbp_df = pd.DataFrame()
     seasonId = get_au_softball_season_id(season)
     url = "https://auprosports.com/proxy.php?request=api/seasons/softball/v1"
-    headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36"}
 
-    response = requests.get(url,headers=headers)
+    response = requests.get(url, headers=headers)
     sport_json_data = json.loads(response.text)
-    
+
     for i in sport_json_data['data']:
-        #print(i)
+        # print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
+            count = 0
             for j in tqdm(i['gameIds']):
-                print(f'\nOn game {j} of {len_game_ids} for {season}.')
+                count += 1
+                print(f'\nOn game {count} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_softball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_softball_pbp(seasonId,j)
+                game_df = get_au_softball_pbp(seasonId, j)
 
-                season_pbp_df = pd.concat([season_pbp_df,game_df],ignore_index=True)
+                season_pbp_df = pd.concat(
+                    [season_pbp_df, game_df], ignore_index=True)
                 del game_df
 
     return season_pbp_df
 
-def get_au_softball_season_player_box(season:int) -> pd.DataFrame():
+
+def get_au_softball_season_player_box(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) softball season, get and parse all box-score game stats for an AU softball season.
     This returns all player game stats, and does not return season stats or game averages.
 
     Parameters
     ----------
     `season` (int, mandatory):
@@ -550,40 +588,44 @@
     ----------
     A pandas DataFrame containing player box score stats a AU season.
 
     """
     season_stats_df = pd.DataFrame()
     seasonId = get_au_softball_season_id(season)
     url = "https://auprosports.com/proxy.php?request=api/seasons/softball/v1"
-    headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
 
-    response = requests.get(url,headers=headers)
+    response = requests.get(url, headers=headers)
     sport_json_data = json.loads(response.text)
-    
+
     for i in sport_json_data['data']:
-        #print(i)
+        # print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
-            for j in tqdm(range(1,len_game_ids+1)):
+            for j in tqdm(range(1, len_game_ids+1)):
                 print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_softball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_softball_game_stats(seasonId,j,get_team_stats=False)
+                game_df = get_au_softball_game_stats(
+                    seasonId, j, get_team_stats=False)
 
-                season_stats_df = pd.concat([season_stats_df,game_df],ignore_index=True)
+                season_stats_df = pd.concat(
+                    [season_stats_df, game_df], ignore_index=True)
                 del game_df
 
     return season_stats_df
 
-def get_au_softball_season_team_box(season:int) -> pd.DataFrame():
+
+def get_au_softball_season_team_box(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) softball season, get and parse all box-score game stats for an AU softball season.
     This returns all player game stats, and does not return season stats or game averages.
 
     Parameters
     ----------
     `season` (int, mandatory):
@@ -593,64 +635,68 @@
     ----------
     A pandas DataFrame containing player box score stats a AU season.
 
     """
     season_stats_df = pd.DataFrame()
     seasonId = get_au_softball_season_id(season)
     url = "https://auprosports.com/proxy.php?request=api/seasons/softball/v1"
-    headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
 
-    response = requests.get(url,headers=headers)
+    response = requests.get(url, headers=headers)
     sport_json_data = json.loads(response.text)
-    
+
     for i in sport_json_data['data']:
-        #print(i)
+        # print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
-            for j in tqdm(range(1,len_game_ids+1)):
+            for j in tqdm(range(1, len_game_ids+1)):
                 print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_softball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_softball_game_stats(seasonId,j,get_team_stats=True)
+                game_df = get_au_softball_game_stats(
+                    seasonId, j, get_team_stats=True)
 
-                season_stats_df = pd.concat([season_stats_df,game_df],ignore_index=True)
+                season_stats_df = pd.concat(
+                    [season_stats_df, game_df], ignore_index=True)
                 del game_df
 
     return season_stats_df
 
 ############################################################################################################################################################################################################################################################
 ##
-## Season Stats
+# Season Stats
 ##
 ############################################################################################################################################################################################################################################################
 
-def get_au_softball_season_player_stats(season:int) -> pd.DataFrame():
+
+def get_au_softball_season_player_stats(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) softball season, get all season player stats for an AU softball season.
 
     Parameters
     ----------
     `season` (int, mandatory):
         The AU softball season you want season player stats from.
 
     Returns
     ----------
     A pandas DataFrame containing season player stats a AU season.
 
     """
     game_stats_df = get_au_softball_season_player_box(season)
-    # ['sport', 'api_version', 'season', 'seasonId', 'weekNumber', 
-    #    'gameNumber', 'seasonType', 'playerId', 'uniformNumber',    
+    # ['sport', 'api_version', 'season', 'seasonId', 'weekNumber',
+    #    'gameNumber', 'seasonType', 'playerId', 'uniformNumber',
     #    'uniformNumberDisplay', 'primaryPositionLk', 'secondaryPositionLk',
-    #    'first_name', 'last_name', 'full_name', 'week', 'game_num', 
+    #    'first_name', 'last_name', 'full_name', 'week', 'game_num',
     #    'season_type', 'G', 'GS', 'batting_PA', 'batting_AB', 'batting_R',
     #    'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI',
     #    'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA',
     #    'batting_CS', 'batting_BA', 'batting_OBP', 'batting_SLG', 'batting_TB',
     #    'batting_SF', 'batting_SH', 'AU_POINTS', 'pitching_W', 'pitching_L',
     #    'pitching_ERA', 'pitching_SHO', 'pitching_CG', 'pitching_SV',
     #    'pitching_IP_str', 'pitching_IP', 'pitching_H', 'pitching_R',
@@ -659,130 +705,153 @@
     #    'pitching_HR9', 'pitching_BB9', 'pitching_SO9', 'pitching_SO/BB',
     #    'pitching_RA9', 'pitching_PI', 'pitching_PI_balls',
     #    'pitching_PI_strikes', 'fielding_position', 'fielding_IP_str',
     #    'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
     #    'fielding_FLD%', 'fielding_CS', 'fielding_CS%', 'fielding_TC',
     #    'fielding_CH', 'fielding_RF/9']
 
-    finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'playerId', 
-        'first_name', 'last_name', 'full_name'],as_index=False)[[
-        'G', 'GS', 'AU_POINTS',
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
+    finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'playerId',
+                                         'first_name', 'last_name', 'full_name'], as_index=False)[[
+                                             'G', 'GS', 'AU_POINTS',
+                                             'batting_PA', 'batting_AB', 'batting_R',
+                                             'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI',
+                                             'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA',
+                                             'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH',
+                                             'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS',
+                                             'pitching_SV', 'pitching_IP',
+                                             'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB',
+                                             'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls',
+                                             'pitching_PI_strikes',
+                                             'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
+                                             'fielding_CS', 'fielding_TC'
+                                         ]].sum()
 
-    finished_df[['G', 'GS', 'AU_POINTS','batting_PA', 'batting_AB', 'batting_R','batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI','batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA','batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS','pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls','pitching_PI_strikes','fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP','fielding_CS', 'fielding_TC']] = finished_df[['G', 'GS', 'AU_POINTS','batting_PA', 'batting_AB', 'batting_R','batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI','batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA','batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS','pitching_SV','pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls','pitching_PI_strikes','fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP','fielding_CS', 'fielding_TC']].astype('int')
+    finished_df[['G', 'GS', 'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']] = finished_df[[
+        'G', 'GS', 'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']].astype('int')
     finished_df['pitching_IP'] = finished_df['pitching_IP'].astype('float')
-    ## Batting
-    finished_df.loc[finished_df['batting_AB'] >= 1, 'batting_BA'] = finished_df['batting_H'] / finished_df['batting_AB']
+    # Batting
+    finished_df.loc[finished_df['batting_AB'] >= 1,
+                    'batting_BA'] = finished_df['batting_H'] / finished_df['batting_AB']
     finished_df['batting_BA'] = finished_df['batting_BA'].round(3)
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_OBP'] = (finished_df['batting_H'] + finished_df['batting_BB'] + finished_df['batting_HBP']) / (finished_df['batting_AB'] + finished_df['batting_BB'] + finished_df['batting_HBP'] + finished_df['batting_SF'])
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_OBP'] = (finished_df['batting_H'] + finished_df['batting_BB'] + finished_df['batting_HBP']) / (
+        finished_df['batting_AB'] + finished_df['batting_BB'] + finished_df['batting_HBP'] + finished_df['batting_SF'])
     finished_df['batting_OBP'] = finished_df['batting_OBP'].round(3)
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_SLG'] = finished_df['batting_TB'] / finished_df['batting_AB']
+    finished_df.loc[finished_df['batting_AB'] > 0,
+                    'batting_SLG'] = finished_df['batting_TB'] / finished_df['batting_AB']
     finished_df['batting_SLG'] = finished_df['batting_SLG'].round(3)
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_OPS'] = finished_df['batting_OBP'] + finished_df['batting_SLG']
+    finished_df.loc[finished_df['batting_AB'] > 0,
+                    'batting_OPS'] = finished_df['batting_OBP'] + finished_df['batting_SLG']
     finished_df['batting_OPS'] = finished_df['batting_OPS'].round(3)
 
     finished_df['batting_OPS+'] = None
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_SecA'] = (finished_df['batting_BB'] + (finished_df['batting_TB'] - finished_df['batting_H']) + (finished_df['batting_SB'] - finished_df['batting_CS'])) / finished_df['batting_AB']
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_SecA'] = (finished_df['batting_BB'] + (
+        finished_df['batting_TB'] - finished_df['batting_H']) + (finished_df['batting_SB'] - finished_df['batting_CS'])) / finished_df['batting_AB']
     finished_df['batting_SecA'] = finished_df['batting_SecA'].round(3)
 
-    finished_df.loc[finished_df['batting_PA'] > 0,'batting_BB%'] = finished_df['batting_BB'] / finished_df['batting_PA']
+    finished_df.loc[finished_df['batting_PA'] > 0,
+                    'batting_BB%'] = finished_df['batting_BB'] / finished_df['batting_PA']
     finished_df['batting_BB%'] = finished_df['batting_BB%'].round(3)
 
-    finished_df.loc[finished_df['batting_PA'] > 0,'batting_K%'] = finished_df['batting_K'] / finished_df['batting_PA']
+    finished_df.loc[finished_df['batting_PA'] > 0,
+                    'batting_K%'] = finished_df['batting_K'] / finished_df['batting_PA']
     finished_df['batting_K%'] = finished_df['batting_K%'].round(3)
-    
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_ISO'] = (finished_df['batting_TB'] - finished_df['batting_H']) / finished_df['batting_AB']
+
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_ISO'] = (
+        finished_df['batting_TB'] - finished_df['batting_H']) / finished_df['batting_AB']
     finished_df['batting_ISO'] = finished_df['batting_ISO'].round(3)
-    
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_BABIP'] = (finished_df['batting_H'] + finished_df['batting_HR']) / (finished_df['batting_AB'] - finished_df['batting_K'] - finished_df['batting_HR'] + finished_df['batting_SF'])
+
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_BABIP'] = (finished_df['batting_H'] + finished_df['batting_HR']) / (
+        finished_df['batting_AB'] - finished_df['batting_K'] - finished_df['batting_HR'] + finished_df['batting_SF'])
     finished_df['batting_BABIP'] = finished_df['batting_BABIP'].round(3)
 
-    finished_df.loc[(finished_df['batting_SB'] > 0) | (finished_df['batting_HR'] > 0),'batting_PSN'] = (2 * finished_df['batting_HR'] * finished_df['batting_SB']) / (finished_df['batting_HR'] * finished_df['batting_SB'])
+    finished_df.loc[(finished_df['batting_SB'] > 0) | (finished_df['batting_HR'] > 0), 'batting_PSN'] = (
+        2 * finished_df['batting_HR'] * finished_df['batting_SB']) / (finished_df['batting_HR'] * finished_df['batting_SB'])
     finished_df['batting_PSN'] = finished_df['batting_PSN'].round(3)
 
-    ## Pitching
-    finished_df['pitching_ERA'] = 9 * (finished_df['pitching_ER'] / finished_df['pitching_IP'])
+    # Pitching
+    finished_df['pitching_ERA'] = 9 * \
+        (finished_df['pitching_ER'] / finished_df['pitching_IP'])
     finished_df['pitching_ERA'] = finished_df['pitching_ERA'].round(3)
 
     finished_df['pitching_ERA+'] = None
     finished_df['pitching_FIP'] = None
     finished_df['pitching_FIP-'] = None
-    finished_df['pitching_WHIP'] = (finished_df['pitching_BB'] + finished_df['pitching_H']) / finished_df['pitching_IP']
+    finished_df['pitching_WHIP'] = (
+        finished_df['pitching_BB'] + finished_df['pitching_H']) / finished_df['pitching_IP']
     finished_df['pitching_WHIP'] = finished_df['pitching_WHIP'].round(3)
 
-    finished_df['pitching_H9'] = (9 * finished_df['pitching_H']) / finished_df['pitching_IP']
+    finished_df['pitching_H9'] = (
+        9 * finished_df['pitching_H']) / finished_df['pitching_IP']
     finished_df['pitching_H9'] = finished_df['pitching_H9'].round(3)
 
-    finished_df['pitching_HR9'] = (9 * finished_df['pitching_HR']) / finished_df['pitching_IP']
+    finished_df['pitching_HR9'] = (
+        9 * finished_df['pitching_HR']) / finished_df['pitching_IP']
     finished_df['pitching_HR9'] = finished_df['pitching_HR9'].round(3)
 
-    finished_df['pitching_BB9'] = (9 * finished_df['pitching_BB']) / finished_df['pitching_IP']
+    finished_df['pitching_BB9'] = (
+        9 * finished_df['pitching_BB']) / finished_df['pitching_IP']
     finished_df['pitching_BB9'] = finished_df['pitching_BB9'].round(3)
 
-    finished_df['pitching_SO9'] = (9 * finished_df['pitching_SO']) / finished_df['pitching_IP']
+    finished_df['pitching_SO9'] = (
+        9 * finished_df['pitching_SO']) / finished_df['pitching_IP']
     finished_df['pitching_SO9'] = finished_df['pitching_SO9'].round(3)
 
-    finished_df['pitching_SO/BB'] = finished_df['pitching_SO'] / finished_df['pitching_BB']
+    finished_df['pitching_SO/BB'] = finished_df['pitching_SO'] / \
+        finished_df['pitching_BB']
     finished_df['pitching_SO/BB'] = finished_df['pitching_SO/BB'].round(3)
 
-    finished_df['pitching_RA9'] = 9 * (finished_df['pitching_R'] / finished_df['pitching_IP'])
+    finished_df['pitching_RA9'] = 9 * \
+        (finished_df['pitching_R'] / finished_df['pitching_IP'])
     finished_df['pitching_RA9'] = finished_df['pitching_RA9'].round(3)
-    
-    ## Fielding
-    finished_df['fielding_FLD%'] = (finished_df['fielding_PO'] + finished_df['fielding_A']) / (finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E'])
+
+    # Fielding
+    finished_df['fielding_FLD%'] = (finished_df['fielding_PO'] + finished_df['fielding_A']) / (
+        finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E'])
     finished_df['fielding_FLD%'] = finished_df['fielding_FLD%'].round(3)
 
-    finished_df['fielding_CH'] = finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E']
+    finished_df['fielding_CH'] = finished_df['fielding_PO'] + \
+        finished_df['fielding_A'] + finished_df['fielding_E']
     finished_df['fielding_CH'] = finished_df['fielding_CH'].round(3)
 
-    #finished_df['fielding_CS%'] = 0
-    #finished_df['fielding_CS%'] = finished_df['fielding_CS%'].round(3)
+    # finished_df['fielding_CS%'] = 0
+    # finished_df['fielding_CS%'] = finished_df['fielding_CS%'].round(3)
 
-    finished_df['fielding_RF/9'] = (9 * (finished_df['fielding_PO'] + finished_df['fielding_A'])) / finished_df['fielding_IP']
+    finished_df['fielding_RF/9'] = (9 * (finished_df['fielding_PO'] +
+                                    finished_df['fielding_A'])) / finished_df['fielding_IP']
     finished_df['fielding_RF/9'] = finished_df['fielding_RF/9'].round(3)
 
     # finished_df.to_csv('test.csv')
     # print(finished_df)
     # print(game_stats_df.columns)
     return finished_df
 
-def get_au_softball_season_team_stats(season:int) -> pd.DataFrame():
+
+def get_au_softball_season_team_stats(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) softball season, get all season team stats for an AU softball season.
 
     Parameters
     ----------
     `season` (int, mandatory):
         The AU softball season you want season player stats from.
 
     Returns
     ----------
     A pandas DataFrame containing season player stats a AU season.
 
     """
     game_stats_df = get_au_softball_season_player_box(season)
-    # ['sport', 'api_version', 'season', 'seasonId', 'weekNumber', 
-    #    'gameNumber', 'seasonType', 'playerId', 'uniformNumber',    
+    # ['sport', 'api_version', 'season', 'seasonId', 'weekNumber',
+    #    'gameNumber', 'seasonType', 'playerId', 'uniformNumber',
     #    'uniformNumberDisplay', 'primaryPositionLk', 'secondaryPositionLk',
-    #    'first_name', 'last_name', 'full_name', 'week', 'game_num', 
+    #    'first_name', 'last_name', 'full_name', 'week', 'game_num',
     #    'season_type', 'G', 'GS', 'batting_PA', 'batting_AB', 'batting_R',
     #    'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI',
     #    'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA',
     #    'batting_CS', 'batting_BA', 'batting_OBP', 'batting_SLG', 'batting_TB',
     #    'batting_SF', 'batting_SH', 'AU_POINTS', 'pitching_W', 'pitching_L',
     #    'pitching_ERA', 'pitching_SHO', 'pitching_CG', 'pitching_SV',
     #    'pitching_IP_str', 'pitching_IP', 'pitching_H', 'pitching_R',
@@ -791,102 +860,124 @@
     #    'pitching_HR9', 'pitching_BB9', 'pitching_SO9', 'pitching_SO/BB',
     #    'pitching_RA9', 'pitching_PI', 'pitching_PI_balls',
     #    'pitching_PI_strikes', 'fielding_position', 'fielding_IP_str',
     #    'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
     #    'fielding_FLD%', 'fielding_CS', 'fielding_CS%', 'fielding_TC',
     #    'fielding_CH', 'fielding_RF/9']
 
-    finished_df = game_stats_df.groupby(['sport', 'api_version', 'season', 'seasonId','teamId'],as_index=False)[[
+    finished_df = game_stats_df.groupby(['sport', 'api_version', 'season', 'seasonId', 'teamId'], as_index=False)[[
         'G', 'AU_POINTS',
         'batting_PA', 'batting_AB', 'batting_R',
         'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI',
         'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA',
-        'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 
+        'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH',
         'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS',
-        'pitching_SV', 'pitching_IP', 
-        'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 
+        'pitching_SV', 'pitching_IP',
+        'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB',
         'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls',
         'pitching_PI_strikes',
         'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
         'fielding_CS', 'fielding_TC'
     ]].sum()
 
-    finished_df[['G',  'AU_POINTS','batting_PA', 'batting_AB', 'batting_R','batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI','batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA','batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS','pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls','pitching_PI_strikes','fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP','fielding_CS', 'fielding_TC']] = finished_df[['G', 'AU_POINTS','batting_PA', 'batting_AB', 'batting_R','batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI','batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA','batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS','pitching_SV','pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls','pitching_PI_strikes','fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP','fielding_CS', 'fielding_TC']].astype('int')
+    finished_df[['G',  'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']] = finished_df[[
+        'G', 'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']].astype('int')
     finished_df['pitching_IP'] = finished_df['pitching_IP'].astype('float')
-    ## Batting
-    finished_df.loc[finished_df['batting_AB'] >= 1, 'batting_BA'] = finished_df['batting_H'] / finished_df['batting_AB']
+    # Batting
+    finished_df.loc[finished_df['batting_AB'] >= 1,
+                    'batting_BA'] = finished_df['batting_H'] / finished_df['batting_AB']
     finished_df['batting_BA'] = finished_df['batting_BA'].round(3)
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_OBP'] = (finished_df['batting_H'] + finished_df['batting_BB'] + finished_df['batting_HBP']) / (finished_df['batting_AB'] + finished_df['batting_BB'] + finished_df['batting_HBP'] + finished_df['batting_SF'])
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_OBP'] = (finished_df['batting_H'] + finished_df['batting_BB'] + finished_df['batting_HBP']) / (
+        finished_df['batting_AB'] + finished_df['batting_BB'] + finished_df['batting_HBP'] + finished_df['batting_SF'])
     finished_df['batting_OBP'] = finished_df['batting_OBP'].round(3)
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_SLG'] = finished_df['batting_TB'] / finished_df['batting_AB']
+    finished_df.loc[finished_df['batting_AB'] > 0,
+                    'batting_SLG'] = finished_df['batting_TB'] / finished_df['batting_AB']
     finished_df['batting_SLG'] = finished_df['batting_SLG'].round(3)
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_OPS'] = finished_df['batting_OBP'] + finished_df['batting_SLG']
+    finished_df.loc[finished_df['batting_AB'] > 0,
+                    'batting_OPS'] = finished_df['batting_OBP'] + finished_df['batting_SLG']
     finished_df['batting_OPS'] = finished_df['batting_OPS'].round(3)
 
     finished_df['batting_OPS+'] = None
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_SecA'] = (finished_df['batting_BB'] + (finished_df['batting_TB'] - finished_df['batting_H']) + (finished_df['batting_SB'] - finished_df['batting_CS'])) / finished_df['batting_AB']
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_SecA'] = (finished_df['batting_BB'] + (
+        finished_df['batting_TB'] - finished_df['batting_H']) + (finished_df['batting_SB'] - finished_df['batting_CS'])) / finished_df['batting_AB']
     finished_df['batting_SecA'] = finished_df['batting_SecA'].round(3)
 
-    finished_df.loc[finished_df['batting_PA'] > 0,'batting_BB%'] = finished_df['batting_BB'] / finished_df['batting_PA']
+    finished_df.loc[finished_df['batting_PA'] > 0,
+                    'batting_BB%'] = finished_df['batting_BB'] / finished_df['batting_PA']
     finished_df['batting_BB%'] = finished_df['batting_BB%'].round(3)
 
-    finished_df.loc[finished_df['batting_PA'] > 0,'batting_K%'] = finished_df['batting_K'] / finished_df['batting_PA']
+    finished_df.loc[finished_df['batting_PA'] > 0,
+                    'batting_K%'] = finished_df['batting_K'] / finished_df['batting_PA']
     finished_df['batting_K%'] = finished_df['batting_K%'].round(3)
-    
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_ISO'] = (finished_df['batting_TB'] - finished_df['batting_H']) / finished_df['batting_AB']
+
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_ISO'] = (
+        finished_df['batting_TB'] - finished_df['batting_H']) / finished_df['batting_AB']
     finished_df['batting_ISO'] = finished_df['batting_ISO'].round(3)
-    
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_BABIP'] = (finished_df['batting_H'] + finished_df['batting_HR']) / (finished_df['batting_AB'] - finished_df['batting_K'] - finished_df['batting_HR'] + finished_df['batting_SF'])
+
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_BABIP'] = (finished_df['batting_H'] + finished_df['batting_HR']) / (
+        finished_df['batting_AB'] - finished_df['batting_K'] - finished_df['batting_HR'] + finished_df['batting_SF'])
     finished_df['batting_BABIP'] = finished_df['batting_BABIP'].round(3)
 
-    finished_df.loc[(finished_df['batting_SB'] > 0) | (finished_df['batting_HR'] > 0),'batting_PSN'] = (2 * finished_df['batting_HR'] * finished_df['batting_SB']) / (finished_df['batting_HR'] * finished_df['batting_SB'])
+    finished_df.loc[(finished_df['batting_SB'] > 0) | (finished_df['batting_HR'] > 0), 'batting_PSN'] = (
+        2 * finished_df['batting_HR'] * finished_df['batting_SB']) / (finished_df['batting_HR'] * finished_df['batting_SB'])
     finished_df['batting_PSN'] = finished_df['batting_PSN'].round(3)
 
-    ## Pitching
-    finished_df['pitching_ERA'] = 9 * (finished_df['pitching_ER'] / finished_df['pitching_IP'])
+    # Pitching
+    finished_df['pitching_ERA'] = 9 * \
+        (finished_df['pitching_ER'] / finished_df['pitching_IP'])
     finished_df['pitching_ERA'] = finished_df['pitching_ERA'].round(3)
 
     finished_df['pitching_ERA+'] = None
     finished_df['pitching_FIP'] = None
     finished_df['pitching_FIP-'] = None
-    finished_df['pitching_WHIP'] = (finished_df['pitching_BB'] + finished_df['pitching_H']) / finished_df['pitching_IP']
+    finished_df['pitching_WHIP'] = (
+        finished_df['pitching_BB'] + finished_df['pitching_H']) / finished_df['pitching_IP']
     finished_df['pitching_WHIP'] = finished_df['pitching_WHIP'].round(3)
 
-    finished_df['pitching_H9'] = (9 * finished_df['pitching_H']) / finished_df['pitching_IP']
+    finished_df['pitching_H9'] = (
+        9 * finished_df['pitching_H']) / finished_df['pitching_IP']
     finished_df['pitching_H9'] = finished_df['pitching_H9'].round(3)
 
-    finished_df['pitching_HR9'] = (9 * finished_df['pitching_HR']) / finished_df['pitching_IP']
+    finished_df['pitching_HR9'] = (
+        9 * finished_df['pitching_HR']) / finished_df['pitching_IP']
     finished_df['pitching_HR9'] = finished_df['pitching_HR9'].round(3)
 
-    finished_df['pitching_BB9'] = (9 * finished_df['pitching_BB']) / finished_df['pitching_IP']
+    finished_df['pitching_BB9'] = (
+        9 * finished_df['pitching_BB']) / finished_df['pitching_IP']
     finished_df['pitching_BB9'] = finished_df['pitching_BB9'].round(3)
 
-    finished_df['pitching_SO9'] = (9 * finished_df['pitching_SO']) / finished_df['pitching_IP']
+    finished_df['pitching_SO9'] = (
+        9 * finished_df['pitching_SO']) / finished_df['pitching_IP']
     finished_df['pitching_SO9'] = finished_df['pitching_SO9'].round(3)
 
-    finished_df['pitching_SO/BB'] = finished_df['pitching_SO'] / finished_df['pitching_BB']
+    finished_df['pitching_SO/BB'] = finished_df['pitching_SO'] / \
+        finished_df['pitching_BB']
     finished_df['pitching_SO/BB'] = finished_df['pitching_SO/BB'].round(3)
 
-    finished_df['pitching_RA9'] = 9 * (finished_df['pitching_R'] / finished_df['pitching_IP'])
+    finished_df['pitching_RA9'] = 9 * \
+        (finished_df['pitching_R'] / finished_df['pitching_IP'])
     finished_df['pitching_RA9'] = finished_df['pitching_RA9'].round(3)
-    
-    ## Fielding
-    finished_df['fielding_FLD%'] = (finished_df['fielding_PO'] + finished_df['fielding_A']) / (finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E'])
+
+    # Fielding
+    finished_df['fielding_FLD%'] = (finished_df['fielding_PO'] + finished_df['fielding_A']) / (
+        finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E'])
     finished_df['fielding_FLD%'] = finished_df['fielding_FLD%'].round(3)
 
-    finished_df['fielding_CH'] = finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E']
+    finished_df['fielding_CH'] = finished_df['fielding_PO'] + \
+        finished_df['fielding_A'] + finished_df['fielding_E']
     finished_df['fielding_CH'] = finished_df['fielding_CH'].round(3)
 
-    #finished_df['fielding_CS%'] = 0
-    #finished_df['fielding_CS%'] = finished_df['fielding_CS%'].round(3)
+    # finished_df['fielding_CS%'] = 0
+    # finished_df['fielding_CS%'] = finished_df['fielding_CS%'].round(3)
 
-    finished_df['fielding_RF/9'] = (9 * (finished_df['fielding_PO'] + finished_df['fielding_A'])) / finished_df['fielding_IP']
+    finished_df['fielding_RF/9'] = (9 * (finished_df['fielding_PO'] +
+                                    finished_df['fielding_A'])) / finished_df['fielding_IP']
     finished_df['fielding_RF/9'] = finished_df['fielding_RF/9'].round(3)
 
     # finished_df.to_csv('test.csv')
     # print(finished_df)
     # print(game_stats_df.columns)
     return finished_df
```

### Comparing `athletes_unlimited_py-0.0.5/athetes_unlimited_py/utils.py` & `athletes_unlimited_py-0.0.6/athetes_unlimited_py/utils.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.5/athetes_unlimited_py/volleyball.py` & `athletes_unlimited_py-0.0.6/athetes_unlimited_py/volleyball.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/PKG-INFO` & `athletes_unlimited_py-0.0.6/athletes_unlimited_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athletes-unlimited-py
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/athletes-unlimited-py
 Project-URL: documentation, https://github.com/armstjc/athletes-unlimited-py/wiki
 Project-URL: repository, https://github.com/armstjc/athletes-unlimited-py.git
```

### Comparing `athletes_unlimited_py-0.0.5/pyproject.toml` & `athletes_unlimited_py-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools","wheel","pyarrow","pandas","tqdm","requests","lxml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "athletes_unlimited_py"
-version = "0.0.5"
+version = "0.0.6"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
 
 authors = [
     {name = "Joseph Armstrong", email="armstrongjoseph08@gmail.com"}
 ]
```

