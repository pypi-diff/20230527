# Comparing `tmp/PlexPreferNonForcedSubs-2.1.7.tar.gz` & `tmp/PlexPreferNonForcedSubs-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlexPreferNonForcedSubs-2.1.7.tar", last modified: Thu May 18 22:46:17 2023, max compression
+gzip compressed data, was "PlexPreferNonForcedSubs-2.1.8.tar", last modified: Sat May 27 20:26:56 2023, max compression
```

## Comparing `PlexPreferNonForcedSubs-2.1.7.tar` & `PlexPreferNonForcedSubs-2.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 22:46:17.818896 PlexPreferNonForcedSubs-2.1.7/
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.1.7/LICENSE
--rw-rw-rw-   0        0        0     6139 2023-05-18 22:46:17.818896 PlexPreferNonForcedSubs-2.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 22:46:17.785897 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs/
--rw-rw-rw-   0        0        0     7512 2023-05-18 22:42:10.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
--rw-rw-rw-   0        0        0        0 2023-05-18 18:48:34.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 22:46:17.815895 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/
--rw-rw-rw-   0        0        0     6139 2023-05-18 22:46:17.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-05-18 22:46:17.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 22:46:17.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-05-18 22:46:17.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 22:46:17.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-18 22:46:17.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5455 2023-05-18 22:03:50.000000 PlexPreferNonForcedSubs-2.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-18 22:46:17.819896 PlexPreferNonForcedSubs-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1546 2023-05-18 22:43:08.000000 PlexPreferNonForcedSubs-2.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 20:26:56.479556 PlexPreferNonForcedSubs-2.1.8/
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.1.8/LICENSE
+-rw-rw-rw-   0        0        0     6151 2023-05-27 20:26:56.479556 PlexPreferNonForcedSubs-2.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-27 20:26:56.444051 PlexPreferNonForcedSubs-2.1.8/PlexPreferNonForcedSubs/
+-rw-rw-rw-   0        0        0     7571 2023-05-27 20:24:38.000000 PlexPreferNonForcedSubs-2.1.8/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 18:48:34.000000 PlexPreferNonForcedSubs-2.1.8/PlexPreferNonForcedSubs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 20:26:56.477557 PlexPreferNonForcedSubs-2.1.8/PlexPreferNonForcedSubs.egg-info/
+-rw-rw-rw-   0        0        0     6151 2023-05-27 20:26:56.000000 PlexPreferNonForcedSubs-2.1.8/PlexPreferNonForcedSubs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-05-27 20:26:56.000000 PlexPreferNonForcedSubs-2.1.8/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 20:26:56.000000 PlexPreferNonForcedSubs-2.1.8/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-05-27 20:26:56.000000 PlexPreferNonForcedSubs-2.1.8/PlexPreferNonForcedSubs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-05-27 20:26:56.000000 PlexPreferNonForcedSubs-2.1.8/PlexPreferNonForcedSubs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-27 20:26:56.000000 PlexPreferNonForcedSubs-2.1.8/PlexPreferNonForcedSubs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5450 2023-05-27 20:24:17.000000 PlexPreferNonForcedSubs-2.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 20:26:56.480557 PlexPreferNonForcedSubs-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1569 2023-05-27 20:25:22.000000 PlexPreferNonForcedSubs-2.1.8/setup.py
```

### Comparing `PlexPreferNonForcedSubs-2.1.7/LICENSE` & `PlexPreferNonForcedSubs-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexPreferNonForcedSubs-2.1.7/PKG-INFO` & `PlexPreferNonForcedSubs-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.1.7
+Version: 2.1.8
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
+Author: RileyXX
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # PlexPreferNonForcedSubs
 
 ## Short Description
