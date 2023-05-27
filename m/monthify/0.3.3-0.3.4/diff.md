# Comparing `tmp/monthify-0.3.3.tar.gz` & `tmp/monthify-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monthify-0.3.3.tar", max compression
+gzip compressed data, was "monthify-0.3.4.tar", max compression
```

## Comparing `monthify-0.3.3.tar` & `monthify-0.3.4.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1133 2023-03-17 12:31:43.173289 monthify-0.3.3/README.md
--rw-r--r--   0        0        0       42 2023-03-23 23:13:51.850450 monthify-0.3.3/monthify/__init__.py
--rw-r--r--   0        0        0       68 2023-03-14 21:44:18.544850 monthify-0.3.3/monthify/__main__.py
--rw-r--r--   0        0        0     1019 2023-04-02 17:01:21.279187 monthify-0.3.3/monthify/auth.py
--rw-r--r--   0        0        0     4367 2023-04-06 01:00:39.802855 monthify-0.3.3/monthify/main.py
--rw-r--r--   0        0        0    18342 2023-04-06 01:04:34.159163 monthify-0.3.3/monthify/script.py
--rw-r--r--   0        0        0      764 2023-03-23 22:17:54.957609 monthify-0.3.3/monthify/track.py
--rw-r--r--   0        0        0     1185 2023-03-23 23:13:51.850450 monthify-0.3.3/monthify/utils.py
--rw-r--r--   0        0        0      683 2023-04-06 01:04:34.159163 monthify-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 monthify-0.3.3/setup.py
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 monthify-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-05-18 06:24:22.438685 monthify-0.3.4/README.md
+-rw-r--r--   0        0        0       42 2023-05-18 06:24:22.439685 monthify-0.3.4/monthify/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-18 06:24:22.439685 monthify-0.3.4/monthify/__main__.py
+-rw-r--r--   0        0        0     1106 2023-05-27 03:11:30.775267 monthify-0.3.4/monthify/auth.py
+-rw-r--r--   0        0        0     4367 2023-05-27 02:45:32.298405 monthify-0.3.4/monthify/main.py
+-rw-r--r--   0        0        0    18611 2023-05-27 03:11:30.776267 monthify-0.3.4/monthify/script.py
+-rw-r--r--   0        0        0      764 2023-05-18 06:24:22.439685 monthify-0.3.4/monthify/track.py
+-rw-r--r--   0        0        0     1185 2023-05-27 02:42:22.456255 monthify-0.3.4/monthify/utils.py
+-rw-r--r--   0        0        0      815 2023-05-27 03:11:30.776267 monthify-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 monthify-0.3.4/PKG-INFO
```

### Comparing `monthify-0.3.3/README.md` & `monthify-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `monthify-0.3.3/monthify/auth.py` & `monthify-0.3.4/monthify/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # Authentication manager
+from collections.abc import Iterable
+
 import spotipy
 from spotipy.oauth2 import SpotifyOAuth
 
 MAX_TRIES = 5
 
 
 class Auth:
-    def __init__(self, CLIENT_ID, CLIENT_SECRET, LOCATION):
+    def __init__(self, CLIENT_ID: str, CLIENT_SECRET: str, LOCATION: str):
         self.client_secret = CLIENT_SECRET
         self.client_id = CLIENT_ID
         self.redirect_uri = "https://open.spotify.com/"
         self.scopes = (
             "user-library-read",
             "playlist-read-private",
             "playlist-modify-private",
         )
         self.location = LOCATION
 
-    def spotipy_init(self, scopes):
+    def spotipy_init(self, scopes: Iterable[str]) -> spotipy.Spotify:
         return spotipy.Spotify(
             retries=MAX_TRIES,
             requests_timeout=10,
             auth_manager=SpotifyOAuth(
                 client_id=self.client_id,
                 client_secret=self.client_secret,
                 redirect_uri=self.redirect_uri,
```

### Comparing `monthify-0.3.3/monthify/main.py` & `monthify-0.3.4/monthify/main.py`

 * *Files identical despite different names*

### Comparing `monthify-0.3.3/monthify/script.py` & `monthify-0.3.4/monthify/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Script
 import sys
+from collections.abc import Iterable
 from datetime import datetime
 from os import makedirs, remove, stat
 from os.path import exists
 from pathlib import Path
 
 from appdirs import user_data_dir
 from cachetools import TTLCache, cached
 from loguru import logger
 from rich.console import Console
 
 from monthify import ERROR, SUCCESS
+from monthify.auth import Auth
 from monthify.track import Track
 from monthify.utils import (
     conditional_decorator,
     normalize_text,
     sort_chronologically,
 )
 
@@ -34,33 +36,39 @@
 )
 logger.remove()
 logger.add(f"{appdata_location}/logs/monthify.log", rotation="00:00", compression="zip")
 console = Console()
 existing_playlists_file = f"{appdata_location}/existing_playlists_file.dat"
 last_run_file = f"{appdata_location}/last_run.txt"
 last_run_format = "%Y-%m-%d %H:%M:%S"
-saved_tracks_cache = TTLCache(maxsize=1000, ttl=86400)
-saved_playlists_cache = TTLCache(maxsize=1000, ttl=86400)
-user_cache = TTLCache(maxsize=1, ttl=86400)
+saved_tracks_cache: TTLCache = TTLCache(maxsize=1000, ttl=86400)
+saved_playlists_cache: TTLCache = TTLCache(maxsize=1000, ttl=86400)
+user_cache: TTLCache = TTLCache(maxsize=1, ttl=86400)
 
 
 class Monthify:
     total_tracks_added = 0
 
