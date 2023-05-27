# Comparing `tmp/parse-torrent-title-2.4.tar.gz` & `tmp/parse-torrent-title-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/platelminto/Documents/dev/python/parse-torrent-title/dist/tmp0WIIuK/parse-torrent-title-2.4.tar", last modified: Thu Nov 11 23:52:00 2021, max compression
+gzip compressed data, was "dist/parse-torrent-title-2.5.tar", last modified: Sat May 27 18:31:24 2023, max compression
```

## Comparing `parse-torrent-title-2.4.tar` & `parse-torrent-title-2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 platelminto  (1000) platelminto  (1000)        0 2021-11-11 23:52:00.000000 parse-torrent-title-2.4/
-drwxrwxr-x   0 platelminto  (1000) platelminto  (1000)        0 2021-11-11 23:52:00.000000 parse-torrent-title-2.4/PTN/
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)     5892 2021-11-06 14:54:01.000000 parse-torrent-title-2.4/PTN/extras.py
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)      662 2021-11-06 14:54:01.000000 parse-torrent-title-2.4/PTN/__init__.py
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    15595 2021-11-06 14:54:01.000000 parse-torrent-title-2.4/PTN/parse.py
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    11144 2021-11-06 14:54:01.000000 parse-torrent-title-2.4/PTN/patterns.py
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)     7236 2021-11-06 14:54:01.000000 parse-torrent-title-2.4/PTN/post.py
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)       81 2020-03-25 03:23:23.000000 parse-torrent-title-2.4/MANIFEST.in
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)     1168 2020-04-08 01:49:32.000000 parse-torrent-title-2.4/LICENSE
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)     8598 2021-11-06 14:54:01.000000 parse-torrent-title-2.4/README.md
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)      132 2021-11-11 23:52:00.000000 parse-torrent-title-2.4/setup.cfg
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    11120 2021-11-11 23:52:00.000000 parse-torrent-title-2.4/PKG-INFO
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)     1201 2021-11-06 14:54:01.000000 parse-torrent-title-2.4/setup.py
-drwxrwxr-x   0 platelminto  (1000) platelminto  (1000)        0 2021-11-11 23:52:00.000000 parse-torrent-title-2.4/tests/
-drwxrwxr-x   0 platelminto  (1000) platelminto  (1000)        0 2021-11-11 23:52:00.000000 parse-torrent-title-2.4/tests/files/
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    23810 2021-02-16 20:55:23.000000 parse-torrent-title-2.4/tests/files/seen_inputs.json
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    36595 2021-11-06 14:54:01.000000 parse-torrent-title-2.4/tests/files/output_standard.json
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    24621 2021-11-06 14:54:01.000000 parse-torrent-title-2.4/tests/files/input.json
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    67631 2021-11-06 14:54:01.000000 parse-torrent-title-2.4/tests/files/output_raw.json
-drwxrwxr-x   0 platelminto  (1000) platelminto  (1000)        0 2021-11-11 23:52:00.000000 parse-torrent-title-2.4/parse_torrent_title.egg-info/
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)        1 2021-11-11 23:52:00.000000 parse-torrent-title-2.4/parse_torrent_title.egg-info/dependency_links.txt
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)        4 2021-11-11 23:52:00.000000 parse-torrent-title-2.4/parse_torrent_title.egg-info/top_level.txt
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)      404 2021-11-11 23:52:00.000000 parse-torrent-title-2.4/parse_torrent_title.egg-info/SOURCES.txt
--rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    11120 2021-11-11 23:52:00.000000 parse-torrent-title-2.4/parse_torrent_title.egg-info/PKG-INFO
+drwxrwxr-x   0 platelminto  (1000) platelminto  (1000)        0 2023-05-27 18:31:24.000000 parse-torrent-title-2.5/
+drwxrwxr-x   0 platelminto  (1000) platelminto  (1000)        0 2023-05-27 18:31:24.000000 parse-torrent-title-2.5/PTN/
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)     7236 2023-03-06 12:09:44.000000 parse-torrent-title-2.5/PTN/post.py
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)     5995 2023-03-06 12:51:32.000000 parse-torrent-title-2.5/PTN/extras.py
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    11217 2023-05-27 18:05:12.000000 parse-torrent-title-2.5/PTN/patterns.py
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)      651 2023-05-27 18:28:18.000000 parse-torrent-title-2.5/PTN/__init__.py
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    15595 2023-03-06 12:09:44.000000 parse-torrent-title-2.5/PTN/parse.py
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)      132 2023-05-27 18:31:24.000000 parse-torrent-title-2.5/setup.cfg
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)     8611 2023-03-06 12:51:32.000000 parse-torrent-title-2.5/README.md
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)     1168 2023-03-06 12:09:44.000000 parse-torrent-title-2.5/LICENSE
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    11157 2023-05-27 18:31:24.000000 parse-torrent-title-2.5/PKG-INFO
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)     1201 2023-03-06 12:09:44.000000 parse-torrent-title-2.5/setup.py
+drwxrwxr-x   0 platelminto  (1000) platelminto  (1000)        0 2023-05-27 18:31:24.000000 parse-torrent-title-2.5/tests/
+drwxrwxr-x   0 platelminto  (1000) platelminto  (1000)        0 2023-05-27 18:31:24.000000 parse-torrent-title-2.5/tests/files/
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    37391 2023-05-27 18:08:40.000000 parse-torrent-title-2.5/tests/files/output_standard.json
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    68861 2023-05-27 18:08:40.000000 parse-torrent-title-2.5/tests/files/output_raw.json
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    25063 2023-05-27 18:07:25.000000 parse-torrent-title-2.5/tests/files/input.json
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)      272 2023-05-24 14:42:25.000000 parse-torrent-title-2.5/tests/files/seen_inputs.json
+drwxrwxr-x   0 platelminto  (1000) platelminto  (1000)        0 2023-05-27 18:31:24.000000 parse-torrent-title-2.5/parse_torrent_title.egg-info/
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)        1 2023-05-27 18:31:24.000000 parse-torrent-title-2.5/parse_torrent_title.egg-info/dependency_links.txt
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)      404 2023-05-27 18:31:24.000000 parse-torrent-title-2.5/parse_torrent_title.egg-info/SOURCES.txt
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)        4 2023-05-27 18:31:24.000000 parse-torrent-title-2.5/parse_torrent_title.egg-info/top_level.txt
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)    11157 2023-05-27 18:31:24.000000 parse-torrent-title-2.5/parse_torrent_title.egg-info/PKG-INFO
+-rw-rw-r--   0 platelminto  (1000) platelminto  (1000)       81 2023-03-06 12:09:44.000000 parse-torrent-title-2.5/MANIFEST.in
```

### Comparing `parse-torrent-title-2.4/PTN/extras.py` & `parse-torrent-title-2.5/PTN/extras.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,39 +12,42 @@
     ("swedish", "Swedish"),
     ("dk|dan(?:ish)?", "Danish"),
     ("ger(?:man)?|deu(?:tsch)?", "German"),
     ("nordic", "Nordic"),
     ("exyu", "ExYu"),
     ("chs|chi(?:nese)?", "Chinese"),
     ("hin(?:di)?", "Hindi"),