-This Python script sets all movies and shows in your local Plex library to English non-forced subtitles by default. It is compatible with Python 3.5 or later and designed to work on any operating system where Python is installed (Windows, macOS, Linux, etc).
+This Python script sets all movies and shows in your local Plex library to English non-forced subtitles by default. It designed to work on Python 3.5 or later and compatible on any operating system where Python is installed (Windows, macOS, Linux, etc).
 
 ## Long Description
 This script utilizes the Plex Python API and sets all movies and shows in your local Plex library to English non-forced subtitles by default. The subtitle preferences will be applied to your Plex profile and remembered on other devices. By default, Plex prefers forced subtitles when available for a given item. However, Plex does not natively allow you to prefer non-forced subtitles, which is why this script was created.
 
 The script has been thoroughly tested and confirmed to be working. Feel free to use the code for your own purposes. I will be running this code periodically on my home server along with some other Plex scripts, such as [Plex Auto Delete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py). Special thanks to everyone who provided assistance! If you encounter any bugs while using this script, please open an issue. Cheers!
 
 ## What are "non-forced" subtitles?
```

### Comparing `PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py` & `PlexPreferNonForcedSubs-2.1.8/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from plexapi.server import PlexServer
 from plexapi.media import SubtitleStream
 import os
 import traceback
 
 def report_error(error_message):
-    github_issue_url = "https://github.com/RileyXX/PlexPreferNonForcedSubs/issues/new?assignees=&labels=&projects=&template=bug_report.yml"
+    github_issue_url = "https://github.com/RileyXX/PlexPreferNonForcedSubs/issues/new?template=bug_report.yml"
     traceback_info = traceback.format_exc()
 
     print("\n--- ERROR ---")
     print(error_message)
     print("Please submit the error to GitHub with the following information:")
     print("-" * 50)
     print(traceback_info)
@@ -51,16 +51,16 @@
 
         for section in plex.library.sections():
             if section.type == 'movie':
                 for movie in section.all():
                     english_subs = movie.subtitleStreams()
                     if english_subs is not None:
                         english_subs = [stream for stream in english_subs if stream is not None and stream.languageCode == 'eng']
-                        non_forced_english_subs = [stream for stream in english_subs if stream is not None and (not stream.forced or ('forced' not in getattr(stream, 'title', '').lower()))]
-                        forced_english_subs = [stream for stream in english_subs if stream is not None and (hasattr(stream, 'title') and stream.title is not None and 'forced' in stream.title.lower())]
+                        non_forced_english_subs = [stream for stream in english_subs if stream is not None and (not stream.forced or (hasattr(stream, 'title') and 'forced' not in (getattr(stream, 'title', '') or '').lower()))]
+                        forced_english_subs = [stream for stream in english_subs if stream is not None and (stream.forced or (hasattr(stream, 'title') and 'forced' in (getattr(stream, 'title', '') or '').lower()))]
                         part = movie.media[0].parts[0]
                         partsid = part.id
                         if forced_english_subs and non_forced_english_subs:
                             non_forced_english_subs[0].setDefault()
                             print(f'\033[92m{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English (Non-Forced)".ljust(status_width)} | {"Y".ljust(changes_width)}\033[0m')
                         elif non_forced_english_subs and not forced_english_subs:
                             print(f'{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English".ljust(status_width)} | {"N".ljust(changes_width)}')
@@ -86,27 +86,27 @@
         for section in plex.library.sections():
             if section.type == 'show':
                 for show in section.all():
                     for episode in show.episodes():
                         english_subs = episode.subtitleStreams()
                         if english_subs is not None:
                             english_subs = [stream for stream in english_subs if stream is not None and stream.languageCode == 'eng']
-                            non_forced_english_subs = [stream for stream in english_subs if stream is not None and (not stream.forced or ('forced' not in getattr(stream, 'title', '').lower()))]
-                            forced_english_subs = [stream for stream in english_subs if stream is not None and (hasattr(stream, 'title') and stream.title is not None and 'forced' in stream.title.lower())]
+                            non_forced_english_subs = [stream for stream in english_subs if stream is not None and (not stream.forced or (hasattr(stream, 'title') and 'forced' not in (getattr(stream, 'title', '') or '').lower()))]
+                            forced_english_subs = [stream for stream in english_subs if stream is not None and (stream.forced or (hasattr(stream, 'title') and 'forced' in (getattr(stream, 'title', '') or '').lower()))]
                             part = episode.media[0].parts[0]
                             partsid = part.id
                             if forced_english_subs and non_forced_english_subs:
                                 non_forced_english_subs[0].setDefault()
                                 print(f'\033[92m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English (Non-Forced)".ljust(status_width)} | {"Y".ljust(changes_width)}\033[0m')
                             elif non_forced_english_subs and not forced_english_subs:
                                 print(f'{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English".ljust(status_width)} | {"N".ljust(changes_width)}')
                             elif not non_forced_english_subs and not forced_english_subs:
                                 print(f'\033[91m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"No Subtitles Found".ljust(status_width)} | {"N".ljust(changes_width)}\033[0m')
                             else:
                                 print(f'\033[91m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English (Forced)".ljust(status_width)} | {"N (Error)".ljust(changes_width)}\033[0m')
 
     except Exception as e:
         error_message = "An error occurred while running the script."