-    def __init__(self, auth, SKIP_PLAYLIST_CREATION, LOGOUT, CREATE_PLAYLIST):
+    def __init__(
+        self,
+        auth: Auth,
+        SKIP_PLAYLIST_CREATION: bool,
+        LOGOUT: bool,
+        CREATE_PLAYLIST: bool,
+    ):
         self.LOGOUT = LOGOUT
         self.logout()
         authentication = auth
         self.sp = authentication.get_spotipy()
         self.SKIP_PLAYLIST_CREATION = SKIP_PLAYLIST_CREATION
         self.CREATE_PLAYLIST = CREATE_PLAYLIST
         self.has_created_playlists = False
         self.current_username = ""
         self.current_display_name = ""
-        self.playlist_names = []
+        self.playlist_names: Iterable[str] = []
         self.already_created_playlists_exists = False
         if (
             exists(existing_playlists_file)
             and stat(existing_playlists_file).st_size != 0
         ):
             if (
                 datetime.now()
@@ -73,25 +81,25 @@
                 with open(existing_playlists_file, "r", encoding="utf_8") as f:
                     self.already_created_playlists = list(f.read().splitlines())
                     self.already_created_playlists_exists = True
         else:
             self.already_created_playlists = []
             self.already_created_playlists_exists = False
 
-        self.already_created_playlists_inter = []
+        self.already_created_playlists_inter: Iterable[str] = []
         if exists(last_run_file):
             if stat(last_run_file).st_size != 0:
                 with open(last_run_file, "r", encoding="utf_8") as f:
                     self.last_run = f.read()
             else:
                 self.last_run = ""
         else:
             self.last_run = ""
 
-        self.playlist_names_with_id = []
+        self.playlist_names_with_id: Iterable[str] = []
         self.name = """
         ___  ___            _   _     _  __       
         |  \/  |           | | | |   (_)/ _|      
         | .  . | ___  _ __ | |_| |__  _| |_ _   _ 
         | |\/| |/ _ \| '_ \| __| '_ \| |  _| | | |
         | |  | | (_) | | | | |_| | | | | | | |_| |
         \_|  |_/\___/|_| |_|\__|_| |_|_|_|  \__, |
@@ -299,15 +307,15 @@
                     and playlist_name in spotify_playlists
                 ):
                     console.print(f"{month} '{year[2:]} playlist already exists")
                 else:
                     name = month + " '" + year[2:]
                     self.create_playlist(name)
 
-        def skip(status: bool):
+        def skip(status: bool) -> None:
             if status is True:
                 console.print("Playlist generation skipped")
                 logger.info("Playlist generation skipped")
             else:
                 logger.info("Playlist generation starting")
                 playlist_loop()
 
@@ -348,25 +356,26 @@
                 dict.fromkeys(self.already_created_playlists)
             )
 
         if self.already_created_playlists:
             with open(existing_playlists_file, "w", encoding="utf_8") as f:
                 f.write("\n".join(self.already_created_playlists))
 
-    def add_to_playlist(self, tracks: list[Track], playlist_id):
+    def add_to_playlist(self, tracks: list[Track], playlist_id: str) -> None:
         """
         Add a list of tracks to a specified playlist using playlist id
         """
         logger.info(
             "Attempting to add tracks to playlist: {playlist}\ntracks: {tracks} ",
             tracks=tracks,
             playlist=str(playlist_id),
         )
         playlist_items = self.get_playlist_items(playlist_id)
-        to_be_added_uris, playlist_uris = [], []
+        to_be_added_uris: list[str] = []
+        playlist_uris: Iterable[str] = []
 
         playlist_uris = tuple(item["track"]["uri"] for item in playlist_items)
 
         for track in reversed(tracks):
             if track.uri in playlist_uris:
                 logger.info(f"Track: {track} already in playlist: {str(playlist_id)}")
                 track_url = f'https://open.{track.uri. replace(":", "/").replace("spotify", "spotify.com")}'
```

### Comparing `monthify-0.3.3/monthify/track.py` & `monthify-0.3.4/monthify/track.py`

 * *Files identical despite different names*

### Comparing `monthify-0.3.3/monthify/utils.py` & `monthify-0.3.4/monthify/utils.py`

 * *Files identical despite different names*

### Comparing `monthify-0.3.3/pyproject.toml` & `monthify-0.3.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monthify"
-version = "0.3.3"
+version = "0.3.4"
 description = "Sorts liked spotify tracks into playlists by the month they were liked."
 authors = ["Madiba Hudson-Quansah <mhquansah@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 loguru = "^0.6.0"
@@ -16,14 +16,19 @@
 
 [tool.poetry.group.dev.dependencies]
 icecream = "^2.1.3"
 pynvim = "^0.4.3"
 pytest = "^7.2.2"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
+types-requests = "^2.31.0.0"
+types-toml = "^0.10.8.6"
+types-appdirs = "^1.4.3.5"
+mypy = "^1.3.0"
+types-cachetools = "^5.3.0.5"
 
 [tool.poetry.scripts]
 monthify = "monthify.main:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `monthify-0.3.3/PKG-INFO` & `monthify-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monthify
-Version: 0.3.3
+Version: 0.3.4
 Summary: Sorts liked spotify tracks into playlists by the month they were liked.
 Author: Madiba Hudson-Quansah
 Author-email: mhquansah@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