-    ("polish", "Polish"),
+    ("polish|poland", "Polish"),
     ("mandarin", "Mandarin"),
     ("kor(?:ean)?", "Korean"),
     ("bengali|bangla", "Bengali"),
     ("kannada", "Kannada"),
     ("tam(?:il)?", "Tamil"),
     ("tel(?:ugu)?", "Telugu"),
     ("marathi", "Marathi"),
     ("mal(?:ayalam)?", "Malayalam"),
     ("japanese|ja?p", "Japanese"),
     ("interslavic", "Interslavic"),
     ("ara(?:bic)?", "Arabic"),
     ("urdu", "Urdu"),
     ("punjabi", "Punjabi"),
     ("portuguese", "Portuguese"),
+    ("albanian?", "Albanian"),
+    ("egypt(?:ian)?", "Egyptian"),
     ("en?(?:g(?:lish)?)?", "English"),  # Must be at end, matches just an 'e'
 ]
 
 genres = [
     ("Sci-?Fi", "Sci-Fi"),
     ("Drama", "Drama"),
     ("Comedy", "Comedy"),
     ("West(?:\.|ern)?", "Western"),
     ("Action", "Action"),
     ("Adventure", "Adventure"),
+    ("Thriller", "Thriller"),
 ]
 
 # Some titles just can't be parsed without breaking everything else, so here
 # are known those known exceptions. They are executed when the parsed_title and
 # incorrect_parse match within a .parse() dict, removing the latter, and replacing
 # the former with actual_title.
 exceptions = [
```

### Comparing `parse-torrent-title-2.4/PTN/__init__.py` & `parse-torrent-title-2.5/PTN/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 else:
     re = pkgutil.find_loader("re").load_module("re")
 
 from .parse import PTN
 
 __author__ = "Giorgio Momigliano"
 __email__ = "gmomigliano@protonmail.com"
-__version__ = "2.4"
+__version__ = "2.5"
 __license__ = "MIT"
 
-ptn = PTN()
-
 
 # TODO change coherent_types default to True in 3.0
 def parse(name, standardise=True, coherent_types=False):
-    return ptn.parse(name, standardise, coherent_types)
+    return PTN().parse(name, standardise, coherent_types)
```

### Comparing `parse-torrent-title-2.4/PTN/parse.py` & `parse-torrent-title-2.5/PTN/parse.py`

 * *Files identical despite different names*

### Comparing `parse-torrent-title-2.4/PTN/patterns.py` & `parse-torrent-title-2.5/PTN/patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,23 +205,23 @@
     ("Zee5", "ZEE5"),
     ("Hallmark", "Hallmark"),
     ("Sony\s?LIV", "SONY LIV"),
 ]
 patterns["codec"] = [
     ("xvid", "Xvid"),
     ("av1", "AV1"),
-    ("[hx]\.?264", "H.264"),
+    ("[hx]{d}?264".format(d=delimiters), "H.264"),
     ("AVC", "H.264"),
     ("HEVC(?:{d}Main{d}?10P?)".format(d=delimiters), "H.265 Main 10"),
     (
-        "[hx]\.?265",
+        "[hx]{d}?265".format(d=delimiters),
         "H.265",
     ),  # Separate from HEVC so if both are present, it won't pollute excess.
     ("HEVC", "H.265"),
-    ("[h]\.?263", "H.263"),
+    ("[h]{d}?263".format(d=delimiters), "H.263"),
     ("VC-1", "VC-1"),
 ]
 patterns["audio"] = get_channel_audio_options(
     [
         ("TrueHD", "Dolby TrueHD"),
         ("Atmos", "Dolby Atmos"),
         ("DD-EX", "Dolby Digital EX"),
@@ -251,17 +251,17 @@
 ]
 patterns["region"] = ("R[0-9]", None, "upper")
 patterns["extended"] = "(EXTENDED(:?.CUT)?)"
 patterns["hardcoded"] = "HC"
 patterns["proper"] = "PROPER"
 patterns["repack"] = "REPACK"
 patterns["fps"] = "([1-9][0-9]{1,2})" + delimiters + "*fps"
-patterns["filetype"] = [("MKV|AVI|(?:SRT|SUB|SSA)$", None, "upper"), ("MP-?4", "MP4")]
+patterns["filetype"] = [(r"\.?(MKV|AVI|(?:SRT|SUB|SSA)$)", None, "upper"), ("MP-?4", "MP4")]
 patterns["widescreen"] = "WS"
-patterns["site"] = "^(\[ ?([^\]]+?) ?\])"
+patterns["site"] = r"^(\[ ?([^\]]+?) ?\])"
 
 lang_list_pattern = (
     r"\b(?:"
     + link_patterns(langs)
     + "(?:"
     + delimiters
     + "+(?:dub(?:bed)?|"
```

### Comparing `parse-torrent-title-2.4/PTN/post.py` & `parse-torrent-title-2.5/PTN/post.py`

 * *Files identical despite different names*

### Comparing `parse-torrent-title-2.4/LICENSE` & `parse-torrent-title-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `parse-torrent-title-2.4/README.md` & `parse-torrent-title-2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 ## Examples
 
 Movies, series (seasons & episodes), and subtitles can be parsed. All meaningful information is
 extracted and returned in a dictionary. Text which couldn't be
 parsed is returned in the `excess` field.
 
 ```py
+import PTN
+
+
 PTN.parse('The Walking Dead S05E03 720p HDTV x264-ASAP[ettv]')
 # {
 #     'encoder': 'ASAP',
 #     'title': 'The Walking Dead',
 #     'season':  5,
 #     'episode': 3,
 #     'resolution': '720p',
```

### Comparing `parse-torrent-title-2.4/PKG-INFO` & `parse-torrent-title-2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-torrent-title
-Version: 2.4
+Version: 2.5
 Summary: Extract media information from torrent-like filename
 Home-page: https://github.com/platelminto/parse-torrent-title
 Author: Giorgio Momigliano
 Author-email: gmomigliano@protonmail.com
 License: MIT
 Description: # parse-torrent-title
         
@@ -55,14 +55,17 @@
         ## Examples
         
         Movies, series (seasons & episodes), and subtitles can be parsed. All meaningful information is
         extracted and returned in a dictionary. Text which couldn't be
         parsed is returned in the `excess` field.
         
         ```py
+        import PTN
+        
+        
         PTN.parse('The Walking Dead S05E03 720p HDTV x264-ASAP[ettv]')
         # {
         #     'encoder': 'ASAP',
         #     'title': 'The Walking Dead',
         #     'season':  5,
         #     'episode': 3,
         #     'resolution': '720p',
```

### Comparing `parse-torrent-title-2.4/setup.py` & `parse-torrent-title-2.5/setup.py`

 * *Files identical despite different names*

### Comparing `parse-torrent-title-2.4/tests/files/output_standard.json` & `parse-torrent-title-2.5/tests/files/output_standard.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736147757255936%*

 * *Differences: {'insert': "[(369, OrderedDict([('audio', 'Dolby Digital 5.1'), ('codec', 'H.264'), ('title', 'The "*

 * *           "Djinn')])), (370, OrderedDict([('genre', 'Drama'), ('language', 'Albanian'), ('title', "*

 * *           "'Hive')])), (371, OrderedDict([('genre', 'Drama'), ('language', 'Egyptian'), ('title', "*

 * *           "'Souad')])), (372, OrderedDict([('genre', 'Drama'), ('language', 'Polish'), ('title', "*

 * *           "'Swinki')])), (373, OrderedDict([('genre', 'Thriller'), ('title', 'Dead Heat on a "*

 * *           "M […]*

```diff
@@ -2071,9 +2071,57 @@
         "audio": "Dual",
         "codec": "H.265",
         "title": "Kimi no Suizou o Tabetai"
     },
     {
         "audio": "Dual",
         "title": "Accel World"
+    },
+    {
+        "audio": "Dolby Digital 5.1",
+        "codec": "H.264",
+        "title": "The Djinn"
+    },
+    {
+        "genre": "Drama",
+        "language": "Albanian",
+        "title": "Hive"
+    },
+    {
+        "genre": "Drama",
+        "language": "Egyptian",
+        "title": "Souad"
+    },
+    {
+        "genre": "Drama",
+        "language": "Polish",
+        "title": "Swinki"
+    },
+    {
+        "genre": "Thriller",
+        "title": "Dead Heat on a Merry Go Round"
+    },
+    {
+        "audio": "Dolby Digital",
+        "codec": "H.264",
+        "filetype": "MP4",
+        "title": "Justified"
+    },
+    {
+        "codec": "H.264",
+        "quality": "Blu-ray",
+        "title": "Movie 43"
+    },
+    {
+        "codec": "H.264",
+        "quality": "Blu-ray",
+        "title": "Mommy"
+    },
+    {
+        "codec": "H.265",
+        "title": "Rendez Vous."
+    },
+    {
+        "filetype": "MKV",
+        "title": "The Best Offer"
     }
 ]
```

### Comparing `parse-torrent-title-2.4/tests/files/input.json` & `parse-torrent-title-2.5/tests/files/input.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736147757255936%*

 * *Differences: {'insert': "[(369, 'The Djinn 2021 1080p BRRip DD5 1 X 264-EVO'), (370, 'Hive [2021 - Albania] "*

 * *           "drama'), (371, 'Souad [2021 - Egypt] drama'), (372, 'Swinki [2009 - Poland] drama'), "*

 * *           "(373, 'Dead Heat on a Merry Go Round [1966 - USA] thriller'), (374, 'Justified - "*

 * *           "Season 1 to 6 - Mp4 x264 AC3 1080p'), (375, 'Movie 43 (2013) 720p BluRay x264 "*

 * *           "-[MoviesFD]'), (376, 'Mommy (2014) French 720p BluRay x264 -[MoviesFD]'), (377, "*

 * *           "'Rendez Vous.2015.DUBBE […]*

```diff
@@ -363,9 +363,19 @@
     "[BDremux] One Piece Movies Collection",
     "[JySzE] Naruto [v2] [R2J] [VFR] [Dual Audio] [Complete] [Extras] [x264]",
     "Attack.on.Titan.S01.S02.S03.1080p.Blu-Ray.Remux.Dual-Audio.TrueHD",
     "Black Clover S01 USBD REMUX",
     "Hero Mask S1 + S2 + Extras [npz][US BD REMUX, 1080p]",
     "[CBT] Nisekoi S1+S2 [BDrip 1920x1080 x264 FLAC]",
     "[YURI] Kimi no Suizou o Tabetai [BD1080p HEVC FLAC][Dual Audio]  v4",
-    "[FFF-Remux][Batch] Accel World 1-24 Dual-Audio 1080p FLAC"
+    "[FFF-Remux][Batch] Accel World 1-24 Dual-Audio 1080p FLAC",
+    "The Djinn 2021 1080p BRRip DD5 1 X 264-EVO",
+    "Hive [2021 - Albania] drama",
+    "Souad [2021 - Egypt] drama",
+    "Swinki [2009 - Poland] drama",
+    "Dead Heat on a Merry Go Round [1966 - USA] thriller",
+    "Justified - Season 1 to 6 - Mp4 x264 AC3 1080p",
+    "Movie 43 (2013) 720p BluRay x264 -[MoviesFD]",
+    "Mommy (2014) French 720p BluRay x264 -[MoviesFD]",
+    "Rendez Vous.2015.DUBBED.1080p.WEBRip.x265-R4RBG[TGx]",
+    "The Best Offer.mkv"
 ]
```

### Comparing `parse-torrent-title-2.4/tests/files/output_raw.json` & `parse-torrent-title-2.5/tests/files/output_raw.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9734263098379193%*

 * *Differences: {'241': "{'encoder': 'iDN'}",*

 * * 'insert': "[(369, OrderedDict([('audio', 'DD5 1'), ('codec', 'X 264'), ('quality', 'BRRip'), "*

 * *           "('resolution', '1080p'), ('title', 'The Djinn'), ('year', 2021)])), (370, "*

 * *           "OrderedDict([('genre', 'drama'), ('language', 'Albania'), ('title', 'Hive'), ('year', "*

 * *           "2021)])), (371, OrderedDict([('genre', 'drama'), ('language', 'Egypt'), ('title', "*

 * *           "'Souad'), ('year', 2021)])), (372, OrderedDict([('genre', 'drama'), ('language', "*

 * *        […]*

```diff
@@ -2331,15 +2331,15 @@
         "quality": "WEBRip",
         "resolution": "1080p",
         "site": "ArMor",
         "title": "Wasp Network",
         "year": 2020
     },
     {
-        "encoder": "CreW",
+        "encoder": "iDN",
         "filetype": "mkv",
         "language": [
             "ITA",
             "ENG"
         ],
         "quality": "Bluray",
         "resolution": "1080p",
@@ -3680,9 +3680,85 @@
         "audio": "Dual-Audio",
         "episode": 24,
         "remux": true,
         "resolution": "1080p",
         "season": 1,
         "site": "FFF-Remux",
         "title": "Accel World"
+    },
+    {
+        "audio": "DD5 1",
+        "codec": "X 264",
+        "quality": "BRRip",
+        "resolution": "1080p",
+        "title": "The Djinn",
+        "year": 2021
+    },
+    {
+        "genre": "drama",
+        "language": "Albania",
+        "title": "Hive",
+        "year": 2021
+    },
+    {
+        "genre": "drama",
+        "language": "Egypt",
+        "title": "Souad",
+        "year": 2021
+    },
+    {
+        "genre": "drama",
+        "language": "Poland",
+        "title": "Swinki",
+        "year": 2009
+    },
+    {
+        "genre": "thriller",
+        "title": "Dead Heat on a Merry Go Round",
+        "year": 1966
+    },
+    {
+        "audio": "AC3",
+        "codec": "x264",
+        "filetype": "Mp4",
+        "resolution": "1080p",
+        "season": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6
+        ],
+        "title": "Justified"
+    },
+    {
+        "codec": "x264",
+        "quality": "BluRay",
+        "resolution": "720p",
+        "site": "MoviesFD",
+        "title": "Movie 43",
+        "year": 2013
+    },
+    {
+        "codec": "x264",
+        "language": "French",
+        "quality": "BluRay",
+        "resolution": "720p",
+        "site": "MoviesFD",
+        "title": "Mommy",
+        "year": 2014
+    },
+    {
+        "codec": "x265",
+        "encoder": "R4RBG",
+        "quality": "WEBRip",
+        "resolution": "1080p",
+        "site": "TGx",
+        "title": "Rendez Vous.",
+        "year": 2015
+    },
+    {
+        "filetype": "mkv",
+        "title": "The Best Offer"
     }
 ]
```

### Comparing `parse-torrent-title-2.4/parse_torrent_title.egg-info/PKG-INFO` & `parse-torrent-title-2.5/parse_torrent_title.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-torrent-title
-Version: 2.4
+Version: 2.5
 Summary: Extract media information from torrent-like filename
 Home-page: https://github.com/platelminto/parse-torrent-title
 Author: Giorgio Momigliano
 Author-email: gmomigliano@protonmail.com
 License: MIT
 Description: # parse-torrent-title
         
@@ -55,14 +55,17 @@
         ## Examples
         
         Movies, series (seasons & episodes), and subtitles can be parsed. All meaningful information is
         extracted and returned in a dictionary. Text which couldn't be
         parsed is returned in the `excess` field.
         
         ```py
+        import PTN
+        
+        
         PTN.parse('The Walking Dead S05E03 720p HDTV x264-ASAP[ettv]')
         # {
         #     'encoder': 'ASAP',
         #     'title': 'The Walking Dead',
         #     'season':  5,
         #     'episode': 3,
         #     'resolution': '720p',
```