-        errorHandling.report_error(error_message)
+        report_error(error_message)
 
 if __name__ == '__main__':
     main()
```

### Comparing `PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/PKG-INFO` & `PlexPreferNonForcedSubs-2.1.8/PlexPreferNonForcedSubs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.1.7
+Version: 2.1.8
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
+Author: RileyXX
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # PlexPreferNonForcedSubs
 
 ## Short Description
-This Python script sets all movies and shows in your local Plex library to English non-forced subtitles by default. It is compatible with Python 3.5 or later and designed to work on any operating system where Python is installed (Windows, macOS, Linux, etc).
+This Python script sets all movies and shows in your local Plex library to English non-forced subtitles by default. It designed to work on Python 3.5 or later and compatible on any operating system where Python is installed (Windows, macOS, Linux, etc).
 
 ## Long Description
 This script utilizes the Plex Python API and sets all movies and shows in your local Plex library to English non-forced subtitles by default. The subtitle preferences will be applied to your Plex profile and remembered on other devices. By default, Plex prefers forced subtitles when available for a given item. However, Plex does not natively allow you to prefer non-forced subtitles, which is why this script was created.
 
 The script has been thoroughly tested and confirmed to be working. Feel free to use the code for your own purposes. I will be running this code periodically on my home server along with some other Plex scripts, such as [Plex Auto Delete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py). Special thanks to everyone who provided assistance! If you encounter any bugs while using this script, please open an issue. Cheers!
 
 ## What are "non-forced" subtitles?
```

### Comparing `PlexPreferNonForcedSubs-2.1.7/README.md` & `PlexPreferNonForcedSubs-2.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # PlexPreferNonForcedSubs
 
 ## Short Description
-This Python script sets all movies and shows in your local Plex library to English non-forced subtitles by default. It is compatible with Python 3.5 or later and designed to work on any operating system where Python is installed (Windows, macOS, Linux, etc).
+This Python script sets all movies and shows in your local Plex library to English non-forced subtitles by default. It designed to work on Python 3.5 or later and compatible on any operating system where Python is installed (Windows, macOS, Linux, etc).
 
 ## Long Description
 This script utilizes the Plex Python API and sets all movies and shows in your local Plex library to English non-forced subtitles by default. The subtitle preferences will be applied to your Plex profile and remembered on other devices. By default, Plex prefers forced subtitles when available for a given item. However, Plex does not natively allow you to prefer non-forced subtitles, which is why this script was created.
 
 The script has been thoroughly tested and confirmed to be working. Feel free to use the code for your own purposes. I will be running this code periodically on my home server along with some other Plex scripts, such as [Plex Auto Delete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py). Special thanks to everyone who provided assistance! If you encounter any bugs while using this script, please open an issue. Cheers!
 
 ## What are "non-forced" subtitles?
```

### Comparing `PlexPreferNonForcedSubs-2.1.7/setup.py` & `PlexPreferNonForcedSubs-2.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '2.1.7'
+VERSION = '2.1.8'
 DESCRIPTION = 'This script will set all movies and shows in your local Plex library to English non forced subtitles by default.'
 LONG_DESCRIPTION = 'This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices.'
 
 # Setting up
 setup(
     name="PlexPreferNonForcedSubs",
     version=VERSION,
+    author="RileyXX",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/RileyXX/PlexPreferNonForcedSubs",
     packages=find_packages(),
     install_requires=['plexapi'],
     keywords=['python', 'video', 'plex', 'subtitles', 'subs'],
```

