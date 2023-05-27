# Comparing `tmp/jupyterlab_language_pack_no_no-3.6.post3.tar.gz` & `tmp/jupyterlab_language_pack_no_no-4.0.post0.tar.gz`

## Comparing `jupyterlab_language_pack_no_no-3.6.post3.tar` & `jupyterlab_language_pack_no_no-4.0.post0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/.copier-answers.yml
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/CONTRIBUTORS.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/dask_labextension.po
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyter_archive.po
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyter_collaboration.po
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyter_resource_usage.po
--rw-r--r--   0        0        0   269921 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab.po
--rw-r--r--   0        0        0    96097 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_git.po
--rw-r--r--   0        0        0    42570 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_lsp.po
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_search_replace.po
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_tour.po
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_widgets.po
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupytext.po
--rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/notebook.po
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/retrolab.po
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/spellchecker.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/LICENSE.txt
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/README.md
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/pyproject.toml
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-3.6.post3/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/.copier-answers.yml
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/dask_labextension.po
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyter_archive.po
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyter_collaboration.po
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyter_resource_usage.po
+-rw-r--r--   0        0        0   194138 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab.po
+-rw-r--r--   0        0        0    96097 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_git.po
+-rw-r--r--   0        0        0    42570 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_lsp.po
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_search_replace.po
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_tour.po
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_widgets.po
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupytext.po
+-rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/notebook.po
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/retrolab.po
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/spellchecker.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/LICENSE.txt
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/README.md
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/pyproject.toml
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 jupyterlab_language_pack_no_no-4.0.post0/PKG-INFO
```

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/dask_labextension.po` & `jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/dask_labextension.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyter_archive.po` & `jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyter_archive.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyter_resource_usage.po` & `jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyter_resource_usage.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_git.po` & `jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_git.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_lsp.po` & `jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_lsp.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_search_replace.po` & `jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_search_replace.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_spreadsheet_editor.po` & `jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_spreadsheet_editor.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_tour.po` & `jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_tour.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_widgets.po` & `jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupyterlab_widgets.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupytext.po` & `jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/jupytext.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/notebook.po` & `jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/notebook.po`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: no\n"
 "X-Crowdin-File: /main/extensions/notebook/locale/notebook.pot\n"
 "X-Crowdin-File-ID: 231\n"
 "Language-Team: Norwegian\n"
 "Language: no_NO\n"
-"PO-Revision-Date: 2023-04-12 17:58\n"
+"PO-Revision-Date: 2023-05-21 14:18\n"
 
 #: /packages/application-extension/schema/menus.json:/description /packages/application-extension/schema/menus.json:/title
 msgctxt "schema"
 msgid "Jupyter Notebook Menu Entries"
 msgstr ""
 
 #: /packages/application-extension/schema/menus.json:/jupyter.lab.menus/main[2]/items[1]/submenu/label
@@ -42,15 +42,15 @@
 #: /packages/application-extension/schema/top.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "Jupyter Notebook Top Area"
 msgstr ""
 
 #: /packages/application-extension/schema/top.json:/properties/visible/description
 msgctxt "settings"
-msgid "Whether to show the top bar or not"
+msgid "Whether to show the top bar or not, yes for always showing, no for always not showing, automatic for adjusting to screen size"
 msgstr ""
 
 #: /packages/application-extension/schema/top.json:/properties/visible/title
 msgctxt "settings"
 msgid "Top Bar Visibility"
 msgstr ""
 
@@ -232,92 +232,88 @@
 msgid "Rename…"
 msgstr ""
 
 #: packages/application-extension/src/index.ts:481
 msgid "Show Header"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:564
+#: packages/application-extension/src/index.ts:571
 msgid "Show %1 in the left sidebar"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:569
+#: packages/application-extension/src/index.ts:576
 msgid "Show %1 in the right sidebar"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:574
+#: packages/application-extension/src/index.ts:581
 msgid "Show %1 in the sidebar"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:689
+#: packages/application-extension/src/index.ts:696
 msgid "Left Sidebar"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:691
+#: packages/application-extension/src/index.ts:698
 msgid "Right Sidebar"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:880
+#: packages/application-extension/src/index.ts:887
 msgid "Toggle Zen Mode"
 msgstr ""
 
-#: packages/application/src/shell.ts:196 packages/application/src/shell.ts:200
+#: packages/application/src/shell.ts:203 packages/application/src/shell.ts:207
 msgid "Collapse %1 side panel"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:116
+#: packages/help-extension/src/index.tsx:114
 msgid "Version: %1"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:117
+#: packages/help-extension/src/index.tsx:115
 msgid "© 2021-2023 Jupyter Notebook Contributors"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:133 packages/help-extension/src/index.tsx:215
+#: packages/help-extension/src/index.tsx:131
 msgid "Dismiss"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:174 packages/help-extension/src/index.tsx:79 packages/lab-extension/src/index.ts:162
+#: packages/help-extension/src/index.tsx:77 packages/lab-extension/src/index.ts:178
 msgid "Help"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:177 packages/help-extension/src/index.tsx:182
-msgid "Keyboard Shortcuts"
-msgstr ""
-
-#: packages/help-extension/src/index.tsx:191
-msgid "Name"
+#: packages/help-extension/src/index.tsx:80
+msgid "About %1"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:192
-msgid "Shortcut"
+#: packages/help-extension/src/index.tsx:92
+msgid "JUPYTER NOTEBOOK ON GITHUB"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:82
-msgid "About %1"
+#: packages/help-extension/src/index.tsx:93
+msgid "CONTRIBUTOR LIST"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:94
-msgid "JUPYTER NOTEBOOK ON GITHUB"
+#: packages/lab-extension/src/index.ts:131
+msgid "Notebook"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:95
-msgid "CONTRIBUTOR LIST"
+#: packages/lab-extension/src/index.ts:132 packages/lab-extension/src/index.ts:142
+msgid "Open in %1"
 msgstr ""
 
-#: packages/lab-extension/src/index.ts:117 packages/lab-extension/src/index.ts:126
-msgid "Open With %1"
+#: packages/lab-extension/src/index.ts:141
+msgid "JupyterLab"
 msgstr ""
 
-#: packages/lab-extension/src/index.ts:165
+#: packages/lab-extension/src/index.ts:181
 msgid "Launch Jupyter Notebook File Browser"
 msgstr ""
 
-#: packages/lab-extension/src/index.ts:81
-msgid "Interface"
+#: packages/lab-extension/src/index.ts:82
+msgid "Open in..."
 msgstr ""
 
 #: packages/notebook-extension/src/index.ts:107
 msgid "Last Checkpoint: %1"
 msgstr ""
 
 #: packages/notebook-extension/src/trusted.tsx:75
```

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/retrolab.po` & `jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/retrolab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/spellchecker.po` & `jupyterlab_language_pack_no_no-4.0.post0/jupyterlab_language_pack_no_NO/locale/no_NO/LC_MESSAGES/spellchecker.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/.gitignore` & `jupyterlab_language_pack_no_no-4.0.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/LICENSE.txt` & `jupyterlab_language_pack_no_no-4.0.post0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/pyproject.toml` & `jupyterlab_language_pack_no_no-4.0.post0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 keywords = ["jupyterlab", "language", "language pack", "localization"]
 dynamic = ["version"]
 
 [project.entry-points."jupyterlab.languagepack"]
 no_NO = "jupyterlab_language_pack_no_NO"
 
-[projects.urls]
+[project.urls]
 homepage = "https://github.com/jupyterlab/language-packs"
 
 [tool.hatch.build]
 artifacts = [
     "CONTRIBUTORS.md"
 ]
```

### Comparing `jupyterlab_language_pack_no_no-3.6.post3/PKG-INFO` & `jupyterlab_language_pack_no_no-4.0.post0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: jupyterlab-language-pack-no-NO
-Version: 3.6.post3
+Version: 4.0.post0
 Summary: JupyterLab Norwegian Bokmål (Norway) Language Pack
+Project-URL: homepage, https://github.com/jupyterlab/language-packs
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2023 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

