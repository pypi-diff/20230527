# Comparing `tmp/jupyterlab_language_pack_de_de-3.6.post3.tar.gz` & `tmp/jupyterlab_language_pack_de_de-4.0.post0.tar.gz`

## Comparing `jupyterlab_language_pack_de_de-3.6.post3.tar` & `jupyterlab_language_pack_de_de-4.0.post0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/.copier-answers.yml
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/CONTRIBUTORS.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/dask_labextension.po
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyter_archive.po
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyter_collaboration.po
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyter_resource_usage.po
--rw-r--r--   0        0        0   296487 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab.po
--rw-r--r--   0        0        0    99067 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_git.po
--rw-r--r--   0        0        0    42869 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_lsp.po
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_search_replace.po
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_tour.po
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_widgets.po
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupytext.po
--rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/notebook.po
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/retrolab.po
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/spellchecker.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/LICENSE.txt
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/README.md
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/pyproject.toml
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-3.6.post3/PKG-INFO
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/.copier-answers.yml
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/dask_labextension.po
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyter_archive.po
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyter_collaboration.po
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyter_resource_usage.po
+-rw-r--r--   0        0        0   216247 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab.po
+-rw-r--r--   0        0        0    99067 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_git.po
+-rw-r--r--   0        0        0    42869 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_lsp.po
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_search_replace.po
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_tour.po
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_widgets.po
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupytext.po
+-rw-r--r--   0        0        0     9836 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/notebook.po
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/retrolab.po
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/spellchecker.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/LICENSE.txt
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/README.md
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/pyproject.toml
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_language_pack_de_de-4.0.post0/PKG-INFO
```

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/CONTRIBUTORS.md` & `jupyterlab_language_pack_de_de-4.0.post0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/dask_labextension.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/dask_labextension.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyter_archive.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyter_archive.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyter_resource_usage.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyter_resource_usage.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab.po`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: de\n"
 "X-Crowdin-File: /main/jupyterlab/locale/jupyterlab.pot\n"
 "X-Crowdin-File-ID: 191\n"
 "Language-Team: German\n"
 "Language: de_DE\n"
-"PO-Revision-Date: 2023-04-30 17:12\n"
+"PO-Revision-Date: 2023-05-21 14:18\n"
 
 #: /examples/federated/md_package/schema/plugin.json:/description /packages/markdownviewer-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Markdown viewer settings."
 msgstr "Markdown-Viewer-Einstellungen."
 
 #: /examples/federated/md_package/schema/plugin.json:/jupyter.lab.setting-icon-label /packages/markdownviewer-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
@@ -27,27 +27,27 @@
 #: /examples/federated/md_package/schema/plugin.json:/properties/fontFamily/description /packages/markdownviewer-extension/schema/plugin.json:/properties/fontFamily/description
 msgctxt "settings"
 msgid "The font family used to render markdown.\n"
 "If `null`, value from current theme is used."
 msgstr "Die Schriftfamilie, die für die Darstellung von Markdown verwendet wird.\n"
 "Wenn `null`, wird der Wert aus dem aktuellen Theme verwendet."
 
-#: /examples/federated/md_package/schema/plugin.json:/properties/fontFamily/title /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/fontFamily/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/fontFamily/title /packages/markdownviewer-extension/schema/plugin.json:/properties/fontFamily/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/fontFamily/title
+#: /examples/federated/md_package/schema/plugin.json:/properties/fontFamily/title /packages/markdownviewer-extension/schema/plugin.json:/properties/fontFamily/title
 msgctxt "settings"
 msgid "Font Family"
 msgstr "Schriftfamilie"
 
 #: /examples/federated/md_package/schema/plugin.json:/properties/fontSize/description /packages/markdownviewer-extension/schema/plugin.json:/properties/fontSize/description
 msgctxt "settings"
 msgid "The size in pixel of the font used to render markdown.\n"
 "If `null`, value from current theme is used."
 msgstr "Die Größe der Schriftart in Pixel, die für die Darstellung von Markdown verwendet wird.\n"
 "Wenn `null`, wird der Wert aus dem aktuellen Theme verwendet."
 
-#: /examples/federated/md_package/schema/plugin.json:/properties/fontSize/title /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/fontSize/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/fontSize/title /packages/markdownviewer-extension/schema/plugin.json:/properties/fontSize/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/fontSize/title
+#: /examples/federated/md_package/schema/plugin.json:/properties/fontSize/title /packages/markdownviewer-extension/schema/plugin.json:/properties/fontSize/title
 msgctxt "settings"
 msgid "Font Size"
 msgstr "Schriftgröße"
 
 #: /examples/federated/md_package/schema/plugin.json:/properties/hideFrontMatter/description /packages/markdownviewer-extension/schema/plugin.json:/properties/hideFrontMatter/description
 msgctxt "settings"
 msgid "Whether to hide YAML front matter.\n"
@@ -67,15 +67,15 @@
 #: /examples/federated/md_package/schema/plugin.json:/properties/lineHeight/description /packages/markdownviewer-extension/schema/plugin.json:/properties/lineHeight/description
 msgctxt "settings"
 msgid "The line height used to render markdown.\n"
 "If `null`, value from current theme is used."
 msgstr "Die Zeilenhöhe, die zum Rendern von Markdown verwendet wird.\n"
 "Wenn `null`, wird der Wert aus dem aktuellen Thema verwendet."
 
-#: /examples/federated/md_package/schema/plugin.json:/properties/lineHeight/title /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/lineHeight/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/lineHeight/title /packages/markdownviewer-extension/schema/plugin.json:/properties/lineHeight/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/lineHeight/title
+#: /examples/federated/md_package/schema/plugin.json:/properties/lineHeight/title /packages/markdownviewer-extension/schema/plugin.json:/properties/lineHeight/title
 msgctxt "settings"
 msgid "Line Height"
 msgstr "Linien Höhe"
 
 #: /examples/federated/md_package/schema/plugin.json:/properties/lineWidth/description /packages/markdownviewer-extension/schema/plugin.json:/properties/lineWidth/description
 msgctxt "settings"
 msgid "The text line width expressed in CSS ch units.\n"
@@ -280,58 +280,29 @@
 msgstr ""
 
 #: /packages/application-extension/schema/shell.json:/properties/layout/title
 msgctxt "settings"
 msgid "Customize shell widget positioning"
 msgstr ""
 
-#: /packages/application-extension/schema/shell.json:/properties/startMode/description /packages/statusbar-extension/schema/plugin.json:/properties/startMode/description
+#: /packages/application-extension/schema/shell.json:/properties/startMode/description
 msgctxt "settings"
 msgid "The mode under which JupyterLab should start. If empty, the mode will be imposed by the URL"
 msgstr ""
 
 #: /packages/application-extension/schema/shell.json:/properties/startMode/title
 msgctxt "settings"
 msgid "Start mode: ``, `single` or `multiple`"
 msgstr ""
 
 #: /packages/application-extension/schema/shell.json:/title
 msgctxt "schema"
 msgid "JupyterLab Shell"
 msgstr ""
 
-#: /packages/application-extension/schema/sidebar.json:/description
-msgctxt "schema"
-msgid "Sidebar layout settings."
-msgstr "Seitenleisten-Layouteinstellungen."
-
-#: /packages/application-extension/schema/sidebar.json:/jupyter.lab.setting-icon-label
-msgctxt "settings"
-msgid "Sidebar"
-msgstr "Seitenleiste"
-
-#: /packages/application-extension/schema/sidebar.json:/properties/overrides/description
-msgctxt "settings"
-msgid "Overrides for where to show sidebar items\n"
-"e.g., {\"jp-debugger-sidebar\": \"left\"}\n"
-"You can also change this by right-clicking the sidebar icons."
-msgstr "Überschreibt, wo die Seitenleiste angezeigt werden soll,\n"
-"z.B. {\"jp-debugger-sidebar\": \"left\"}\n"
-"Sie können dies auch ändern, indem Sie mit der rechten Maustaste auf die Seitenleistensymbole klicken."
-
-#: /packages/application-extension/schema/sidebar.json:/properties/overrides/title
-msgctxt "settings"
-msgid "Overrides"
-msgstr "Überschreibungen"
-
-#: /packages/application-extension/schema/sidebar.json:/title
-msgctxt "schema"
-msgid "Sidebar"
-msgstr "Seitenleiste"
-
 #: /packages/application-extension/schema/top-bar.json:/definitions/toolbarItem/properties/disabled/title /packages/cell-toolbar-extension/schema/plugin.json:/definitions/toolbarItem/properties/disabled/title /packages/csvviewer-extension/schema/csv.json:/definitions/toolbarItem/properties/disabled/title /packages/csvviewer-extension/schema/tsv.json:/definitions/toolbarItem/properties/disabled/title /packages/filebrowser-extension/schema/widget.json:/definitions/toolbarItem/properties/disabled/title /packages/fileeditor-extension/schema/plugin.json:/definitions/toolbarItem/properties/disabled/title /packages/htmlviewer-extension/schema/plugin.json:/definitions/toolbarItem/properties/disabled/title /packages/notebook-extension/schema/panel.json:/definitions/toolbarItem/properties/disabled/title
 msgctxt "settings"
 msgid "Whether the item is ignored or not"
 msgstr ""
 
 #: /packages/application-extension/schema/top-bar.json:/definitions/toolbarItem/properties/icon/description /packages/cell-toolbar-extension/schema/plugin.json:/definitions/toolbarItem/properties/icon/description /packages/csvviewer-extension/schema/csv.json:/definitions/toolbarItem/properties/icon/description /packages/csvviewer-extension/schema/tsv.json:/definitions/toolbarItem/properties/icon/description /packages/filebrowser-extension/schema/widget.json:/definitions/toolbarItem/properties/icon/description /packages/fileeditor-extension/schema/plugin.json:/definitions/toolbarItem/properties/icon/description /packages/htmlviewer-extension/schema/plugin.json:/definitions/toolbarItem/properties/icon/description /packages/notebook-extension/schema/panel.json:/definitions/toolbarItem/properties/icon/description
 msgctxt "settings"
@@ -600,159 +571,37 @@
 msgstr ""
 
 #: /packages/celltags-extension/schema/plugin.json:/title /packages/notebook-extension/schema/tools.json:/title
 msgctxt "schema"
 msgid "Common tools"
 msgstr "Gewöhnliche Werkzeuge"
 
-#: /packages/codemirror-extension/schema/commands.json:/description /packages/codemirror-extension/schema/plugin.json:/description
+#: /packages/codemirror-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Text editor settings for all CodeMirror editors."
 msgstr "Texteditor-Einstellungen für alle CodeMirror-Editoren."
 
-#: /packages/codemirror-extension/schema/commands.json:/jupyter.lab.menus/main[0]/items[1]/submenu/label /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[1]/items[1]/submenu/label
-msgctxt "menu"
-msgid "Text Editor Syntax Highlighting"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/jupyter.lab.menus/main[1]/items[0]/submenu/label
-msgctxt "menu"
-msgid "Text Editor Key Map"
-msgstr "Texteditor-Tastenbelegung"
-
-#: /packages/codemirror-extension/schema/commands.json:/jupyter.lab.menus/main[1]/items[1]/submenu/label /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[2]/items[5]/submenu/label
-msgctxt "menu"
-msgid "Text Editor Theme"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/jupyter.lab.setting-icon-label /packages/codemirror-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
+#: /packages/codemirror-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "CodeMirror"
 msgstr ""
 
-#: /packages/codemirror-extension/schema/commands.json:/properties/keyMap/description
-msgctxt "settings"
-msgid "Configures the keymap to use"
-msgstr "Konfiguriert die zu verwendende Tastaturbelegung"
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/keyMap/title
-msgctxt "settings"
-msgid "Key Map"
-msgstr "Tastenbelegung"
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/lineWiseCopyCut/description /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWiseCopyCut/description /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWiseCopyCut/description
-msgctxt "settings"
-msgid "When enabled, which is the default, doing copy or cut when there is no selection will copy or cut the whole lines that have cursors on them."
-msgstr "Wenn diese Funktion aktiviert ist (Standardeinstellung), werden beim Kopieren oder Ausschneiden ohne Auswahl die gesamten Zeilen mit Cursor kopiert oder ausgeschnitten."
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/lineWiseCopyCut/title /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWiseCopyCut/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWiseCopyCut/title
-msgctxt "settings"
-msgid "Line-wise Ctrl-C"
-msgstr "Zeilenweise Strg-C"
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/scrollPastEnd/description
-msgctxt "settings"
-msgid "Whether to scroll past the end of text document"
-msgstr "Ob über das Ende des Textdokuments hinaus gescrollt werden soll"
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/scrollPastEnd/title /packages/fileeditor-extension/schema/plugin.json:/properties/scrollPastEnd/title
-msgctxt "settings"
-msgid "Scroll behavior"
-msgstr "Scroll-Verhalten"
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/selectionPointer/description
-msgctxt "settings"
-msgid "Control the mouse cursor appearance when hovering over the selection. Value is boolean or string, e.g. 'pointer'."
-msgstr "Steuert das Aussehen des Mauszeigers, wenn er über der Auswahl schwebt. Der Wert ist boolean oder string, z. B. \"Zeiger\"."
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/selectionPointer/oneOf[0]/title
-msgctxt "settings"
-msgid "Use default"
-msgstr "Standard verwenden"
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/selectionPointer/oneOf[1]/title
-msgctxt "settings"
-msgid "Cursor pointer name"
-msgstr "Name des Cursor-Zeigers"
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/selectionPointer/title
-msgctxt "settings"
-msgid "Selection Pointer"
-msgstr "Auswahl-Zeiger"
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/styleActiveLine/description
-msgctxt "settings"
-msgid "Highlight active line. Value is boolean, or { nonEmpty: boolean }."
-msgstr "Aktive Zeile hervorheben. Wert ist boolean, oder { nonEmpty: boolean }."
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/styleActiveLine/oneOf[0]/title
-msgctxt "settings"
-msgid "Boolean"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/styleActiveLine/oneOf[1]/title
-msgctxt "settings"
-msgid "Object"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/styleActiveLine/title
-msgctxt "settings"
-msgid "Style Active Line"
-msgstr "Aktive Zeile formatieren"
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/styleSelectedText/title
-msgctxt "settings"
-msgid "Style Selected Text"
-msgstr "Ausgewählten Text formatieren"
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/theme/description
-msgctxt "settings"
-msgid "CSS file defining the corresponding\n"
-".cm-s-[name] styles is loaded"
-msgstr "CSS-Datei, die die entsprechenden\n"
-".cm-s-[name] Stile definiert, wird geladen"
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/theme/title /packages/terminal-extension/schema/plugin.json:/properties/theme/title
-msgctxt "settings"
-msgid "Theme"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/title /packages/codemirror-extension/schema/plugin.json:/title
-msgctxt "schema"
-msgid "CodeMirror"
-msgstr ""
-
 #: /packages/codemirror-extension/schema/plugin.json:/properties/defaultConfig/description
 msgctxt "settings"
 msgid "Base configuration used by all CodeMirror editors."
 msgstr ""
 
 #: /packages/codemirror-extension/schema/plugin.json:/properties/defaultConfig/title
 msgctxt "settings"
 msgid "Default editor configuration"
 msgstr ""
 
-#: /packages/completer-extension/schema/consoles.json:/description /packages/console-extension/schema/completer.json:/description
+#: /packages/codemirror-extension/schema/plugin.json:/title
 msgctxt "schema"
-msgid "Console completer settings."
-msgstr "Console Completer Einstellungen."
-
-#: /packages/completer-extension/schema/consoles.json:/title /packages/console-extension/schema/completer.json:/title
-msgctxt "schema"
-msgid "Console Completer"
-msgstr "Konsolenvervollständigung"
-
-#: /packages/completer-extension/schema/files.json:/description /packages/fileeditor-extension/schema/completer.json:/description
-msgctxt "schema"
-msgid "File editor completer settings."
-msgstr "File Editor Completer Einstellungen."
-
-#: /packages/completer-extension/schema/files.json:/title /packages/fileeditor-extension/schema/completer.json:/title
-msgctxt "schema"
-msgid "File Editor Completer"
+msgid "CodeMirror"
 msgstr ""
 
 #: /packages/completer-extension/schema/manager.json:/description
 msgctxt "schema"
 msgid "Code Completion settings."
 msgstr ""
 
@@ -802,94 +651,34 @@
 msgstr ""
 
 #: /packages/completer-extension/schema/manager.json:/title
 msgctxt "schema"
 msgid "Code Completion"
 msgstr "Code-Vervollständigung"
 
-#: /packages/completer-extension/schema/notebooks.json:/description /packages/notebook-extension/schema/completer.json:/description
+#: /packages/console-extension/schema/completer.json:/description
 msgctxt "schema"
-msgid "Notebook completer settings."
-msgstr "Notebook Completer Einstellungen."
+msgid "Console completer settings."
+msgstr "Console Completer Einstellungen."
 
-#: /packages/completer-extension/schema/notebooks.json:/title /packages/notebook-extension/schema/completer.json:/title
+#: /packages/console-extension/schema/completer.json:/title
 msgctxt "schema"
-msgid "Notebook Completer"
-msgstr ""
+msgid "Console Completer"
+msgstr "Konsolenvervollständigung"
 
 #: /packages/console-extension/schema/foreign.json:/description
 msgctxt "schema"
 msgid "Code Console Foreign plugin settings."
 msgstr "Code Console Fremd-Plugin Einstellungen."
 
 #: /packages/console-extension/schema/foreign.json:/title
 msgctxt "schema"
 msgid "Code Console Foreign plugin"
 msgstr "Code Console Fremd-Plugin"
 
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/autoClosingBrackets/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/autoClosingBrackets/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/autoClosingBrackets/title
-msgctxt "settings"
-msgid "Auto Closing Brackets"
-msgstr "Automatisch schließende Klammern"
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/codeFolding/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/codeFolding/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/codeFolding/title
-msgctxt "settings"
-msgid "Code Folding"
-msgstr "Code-Faltung"
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/cursorBlinkRate/description /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/cursorBlinkRate/description /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/cursorBlinkRate/description
-msgctxt "settings"
-msgid "Half-period in milliseconds used for cursor blinking. The default blink rate is 530ms. By setting this to zero, blinking can be disabled. A negative value hides the cursor entirely."
-msgstr "Halbwertszeit in Millisekunden, die für das Blinken des Cursors verwendet wird. Die Standard-Blinkrate beträgt 530 ms. Wenn Sie diesen Wert auf Null setzen, kann das Blinken deaktiviert werden. Ein negativer Wert blendet den Cursor vollständig aus."
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/cursorBlinkRate/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/cursorBlinkRate/title
-msgctxt "settings"
-msgid "Cursor Blinking Rate"
-msgstr "Blinkfrequenz des Cursors"
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/insertSpaces/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/insertSpaces/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/insertSpaces/title
-msgctxt "settings"
-msgid "Insert Spaces"
-msgstr "Leerzeichen einfügen"
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/lineNumbers/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/lineNumbers/title
-msgctxt "settings"
-msgid "Show Line Numbers"
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWrap/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/lineWrap/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWrap/title
-msgctxt "settings"
-msgid "Line Wrap"
-msgstr "Zeilenumbruch"
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/matchBrackets/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/matchBrackets/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/matchBrackets/title
-msgctxt "settings"
-msgid "Match Brackets"
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/readOnly/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/readOnly/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/readOnly/title
-msgctxt "settings"
-msgid "Read Only"
-msgstr "Nur Lesen"
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/rulers/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/rulers/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/rulers/title
-msgctxt "settings"
-msgid "Rulers"
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/tabSize/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/tabSize/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/tabSize/title
-msgctxt "settings"
-msgid "Tab Size"
-msgstr "Tabgröße"
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/wordWrapColumn/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/wordWrapColumn/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/wordWrapColumn/title
-msgctxt "settings"
-msgid "Word Wrap Column"
-msgstr ""
-
 #: /packages/console-extension/schema/tracker.json:/description
 msgctxt "schema"
 msgid "Code Console settings."
 msgstr "Code Konsole Einstellungen."
 
 #: /packages/console-extension/schema/tracker.json:/jupyter.lab.menus/main[1]/items[1]/submenu/label
 msgctxt "menu"
@@ -911,19 +700,14 @@
 #: /packages/console-extension/schema/tracker.json:/properties/interactionMode/title
 msgctxt "settings"
 msgid "Interaction mode"
 msgstr "Interaktionsmodus"
 
 #: /packages/console-extension/schema/tracker.json:/properties/promptCellConfig/description
 msgctxt "settings"
-msgid "The configuration for all prompt cells."
-msgstr "Die Konfiguration für alle Prompt-Zellen."
-
-#: /packages/console-extension/schema/tracker.json:/properties/promptCellConfig/description
-msgctxt "settings"
 msgid "The configuration for all prompt cells; it will override the CodeMirror default configuration."
 msgstr ""
 
 #: /packages/console-extension/schema/tracker.json:/properties/promptCellConfig/title
 msgctxt "settings"
 msgid "Prompt Cell Configuration"
 msgstr "Prompt-Zellen-Konfiguration"
@@ -1171,61 +955,25 @@
 msgstr ""
 
 #: /packages/extensionmanager-extension/schema/plugin.json:/properties/disclaimed/title
 msgctxt "settings"
 msgid "Disclaimed Status"
 msgstr "Abgelehnt-Status"
 
-#: /packages/extensionmanager-extension/schema/plugin.json:/properties/enableCdn/description
-msgctxt "settings"
-msgid "Enables using the Content Delivery Network (CDN) to fetch full package data.  Otherwise, the configured NPM registry will be used. Due to a lack of CORS support by NPM registry, only disable if supplying a custom registry"
-msgstr ""
-
-#: /packages/extensionmanager-extension/schema/plugin.json:/properties/enableCdn/title
-msgctxt "settings"
-msgid "Enable Content Delivery Network (CDN)"
-msgstr ""
-
-#: /packages/extensionmanager-extension/schema/plugin.json:/properties/enabled/description
-msgctxt "settings"
-msgid "Enables extension manager (requires Node.js/npm).\n"
-"WARNING: installing untrusted extensions may be unsafe."
-msgstr ""
-
 #: /packages/extensionmanager-extension/schema/plugin.json:/properties/enabled/description
 msgctxt "settings"
 msgid "Enables extension manager.\n"
 "WARNING: installing untrusted extensions may be unsafe."
 msgstr ""
 
 #: /packages/extensionmanager-extension/schema/plugin.json:/properties/enabled/title
 msgctxt "settings"
 msgid "Enabled Status"
 msgstr "Aktiviert-Status"
 
-#: /packages/extensionmanager-extension/schema/plugin.json:/properties/npmCdn/description
-msgctxt "settings"
-msgid "The URI of the Content Delivery Network (CDN) to use for fetching full package data"
-msgstr ""
-
-#: /packages/extensionmanager-extension/schema/plugin.json:/properties/npmCdn/title
-msgctxt "settings"
-msgid "NPM Content Delivery Network (CDN)"
-msgstr ""
-
-#: /packages/extensionmanager-extension/schema/plugin.json:/properties/npmRegistry/description
-msgctxt "settings"
-msgid "The URI of the NPM registry to use for searching for jupyterlab extensions"
-msgstr ""
-
-#: /packages/extensionmanager-extension/schema/plugin.json:/properties/npmRegistry/title
-msgctxt "settings"
-msgid "NPM Registry"
-msgstr ""
-
 #: /packages/extensionmanager-extension/schema/plugin.json:/title
 msgctxt "schema"
 msgid "Extension Manager"
 msgstr "Erweiterungsmanager"
 
 #: /packages/filebrowser-extension/schema/browser.json:/description
 msgctxt "schema"
@@ -1275,19 +1023,14 @@
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showFileSizeColumn/title
 msgctxt "settings"
 msgid "Show file size column"
 msgstr "Dateigrößenspalte anzeigen"
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showHiddenFiles/description
 msgctxt "settings"
-msgid "Whether to show hidden files"
-msgstr "Ob versteckte Dateien angezeigt werden sollen"
-
-#: /packages/filebrowser-extension/schema/browser.json:/properties/showHiddenFiles/description
-msgctxt "settings"
 msgid "Whether to show hidden files. The server parameter `ContentsManager.allow_hidden` must be set to `True` to display hidden files."
 msgstr ""
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showHiddenFiles/title
 msgctxt "settings"
 msgid "Show hidden files"
 msgstr "Versteckte Dateien anzeigen"
@@ -1379,53 +1122,51 @@
 msgstr ""
 
 #: /packages/filebrowser-extension/schema/widget.json:/title
 msgctxt "schema"
 msgid "File Browser Widget"
 msgstr ""
 
-#: /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/cursorBlinkRate/title
-msgctxt "settings"
-msgid "Cursor blinking rate"
-msgstr "Blinkfrequenz des Cursors"
-
-#: /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/lineNumbers/title
-msgctxt "settings"
-msgid "Line Numbers"
-msgstr "Zeilennummern"
+#: /packages/fileeditor-extension/schema/completer.json:/description
+msgctxt "schema"
+msgid "File editor completer settings."
+msgstr "File Editor Completer Einstellungen."
 
-#: /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/showTrailingSpace/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/showTrailingSpace/title
-msgctxt "settings"
-msgid "Show Trailing Space"
+#: /packages/fileeditor-extension/schema/completer.json:/title
+msgctxt "schema"
+msgid "File Editor Completer"
 msgstr ""
 
 #: /packages/fileeditor-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Text editor settings."
 msgstr "Texteditor Einstellungen."
 
-#: /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[1]/items[1]/submenu/label /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[2]/items[1]/submenu/label
+#: /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[1]/items[1]/submenu/label
+msgctxt "menu"
+msgid "Text Editor Syntax Highlighting"
+msgstr ""
+
+#: /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[2]/items[1]/submenu/label
 msgctxt "menu"
 msgid "Text Editor Indentation"
 msgstr "Einrückung im Texteditor"
 
+#: /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[2]/items[5]/submenu/label
+msgctxt "menu"
+msgid "Text Editor Theme"
+msgstr ""
+
 #: /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "Editor"
 msgstr "Editor"
 
 #: /packages/fileeditor-extension/schema/plugin.json:/properties/editorConfig/description
 msgctxt "settings"
-msgid "The configuration for all text editors.\n"
-"If `fontFamily`, `fontSize` or `lineHeight` are `null`,\n"
-"values from current theme are used."
-msgstr ""
-
-#: /packages/fileeditor-extension/schema/plugin.json:/properties/editorConfig/description
-msgctxt "settings"
 msgid "The configuration for all text editors; it will override the CodeMirror default configuration.\n"
 "If `fontFamily`, `fontSize` or `lineHeight` are `null`,\n"
 "values from current theme are used."
 msgstr ""
 
 #: /packages/fileeditor-extension/schema/plugin.json:/properties/editorConfig/title
 msgctxt "settings"
@@ -1433,14 +1174,19 @@
 msgstr "Editor-Konfiguration"
 
 #: /packages/fileeditor-extension/schema/plugin.json:/properties/scrollPastEnd/description
 msgctxt "settings"
 msgid "Whether to scroll past the end of text document."
 msgstr ""
 
+#: /packages/fileeditor-extension/schema/plugin.json:/properties/scrollPastEnd/title
+msgctxt "settings"
+msgid "Scroll behavior"
+msgstr "Scroll-Verhalten"
+
 #: /packages/fileeditor-extension/schema/plugin.json:/properties/toolbar/description
 msgctxt "settings"
 msgid "Note: To disable a toolbar item,\n"
 "copy it to User Preferences and add the\n"
 "\"disabled\" key. Toolbar description:"
 msgstr ""
 
@@ -1506,20 +1252,20 @@
 msgstr ""
 
 #: /packages/htmlviewer-extension/schema/plugin.json:/title
 msgctxt "schema"
 msgid "HTML Viewer"
 msgstr "HTML-Betrachter"
 
-#: /packages/hub-extension/schema/menu.json:/description /packages/hub-extension/schema/plugin.json:/description
+#: /packages/hub-extension/schema/menu.json:/description
 msgctxt "schema"
 msgid "JupyterHub settings."
 msgstr "JupyterHub-Einstellungen."
 
-#: /packages/hub-extension/schema/menu.json:/title /packages/hub-extension/schema/plugin.json:/title
+#: /packages/hub-extension/schema/menu.json:/title
 msgctxt "schema"
 msgid "JupyterHub"
 msgstr "JupyterHub"
 
 #: /packages/imageviewer-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Image viewer settings."
@@ -1798,14 +1544,24 @@
 msgstr ""
 
 #: /packages/metadataform-extension/schema/metadataforms.json:/title
 msgctxt "schema"
 msgid "Metadata Form"
 msgstr ""
 
+#: /packages/notebook-extension/schema/completer.json:/description
+msgctxt "schema"
+msgid "Notebook completer settings."
+msgstr "Notebook Completer Einstellungen."
+
+#: /packages/notebook-extension/schema/completer.json:/title
+msgctxt "schema"
+msgid "Notebook Completer"
+msgstr ""
+
 #: /packages/notebook-extension/schema/export.json:/description
 msgctxt "schema"
 msgid "Notebook Export settings."
 msgstr "Notebook-Export-Einstellungen."
 
 #: /packages/notebook-extension/schema/export.json:/jupyter.lab.menus/main[0]/items[1]/submenu/label
 msgctxt "menu"
@@ -1881,19 +1637,14 @@
 #: /packages/notebook-extension/schema/tracker.json:/properties/autoStartDefaultKernel/title
 msgctxt "settings"
 msgid "Automatically Start Preferred Kernel"
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/codeCellConfig/description
 msgctxt "settings"
-msgid "The configuration for all code cells."
-msgstr "Die Konfiguration für alle Codezellen."
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/codeCellConfig/description
-msgctxt "settings"
 msgid "The configuration for all code cells; it will override the CodeMirror default configuration."
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/codeCellConfig/title
 msgctxt "settings"
 msgid "Code Cell Configuration"
 msgstr "Code-Zellen-Konfiguration"
@@ -1914,24 +1665,14 @@
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/documentWideUndoRedo/title
 msgctxt "settings"
 msgid "Enable undo/redo actions at the notebook document level."
 msgstr ""
 
-#: /packages/notebook-extension/schema/tracker.json:/properties/experimentalDisableDocumentWideUndoRedo/description
-msgctxt "settings"
-msgid "Disable the undo/redo on the notebook document level, so actions independent cells can have their own history. The undo/redo never applies on the outputs, in other words, outputs don't have history. A moved cell completely looses history capability for now."
-msgstr ""
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/experimentalDisableDocumentWideUndoRedo/title
-msgctxt "settings"
-msgid "Experimental settings to enable the undo/redo on the notebook document level."
-msgstr ""
-
 #: /packages/notebook-extension/schema/tracker.json:/properties/inputHistoryScope/description
 msgctxt "settings"
 msgid "Whether the line history for standard input (e.g. the ipdb prompt) should kept separately for different kernel sessions (`session`) or combined (`global`)."
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/inputHistoryScope/title
 msgctxt "settings"
@@ -1956,19 +1697,14 @@
 #: /packages/notebook-extension/schema/tracker.json:/properties/kernelStatus/title
 msgctxt "settings"
 msgid "Kernel status icon configuration"
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/markdownCellConfig/description
 msgctxt "settings"
-msgid "The configuration for all markdown cells."
-msgstr "Die Konfiguration für alle Markdown-Zellen."
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/markdownCellConfig/description
-msgctxt "settings"
 msgid "The configuration for all markdown cells; it will override the CodeMirror default configuration."
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/markdownCellConfig/title
 msgctxt "settings"
 msgid "Markdown Cell Configuration"
 msgstr "Konfiguration der Markdown-Zelle"
@@ -1979,61 +1715,26 @@
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/maxNumberOutputs/title
 msgctxt "settings"
 msgid "The maximum number of output cells to be rendered in the output area."
 msgstr ""
 
-#: /packages/notebook-extension/schema/tracker.json:/properties/numberCellsToRenderDirectly/description
-msgctxt "settings"
-msgid "Define the number of cells to render directly when virtual notebook intersection observer is available"
-msgstr ""
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/numberCellsToRenderDirectly/title
-msgctxt "settings"
-msgid "Number of cells to render directly"
-msgstr "Anzahl der direkt darzustellenden Zellen"
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/observedBottomMargin/description
-msgctxt "settings"
-msgid "Defines the observed bottom margin for the virtual notebook, set a positive number of pixels to render cells below the visible view"
-msgstr ""
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/observedBottomMargin/title
-msgctxt "settings"
-msgid "Observed bottom margin"
-msgstr ""
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/observedTopMargin/description
-msgctxt "settings"
-msgid "Defines the observed top margin for the virtual notebook, set a positive number of pixels to render cells above the visible view"
-msgstr ""
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/observedTopMargin/title
-msgctxt "settings"
-msgid "Observed top margin"
-msgstr ""
-
 #: /packages/notebook-extension/schema/tracker.json:/properties/overscanCount/description
 msgctxt "settings"
 msgid "In 'full' windowing mode, this is the number of cells above and below the viewport."
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/overscanCount/title
 msgctxt "settings"
 msgid "Number of cells to render outside de the viewport"
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/rawCellConfig/description
 msgctxt "settings"
-msgid "The configuration for all raw cells."
-msgstr ""
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/rawCellConfig/description
-msgctxt "settings"
 msgid "The configuration for all raw cells; it will override the CodeMirror default configuration."
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/rawCellConfig/title
 msgctxt "settings"
 msgid "Raw Cell Configuration"
 msgstr ""
@@ -2044,34 +1745,14 @@
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/recordTiming/title
 msgctxt "settings"
 msgid "Recording timing"
 msgstr "Aufnahmezeitpunkt"
 
-#: /packages/notebook-extension/schema/tracker.json:/properties/remainingTimeBeforeRescheduling/description
-msgctxt "settings"
-msgid "Define the remaining time in milliseconds before virtual notebook rendering is rescheduled. Set 0 if you want to disable any rescheduling"
-msgstr ""
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/remainingTimeBeforeRescheduling/title
-msgctxt "settings"
-msgid "Remaining time in milliseconds before virtual notebook rendering is rescheduled"
-msgstr ""
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/renderCellOnIdle/description
-msgctxt "settings"
-msgid "Defines if the placeholder cells should be rendered when the browser is idle"
-msgstr ""
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/renderCellOnIdle/title
-msgctxt "settings"
-msgid "Render cell on browser idle time"
-msgstr ""
-
 #: /packages/notebook-extension/schema/tracker.json:/properties/renderingLayout/description
 msgctxt "settings"
 msgid "Global setting to define the rendering layout in notebooks. 'default' or 'side-by-side' are supported."
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/renderingLayout/title
 msgctxt "settings"
@@ -2136,15 +1817,15 @@
 #: /packages/notebook-extension/schema/tracker.json:/properties/sideBySideRightMarginOverride/title
 msgctxt "settings"
 msgid "Side-by-side right margin override"
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/windowingMode/description
 msgctxt "settings"
-msgid "'defer': Wait for idle CPU cycles to attach out of viewport cells - 'full': Attach to the DOM only cells in viewport - 'none': Attach all cells to the viewport"
+msgid "'defer': Improve loading time - Wait for idle CPU cycles to attach out of viewport cells - 'full': Best performance with side effects - Attach to the DOM only cells in viewport - 'none': Worst performance without side effects - Attach all cells to the viewport"
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/windowingMode/title
 msgctxt "settings"
 msgid "Windowing mode"
 msgstr ""
 
@@ -2224,19 +1905,14 @@
 msgstr "Statusleisten-Einstellungen."
 
 #: /packages/statusbar-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "Status Bar"
 msgstr "Statusleiste"
 
-#: /packages/statusbar-extension/schema/plugin.json:/properties/startMode/title
-msgctxt "settings"
-msgid "Start mode: ``, `single`or `multiple`"
-msgstr ""
-
 #: /packages/statusbar-extension/schema/plugin.json:/properties/visible/description
 msgctxt "settings"
 msgid "Whether to show status bar or not"
 msgstr "Ob die Statusleiste angezeigt werden soll oder nicht"
 
 #: /packages/statusbar-extension/schema/plugin.json:/properties/visible/title
 msgctxt "settings"
@@ -2349,74 +2025,44 @@
 msgstr "Ausschalten beim Schließen"
 
 #: /packages/terminal-extension/schema/plugin.json:/properties/theme/description
 msgctxt "settings"
 msgid "The theme for the terminal."
 msgstr "Das Theme des Terminals."
 
+#: /packages/terminal-extension/schema/plugin.json:/properties/theme/title
+msgctxt "settings"
+msgid "Theme"
+msgstr ""
+
 #: /packages/terminal-extension/schema/plugin.json:/title
 msgctxt "schema"
 msgid "Terminal"
 msgstr "Terminal"
 
-#: /packages/toc-extension/schema/plugin.json:/description
+#: /packages/toc-extension/schema/registry.json:/description
 msgctxt "schema"
-msgid "Table of contents settings."
-msgstr "Inhaltsverzeichnis-Einstellungen."
+msgid "Default table of contents settings."
+msgstr ""
 
-#: /packages/toc-extension/schema/plugin.json:/jupyter.lab.setting-icon-label /packages/toc-extension/schema/registry.json:/jupyter.lab.setting-icon-label
+#: /packages/toc-extension/schema/registry.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "Table of Contents"
 msgstr "Inhaltsverzeichnis"
 
-#: /packages/toc-extension/schema/plugin.json:/properties/includeOutput/description
+#: /packages/toc-extension/schema/registry.json:/properties/includeOutput/description
 msgctxt "settings"
-msgid "Whether to include cell output in headings"
-msgstr "Ob die Zellausgabe in Überschriften einbezogen werden soll"
+msgid "Whether to include cell output in headings or not."
+msgstr ""
 
-#: /packages/toc-extension/schema/plugin.json:/properties/includeOutput/title /packages/toc-extension/schema/registry.json:/properties/includeOutput/title
+#: /packages/toc-extension/schema/registry.json:/properties/includeOutput/title
 msgctxt "settings"
 msgid "Include cell output in headings"
 msgstr "Zellausgaben in Überschriften einbeziehen"
 
-#: /packages/toc-extension/schema/plugin.json:/properties/numberingH1/description
-msgctxt "settings"
-msgid "Whether to number first-level headings"
-msgstr "Nummerierung der Überschriften der ersten Ebene"
-
-#: /packages/toc-extension/schema/plugin.json:/properties/numberingH1/title
-msgctxt "settings"
-msgid "Enable h1 numbering"
-msgstr "H1-Nummerierung einschalten"
-
-#: /packages/toc-extension/schema/plugin.json:/properties/syncCollapseState/description
-msgctxt "settings"
-msgid "If set to true, when a header is collapsed in the table of contents the corresponding section in the notebook is collapsed as well and vice versa."
-msgstr "Wenn diese Option auf \"true\" gesetzt ist, wird beim Ausklappen einer Überschrift im Inhaltsverzeichnis der entsprechende Abschnitt im Notizbuch ebenfalls ausgeklappt und umgekehrt."
-
-#: /packages/toc-extension/schema/plugin.json:/properties/syncCollapseState/title /packages/toc-extension/schema/registry.json:/properties/syncCollapseState/title
-msgctxt "settings"
-msgid "Synchronize collapse state"
-msgstr ""
-
-#: /packages/toc-extension/schema/plugin.json:/title /packages/toc-extension/schema/registry.json:/title
-msgctxt "schema"
-msgid "Table of Contents"
-msgstr "Inhaltsverzeichnis"
-
-#: /packages/toc-extension/schema/registry.json:/description
-msgctxt "schema"
-msgid "Default table of contents settings."
-msgstr ""
-
-#: /packages/toc-extension/schema/registry.json:/properties/includeOutput/description
-msgctxt "settings"
-msgid "Whether to include cell output in headings or not."
-msgstr ""
-
 #: /packages/toc-extension/schema/registry.json:/properties/maximalDepth/title
 msgctxt "settings"
 msgid "Maximal headings depth"
 msgstr ""
 
 #: /packages/toc-extension/schema/registry.json:/properties/numberHeaders/description
 msgctxt "settings"
@@ -2439,14 +2085,24 @@
 msgstr ""
 
 #: /packages/toc-extension/schema/registry.json:/properties/syncCollapseState/description
 msgctxt "settings"
 msgid "If set to true, when a heading is collapsed in the table of contents the corresponding section in the document is collapsed as well and vice versa. This inhibits the cell output headings."
 msgstr ""
 
+#: /packages/toc-extension/schema/registry.json:/properties/syncCollapseState/title
+msgctxt "settings"
+msgid "Synchronize collapse state"
+msgstr ""
+
+#: /packages/toc-extension/schema/registry.json:/title
+msgctxt "schema"
+msgid "Table of Contents"
+msgstr "Inhaltsverzeichnis"
+
 #: /packages/tooltip-extension/schema/consoles.json:/description
 msgctxt "schema"
 msgid "Console tooltip settings."
 msgstr "Einstellungen für Konsolen-Tooltips."
 
 #: /packages/tooltip-extension/schema/consoles.json:/title
 msgctxt "schema"
@@ -2519,110 +2175,110 @@
 msgstr "Präfix für lokalisierte Zeichenfolgen"
 
 #: /packages/translation-extension/schema/plugin.json:/title
 msgctxt "schema"
 msgid "Language"
 msgstr "Sprache"
 
-#: packages/application-extension/src/index.tsx:1078 packages/application-extension/src/index.tsx:1083 packages/application-extension/src/index.tsx:933
+#: packages/application-extension/src/index.tsx:1078 packages/application-extension/src/index.tsx:1083
 msgid "Property Inspector"
 msgstr "Eigenschaften-Inspektor"
 
-#: packages/application-extension/src/index.tsx:111 packages/application-extension/src/index.tsx:132 packages/apputils-extension/src/index.ts:308 packages/apputils-extension/src/index.ts:319 packages/documentsearch-extension/src/index.ts:254 packages/documentsearch-extension/src/index.ts:258 packages/documentsearch-extension/src/index.ts:262 packages/documentsearch-extension/src/index.ts:326 packages/logconsole-extension/src/index.tsx:242 packages/logconsole-extension/src/index.tsx:253 packages/mainmenu-extension/src/index.ts:228 packages/mainmenu-extension/src/index.ts:232 packages/mainmenu-extension/src/index.ts:236 packages/mainmenu-extension/src/index.ts:240 packages/mainmenu-extension/src/index.ts:242 packages/mainmenu-extension/src/index.ts:250 packages/statusbar-extension/src/index.ts:48 packages/statusbar-extension/src/index.ts:74
-msgid "Main Area"
-msgstr "Hauptbereich"
-
-#: packages/application-extension/src/index.tsx:115 packages/application-extension/src/index.tsx:136
-msgid "Shift+Right Click for Browser Menu"
-msgstr "Shift+Rechtsklick für das Browsermenü"
-
-#: packages/application-extension/src/index.tsx:1171 packages/statusbar-extension/src/index.ts:381
+#: packages/application-extension/src/index.tsx:1171
 msgid "Simple Interface (%1)"
 msgstr "Einfache Oberfläche (%1)"
 
-#: packages/application-extension/src/index.tsx:1173 packages/application-extension/src/index.tsx:340 packages/application-extension/src/index.tsx:385 packages/statusbar-extension/src/index.ts:383
+#: packages/application-extension/src/index.tsx:1173 packages/application-extension/src/index.tsx:385
 msgid "Simple Interface"
 msgstr "Einfache Oberfläche"
 
-#: packages/application-extension/src/index.tsx:1181 packages/statusbar-extension/src/index.ts:391
+#: packages/application-extension/src/index.tsx:1181
 msgid "Simple"
 msgstr "Einfach"
 
-#: packages/application-extension/src/index.tsx:1208 packages/application-extension/src/index.tsx:1402
-msgid "Switch Sidebar Side"
-msgstr "Seite der Seitenleiste wechseln"
-
-#: packages/application-extension/src/index.tsx:1220 packages/application-extension/src/index.tsx:791 packages/application-extension/src/index.tsx:989 packages/apputils/src/toolbar/factory.ts:28 packages/apputils/src/toolbar/factory.ts:33 packages/extensionmanager/src/model.ts:504 packages/extensionmanager/src/model.ts:526 packages/mainmenu-extension/src/index.ts:770 packages/mainmenu-extension/src/index.ts:942
+#: packages/application-extension/src/index.tsx:1220 packages/application-extension/src/index.tsx:791 packages/apputils/src/toolbar/factory.ts:33 packages/extensionmanager/src/model.ts:504 packages/extensionmanager/src/model.ts:526 packages/mainmenu-extension/src/index.ts:770
 msgid "Information"
 msgstr "Informationen"
 
-#: packages/application-extension/src/index.tsx:1221 packages/application-extension/src/index.tsx:990
+#: packages/application-extension/src/index.tsx:1221
 msgid "Context menu customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr "Die Anpassung des Kontextmenüs hat sich geändert. Sie müssen JupyterLab neu laden, um die Änderungen zu sehen."
 
-#: packages/application-extension/src/index.tsx:1226 packages/application-extension/src/index.tsx:797 packages/application-extension/src/index.tsx:995 packages/apputils/src/toolbar/factory.ts:34 packages/apputils/src/toolbar/factory.ts:39 packages/docmanager-extension/src/index.tsx:654 packages/docmanager-extension/src/index.tsx:739 packages/docprovider/src/yprovider.ts:135 packages/mainmenu-extension/src/index.ts:776 packages/mainmenu-extension/src/index.ts:948
+#: packages/application-extension/src/index.tsx:1226 packages/application-extension/src/index.tsx:797 packages/apputils/src/toolbar/factory.ts:39 packages/docmanager-extension/src/index.tsx:739 packages/mainmenu-extension/src/index.ts:776
 msgid "Reload"
 msgstr "Neu laden"
 
-#: packages/application-extension/src/index.tsx:200 packages/application-extension/src/index.tsx:205
+#: packages/application-extension/src/index.tsx:132 packages/apputils-extension/src/index.ts:319 packages/documentsearch-extension/src/index.ts:326 packages/logconsole-extension/src/index.tsx:246 packages/mainmenu-extension/src/index.ts:236 packages/mainmenu-extension/src/index.ts:240 packages/mainmenu-extension/src/index.ts:250 packages/statusbar-extension/src/index.ts:48
+msgid "Main Area"
+msgstr "Hauptbereich"
+
+#: packages/application-extension/src/index.tsx:136
+msgid "Shift+Right Click for Browser Menu"
+msgstr "Shift+Rechtsklick für das Browsermenü"
+
+#: packages/application-extension/src/index.tsx:1402
+msgid "Switch Sidebar Side"
+msgstr "Seite der Seitenleiste wechseln"
+
+#: packages/application-extension/src/index.tsx:205
 msgid "Close Tab"
 msgstr "Tab schließen"
 
-#: packages/application-extension/src/index.tsx:214 packages/application-extension/src/index.tsx:219
+#: packages/application-extension/src/index.tsx:219
 msgid "Close All Other Tabs"
 msgstr "Alle anderen Tabs schließen"
 
-#: packages/application-extension/src/index.tsx:234 packages/application-extension/src/index.tsx:239
+#: packages/application-extension/src/index.tsx:239
 msgid "Close Tabs to Right"
 msgstr "Tabs zur rechten Seite schließen"
 
-#: packages/application-extension/src/index.tsx:249 packages/application-extension/src/index.tsx:254
+#: packages/application-extension/src/index.tsx:254
 msgid "Activate Next Tab"
 msgstr "Nächsten Tab aktivieren"
 
-#: packages/application-extension/src/index.tsx:256 packages/application-extension/src/index.tsx:261
+#: packages/application-extension/src/index.tsx:261
 msgid "Activate Previous Tab"
 msgstr "Zuletzt benutzten Tab aktivieren"
 
-#: packages/application-extension/src/index.tsx:263 packages/application-extension/src/index.tsx:268
+#: packages/application-extension/src/index.tsx:268
 msgid "Activate Next Tab Bar"
 msgstr "Nächsten Tab aktivieren"
 
-#: packages/application-extension/src/index.tsx:270 packages/application-extension/src/index.tsx:275
+#: packages/application-extension/src/index.tsx:275
 msgid "Activate Previous Tab Bar"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:277 packages/application-extension/src/index.tsx:282
+#: packages/application-extension/src/index.tsx:282
 msgid "Close All Tabs"
 msgstr "Alle Tabs schließen"
 
-#: packages/application-extension/src/index.tsx:284 packages/application-extension/src/index.tsx:300
-msgid "Show Left Sidebar"
-msgstr "Linke Seitenleiste anzeigen"
-
 #: packages/application-extension/src/index.tsx:289
 msgid "Show Header"
 msgstr "Kopfzeile anzeigen"
 
-#: packages/application-extension/src/index.tsx:300 packages/application-extension/src/index.tsx:316
+#: packages/application-extension/src/index.tsx:300
+msgid "Show Left Sidebar"
+msgstr "Linke Seitenleiste anzeigen"
+
+#: packages/application-extension/src/index.tsx:316
 msgid "Show Right Sidebar"
 msgstr "Rechte Seitenleiste anzeigen"
 
-#: packages/application-extension/src/index.tsx:316 packages/application-extension/src/index.tsx:354
-msgid "Presentation Mode"
-msgstr "Präsentationsmodus"
-
 #: packages/application-extension/src/index.tsx:334
 msgid "Show Right Activity Bar"
 msgstr "Rechte Aktivitätsleiste anzeigen"
 
 #: packages/application-extension/src/index.tsx:335
 msgid "Show Left Activity Bar"
 msgstr "Linke Aktivitätsleiste anzeigen"
 
+#: packages/application-extension/src/index.tsx:354
+msgid "Presentation Mode"
+msgstr "Präsentationsmodus"
+
 #: packages/application-extension/src/index.tsx:365
 msgid "Set %1 mode."
 msgstr ""
 
 #: packages/application-extension/src/index.tsx:366
 msgid "Set the layout `mode`."
 msgstr ""
@@ -2631,534 +2287,530 @@
 msgid "The layout `mode` can be \"single-document\" or \"multiple-document\"."
 msgstr ""
 
 #: packages/application-extension/src/index.tsx:397
 msgid "Reset Default Layout"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:431 packages/application-extension/src/index.tsx:527
+#: packages/application-extension/src/index.tsx:527
 msgid "Error Registering Plugins"
 msgstr "Fehler beim Registrieren von Plugins"
 
-#: packages/application-extension/src/index.tsx:481 packages/application-extension/src/index.tsx:577 packages/extensionmanager/src/build-helper.tsx:27
+#: packages/application-extension/src/index.tsx:577
 msgid "Build Complete"
 msgstr "Build abgeschlossen"
 
-#: packages/application-extension/src/index.tsx:484 packages/application-extension/src/index.tsx:580 packages/extensionmanager/src/build-helper.tsx:30
+#: packages/application-extension/src/index.tsx:580
 msgid "Build successfully completed, reload page?"
 msgstr "Build erfolgreich abgeschlossen, Seite neu laden?"
 
-#: packages/application-extension/src/index.tsx:486 packages/application-extension/src/index.tsx:582 packages/extensionmanager/src/build-helper.tsx:32
+#: packages/application-extension/src/index.tsx:582
 msgid "You will lose any unsaved changes."
 msgstr "Alle nicht gespeicherten Änderungen gehen verloren."
 
-#: packages/application-extension/src/index.tsx:491 packages/application-extension/src/index.tsx:587 packages/extensionmanager/src/build-helper.tsx:37
+#: packages/application-extension/src/index.tsx:587
 msgid "Reload Without Saving"
 msgstr "Neu laden ohne zu speichern"
 
-#: packages/application-extension/src/index.tsx:494 packages/application-extension/src/index.tsx:590 packages/extensionmanager/src/build-helper.tsx:40
+#: packages/application-extension/src/index.tsx:590
 msgid "Save and Reload"
 msgstr "Speichern und neu laden"
 
-#: packages/application-extension/src/index.tsx:507 packages/application-extension/src/index.tsx:603 packages/extensionmanager/src/build-helper.tsx:53
+#: packages/application-extension/src/index.tsx:603
 msgid "Save Failed"
 msgstr "Speichern fehlgeschlagen"
 
-#: packages/application-extension/src/index.tsx:516 packages/application-extension/src/index.tsx:612 packages/extensionmanager/src/build-helper.tsx:63
+#: packages/application-extension/src/index.tsx:612
 msgid "Build Failed"
 msgstr "Build-Fehler"
 
-#: packages/application-extension/src/index.tsx:534 packages/application-extension/src/index.tsx:630
+#: packages/application-extension/src/index.tsx:630
 msgid "JupyterLab build is suggested:"
 msgstr "JupyterLab Build wird empfohlen:"
 
-#: packages/application-extension/src/index.tsx:541 packages/application-extension/src/index.tsx:637
+#: packages/application-extension/src/index.tsx:637
 msgid "Build Recommended"
 msgstr "Build empfohlen"
 
-#: packages/application-extension/src/index.tsx:545 packages/application-extension/src/index.tsx:641
+#: packages/application-extension/src/index.tsx:641
 msgid "Build"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:608 packages/application-extension/src/index.tsx:707
+#: packages/application-extension/src/index.tsx:707
 msgid "Are you sure you want to exit JupyterLab?\n\n"
 "Any unsaved changes will be lost."
 msgstr "Sind Sie sicher, dass Sie JupyterLab beenden möchten?\n\n"
 "Alle nicht gespeicherten Änderungen gehen verloren."
 
-#: packages/application-extension/src/index.tsx:781 packages/application-extension/src/index.tsx:925
+#: packages/application-extension/src/index.tsx:792
+msgid "User layout customization has changed. You may need to reload JupyterLab to see the changes."
+msgstr ""
+
+#: packages/application-extension/src/index.tsx:925
 msgid "The path: %1 was not found. JupyterLab redirected to: %2"
 msgstr "Der Pfad: %1 wurde nicht gefunden. JupyterLab weitergeleitet zu: %2"
 
-#: packages/application-extension/src/index.tsx:790 packages/application-extension/src/index.tsx:934
+#: packages/application-extension/src/index.tsx:934
 msgid "Path Not Found"
 msgstr "Pfad nicht gefunden"
 
-#: packages/application-extension/src/index.tsx:792
-msgid "User layout customization has changed. You may need to reload JupyterLab to see the changes."
-msgstr ""
-
 #: packages/application/src/connectionlost.ts:19
 msgid "Server Connection Error"
 msgstr "Server-Verbindungsfehler"
 
 #: packages/application/src/connectionlost.ts:20
 msgid "A connection to the Jupyter server could not be established.\n"
 "JupyterLab will continue trying to reconnect.\n"
 "Check your network connection or Jupyter server configuration.\n"
 msgstr "Eine Verbindung zum Jupyter-Server konnte nicht hergestellt werden.\n"
 "JupyterLab wird weiterhin versuchen, die Verbindung wiederherzustellen.\n"
 "Überprüfe deine Netzwerkverbindung oder die Konfiguration des Jupyter-Servers.\n"
 
-#: packages/application/src/shell.ts:253 packages/application/src/shell.ts:698
+#: packages/application/src/shell.ts:713
 msgid "main"
 msgstr ""
 
-#: packages/application/src/shell.ts:288 packages/application/src/shell.ts:292 packages/application/src/shell.ts:701 packages/application/src/shell.ts:705
+#: packages/application/src/shell.ts:716 packages/application/src/shell.ts:720
 msgid "main sidebar"
 msgstr "Hauptseitenleiste"
 
-#: packages/application/src/shell.ts:301 packages/application/src/shell.ts:305 packages/application/src/shell.ts:709 packages/application/src/shell.ts:713
+#: packages/application/src/shell.ts:724 packages/application/src/shell.ts:728
 msgid "alternate sidebar"
 msgstr "alternative Seitenleiste"
 
 #: packages/application/src/utils.ts:148
 msgid "%1 and %2"
 msgstr "%1 und %2"
 
-#: packages/apputils-extension/src/announcements.ts:102 packages/apputils-extension/src/announcements.ts:95
+#: packages/apputils-extension/src/announcements.ts:102
 msgid "Would you like to receive official Jupyter news?\n"
 "Please read the privacy policy."
 msgstr ""
 
-#: packages/apputils-extension/src/announcements.ts:103 packages/apputils-extension/src/announcements.ts:110
+#: packages/apputils-extension/src/announcements.ts:110
 msgid "Open privacy policy"
 msgstr "Datenschutzerklärung öffnen"
 
-#: packages/apputils-extension/src/announcements.ts:109 packages/apputils-extension/src/announcements.ts:116
+#: packages/apputils-extension/src/announcements.ts:116
 msgid "Privacy policies"
 msgstr "Datenschutzerklärungen"
 
-#: packages/apputils-extension/src/announcements.ts:119 packages/apputils-extension/src/announcements.ts:126 packages/extensionmanager/src/widget.tsx:434
+#: packages/apputils-extension/src/announcements.ts:126 packages/extensionmanager/src/widget.tsx:434
 msgid "Yes"
 msgstr "Ja"
 
-#: packages/apputils-extension/src/announcements.ts:136 packages/apputils-extension/src/announcements.ts:143 packages/extensionmanager/src/widget.tsx:424
+#: packages/apputils-extension/src/announcements.ts:143 packages/extensionmanager/src/widget.tsx:424
 msgid "No"
 msgstr "Nein"
 
-#: packages/apputils-extension/src/announcements.ts:171 packages/apputils-extension/src/announcements.ts:178
+#: packages/apputils-extension/src/announcements.ts:180
 msgid "Hide"
 msgstr "Ausblenden"
 
-#: packages/apputils-extension/src/announcements.ts:172 packages/apputils-extension/src/announcements.ts:179
+#: packages/apputils-extension/src/announcements.ts:181
 msgid "Never show this notification again."
 msgstr "Diese Benachrichtigung nicht erneut anzeigen."
 
-#: packages/apputils-extension/src/announcements.ts:232 packages/apputils-extension/src/announcements.ts:239
+#: packages/apputils-extension/src/announcements.ts:243
 msgid "Do not check for updates"
 msgstr "Nicht auf Aktualisierungen prüfen"
 
-#: packages/apputils-extension/src/announcements.ts:233 packages/apputils-extension/src/announcements.ts:240
+#: packages/apputils-extension/src/announcements.ts:244
 msgid "If pressed, you will not be prompted if a new JupyterLab version is found."
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:210 packages/apputils-extension/src/index.ts:219
+#: packages/apputils-extension/src/index.ts:219
 msgid "Loading…"
 msgstr "Wird geladen..."
 
-#: packages/apputils-extension/src/index.ts:211 packages/apputils-extension/src/index.ts:220
+#: packages/apputils-extension/src/index.ts:220
 msgid "The loading screen is taking a long time.\n"
 "Would you like to clear the workspace or keep waiting?"
 msgstr "Der Ladebildschirm dauert sehr lange.\n"
 "Möchten Sie den Arbeitsbereich löschen oder weiter warten?"
 
-#: packages/apputils-extension/src/index.ts:214 packages/apputils-extension/src/index.ts:223
+#: packages/apputils-extension/src/index.ts:223
 msgid "Keep Waiting"
 msgstr "Weiter warten"
 
-#: packages/apputils-extension/src/index.ts:215 packages/apputils-extension/src/index.ts:224
+#: packages/apputils-extension/src/index.ts:224
 msgid "Clear Workspace"
 msgstr "Arbeitsbereich löschen"
 
-#: packages/apputils-extension/src/index.ts:280 packages/apputils-extension/src/index.ts:290
+#: packages/apputils-extension/src/index.ts:290
 msgid "Print…"
 msgstr "Drucken…"
 
-#: packages/apputils-extension/src/index.ts:310 packages/apputils-extension/src/index.ts:321
+#: packages/apputils-extension/src/index.ts:321
 msgid "Show Header Above Content"
 msgstr "Kopfzeile über dem Inhalt anzeigen"
 
 #: packages/apputils-extension/src/index.ts:429
 msgid "Load state for the current workspace."
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:477 packages/apputils-extension/src/index.ts:493
+#: packages/apputils-extension/src/index.ts:493
 msgid "Reset Application State"
 msgstr "Anwendungsstatus zurücksetzen"
 
 #: packages/apputils-extension/src/index.ts:504
 msgid "Reset state when loading for the workspace."
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:568 packages/apputils-extension/src/index.ts:595
+#: packages/apputils-extension/src/index.ts:595
 msgid "Run First Enabled Command"
 msgstr "Ersten aktivierten Befehl ausführen"
 
-#: packages/apputils-extension/src/index.ts:584 packages/apputils-extension/src/index.ts:613
+#: packages/apputils-extension/src/index.ts:613
 msgid "Run All Enabled Commands Passed as Args"
 msgstr ""
 
 #: packages/apputils-extension/src/index.ts:634
 msgid "Show Keyboard Shortcuts"
 msgstr ""
 
 #: packages/apputils-extension/src/index.ts:635
 msgid "Show relevant keyboard shortcuts for the current active widget"
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:655 packages/help-extension/src/index.tsx:182 packages/help-extension/src/index.tsx:183 packages/help-extension/src/index.tsx:212 packages/help-extension/src/index.tsx:217 packages/help-extension/src/index.tsx:244 packages/help-extension/src/index.tsx:479 packages/help-extension/src/index.tsx:485 packages/help-extension/src/index.tsx:90
+#: packages/apputils-extension/src/index.ts:655 packages/help-extension/src/index.tsx:183 packages/help-extension/src/index.tsx:217 packages/help-extension/src/index.tsx:479 packages/help-extension/src/index.tsx:90
 msgid "Help"
 msgstr "Hilfe"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:156 packages/apputils-extension/src/notificationplugin.tsx:160 packages/apputils-extension/src/notificationplugin.tsx:347 packages/apputils-extension/src/notificationplugin.tsx:351
+#: packages/apputils-extension/src/notificationplugin.tsx:166 packages/apputils-extension/src/notificationplugin.tsx:353
 msgid "%1 notification"
 msgid_plural "%1 notifications"
 msgstr[0] "%1 Benachrichtigung"
 msgstr[1] "%1 Benachrichtigungen"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:157 packages/apputils-extension/src/notificationplugin.tsx:161 packages/apputils-extension/src/notificationplugin.tsx:348 packages/apputils-extension/src/notificationplugin.tsx:352
+#: packages/apputils-extension/src/notificationplugin.tsx:167 packages/apputils-extension/src/notificationplugin.tsx:354
 msgid "No notifications"
 msgstr "Keine Benachrichtigungen"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:166 packages/apputils-extension/src/notificationplugin.tsx:170
+#: packages/apputils-extension/src/notificationplugin.tsx:176
 msgid "Dismiss all notifications"
 msgstr "Alle Benachrichtigungen verwerfen"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:173 packages/apputils-extension/src/notificationplugin.tsx:177
+#: packages/apputils-extension/src/notificationplugin.tsx:183
 msgid "Hide notifications"
 msgstr "Benachrichtigungen ausblenden"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:218 packages/apputils-extension/src/notificationplugin.tsx:222
+#: packages/apputils-extension/src/notificationplugin.tsx:229
 msgid "Dismiss notification"
 msgstr "Benachrichtigung verwerfen"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:395 packages/apputils-extension/src/notificationplugin.tsx:400
+#: packages/apputils-extension/src/notificationplugin.tsx:402
 msgid "Emit a notification"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:396 packages/apputils-extension/src/notificationplugin.tsx:401
+#: packages/apputils-extension/src/notificationplugin.tsx:403
 msgid "Notification is described by {message: string, type?: string, options?: {autoClose?: number | false, actions: {label: string, commandId: string, args?: ReadOnlyJSONObject, caption?: string, className?: string}[], data?: ReadOnlyJSONValue}}."
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:433 packages/apputils-extension/src/notificationplugin.tsx:438
+#: packages/apputils-extension/src/notificationplugin.tsx:440
 msgid "Update a notification"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:434 packages/apputils-extension/src/notificationplugin.tsx:439
+#: packages/apputils-extension/src/notificationplugin.tsx:441
 msgid "Notification is described by {id: string, message: string, type?: string, options?: {autoClose?: number | false, actions: {label: string, commandId: string, args?: ReadOnlyJSONObject, caption?: string, className?: string}[], data?: ReadOnlyJSONValue}}."
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:473 packages/apputils-extension/src/notificationplugin.tsx:478
+#: packages/apputils-extension/src/notificationplugin.tsx:480
 msgid "Dismiss a notification"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:597 packages/apputils-extension/src/notificationplugin.tsx:599
+#: packages/apputils-extension/src/notificationplugin.tsx:601
 msgid "Show Notifications"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:647 packages/apputils-extension/src/notificationplugin.tsx:649
+#: packages/apputils-extension/src/notificationplugin.tsx:688
 msgid "Hide notification"
 msgstr ""
 
 #: packages/apputils-extension/src/palette.ts:101
 msgid "Command Palette Section"
 msgstr "Abschnitt Befehlspalette"
 
-#: packages/apputils-extension/src/palette.ts:141 packages/apputils-extension/src/palette.ts:142
+#: packages/apputils-extension/src/palette.ts:141
 msgid "Commands (%1)"
 msgstr "Befehle (%1)"
 
-#: packages/apputils-extension/src/palette.ts:143 packages/apputils-extension/src/palette.ts:144 packages/apputils-extension/src/palette.ts:208 packages/apputils-extension/src/palette.ts:209
+#: packages/apputils-extension/src/palette.ts:143 packages/apputils-extension/src/palette.ts:208
 msgid "Commands"
 msgstr "Befehle"
 
-#: packages/apputils-extension/src/palette.ts:159 packages/apputils-extension/src/palette.ts:160
+#: packages/apputils-extension/src/palette.ts:159
 msgid "Activate Command Palette"
 msgstr "Befehlspalette aktivieren"
 
-#: packages/apputils-extension/src/palette.ts:162 packages/apputils-extension/src/palette.ts:163 packages/extensionmanager/src/widget.tsx:742
+#: packages/apputils-extension/src/palette.ts:162
 msgid "SEARCH"
 msgstr "SUCHEN"
 
 #: packages/apputils-extension/src/palette.ts:42
 msgid "Command Palette"
 msgstr "Befehlspalette"
 
 #: packages/apputils-extension/src/shortcuts.tsx:183
 msgid "Keyboard Shortcuts"
 msgstr ""
 
-#: packages/apputils-extension/src/shortcuts.tsx:187 packages/docmanager/src/widgetmanager.ts:397 packages/docmanager/src/widgetmanager.ts:399 packages/filebrowser/src/listing.ts:1140 packages/filebrowser/src/listing.ts:1399 packages/running-extension/src/opentabs.ts:86 packages/running-extension/src/opentabs.ts:87
+#: packages/apputils-extension/src/shortcuts.tsx:187 packages/docmanager/src/widgetmanager.ts:397 packages/filebrowser/src/listing.ts:1399 packages/running-extension/src/opentabs.ts:86
 msgid "Close"
 msgstr "Schließen"
 
-#: packages/apputils-extension/src/themesplugins.ts:103 packages/apputils-extension/src/themesplugins.ts:131
-msgid "Theme Scrollbars"
-msgstr "Theme Scrollleiste"
-
-#: packages/apputils-extension/src/themesplugins.ts:110 packages/apputils-extension/src/themesplugins.ts:138
-msgid "waiting for fonts"
-msgstr "Warte auf Schriftarten"
-
 #: packages/apputils-extension/src/themesplugins.ts:112
 msgid "Switch to the provided `theme`."
 msgstr ""
 
-#: packages/apputils-extension/src/themesplugins.ts:117 packages/apputils-extension/src/themesplugins.ts:89
+#: packages/apputils-extension/src/themesplugins.ts:117
 msgid "Use Theme: %1"
 msgstr "Verwende Theme: %1"
 
-#: packages/apputils-extension/src/themesplugins.ts:121 packages/apputils-extension/src/themesplugins.ts:149
+#: packages/apputils-extension/src/themesplugins.ts:131
+msgid "Theme Scrollbars"
+msgstr "Theme Scrollleiste"
+
+#: packages/apputils-extension/src/themesplugins.ts:138
+msgid "waiting for fonts"
+msgstr "Warte auf Schriftarten"
+
+#: packages/apputils-extension/src/themesplugins.ts:149
 msgid "Increase Code Font Size"
 msgstr "Code-Schriftgröße erhöhen"
 
-#: packages/apputils-extension/src/themesplugins.ts:123 packages/apputils-extension/src/themesplugins.ts:151
+#: packages/apputils-extension/src/themesplugins.ts:151
 msgid "Increase Content Font Size"
 msgstr "Inhalt-Schriftgröße erhöhen"
 
-#: packages/apputils-extension/src/themesplugins.ts:125 packages/apputils-extension/src/themesplugins.ts:153
+#: packages/apputils-extension/src/themesplugins.ts:153
 msgid "Increase UI Font Size"
 msgstr "UI Schriftgröße vergrößern"
 
-#: packages/apputils-extension/src/themesplugins.ts:127 packages/apputils-extension/src/themesplugins.ts:155 packages/fileeditor-extension/src/commands.ts:280 packages/fileeditor-extension/src/commands.ts:298
+#: packages/apputils-extension/src/themesplugins.ts:155 packages/fileeditor-extension/src/commands.ts:280
 msgid "Increase Font Size"
 msgstr "Schriftgröße vergrößern"
 
-#: packages/apputils-extension/src/themesplugins.ts:137 packages/apputils-extension/src/themesplugins.ts:165
+#: packages/apputils-extension/src/themesplugins.ts:165
 msgid "Decrease Code Font Size"
 msgstr "Code-Schriftgröße verringern"
 
-#: packages/apputils-extension/src/themesplugins.ts:139 packages/apputils-extension/src/themesplugins.ts:167
+#: packages/apputils-extension/src/themesplugins.ts:167
 msgid "Decrease Content Font Size"
 msgstr "Inhalt-Schriftgröße verringern"
 
-#: packages/apputils-extension/src/themesplugins.ts:141 packages/apputils-extension/src/themesplugins.ts:169
+#: packages/apputils-extension/src/themesplugins.ts:169
 msgid "Decrease UI Font Size"
 msgstr "UI Schriftgröße verkleinern"
 
-#: packages/apputils-extension/src/themesplugins.ts:143 packages/apputils-extension/src/themesplugins.ts:171 packages/fileeditor-extension/src/commands.ts:284 packages/fileeditor-extension/src/commands.ts:302
+#: packages/apputils-extension/src/themesplugins.ts:171 packages/fileeditor-extension/src/commands.ts:284
 msgid "Decrease Font Size"
 msgstr "Schriftgröße verkleinern"
 
-#: packages/apputils-extension/src/themesplugins.ts:202 packages/apputils-extension/src/themesplugins.ts:231 packages/codemirror/src/extension.ts:851
+#: packages/apputils-extension/src/themesplugins.ts:231 packages/codemirror/src/extension.ts:851
 msgid "Theme"
 msgstr ""
 
-#: packages/apputils-extension/src/workspacesplugin.ts:181 packages/apputils-extension/src/workspacesplugin.ts:189
+#: packages/apputils-extension/src/workspacesplugin.ts:181
 msgid "Workspace loader"
 msgstr "Arbeitsbereich-Loader"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:266 packages/apputils-extension/src/workspacesplugin.ts:272 packages/apputils-extension/src/workspacesplugin.ts:274 packages/apputils-extension/src/workspacesplugin.ts:280 packages/docmanager/src/widgetmanager.ts:436 packages/docmanager/src/widgetmanager.ts:438 packages/docregistry/src/context.ts:1019 packages/docregistry/src/context.ts:1035 packages/docregistry/src/context.ts:1042 packages/docregistry/src/context.ts:1101 packages/docregistry/src/context.ts:1108
+#: packages/apputils-extension/src/workspacesplugin.ts:266 packages/apputils-extension/src/workspacesplugin.ts:272 packages/docmanager/src/widgetmanager.ts:436 packages/docregistry/src/context.ts:1019
 msgid "Save"
 msgstr "Speichern"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:268 packages/apputils-extension/src/workspacesplugin.ts:276 packages/apputils-extension/src/workspacesplugin.ts:79 packages/apputils-extension/src/workspacesplugin.ts:82
+#: packages/apputils-extension/src/workspacesplugin.ts:268 packages/apputils-extension/src/workspacesplugin.ts:79
 msgid "Save Current Workspace As…"
 msgstr "Aktuellen Arbeitsbereich speichern unter.."
 
-#: packages/apputils-extension/src/workspacesplugin.ts:278 packages/apputils/src/dialog.tsx:763 packages/apputils/src/dialog.tsx:862 packages/apputils/src/sessioncontext.tsx:1292 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:625 packages/debugger-extension/src/index.ts:696 packages/debugger/src/panels/breakpoints/index.ts:66 packages/docmanager-extension/src/index.tsx:1015 packages/docmanager-extension/src/index.tsx:653 packages/docmanager-extension/src/index.tsx:703 packages/docmanager-extension/src/index.tsx:994 packages/docmanager/src/dialogs.ts:115 packages/docmanager/src/dialogs.ts:52 packages/docmanager/src/widgetmanager.ts:444 packages/extensionmanager/src/companions.tsx:216 packages/filebrowser/src/listing.ts:415 packages/filebrowser/src/listing.ts:429 packages/filebrowser/src/model.ts:449 packages/filebrowser/src/model.ts:456 packages/filebrowser/src/opendialog.ts:87 packages/notebook/src/actions.tsx:1911 packages/notebook/src/searchprovider.ts:504 packages/running/src/index.tsx:232 packages/settingeditor/src/plugineditor.ts:132 packages/settingeditor/src/plugineditor.ts:137 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/shortcuts-extension/src/components/ShortcutItem.tsx:247 packages/translation-extension/src/index.ts:138 packages/translation-extension/src/index.ts:147
-msgid "Cancel"
-msgstr "Abbrechen"
-
-#: packages/apputils-extension/src/workspacesplugin.ts:72 packages/apputils-extension/src/workspacesplugin.ts:75
+#: packages/apputils-extension/src/workspacesplugin.ts:72
 msgid "JupyterLab workspace File"
 msgstr "JupyterLab-Arbeitsbereich-Datei"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:93 packages/apputils-extension/src/workspacesplugin.ts:96
+#: packages/apputils-extension/src/workspacesplugin.ts:93
 msgid "Save Current Workspace"
 msgstr "Aktuellen Arbeitsbereich speichern"
 
-#: packages/apputils/src/dialog.tsx:47 packages/help-extension/src/index.tsx:153 packages/help-extension/src/index.tsx:395 packages/help-extension/src/index.tsx:404 packages/hub-extension/src/index.ts:161 packages/hub-extension/src/index.ts:173 packages/lsp/src/adapters/adapter.ts:470 packages/mainmenu-extension/src/index.ts:548 packages/mainmenu-extension/src/index.ts:551
+#: packages/apputils/src/dialog.tsx:47 packages/help-extension/src/index.tsx:153 packages/help-extension/src/index.tsx:404 packages/hub-extension/src/index.ts:173 packages/lsp/src/adapters/adapter.ts:470 packages/mainmenu-extension/src/index.ts:548
 msgid "Dismiss"
 msgstr "Verwerfen"
 
-#: packages/apputils/src/dialog.tsx:763 packages/docmanager-extension/src/index.tsx:642 packages/docmanager-extension/src/index.tsx:687 packages/docmanager-extension/src/index.tsx:750 packages/docmanager-extension/src/index.tsx:761 packages/docmanager-extension/src/index.tsx:874 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:508 packages/extensionmanager/src/model.ts:531 packages/notebook/src/actions.tsx:1903 packages/notebook/src/actions.tsx:1912 packages/notebook/src/actions.tsx:1984 packages/notebook/src/actions.tsx:2155 packages/notebook/src/actions.tsx:2165 packages/notebook/src/default-toolbar.tsx:70 packages/notebook/src/model.ts:373 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:213 packages/notebook/src/panel.ts:219 packages/notebook/src/searchprovider.ts:505 packages/settingeditor/src/plugineditor.ts:133 packages/settingeditor/src/plugineditor.ts:138
+#: packages/apputils/src/dialog.tsx:763 packages/apputils/src/dialog.tsx:862 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:696 packages/filebrowser/src/listing.ts:429 packages/filebrowser/src/model.ts:449 packages/notebook/src/searchprovider.ts:514 packages/settingeditor/src/plugineditor.ts:132 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/translation-extension/src/index.ts:147
+msgid "Cancel"
+msgstr "Abbrechen"
+
+#: packages/apputils/src/dialog.tsx:763 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:508 packages/extensionmanager/src/model.ts:531 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:234 packages/notebook/src/searchprovider.ts:515 packages/settingeditor/src/plugineditor.ts:133
 msgid "Ok"
 msgstr ""
 
-#: packages/apputils/src/kernelstatuses.ts:17 packages/apputils/src/kernelstatuses.tsx:29
+#: packages/apputils/src/kernelstatuses.tsx:210 packages/apputils/src/sessioncontext.tsx:1746 packages/apputils/src/sessioncontext.tsx:631
+msgid "No Kernel"
+msgstr "Kein Kernel"
+
+#: packages/apputils/src/kernelstatuses.tsx:29
 msgid "Unknown"
 msgstr "Unbekannt"
 
-#: packages/apputils/src/kernelstatuses.ts:18 packages/apputils/src/kernelstatuses.tsx:30
+#: packages/apputils/src/kernelstatuses.tsx:30
 msgid "Starting"
 msgstr "Starten"
 
-#: packages/apputils/src/kernelstatuses.ts:19 packages/apputils/src/kernelstatuses.tsx:31
+#: packages/apputils/src/kernelstatuses.tsx:31
 msgid "Idle"
 msgstr "Leerlauf"
 
-#: packages/apputils/src/kernelstatuses.ts:20 packages/apputils/src/kernelstatuses.tsx:32
+#: packages/apputils/src/kernelstatuses.tsx:32
 msgid "Busy"
 msgstr "Beschäftigt"
 
-#: packages/apputils/src/kernelstatuses.ts:21 packages/apputils/src/kernelstatuses.tsx:33
+#: packages/apputils/src/kernelstatuses.tsx:33
 msgid "Terminating"
 msgstr "Beenden"
 
-#: packages/apputils/src/kernelstatuses.ts:22 packages/apputils/src/kernelstatuses.tsx:34
+#: packages/apputils/src/kernelstatuses.tsx:34
 msgid "Restarting"
 msgstr "Wird neugestartet"
 
-#: packages/apputils/src/kernelstatuses.ts:23 packages/apputils/src/kernelstatuses.tsx:35
+#: packages/apputils/src/kernelstatuses.tsx:35
 msgid "Autorestarting"
 msgstr "Automatisches Neustarten"
 
-#: packages/apputils/src/kernelstatuses.ts:24 packages/apputils/src/kernelstatuses.tsx:36
+#: packages/apputils/src/kernelstatuses.tsx:36
 msgid "Dead"
 msgstr ""
 
-#: packages/apputils/src/kernelstatuses.ts:25 packages/apputils/src/kernelstatuses.tsx:37
+#: packages/apputils/src/kernelstatuses.tsx:37
 msgid "Connected"
 msgstr "Verbunden"
 
-#: packages/apputils/src/kernelstatuses.ts:26 packages/apputils/src/kernelstatuses.tsx:38
+#: packages/apputils/src/kernelstatuses.tsx:38
 msgid "Connecting"
 msgstr "Verbindung wird hergestellt"
 
-#: packages/apputils/src/kernelstatuses.ts:27 packages/apputils/src/kernelstatuses.tsx:39
+#: packages/apputils/src/kernelstatuses.tsx:39
 msgid "Disconnected"
 msgstr "Getrennt"
 
-#: packages/apputils/src/kernelstatuses.ts:28 packages/apputils/src/kernelstatuses.tsx:40
+#: packages/apputils/src/kernelstatuses.tsx:40
 msgid "Initializing"
 msgstr "Initialisiere"
 
-#: packages/apputils/src/kernelstatuses.tsx:210 packages/apputils/src/sessioncontext.tsx:1689 packages/apputils/src/sessioncontext.tsx:1746 packages/apputils/src/sessioncontext.tsx:613 packages/apputils/src/sessioncontext.tsx:631 packages/statusbar/src/defaults/kernelStatus.tsx:185
-msgid "No Kernel"
-msgstr "Kein Kernel"
-
-#: packages/apputils/src/kernelstatuses.tsx:62 packages/statusbar/src/defaults/kernelStatus.tsx:36
+#: packages/apputils/src/kernelstatuses.tsx:62
 msgid "Change kernel for %1"
 msgstr "Kernel für %1 ändern"
 
 #: packages/apputils/src/mainareawidget.ts:47
 msgid "notebook content"
 msgstr "Notebook-Inhalt"
 
 #: packages/apputils/src/mainareawidget.ts:50
 msgid "notebook actions"
 msgstr "Notebook-Aktionen"
 
-#: packages/apputils/src/runningSessions.tsx:115 packages/statusbar/src/defaults/runningSessions.tsx:111
+#: packages/apputils/src/runningSessions.tsx:115
 msgid "%1 Terminals, %2 Kernel sessions"
 msgstr "%1 Terminals, %2 Kernel-Sitzungen"
 
-#: packages/apputils/src/sessioncontext.tsx:1019 packages/apputils/src/sessioncontext.tsx:1051
+#: packages/apputils/src/sessioncontext.tsx:1051
 msgid "Error Starting Kernel"
 msgstr "Fehler beim Starten des Kernels"
 
-#: packages/apputils/src/sessioncontext.tsx:1298 packages/apputils/src/sessioncontext.tsx:1341 packages/filebrowser/src/opendialog.ts:83 packages/filebrowser/src/opendialog.ts:89
+#: packages/apputils/src/sessioncontext.tsx:1341 packages/filebrowser/src/opendialog.ts:83
 msgid "Select"
 msgstr "Auswählen"
 
-#: packages/apputils/src/sessioncontext.tsx:1302 packages/apputils/src/sessioncontext.tsx:1348
+#: packages/apputils/src/sessioncontext.tsx:1348
 msgid "Select Kernel"
 msgstr "Kernel auswählen"
 
 #: packages/apputils/src/sessioncontext.tsx:1353
 msgid "Always start the preferred kernel"
 msgstr ""
 
 #: packages/apputils/src/sessioncontext.tsx:1354
 msgid "Remember my choice and always start the preferred kernel"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1355 packages/apputils/src/sessioncontext.tsx:1415
+#: packages/apputils/src/sessioncontext.tsx:1415
 msgid "Restart Kernel?"
 msgstr "Kernel neu starten?"
 
-#: packages/apputils/src/sessioncontext.tsx:1356
-msgid "Do you want to restart the current kernel? All variables will be lost."
-msgstr "Möchtest du den aktuellen Kernel neu starten? Alle Variablen gehen verloren."
-
-#: packages/apputils/src/sessioncontext.tsx:1410 packages/apputils/src/sessioncontext.tsx:1473
-msgid "Select kernel for:"
-msgstr "Kernel auswählen:"
-
 #: packages/apputils/src/sessioncontext.tsx:1416
 msgid "Do you want to restart the kernel of %1? All variables will be lost."
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1550 packages/apputils/src/sessioncontext.tsx:1607
+#: packages/apputils/src/sessioncontext.tsx:1473
+msgid "Select kernel for:"
+msgstr "Kernel auswählen:"
+
+#: packages/apputils/src/sessioncontext.tsx:1607
 msgid "Start Preferred Kernel"
 msgstr "Bevorzugten Kernel starten"
 
-#: packages/apputils/src/sessioncontext.tsx:1565 packages/apputils/src/sessioncontext.tsx:1622
+#: packages/apputils/src/sessioncontext.tsx:1622
 msgid "Start Other Kernel"
 msgstr "Anderen Kernel starten"
 
-#: packages/apputils/src/sessioncontext.tsx:1622 packages/apputils/src/sessioncontext.tsx:1679
+#: packages/apputils/src/sessioncontext.tsx:1679
 msgid "Use Kernel from Preferred Session"
 msgstr "Kernel aus bevorzugter Sitzung verwenden"
 
-#: packages/apputils/src/sessioncontext.tsx:1637 packages/apputils/src/sessioncontext.tsx:1694
+#: packages/apputils/src/sessioncontext.tsx:1694
 msgid "Use Kernel from Other Session"
 msgstr "Kernel aus anderer Sitzung verwenden"
 
-#: packages/apputils/src/sessioncontext.tsx:1687 packages/apputils/src/sessioncontext.tsx:1744
+#: packages/apputils/src/sessioncontext.tsx:1744
 msgid "Use No Kernel"
 msgstr "Keinen Kernel verwenden"
 
-#: packages/apputils/src/sessioncontext.tsx:1711 packages/apputils/src/sessioncontext.tsx:1768
+#: packages/apputils/src/sessioncontext.tsx:1768
 msgid "Path:"
 msgstr "Pfad:"
 
-#: packages/apputils/src/sessioncontext.tsx:1712 packages/apputils/src/sessioncontext.tsx:1769
+#: packages/apputils/src/sessioncontext.tsx:1769
 msgid "Name:"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1713 packages/apputils/src/sessioncontext.tsx:1770
+#: packages/apputils/src/sessioncontext.tsx:1770
 msgid "Kernel Name:"
 msgstr "Kernelname:"
 
-#: packages/apputils/src/sessioncontext.tsx:1714 packages/apputils/src/sessioncontext.tsx:1771
+#: packages/apputils/src/sessioncontext.tsx:1771
 msgid "Kernel Id:"
 msgstr "Kernel-Id:"
 
-#: packages/apputils/src/thememanager.ts:362 packages/apputils/src/thememanager.ts:371 packages/apputils/src/thememanager.ts:373
+#: packages/apputils/src/thememanager.ts:371
 msgid "Neither theme %1 nor default %2 loaded."
 msgstr "Weder Theme %1 noch Standard %2 geladen."
 
-#: packages/apputils/src/thememanager.ts:446 packages/apputils/src/thememanager.ts:455 packages/apputils/src/thememanager.ts:457
+#: packages/apputils/src/thememanager.ts:455
 msgid "Error Loading Theme"
 msgstr "Fehler beim Laden des Themas"
 
-#: packages/apputils/src/thememanager.ts:448 packages/apputils/src/thememanager.ts:457 packages/apputils/src/thememanager.ts:459 packages/docmanager-extension/src/index.tsx:406 packages/extensionmanager/src/companions.tsx:218 packages/extensionmanager/src/dialog.tsx:39 packages/extensionmanager/src/widget.tsx:354 packages/extensionmanager/src/widget.tsx:355
+#: packages/apputils/src/thememanager.ts:457
 msgid "OK"
 msgstr ""
 
-#: packages/apputils/src/toolbar/factory.ts:29 packages/apputils/src/toolbar/factory.ts:34
+#: packages/apputils/src/toolbar/factory.ts:34
 msgid "Toolbar customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr ""
 
-#: packages/apputils/src/toolbar/widget.tsx:1274 packages/apputils/src/toolbar/widget.tsx:168
+#: packages/apputils/src/toolbar/widget.tsx:168
 msgid "Switch kernel"
 msgstr "Kernel wechseln"
 
-#: packages/apputils/src/toolbar/widget.tsx:1314 packages/apputils/src/toolbar/widget.tsx:208
+#: packages/apputils/src/toolbar/widget.tsx:208
 msgid "Kernel %1"
 msgstr ""
 
-#: packages/apputils/src/toolbar/widget.tsx:56 packages/apputils/src/toolbar/widget.tsx:610 packages/mainmenu-extension/src/index.ts:469 packages/mainmenu-extension/src/index.ts:472 packages/notebook-extension/src/index.ts:2453
+#: packages/apputils/src/toolbar/widget.tsx:56 packages/mainmenu-extension/src/index.ts:469 packages/notebook-extension/src/index.ts:2453
 msgid "Interrupt the kernel"
 msgstr "Kernel unterbrechen"
 
-#: packages/apputils/src/toolbar/widget.tsx:635 packages/apputils/src/toolbar/widget.tsx:80 packages/mainmenu-extension/src/index.ts:494 packages/notebook-extension/src/index.ts:2321
+#: packages/apputils/src/toolbar/widget.tsx:80 packages/mainmenu-extension/src/index.ts:494 packages/notebook-extension/src/index.ts:2321
 msgid "Restart the kernel"
 msgstr "Kernel neu starten"
 
 #: packages/cells/src/placeholder.ts:85
 msgid "Click to expand"
 msgstr ""
 
@@ -3180,70 +2832,42 @@
 msgstr[0] "%1 Zelle ausgeblendet"
 msgstr[1] "%1 Zellen ausgeblendet"
 
 #: packages/cells/src/widget.ts:2338
 msgid "Raw Cell Content"
 msgstr ""
 
-#: packages/celltags-extension/src/celltag.tsx:211 packages/celltags/src/addwidget.ts:159 packages/celltags/src/addwidget.ts:31
+#: packages/celltags-extension/src/celltag.tsx:211
 msgid "Add Tag"
 msgstr "Tag hinzufügen"
 
-#: packages/celltags/src/tool.ts:200
-msgid "Cell Tags"
-msgstr "Zellen Tags"
-
-#: packages/codeeditor/src/jsoneditor.ts:315 packages/codeeditor/src/jsoneditor.ts:327 packages/codeeditor/src/jsoneditor.ts:78
+#: packages/codeeditor/src/jsoneditor.ts:315
 msgid "No data!"
 msgstr "Keine Daten!"
 
-#: packages/codeeditor/src/jsoneditor.ts:58 packages/codeeditor/src/jsoneditor.ts:59
+#: packages/codeeditor/src/jsoneditor.ts:59
 msgid "Revert changes to data"
 msgstr "Änderungen an Daten zurücksetzen"
 
-#: packages/codeeditor/src/jsoneditor.ts:63 packages/codeeditor/src/jsoneditor.ts:64
+#: packages/codeeditor/src/jsoneditor.ts:64
 msgid "Commit changes to data"
 msgstr "Änderungen an Daten festschreiben"
 
-#: packages/codeeditor/src/lineCol.tsx:131 packages/statusbar/src/defaults/lineCol.tsx:133
+#: packages/codeeditor/src/lineCol.tsx:131
 msgid "Go to line number between 1 and %1"
 msgstr "Gehe zu Zeilennummer zwischen 1 und %1"
 
-#: packages/codeeditor/src/lineCol.tsx:229 packages/statusbar/src/defaults/lineCol.tsx:231
+#: packages/codeeditor/src/lineCol.tsx:229
 msgid "Ln %1, Col %2"
 msgstr "Z %1, Sp %2"
 
-#: packages/codeeditor/src/lineCol.tsx:230 packages/statusbar/src/defaults/lineCol.tsx:232
+#: packages/codeeditor/src/lineCol.tsx:230
 msgid "Go to line number…"
 msgstr "Gehe zu Zeilennummer …"
 
-#: packages/codemirror-extension/src/index.ts:297 packages/codemirror/src/theme.ts:215
-msgid "codemirror"
-msgstr ""
-
-#: packages/codemirror-extension/src/index.ts:314
-msgid "Sublime Text"
-msgstr ""
-
-#: packages/codemirror-extension/src/index.ts:329 packages/documentsearch-extension/src/index.ts:168 packages/documentsearch-extension/src/index.ts:229 packages/fileeditor-extension/src/commands.ts:525
-msgid "Find…"
-msgstr "Suchen…"
-
-#: packages/codemirror-extension/src/index.ts:342 packages/fileeditor-extension/src/commands.ts:538 packages/mainmenu-extension/src/index.ts:313 packages/mainmenu-extension/src/index.ts:324
-msgid "Go to Line…"
-msgstr "Zur Zeile springen…"
-
-#: packages/codemirror/src/editor.ts:1144
-msgid "Code Editor out of Sync"
-msgstr "Code-Editor nicht synchronisiert"
-
-#: packages/codemirror/src/editor.ts:1145
-msgid "Please open your browser JavaScript console for bug report instructions"
-msgstr "Bitte öffne die JavaScript-Konsole deines Browsers für Bug-Report-Anweisungen"
-
 #: packages/codemirror/src/extension.ts:608
 msgid "Auto Closing Brackets"
 msgstr "Automatisch schließende Klammern"
 
 #: packages/codemirror/src/extension.ts:617
 msgid "Code Folding"
 msgstr "Code-Faltung"
@@ -3272,23 +2896,23 @@
 msgid "Indentation unit"
 msgstr "Einrückungseinheit"
 
 #: packages/codemirror/src/extension.ts:675
 msgid "The indentation is a `Tab` or the number of spaces. This defaults to 4 spaces."
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:702 packages/fileeditor-extension/src/commands.ts:329
+#: packages/codemirror/src/extension.ts:702
 msgid "Line Numbers"
 msgstr "Zeilennummern"
 
 #: packages/codemirror/src/extension.ts:711
 msgid "Line Wrap"
 msgstr "Zeilenumbruch"
 
-#: packages/codemirror/src/extension.ts:720 packages/fileeditor-extension/src/commands.ts:420 packages/fileeditor-extension/src/commands.ts:421 packages/fileeditor-extension/src/commands.ts:428 packages/mainmenu-extension/src/index.ts:588 packages/mainmenu-extension/src/index.ts:593
+#: packages/codemirror/src/extension.ts:720 packages/fileeditor-extension/src/commands.ts:421 packages/fileeditor-extension/src/commands.ts:428 packages/mainmenu-extension/src/index.ts:588
 msgid "Match Brackets"
 msgstr ""
 
 #: packages/codemirror/src/extension.ts:733
 msgid "Rectangular selection"
 msgstr "Rechteckige Auswahl"
 
@@ -3372,19 +2996,19 @@
 msgid "Go to line"
 msgstr ""
 
 #: packages/codemirror/src/extension.ts:878
 msgid "go"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:879 packages/documentsearch/src/searchoverlay.tsx:124 packages/documentsearch/src/searchview.tsx:154 packages/documentsearch/src/searchview.tsx:159
+#: packages/codemirror/src/extension.ts:879 packages/documentsearch/src/searchview.tsx:154 packages/documentsearch/src/searchview.tsx:159
 msgid "Find"
 msgstr "Suchen"
 
-#: packages/codemirror/src/extension.ts:880 packages/documentsearch/src/searchoverlay.tsx:173 packages/documentsearch/src/searchoverlay.tsx:191 packages/documentsearch/src/searchview.tsx:217 packages/documentsearch/src/searchview.tsx:221 packages/documentsearch/src/searchview.tsx:248
+#: packages/codemirror/src/extension.ts:880 packages/documentsearch/src/searchview.tsx:217 packages/documentsearch/src/searchview.tsx:221 packages/documentsearch/src/searchview.tsx:248
 msgid "Replace"
 msgstr "Ersetzen"
 
 #: packages/codemirror/src/extension.ts:881
 msgid "next"
 msgstr "weiter"
 
@@ -3624,15 +3248,15 @@
 msgid "Swift"
 msgstr "Swift"
 
 #: packages/codemirror/src/language.ts:1477
 msgid "sTeX"
 msgstr "sTeX"
 
-#: packages/codemirror/src/language.ts:1486 packages/notebook-extension/src/index.ts:2868 packages/notebook-extension/src/index.ts:3678
+#: packages/codemirror/src/language.ts:1486 packages/notebook-extension/src/index.ts:3678
 msgid "LaTeX"
 msgstr "LaTeX"
 
 #: packages/codemirror/src/language.ts:1497
 msgid "SystemVerilog"
 msgstr "SystemVerilog"
 
@@ -3736,15 +3360,15 @@
 msgid "CQL"
 msgstr ""
 
 #: packages/codemirror/src/language.ts:336
 msgid "CSS"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:346 packages/notebook-extension/src/index.ts:2867 packages/notebook-extension/src/index.ts:3677
+#: packages/codemirror/src/language.ts:346 packages/notebook-extension/src/index.ts:3677
 msgid "HTML"
 msgstr ""
 
 #: packages/codemirror/src/language.ts:357
 msgid "Java"
 msgstr ""
 
@@ -3760,15 +3384,15 @@
 msgid "JSX"
 msgstr ""
 
 #: packages/codemirror/src/language.ts:405
 msgid "MariaDB SQL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:413 packages/notebook-extension/src/index.ts:2869 packages/notebook-extension/src/index.ts:3679 packages/notebook/src/default-toolbar.tsx:360 packages/notebook/src/default-toolbar.tsx:379
+#: packages/codemirror/src/language.ts:413 packages/notebook-extension/src/index.ts:3679 packages/notebook/src/default-toolbar.tsx:379
 msgid "Markdown"
 msgstr ""
 
 #: packages/codemirror/src/language.ts:423
 msgid "MS SQL"
 msgstr ""
 
@@ -3992,211 +3616,179 @@
 msgid "HTTP"
 msgstr "HTTP"
 
 #: packages/codemirror/src/language.ts:996
 msgid "IDL"
 msgstr "IDL"
 
-#: packages/codemirror/src/syntaxstatus.tsx:66 packages/fileeditor/src/syntaxstatus.tsx:66
-msgid "Change text editor syntax highlighting"
-msgstr "Syntaxhervorhebung des Texteditors ändern"
-
-#: packages/collaboration-extension/src/index.ts:163
-msgid "User info"
-msgstr ""
-
-#: packages/collaboration-extension/src/index.ts:164
-msgid "User information"
-msgstr "Benutzerinformationen"
-
-#: packages/collaboration-extension/src/index.ts:176
-msgid "Online Collaborators"
+#: packages/codemirror/src/theme.ts:215
+msgid "codemirror"
 msgstr ""
 
-#: packages/console-extension/src/foreign.ts:65 packages/console-extension/src/foreign.ts:66 packages/console-extension/src/index.ts:155 packages/console-extension/src/index.ts:203 packages/console-extension/src/index.ts:262 packages/console-extension/src/index.ts:311 packages/console-extension/src/index.ts:483 packages/console-extension/src/index.ts:530 packages/console/src/panel.ts:331 packages/console/src/panel.ts:333 packages/launcher/src/index.tsx:150 packages/launcher/src/index.tsx:155 packages/launcher/src/widget.tsx:116 packages/launcher/src/widget.tsx:121
+#: packages/console-extension/src/foreign.ts:66 packages/console-extension/src/index.ts:262 packages/console-extension/src/index.ts:311 packages/console-extension/src/index.ts:530 packages/console/src/panel.ts:333 packages/launcher/src/widget.tsx:116 packages/launcher/src/widget.tsx:121
 msgid "Console"
 msgstr "Konsole"
 
-#: packages/console-extension/src/foreign.ts:79 packages/console-extension/src/foreign.ts:80
+#: packages/console-extension/src/foreign.ts:80
 msgid "Show All Kernel Activity"
 msgstr "Alle Kernel-Aktivitäten anzeigen"
 
-#: packages/console-extension/src/index.ts:418 packages/console-extension/src/index.ts:464
+#: packages/console-extension/src/index.ts:464
 msgid "Auto Close Brackets for Code Console Prompt"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:472 packages/console-extension/src/index.ts:519
-msgid "New Console"
-msgstr "Neue Konsole"
-
 #: packages/console-extension/src/index.ts:490
 msgid "Open a console for the provided `path`."
 msgstr ""
 
-#: packages/console-extension/src/index.ts:507 packages/console-extension/src/index.ts:554
+#: packages/console-extension/src/index.ts:519
+msgid "New Console"
+msgstr "Neue Konsole"
+
+#: packages/console-extension/src/index.ts:554
 msgid "Clear Console Cells"
 msgstr "Konsolenzellen leeren"
 
-#: packages/console-extension/src/index.ts:519 packages/console-extension/src/index.ts:566
+#: packages/console-extension/src/index.ts:566
 msgid "Run Cell (unforced)"
 msgstr "Zelle ausführen (unerzwungen)"
 
-#: packages/console-extension/src/index.ts:531 packages/console-extension/src/index.ts:578
+#: packages/console-extension/src/index.ts:578
 msgid "Run Cell (forced)"
 msgstr "Zelle ausführen (erzwungen)"
 
-#: packages/console-extension/src/index.ts:543 packages/console-extension/src/index.ts:590
+#: packages/console-extension/src/index.ts:590
 msgid "Insert Line Break"
 msgstr "Zeilenumbruch einfügen"
 
-#: packages/console-extension/src/index.ts:555 packages/console-extension/src/index.ts:602
+#: packages/console-extension/src/index.ts:602
 msgid "Replace Selection in Console"
 msgstr "Auswahl in Konsole ersetzen"
 
-#: packages/console-extension/src/index.ts:568 packages/console-extension/src/index.ts:615 packages/mainmenu-extension/src/index.ts:468 packages/mainmenu-extension/src/index.ts:471 packages/notebook-extension/src/index.ts:1852 packages/notebook-extension/src/index.ts:2452
+#: packages/console-extension/src/index.ts:615 packages/mainmenu-extension/src/index.ts:468 packages/notebook-extension/src/index.ts:2452
 msgid "Interrupt Kernel"
 msgstr "Kernel unterbrechen"
 
-#: packages/console-extension/src/index.ts:583 packages/console-extension/src/index.ts:630 packages/mainmenu-extension/src/index.ts:493 packages/notebook-extension/src/index.ts:1724 packages/notebook-extension/src/index.ts:2320
+#: packages/console-extension/src/index.ts:630 packages/mainmenu-extension/src/index.ts:493 packages/notebook-extension/src/index.ts:2320
 msgid "Restart Kernel…"
 msgstr "Kernel neu starten…"
 
-#: packages/console-extension/src/index.ts:598 packages/console-extension/src/index.ts:654
+#: packages/console-extension/src/index.ts:642 packages/lsp-extension/src/index.ts:275 packages/mainmenu-extension/src/index.ts:375 packages/mainmenu-extension/src/index.ts:385 packages/running/src/index.tsx:161 packages/terminal-extension/src/index.ts:322
+msgid "Shut Down"
+msgstr "Herunterfahren"
+
+#: packages/console-extension/src/index.ts:654
 msgid "Close and Shut Down…"
 msgstr "Schließen und herunterfahren…"
 
-#: packages/console-extension/src/index.ts:605 packages/console-extension/src/index.ts:661
+#: packages/console-extension/src/index.ts:661
 msgid "Shut down the console?"
 msgstr "Konsole herunterfahren?"
 
-#: packages/console-extension/src/index.ts:606 packages/console-extension/src/index.ts:662 packages/console-extension/src/index.ts:685 packages/notebook-extension/src/index.ts:1747 packages/notebook-extension/src/index.ts:2357 packages/notebook-extension/src/index.ts:2654
+#: packages/console-extension/src/index.ts:662 packages/notebook-extension/src/index.ts:2357
 msgid "Are you sure you want to close \"%1\"?"
 msgstr "Bist du sicher, dass du %1 schließen möchten?"
 
-#: packages/console-extension/src/index.ts:642 packages/lsp-extension/src/index.ts:275 packages/mainmenu-extension/src/index.ts:375 packages/mainmenu-extension/src/index.ts:382 packages/mainmenu-extension/src/index.ts:385 packages/mainmenu-extension/src/index.ts:392 packages/running-extension/src/kernels.ts:39 packages/running/src/index.tsx:142 packages/running/src/index.tsx:161 packages/terminal-extension/src/index.ts:302 packages/terminal-extension/src/index.ts:322
-msgid "Shut Down"
-msgstr "Herunterfahren"
-
-#: packages/console-extension/src/index.ts:646 packages/console-extension/src/index.ts:705 packages/mainmenu-extension/src/index.ts:519 packages/mainmenu-extension/src/index.ts:530 packages/notebook-extension/src/index.ts:2225 packages/notebook-extension/src/index.ts:3059
-msgid "Change Kernel…"
-msgstr "Kernel wechseln…"
-
-#: packages/console-extension/src/index.ts:681
-msgid "Shutdown Console"
-msgstr "Konsole herunterfahren"
-
 #: packages/console-extension/src/index.ts:684
 msgid "Inject some code in a console."
 msgstr ""
 
-#: packages/console-extension/src/index.ts:684
-msgid "Shut down the Console?"
-msgstr "Konsole herunterfahren?"
-
-#: packages/console-extension/src/index.ts:706
-msgid "Restart Kernel and Clear Console"
-msgstr "Kernel neu starten und Konsole leeren"
+#: packages/console-extension/src/index.ts:705 packages/mainmenu-extension/src/index.ts:519 packages/notebook-extension/src/index.ts:3059
+msgid "Change Kernel…"
+msgstr "Kernel wechseln…"
 
 #: packages/console-extension/src/index.ts:717 packages/mainmenu-extension/src/index.ts:754 packages/notebook-extension/src/index.ts:3070
 msgid "Get Kernel"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:737
-msgid "Run Cell"
-msgstr "Zelle ausführen"
-
-#: packages/console-extension/src/index.ts:744
-msgid "Clear Console Cell"
-msgstr "Konsolenzelle leeren"
-
-#: packages/console-extension/src/index.ts:757 packages/console-extension/src/index.ts:799
+#: packages/console-extension/src/index.ts:799
 msgid "Execute with Shift+Enter"
 msgstr "Ausführen mit Shift+Enter"
 
-#: packages/console-extension/src/index.ts:758 packages/console-extension/src/index.ts:800
+#: packages/console-extension/src/index.ts:800
 msgid "Execute with Enter"
 msgstr "Ausführen mit Enter"
 
 #: packages/console-extension/src/index.ts:844 packages/fileeditor-extension/src/commands.ts:1005 packages/notebook-extension/src/index.ts:1974
 msgid "Display the completion helper."
 msgstr ""
 
 #: packages/console-extension/src/index.ts:855 packages/fileeditor-extension/src/commands.ts:1016 packages/notebook-extension/src/index.ts:1984
 msgid "Select the completion suggestion."
 msgstr ""
 
-#: packages/console/src/panel.ts:314 packages/console/src/panel.ts:316
+#: packages/console/src/panel.ts:316
 msgid "Name: %1\n"
 msgstr "Name: %1\n"
 
-#: packages/console/src/panel.ts:315 packages/console/src/panel.ts:317
+#: packages/console/src/panel.ts:317
 msgid "Directory: %1\n"
 msgstr "Verzeichnis: %1\n"
 
-#: packages/console/src/panel.ts:316 packages/console/src/panel.ts:318
+#: packages/console/src/panel.ts:318
 msgid "Kernel: %1"
 msgstr "Kernel: %1"
 
-#: packages/console/src/panel.ts:319 packages/console/src/panel.ts:321
+#: packages/console/src/panel.ts:321
 msgid "\n"
 "Connected: %1"
 msgstr "\n"
 "Verbunden: %1"
 
-#: packages/console/src/panel.ts:326 packages/console/src/panel.ts:328
+#: packages/console/src/panel.ts:328
 msgid "\n"
 "Last Execution: %1"
 msgstr "\n"
 "Letzte Ausführung: %1"
 
-#: packages/console/src/panel.ts:66 packages/console/src/panel.ts:67
+#: packages/console/src/panel.ts:66
 msgid "Console %1"
 msgstr "Konsole %1"
 
 #: packages/csvviewer-extension/src/index.ts:134
 msgid "CSV Viewer"
 msgstr "CSV-Betrachter"
 
-#: packages/csvviewer-extension/src/index.ts:212 packages/csvviewer-extension/src/index.ts:219 packages/csvviewer-extension/src/index.ts:362 packages/csvviewer-extension/src/index.ts:369 packages/csvviewer-extension/src/index.ts:92
+#: packages/csvviewer-extension/src/index.ts:212 packages/csvviewer-extension/src/index.ts:219 packages/csvviewer-extension/src/index.ts:362 packages/csvviewer-extension/src/index.ts:369
 msgid "Go to Line"
 msgstr "Zur Zeile springen"
 
 #: packages/csvviewer-extension/src/index.ts:284
 msgid "TSV Viewer"
 msgstr "TSV-Betrachter"
 
-#: packages/csvviewer/src/toolbar.ts:119 packages/csvviewer/src/toolbar.ts:133
+#: packages/csvviewer/src/toolbar.ts:119
 msgid "tab"
 msgstr "Tab"
 
-#: packages/csvviewer/src/toolbar.ts:120 packages/csvviewer/src/toolbar.ts:134
+#: packages/csvviewer/src/toolbar.ts:120
 msgid "pipe"
 msgstr "Pipe"
 
-#: packages/csvviewer/src/toolbar.ts:121 packages/csvviewer/src/toolbar.ts:135
+#: packages/csvviewer/src/toolbar.ts:121
 msgid "hash"
 msgstr "Hash"
 
-#: packages/csvviewer/src/toolbar.ts:127 packages/csvviewer/src/toolbar.ts:141
+#: packages/csvviewer/src/toolbar.ts:127
 msgid "Delimiter: "
 msgstr "Trennzeichen: "
 
-#: packages/debugger-extension/src/index.ts:192 packages/debugger-extension/src/index.ts:193 packages/debugger-extension/src/index.ts:214 packages/debugger-extension/src/index.ts:215
+#: packages/debugger-extension/src/index.ts:214 packages/debugger-extension/src/index.ts:215
 msgid "Restart Kernel and Debug…"
 msgstr "Kernel neu starten und debuggen.."
 
-#: packages/debugger-extension/src/index.ts:339 packages/debugger-extension/src/index.ts:340 packages/debugger-extension/src/index.ts:373 packages/debugger-extension/src/index.ts:374
+#: packages/debugger-extension/src/index.ts:373 packages/debugger-extension/src/index.ts:374
 msgid "Inspect Variable"
 msgstr "Variable inspizieren"
 
-#: packages/debugger-extension/src/index.ts:403 packages/debugger-extension/src/index.ts:440
+#: packages/debugger-extension/src/index.ts:440
 msgid "Render Variable"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:404 packages/debugger-extension/src/index.ts:441
+#: packages/debugger-extension/src/index.ts:441
 msgid "Render variable according to its mime type"
 msgstr ""
 
 #: packages/debugger-extension/src/index.ts:518
 msgid "Copy to Clipboard"
 msgstr "In die Zwischenablage kopieren"
 
@@ -4208,423 +3800,399 @@
 msgid "Copy Variable to Globals"
 msgstr ""
 
 #: packages/debugger-extension/src/index.ts:537
 msgid "Copy variable to globals scope"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:616 packages/debugger-extension/src/index.ts:617 packages/debugger-extension/src/index.ts:623 packages/debugger-extension/src/index.ts:687 packages/debugger-extension/src/index.ts:688 packages/debugger-extension/src/index.ts:694
+#: packages/debugger-extension/src/index.ts:687 packages/debugger-extension/src/index.ts:688 packages/debugger-extension/src/index.ts:694
 msgid "Evaluate Code"
 msgstr "Code auswerten"
 
-#: packages/debugger-extension/src/index.ts:624 packages/debugger-extension/src/index.ts:695
+#: packages/debugger-extension/src/index.ts:695
 msgid "Evaluate"
 msgstr "Bewerten"
 
-#: packages/debugger-extension/src/index.ts:653 packages/debugger-extension/src/index.ts:658 packages/debugger-extension/src/index.ts:728 packages/debugger-extension/src/index.ts:733
+#: packages/debugger-extension/src/index.ts:728 packages/debugger-extension/src/index.ts:733
 msgid "Continue"
 msgstr "Fortfahren"
 
-#: packages/debugger-extension/src/index.ts:654 packages/debugger-extension/src/index.ts:659 packages/debugger-extension/src/index.ts:729 packages/debugger-extension/src/index.ts:734
+#: packages/debugger-extension/src/index.ts:729 packages/debugger-extension/src/index.ts:734
 msgid "Pause"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:678 packages/debugger-extension/src/index.ts:679 packages/debugger-extension/src/index.ts:753 packages/debugger-extension/src/index.ts:754
+#: packages/debugger-extension/src/index.ts:753 packages/debugger-extension/src/index.ts:754
 msgid "Terminate"
 msgstr "Beenden"
 
-#: packages/debugger-extension/src/index.ts:689 packages/debugger-extension/src/index.ts:690 packages/debugger-extension/src/index.ts:764 packages/debugger-extension/src/index.ts:765
+#: packages/debugger-extension/src/index.ts:764 packages/debugger-extension/src/index.ts:765
 msgid "Next"
 msgstr "Weiter"
 
-#: packages/debugger-extension/src/index.ts:699 packages/debugger-extension/src/index.ts:700 packages/debugger-extension/src/index.ts:774 packages/debugger-extension/src/index.ts:775
+#: packages/debugger-extension/src/index.ts:774 packages/debugger-extension/src/index.ts:775
 msgid "Step In"
 msgstr "Schritt hinein"
 
-#: packages/debugger-extension/src/index.ts:709 packages/debugger-extension/src/index.ts:710 packages/debugger-extension/src/index.ts:784 packages/debugger-extension/src/index.ts:785
+#: packages/debugger-extension/src/index.ts:784 packages/debugger-extension/src/index.ts:785
 msgid "Step Out"
 msgstr "Schritt heraus"
 
-#: packages/debugger-extension/src/index.ts:719 packages/debugger-extension/src/index.ts:727
-msgid "Enable / Disable pausing on exceptions"
-msgstr ""
-
-#: packages/debugger-extension/src/index.ts:724
-msgid "Disable pausing on exceptions"
-msgstr ""
-
-#: packages/debugger-extension/src/index.ts:725
-msgid "Enable pausing on exceptions"
-msgstr ""
-
-#: packages/debugger-extension/src/index.ts:726
-msgid "Kernel does not support pausing on exceptions."
+#: packages/debugger-extension/src/index.ts:811
+msgid "Select a filter for breakpoints on exception"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:775 packages/debugger-extension/src/index.ts:859
+#: packages/debugger-extension/src/index.ts:859
 msgid "Debugger section"
 msgstr "Debugger-Abschnitt"
 
-#: packages/debugger-extension/src/index.ts:780 packages/debugger-extension/src/index.ts:861 packages/debugger-extension/src/index.ts:873
+#: packages/debugger-extension/src/index.ts:861 packages/debugger-extension/src/index.ts:873
 msgid "Debugger"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:811
-msgid "Select a filter for breakpoints on exception"
+#: packages/debugger-extension/src/index.ts:866
+msgid "Debugger Panel"
 msgstr ""
 
-#: packages/debugger/src/handler.ts:39 packages/debugger/src/handler.ts:57
+#: packages/debugger/src/handler.ts:39
 msgid "Enable Debugger"
 msgstr "Debugger einschalten"
 
-#: packages/debugger/src/handler.ts:41 packages/debugger/src/handler.ts:59
+#: packages/debugger/src/handler.ts:41
 msgid "Disable Debugger"
 msgstr "Debugger ausschalten"
 
-#: packages/debugger/src/handler.ts:42 packages/debugger/src/handler.ts:60
+#: packages/debugger/src/handler.ts:42
 msgid "Select a kernel that supports debugging to enable debugger"
 msgstr "Wählen Sie einen Kernel, der Debugging unterstützt, um den Debugger zu aktivieren"
 
-#: packages/debugger/src/panels/breakpoints/header.ts:25 packages/debugger/src/panels/breakpoints/index.ts:28 packages/debugger/src/panels/breakpoints/index.ts:39
+#: packages/debugger/src/panels/breakpoints/index.ts:28
 msgid "Breakpoints"
 msgstr "Haltepunkte"
 
 #: packages/debugger/src/panels/breakpoints/index.ts:38
 msgid "Pause on exception filter"
 msgstr ""
 
-#: packages/debugger/src/panels/breakpoints/index.ts:51 packages/debugger/src/panels/breakpoints/index.ts:62 packages/debugger/src/panels/breakpoints/index.ts:63 packages/debugger/src/panels/breakpoints/index.ts:74
+#: packages/debugger/src/panels/breakpoints/index.ts:51 packages/debugger/src/panels/breakpoints/index.ts:63
 msgid "Remove All Breakpoints"
 msgstr "Alle Haltepunkte löschen"
 
-#: packages/debugger/src/panels/breakpoints/index.ts:52 packages/debugger/src/panels/breakpoints/index.ts:63
+#: packages/debugger/src/panels/breakpoints/index.ts:52
 msgid "Are you sure you want to remove all breakpoints?"
 msgstr "Sind Sie sicher, dass Sie alle Breakpoints  entfernen wollen?"
 
-#: packages/debugger/src/panels/breakpoints/index.ts:54 packages/debugger/src/panels/breakpoints/index.ts:65
+#: packages/debugger/src/panels/breakpoints/index.ts:54
 msgid "Remove breakpoints"
 msgstr "Breakpoints entfernen"
 
-#: packages/debugger/src/panels/callstack/header.ts:25 packages/debugger/src/panels/callstack/index.ts:27
+#: packages/debugger/src/panels/callstack/index.ts:27
 msgid "Callstack"
 msgstr "Aufrufstapel"
 
 #: packages/debugger/src/panels/kernelSources/body.tsx:83
 msgid "Fail to get source"
 msgstr ""
 
 #: packages/debugger/src/panels/kernelSources/body.tsx:84
 msgid "Fail to get '%1' source:\n"
 "%2"
 msgstr ""
 
-#: packages/debugger/src/panels/kernelSources/header.tsx:32 packages/debugger/src/panels/kernelSources/index.tsx:33 packages/debugger/src/panels/kernelSources/index.tsx:34
+#: packages/debugger/src/panels/kernelSources/index.tsx:33
 msgid "Kernel Sources"
 msgstr ""
 
-#: packages/debugger/src/panels/kernelSources/index.tsx:49 packages/debugger/src/panels/kernelSources/index.tsx:53
+#: packages/debugger/src/panels/kernelSources/index.tsx:49
 msgid "Toggle search filter"
 msgstr ""
 
-#: packages/debugger/src/panels/kernelSources/index.tsx:61 packages/debugger/src/panels/kernelSources/index.tsx:65
+#: packages/debugger/src/panels/kernelSources/index.tsx:61
 msgid "Fail to get kernel sources"
 msgstr ""
 
-#: packages/debugger/src/panels/kernelSources/index.tsx:62 packages/debugger/src/panels/kernelSources/index.tsx:66
+#: packages/debugger/src/panels/kernelSources/index.tsx:62
 msgid "Fail to get kernel sources:\n"
 "%2"
 msgstr ""
 
-#: packages/debugger/src/panels/kernelSources/index.tsx:66 packages/debugger/src/panels/kernelSources/index.tsx:70
+#: packages/debugger/src/panels/kernelSources/index.tsx:66
 msgid "Refresh kernel sources"
 msgstr ""
 
-#: packages/debugger/src/panels/sources/header.tsx:34 packages/debugger/src/panels/sources/index.tsx:29 packages/shortcuts-extension/src/components/TopNav.tsx:185 packages/shortcuts-extension/src/components/TopNav.tsx:277
+#: packages/debugger/src/panels/sources/index.tsx:29 packages/shortcuts-extension/src/components/TopNav.tsx:185
 msgid "Source"
 msgstr "Quelltext"
 
-#: packages/debugger/src/panels/sources/index.ts:48 packages/debugger/src/panels/sources/index.tsx:42
+#: packages/debugger/src/panels/sources/index.tsx:42
 msgid "Open in the Main Area"
 msgstr "Im Hauptbereich öffnen"
 
 #: packages/debugger/src/panels/variables/gridpanel.ts:218
 msgid "Type"
 msgstr ""
 
 #: packages/debugger/src/panels/variables/gridpanel.ts:218
 msgid "Value"
 msgstr ""
 
-#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:1878 packages/filebrowser/src/listing.ts:2258
+#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:2258
 msgid "Name"
 msgstr ""
 
-#: packages/debugger/src/panels/variables/header.ts:25 packages/debugger/src/panels/variables/index.ts:33
+#: packages/debugger/src/panels/variables/index.ts:33
 msgid "Variables"
 msgstr "Variablen"
 
 #: packages/debugger/src/panels/variables/index.ts:78
 msgid "Tree View"
 msgstr "Baumansicht"
 
 #: packages/debugger/src/panels/variables/index.ts:85
 msgid "Table View"
 msgstr "Tabellenansicht"
 
-#: packages/debugger/src/panels/variables/mimerenderer.ts:53 packages/debugger/src/panels/variables/mimerenderer.ts:58
+#: packages/debugger/src/panels/variables/mimerenderer.ts:58
 msgid "The variable is undefined in the active context."
 msgstr ""
 
-#: packages/debugger/src/panels/variables/scope.tsx:51 packages/debugger/src/panels/variables/scope.tsx:53
+#: packages/debugger/src/panels/variables/scope.tsx:51
 msgid "Scope"
 msgstr "Gültigkeitsbereich"
 
 #: packages/debugger/src/panels/variables/tree.tsx:275
 msgid "Render variable: %1"
 msgstr ""
 
-#: packages/debugger/src/panels/variables/tree.tsx:282
-msgid "Render variable"
-msgstr ""
-
 #: packages/debugger/src/service.ts:378
 msgid "Globals"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1002 packages/docmanager-extension/src/index.tsx:1113 packages/docmanager-extension/src/index.tsx:981
+#: packages/docmanager-extension/src/index.tsx:1060
+msgid "New View for %1"
+msgstr "Neue Ansicht für %1"
+
+#: packages/docmanager-extension/src/index.tsx:1084
+msgid "Rename%1…"
+msgstr "Umbenennen%1…"
+
+#: packages/docmanager-extension/src/index.tsx:1098
+msgid "Duplicate %1"
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:1113
 msgid "Delete %1"
 msgstr "%1 löschen"
 
-#: packages/docmanager-extension/src/index.tsx:1009 packages/docmanager-extension/src/index.tsx:1030 packages/docmanager-extension/src/index.tsx:1141
-msgid "Show in File Browser"
-msgstr "Im Dateibrowser anzeigen"
-
-#: packages/docmanager-extension/src/index.tsx:1012 packages/docmanager-extension/src/index.tsx:1016 packages/docmanager-extension/src/index.tsx:1123 packages/docmanager-extension/src/index.tsx:1127 packages/docmanager-extension/src/index.tsx:991 packages/docmanager-extension/src/index.tsx:995 packages/filebrowser-extension/src/index.ts:819 packages/filebrowser-extension/src/index.ts:922 packages/filebrowser/src/listing.ts:412 packages/filebrowser/src/listing.ts:416 packages/filebrowser/src/listing.ts:426 packages/filebrowser/src/listing.ts:430
+#: packages/docmanager-extension/src/index.tsx:1123 packages/docmanager-extension/src/index.tsx:1127 packages/filebrowser-extension/src/index.ts:922 packages/filebrowser/src/listing.ts:426 packages/filebrowser/src/listing.ts:430
 msgid "Delete"
 msgstr "Löschen"
 
-#: packages/docmanager-extension/src/index.tsx:1013 packages/docmanager-extension/src/index.tsx:1124 packages/docmanager-extension/src/index.tsx:992
+#: packages/docmanager-extension/src/index.tsx:1124
 msgid "Are you sure you want to delete %1"
 msgstr "Bist du sicher, dass du %1 löschen möchtest"
 
-#: packages/docmanager-extension/src/index.tsx:1060 packages/docmanager-extension/src/index.tsx:943 packages/docmanager-extension/src/index.tsx:964
-msgid "New View for %1"
-msgstr "Neue Ansicht für %1"
+#: packages/docmanager-extension/src/index.tsx:1141
+msgid "Show in File Browser"
+msgstr "Im Dateibrowser anzeigen"
 
-#: packages/docmanager-extension/src/index.tsx:1075 packages/docmanager-extension/src/index.tsx:1096
-msgid "Are you sure you want to revert the %1 to the latest checkpoint? "
-msgstr "Sind Sie sicher, dass Sie %1 auf den letzten Kontrollpunkt zurücksetzen möchten? "
+#: packages/docmanager-extension/src/index.tsx:1207
+msgid "Are you sure you want to revert the %1 to checkpoint? "
+msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1081 packages/docmanager-extension/src/index.tsx:1102 packages/docmanager-extension/src/index.tsx:1213
+#: packages/docmanager-extension/src/index.tsx:1213
 msgid "This cannot be undone."
 msgstr "Dies kann nicht rückgängig gemacht werden."
 
-#: packages/docmanager-extension/src/index.tsx:1084 packages/docmanager-extension/src/index.tsx:967 packages/docmanager-extension/src/index.tsx:988
-msgid "Rename%1…"
-msgstr "Umbenennen%1…"
-
-#: packages/docmanager-extension/src/index.tsx:1088 packages/docmanager-extension/src/index.tsx:1109 packages/docmanager-extension/src/index.tsx:1220
+#: packages/docmanager-extension/src/index.tsx:1220
 msgid "The checkpoint was last updated at: "
 msgstr "Der Kontrollpunkt wurde zuletzt aktualisiert um: "
 
-#: packages/docmanager-extension/src/index.tsx:1098
-msgid "Duplicate %1"
-msgstr ""
-
-#: packages/docmanager-extension/src/index.tsx:1207
-msgid "Are you sure you want to revert the %1 to checkpoint? "
-msgstr ""
-
 #: packages/docmanager-extension/src/index.tsx:1254
 msgid "Choose a checkpoint"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:271 packages/docmanager-extension/src/index.tsx:344
+#: packages/docmanager-extension/src/index.tsx:344
 msgid "Overrides for the default viewers for file types.\n"
 "Specify a mapping from file type name to document viewer name, for example:\n\n"
 "defaultViewers: {\n"
 "  markdown: \"Markdown Preview\"\n"
 "}\n\n"
 "If you specify non-existent file types or viewers, or if a viewer cannot\n"
 "open a given file type, the override will not function.\n\n"
 "Available viewers:\n"
 "%1\n\n"
 "Available file types:\n"
 "%2"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:395 packages/docmanager-extension/src/index.tsx:474 packages/filebrowser-extension/src/index.ts:343 packages/filebrowser-extension/src/index.ts:367
+#: packages/docmanager-extension/src/index.tsx:474 packages/filebrowser-extension/src/index.ts:367
 msgid "Download"
 msgstr "Herunterladen"
 
-#: packages/docmanager-extension/src/index.tsx:396 packages/docmanager-extension/src/index.tsx:475
+#: packages/docmanager-extension/src/index.tsx:475
 msgid "Download the file to your computer"
 msgstr "Datei auf Ihren Computer herunterladen"
 
-#: packages/docmanager-extension/src/index.tsx:404 packages/docmanager-extension/src/index.tsx:483
+#: packages/docmanager-extension/src/index.tsx:483
 msgid "Cannot Download"
 msgstr "Herunterladen nicht möglich"
 
-#: packages/docmanager-extension/src/index.tsx:405 packages/docmanager-extension/src/index.tsx:484 packages/docmanager-extension/src/index.tsx:641 packages/docmanager-extension/src/index.tsx:686 packages/docmanager-extension/src/index.tsx:726 packages/docmanager-extension/src/index.tsx:749 packages/docmanager-extension/src/index.tsx:771 packages/docmanager-extension/src/index.tsx:844 packages/docmanager-extension/src/index.tsx:873 packages/docmanager-extension/src/index.tsx:968
+#: packages/docmanager-extension/src/index.tsx:484 packages/docmanager-extension/src/index.tsx:726 packages/docmanager-extension/src/index.tsx:771 packages/docmanager-extension/src/index.tsx:844 packages/docmanager-extension/src/index.tsx:968
 msgid "No context found for current widget!"
 msgstr "Kein Kontext für aktuelles Widget gefunden!"
 
-#: packages/docmanager-extension/src/index.tsx:414 packages/docmanager-extension/src/index.tsx:493 packages/docmanager-extension/src/index.tsx:550 packages/docmanager-extension/src/index.tsx:634 packages/filebrowser-extension/src/index.ts:1074 packages/filebrowser-extension/src/index.ts:1200 packages/filebrowser-extension/src/index.ts:566 packages/filebrowser-extension/src/index.ts:790 packages/filebrowser-extension/src/index.ts:892 packages/filebrowser-extension/src/index.ts:968 packages/htmlviewer-extension/src/index.tsx:180 packages/htmlviewer-extension/src/index.tsx:206
+#: packages/docmanager-extension/src/index.tsx:493 packages/docmanager-extension/src/index.tsx:634 packages/filebrowser-extension/src/index.ts:1074 packages/filebrowser-extension/src/index.ts:566 packages/filebrowser-extension/src/index.ts:892 packages/htmlviewer-extension/src/index.tsx:206
 msgid "File Operations"
 msgstr "Dateioperationen"
 
-#: packages/docmanager-extension/src/index.tsx:461 packages/docmanager-extension/src/index.tsx:542 packages/filebrowser-extension/src/index.ts:671 packages/filebrowser-extension/src/index.ts:772
+#: packages/docmanager-extension/src/index.tsx:542 packages/filebrowser-extension/src/index.ts:772
 msgid "Open in New Browser Tab"
 msgstr "In neuem Tab öffnen"
 
-#: packages/docmanager-extension/src/index.tsx:587 packages/docmanager-extension/src/index.tsx:670 packages/filebrowser/src/browser.ts:236 packages/filebrowser/src/browser.ts:282 packages/filebrowser/src/browser.ts:312 packages/logconsole-extension/src/index.tsx:381 packages/logconsole-extension/src/index.tsx:392
+#: packages/docmanager-extension/src/index.tsx:670 packages/filebrowser/src/browser.ts:236 packages/logconsole-extension/src/index.tsx:376
 msgid "Error"
 msgstr "Fehler"
 
-#: packages/docmanager-extension/src/index.tsx:625 packages/docmanager-extension/src/index.tsx:647 packages/docmanager-extension/src/index.tsx:710 packages/docmanager-extension/src/index.tsx:732
+#: packages/docmanager-extension/src/index.tsx:704
+msgid "Open the provided `path`."
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:710 packages/docmanager-extension/src/index.tsx:732
 msgid "Reload %1 from Disk"
 msgstr "%1 von der Festplatte neu laden"
 
-#: packages/docmanager-extension/src/index.tsx:629 packages/docmanager-extension/src/index.tsx:714
+#: packages/docmanager-extension/src/index.tsx:714
 msgid "Reload contents from disk"
 msgstr "Inhalte von der Festplatte neu laden"
 
-#: packages/docmanager-extension/src/index.tsx:640 packages/docmanager-extension/src/index.tsx:725
+#: packages/docmanager-extension/src/index.tsx:725
 msgid "Cannot Reload"
 msgstr "Kann nicht neu laden"
 
-#: packages/docmanager-extension/src/index.tsx:648 packages/docmanager-extension/src/index.tsx:733
+#: packages/docmanager-extension/src/index.tsx:733
 msgid "Are you sure you want to reload the %1 from the disk?"
 msgstr "Sind Sie sicher, dass Sie die %1 von der Festplatte neu laden wollen?"
 
-#: packages/docmanager-extension/src/index.tsx:671
-msgid "Revert %1 to Checkpoint"
-msgstr "%1 auf Kontrollpunkt zurücksetzen"
+#: packages/docmanager-extension/src/index.tsx:756
+msgid "Revert %1 to Checkpoint…"
+msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:675 packages/docmanager-extension/src/index.tsx:760
+#: packages/docmanager-extension/src/index.tsx:760
 msgid "Revert contents to previous checkpoint"
 msgstr "Inhalt auf den vorherigen Kontrollpunkt zurücksetzen"
 
-#: packages/docmanager-extension/src/index.tsx:685 packages/docmanager-extension/src/index.tsx:770
+#: packages/docmanager-extension/src/index.tsx:770
 msgid "Cannot Revert"
 msgstr "Rückgängig machen nicht möglich"
 
-#: packages/docmanager-extension/src/index.tsx:700 packages/docmanager-extension/src/index.tsx:793
-msgid "Revert %1 to checkpoint"
-msgstr "%1 auf Kontrollpunkt zurücksetzen"
+#: packages/docmanager-extension/src/index.tsx:779
+msgid "No checkpoints"
+msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:704
-msgid "Open the provided `path`."
+#: packages/docmanager-extension/src/index.tsx:780
+msgid "No checkpoints are available for this %1."
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:704 packages/docmanager-extension/src/index.tsx:797 packages/docregistry/src/context.ts:805 packages/docregistry/src/context.ts:851 packages/docregistry/src/context.ts:869 packages/docregistry/src/context.ts:874 packages/docregistry/src/context.ts:892
+#: packages/docmanager-extension/src/index.tsx:793
+msgid "Revert %1 to checkpoint"
+msgstr "%1 auf Kontrollpunkt zurücksetzen"
+
+#: packages/docmanager-extension/src/index.tsx:797 packages/docregistry/src/context.ts:805
 msgid "Revert"
 msgstr "Zurücksetzen"
 
-#: packages/docmanager-extension/src/index.tsx:725 packages/docmanager-extension/src/index.tsx:820
+#: packages/docmanager-extension/src/index.tsx:820
 msgid "In collaborative mode, the document is saved automatically after every change"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:731 packages/docmanager-extension/src/index.tsx:826
+#: packages/docmanager-extension/src/index.tsx:826
 msgid "Save and create checkpoint"
 msgstr "Speichern und Kontrollpunkt erstellen"
 
-#: packages/docmanager-extension/src/index.tsx:737 packages/docmanager-extension/src/index.tsx:832
+#: packages/docmanager-extension/src/index.tsx:832
 msgid "Save %1"
 msgstr "%1 speichern"
 
-#: packages/docmanager-extension/src/index.tsx:748 packages/docmanager-extension/src/index.tsx:759 packages/docmanager-extension/src/index.tsx:843 packages/docmanager-extension/src/index.tsx:854 packages/docmanager-extension/src/index.tsx:872 packages/docmanager-extension/src/index.tsx:967 packages/notebook/src/default-toolbar.tsx:68
+#: packages/docmanager-extension/src/index.tsx:843 packages/docmanager-extension/src/index.tsx:854 packages/docmanager-extension/src/index.tsx:967 packages/notebook/src/default-toolbar.tsx:68
 msgid "Cannot Save"
 msgstr "Speichern nicht möglich"
 
-#: packages/docmanager-extension/src/index.tsx:756
-msgid "Revert %1 to Checkpoint…"
-msgstr ""
-
-#: packages/docmanager-extension/src/index.tsx:760 packages/docmanager-extension/src/index.tsx:855 packages/notebook/src/default-toolbar.tsx:69
+#: packages/docmanager-extension/src/index.tsx:855 packages/notebook/src/default-toolbar.tsx:69
 msgid "Document is read-only"
 msgstr "Dokument ist schreibgeschützt"
 
-#: packages/docmanager-extension/src/index.tsx:775 packages/docmanager-extension/src/index.tsx:870
+#: packages/docmanager-extension/src/index.tsx:870
 msgid "Rename file"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:776 packages/docmanager-extension/src/index.tsx:871 packages/docmanager/src/dialogs.ts:53 packages/docmanager/src/dialogs.ts:57 packages/filebrowser-extension/src/index.ts:1087 packages/filebrowser-extension/src/index.ts:1197
+#: packages/docmanager-extension/src/index.tsx:871 packages/docmanager/src/dialogs.ts:57 packages/filebrowser-extension/src/index.ts:1197
 msgid "Rename"
 msgstr "Umbenennen"
 
-#: packages/docmanager-extension/src/index.tsx:777 packages/docmanager-extension/src/index.tsx:872
+#: packages/docmanager-extension/src/index.tsx:872
 msgid "File name"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:779
-msgid "No checkpoints"
-msgstr ""
-
-#: packages/docmanager-extension/src/index.tsx:780
-msgid "No checkpoints are available for this %1."
-msgstr ""
-
-#: packages/docmanager-extension/src/index.tsx:781 packages/docmanager-extension/src/index.tsx:876 packages/docmanager/src/widgetmanager.ts:414 packages/docmanager/src/widgetmanager.ts:416
+#: packages/docmanager-extension/src/index.tsx:876 packages/docmanager/src/widgetmanager.ts:414
 msgid "Do not ask me again."
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:782 packages/docmanager-extension/src/index.tsx:877
+#: packages/docmanager-extension/src/index.tsx:877
 msgid "If checked, you will not be asked to rename future untitled files when saving them."
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:839 packages/docmanager-extension/src/index.tsx:934
+#: packages/docmanager-extension/src/index.tsx:934
 msgid "Save All"
 msgstr "Alles speichern"
 
-#: packages/docmanager-extension/src/index.tsx:840 packages/docmanager-extension/src/index.tsx:935
+#: packages/docmanager-extension/src/index.tsx:935
 msgid "Save all open documents"
 msgstr "Alle geöffneten Dokumente speichern"
 
-#: packages/docmanager-extension/src/index.tsx:863 packages/docmanager-extension/src/index.tsx:958
+#: packages/docmanager-extension/src/index.tsx:958
 msgid "Save %1 As…"
 msgstr "%1 speichern als …"
 
-#: packages/docmanager-extension/src/index.tsx:864 packages/docmanager-extension/src/index.tsx:959
+#: packages/docmanager-extension/src/index.tsx:959
 msgid "Save with new path"
 msgstr "Mit neuem Pfad speichern"
 
-#: packages/docmanager-extension/src/index.tsx:883 packages/docmanager-extension/src/index.tsx:904 packages/docmanager-extension/src/index.tsx:999
+#: packages/docmanager-extension/src/index.tsx:999
 msgid "Autosave Documents"
 msgstr "Dokumente automatisch speichern"
 
-#: packages/docmanager/src/dialogs.ts:112 packages/docmanager/src/dialogs.ts:114
+#: packages/docmanager/src/dialogs.ts:114
 msgid "Overwrite file?"
 msgstr "Datei überschreiben?"
 
-#: packages/docmanager/src/dialogs.ts:113 packages/docmanager/src/dialogs.ts:115
+#: packages/docmanager/src/dialogs.ts:115
 msgid "\"%1\" already exists, overwrite?"
 msgstr "\"%1\" existiert bereits, überschreiben?"
 
-#: packages/docmanager/src/dialogs.ts:116 packages/docmanager/src/dialogs.ts:118 packages/docregistry/src/context.ts:809 packages/docregistry/src/context.ts:845 packages/docregistry/src/context.ts:853 packages/docregistry/src/context.ts:865 packages/docregistry/src/context.ts:876 packages/docregistry/src/context.ts:887 packages/docregistry/src/context.ts:888 packages/docregistry/src/context.ts:898 packages/docregistry/src/context.ts:910 packages/docregistry/src/context.ts:921 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutInput.tsx:499 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231 packages/shortcuts-extension/src/components/ShortcutItem.tsx:254
+#: packages/docmanager/src/dialogs.ts:118 packages/docregistry/src/context.ts:809 packages/docregistry/src/context.ts:845 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231
 msgid "Overwrite"
 msgstr "Überschreiben"
 
-#: packages/docmanager/src/dialogs.ts:180 packages/docmanager/src/dialogs.ts:182
+#: packages/docmanager/src/dialogs.ts:182
 msgid "File Path"
 msgstr "Dateipfad"
 
-#: packages/docmanager/src/dialogs.ts:185 packages/docmanager/src/dialogs.ts:187
+#: packages/docmanager/src/dialogs.ts:187
 msgid "New Name"
 msgstr "Neuer Name"
 
-#: packages/docmanager/src/dialogs.ts:48 packages/docmanager/src/dialogs.ts:52
+#: packages/docmanager/src/dialogs.ts:52
 msgid "Rename File"
 msgstr "Datei umbenennen"
 
-#: packages/docmanager/src/dialogs.ts:61 packages/docmanager/src/dialogs.ts:65 packages/filebrowser/src/listing.ts:1527 packages/filebrowser/src/listing.ts:1875
+#: packages/docmanager/src/dialogs.ts:65 packages/filebrowser/src/listing.ts:1875
 msgid "Rename Error"
 msgstr "Fehler beim Umbenennen"
 
-#: packages/docmanager/src/dialogs.ts:63 packages/docmanager/src/dialogs.ts:67
+#: packages/docmanager/src/dialogs.ts:67
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr "\"%1\" ist kein gültiger Name für eine Datei. Namen müssen eine Länge größer Null haben und dürfen \"/\", \"\\\" und \":\" nicht enthalten"
 
 #: packages/docmanager/src/savingstatus.tsx:58
 msgid "Saving completed"
 msgstr "Speichern abgeschlossen"
 
@@ -4650,182 +4218,162 @@
 msgid "Last Saved: %1\n"
 msgstr "Zuletzt gespeichert: %1\n"
 
 #: packages/docmanager/src/widgetmanager.ts:306
 msgid "Last Checkpoint: %1"
 msgstr "Letzter Kontrollpunkt: %1"
 
-#: packages/docmanager/src/widgetmanager.ts:397 packages/docmanager/src/widgetmanager.ts:399
+#: packages/docmanager/src/widgetmanager.ts:397
 msgid "Close and save"
 msgstr "Schließen und speichern"
 
-#: packages/docmanager/src/widgetmanager.ts:404 packages/docmanager/src/widgetmanager.ts:406
+#: packages/docmanager/src/widgetmanager.ts:404
 msgid "Close without saving"
 msgstr "Schließen ohne zu speichern"
 
-#: packages/docmanager/src/widgetmanager.ts:409 packages/docmanager/src/widgetmanager.ts:411 packages/notebook/src/searchprovider.ts:499
+#: packages/docmanager/src/widgetmanager.ts:409 packages/notebook/src/searchprovider.ts:509
 msgid "Confirmation"
 msgstr "Bestätigung"
 
-#: packages/docmanager/src/widgetmanager.ts:410 packages/docmanager/src/widgetmanager.ts:412
+#: packages/docmanager/src/widgetmanager.ts:410
 msgid "Please confirm you want to close \"%1\"."
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:415 packages/docmanager/src/widgetmanager.ts:417
+#: packages/docmanager/src/widgetmanager.ts:415
 msgid "If checked, no confirmation to close a document will be asked in the future."
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:437 packages/docmanager/src/widgetmanager.ts:439
+#: packages/docmanager/src/widgetmanager.ts:437
 msgid "Save as"
 msgstr "Speichern unter"
 
-#: packages/docmanager/src/widgetmanager.ts:439 packages/docmanager/src/widgetmanager.ts:441
+#: packages/docmanager/src/widgetmanager.ts:439
 msgid "Save your work"
 msgstr "Speichere deine Arbeit"
 
-#: packages/docmanager/src/widgetmanager.ts:440 packages/docmanager/src/widgetmanager.ts:442
+#: packages/docmanager/src/widgetmanager.ts:440
 msgid "Save changes in \"%1\" before closing?"
 msgstr "Änderungen in „%1“ vor dem Schließen speichern?"
 
-#: packages/docmanager/src/widgetmanager.ts:443 packages/docmanager/src/widgetmanager.ts:445
+#: packages/docmanager/src/widgetmanager.ts:443
 msgid "Discard"
 msgstr "Verwerfen"
 
-#: packages/docprovider/src/yprovider.ts:131
-msgid "Session expired"
-msgstr "Sitzung abgelaufen"
-
-#: packages/docprovider/src/yprovider.ts:132
-msgid "The document session expired. You need to reload this browser tab."
-msgstr ""
-
 #: packages/docregistry/src/context.ts:1021
 msgid "Save File As…"
 msgstr "Datei speichern als…"
 
-#: packages/docregistry/src/context.ts:1037 packages/docregistry/src/context.ts:1103
-msgid "Save File As.."
-msgstr "Datei speichern als.."
-
-#: packages/docregistry/src/context.ts:631 packages/docregistry/src/context.ts:642 packages/docregistry/src/context.ts:665 packages/docregistry/src/context.ts:894 packages/docregistry/src/context.ts:958
+#: packages/docregistry/src/context.ts:631 packages/docregistry/src/context.ts:894
 msgid "File Save Error for %1"
 msgstr "Fehler beim Speichern der Datei für %1"
 
-#: packages/docregistry/src/context.ts:686 packages/docregistry/src/context.ts:695 packages/docregistry/src/context.ts:709 packages/docregistry/src/context.ts:744 packages/docregistry/src/context.ts:767
+#: packages/docregistry/src/context.ts:695
 msgid "File Load Error for %1"
 msgstr "Dateiladefehler für %1"
 
-#: packages/docregistry/src/context.ts:798 packages/docregistry/src/context.ts:845 packages/docregistry/src/context.ts:868
+#: packages/docregistry/src/context.ts:798
 msgid "\"%1\" has changed on disk since the last time it was opened or saved.\n"
 "Do you want to overwrite the file on disk with the version open here,\n"
 "or load the version on disk (revert)?"
 msgstr "\"%1\" hat sich seit dem letzten Öffnen oder Speichern auf der Festplatte geändert.\n"
 "Möchten Sie die Datei auf der Festplatte mit der hier geöffneten Version überschreiben,\n"
 "oder die Version auf der Festplatte laden (zurücksetzen)?"
 
-#: packages/docregistry/src/context.ts:814 packages/docregistry/src/context.ts:857 packages/docregistry/src/context.ts:880
+#: packages/docregistry/src/context.ts:814
 msgid "File Changed"
 msgstr "Datei geändert"
 
-#: packages/docregistry/src/context.ts:840 packages/docregistry/src/context.ts:882 packages/docregistry/src/context.ts:905
+#: packages/docregistry/src/context.ts:840
 msgid "\"%1\" already exists. Do you want to replace it?"
 msgstr "\"%1\" existiert bereits. Möchtest du es ersetzen?"
 
-#: packages/docregistry/src/context.ts:849 packages/docregistry/src/context.ts:890 packages/docregistry/src/context.ts:913
+#: packages/docregistry/src/context.ts:849
 msgid "File Overwrite?"
 msgstr "Datei überschreiben?"
 
-#: packages/docregistry/src/mimedocument.ts:174 packages/docregistry/src/mimedocument.ts:70 packages/markdownviewer/src/widget.ts:201 packages/markdownviewer/src/widget.ts:211
+#: packages/docregistry/src/mimedocument.ts:174 packages/docregistry/src/mimedocument.ts:70 packages/markdownviewer/src/widget.ts:211
 msgid "Renderer Failure: %1"
 msgstr "Renderer-Fehler: %1"
 
-#: packages/docregistry/src/registry.ts:1287 packages/docregistry/src/registry.ts:1352
+#: packages/docregistry/src/registry.ts:1287
 msgid "default"
 msgstr "Standard"
 
-#: packages/docregistry/src/registry.ts:1310 packages/docregistry/src/registry.ts:1375
+#: packages/docregistry/src/registry.ts:1310
 msgid "Text"
 msgstr "Text"
 
-#: packages/docregistry/src/registry.ts:1333 packages/docregistry/src/registry.ts:1398 packages/launcher/src/index.tsx:149 packages/launcher/src/index.tsx:154 packages/launcher/src/widget.tsx:115 packages/launcher/src/widget.tsx:120 packages/notebook-extension/src/index.ts:1210 packages/notebook-extension/src/index.ts:1482 packages/notebook-extension/src/index.ts:1519 packages/notebook-extension/src/index.ts:1902 packages/notebook-extension/src/index.ts:1938 packages/notebook-extension/src/index.ts:760
+#: packages/docregistry/src/registry.ts:1333 packages/launcher/src/widget.tsx:115 packages/launcher/src/widget.tsx:120 packages/notebook-extension/src/index.ts:1210 packages/notebook-extension/src/index.ts:1902 packages/notebook-extension/src/index.ts:1938
 msgid "Notebook"
 msgstr "Notebook"
 
-#: packages/docregistry/src/registry.ts:1358 packages/docregistry/src/registry.ts:1423
+#: packages/docregistry/src/registry.ts:1358
 msgid "Directory"
 msgstr "Verzeichnis"
 
-#: packages/docregistry/src/registry.ts:1385 packages/docregistry/src/registry.ts:1450 packages/fileeditor-extension/src/commands.ts:810 packages/fileeditor-extension/src/commands.ts:989
+#: packages/docregistry/src/registry.ts:1385 packages/fileeditor-extension/src/commands.ts:810
 msgid "Markdown File"
 msgstr "Markdown-Datei"
 
-#: packages/docregistry/src/registry.ts:1392 packages/docregistry/src/registry.ts:1457
+#: packages/docregistry/src/registry.ts:1392
 msgid "PDF File"
 msgstr "PDF-Datei"
 
-#: packages/docregistry/src/registry.ts:1399 packages/docregistry/src/registry.ts:1464 packages/fileeditor-extension/src/index.ts:209 packages/fileeditor-extension/src/index.ts:329
+#: packages/docregistry/src/registry.ts:1399 packages/fileeditor-extension/src/index.ts:329
 msgid "Python File"
 msgstr "Python-Datei"
 
-#: packages/docregistry/src/registry.ts:1406 packages/docregistry/src/registry.ts:1471
+#: packages/docregistry/src/registry.ts:1406
 msgid "JSON File"
 msgstr "JSON-Datei"
 
-#: packages/docregistry/src/registry.ts:1413 packages/docregistry/src/registry.ts:1478 packages/fileeditor-extension/src/index.ts:221 packages/fileeditor-extension/src/index.ts:341
+#: packages/docregistry/src/registry.ts:1413 packages/fileeditor-extension/src/index.ts:341
 msgid "Julia File"
 msgstr "Julia-Datei"
 
-#: packages/docregistry/src/registry.ts:1420 packages/docregistry/src/registry.ts:1485
+#: packages/docregistry/src/registry.ts:1420
 msgid "CSV File"
 msgstr "CSV-Datei"
 
-#: packages/docregistry/src/registry.ts:1427 packages/docregistry/src/registry.ts:1492
+#: packages/docregistry/src/registry.ts:1427
 msgid "TSV File"
 msgstr "TSV-Datei"
 
-#: packages/docregistry/src/registry.ts:1434 packages/docregistry/src/registry.ts:1499 packages/fileeditor-extension/src/index.ts:233 packages/fileeditor-extension/src/index.ts:353
+#: packages/docregistry/src/registry.ts:1434 packages/fileeditor-extension/src/index.ts:353
 msgid "R File"
 msgstr "R-Datei"
 
-#: packages/docregistry/src/registry.ts:1441 packages/docregistry/src/registry.ts:1506
+#: packages/docregistry/src/registry.ts:1441
 msgid "YAML File"
 msgstr "YAML-Datei"
 
-#: packages/docregistry/src/registry.ts:1448 packages/docregistry/src/registry.ts:1456 packages/docregistry/src/registry.ts:1464 packages/docregistry/src/registry.ts:1472 packages/docregistry/src/registry.ts:1480 packages/docregistry/src/registry.ts:1488 packages/docregistry/src/registry.ts:1496 packages/docregistry/src/registry.ts:1513 packages/docregistry/src/registry.ts:1521 packages/docregistry/src/registry.ts:1529 packages/docregistry/src/registry.ts:1537 packages/docregistry/src/registry.ts:1545 packages/docregistry/src/registry.ts:1553 packages/docregistry/src/registry.ts:1561 packages/imageviewer-extension/src/index.ts:119
+#: packages/docregistry/src/registry.ts:1448 packages/docregistry/src/registry.ts:1456 packages/docregistry/src/registry.ts:1464 packages/docregistry/src/registry.ts:1472 packages/docregistry/src/registry.ts:1480 packages/docregistry/src/registry.ts:1488 packages/docregistry/src/registry.ts:1496 packages/imageviewer-extension/src/index.ts:119
 msgid "Image"
 msgstr "Bild"
 
-#: packages/documentsearch-extension/src/index.ts:183 packages/documentsearch-extension/src/index.ts:248
+#: packages/documentsearch-extension/src/index.ts:229 packages/fileeditor-extension/src/commands.ts:525
+msgid "Find…"
+msgstr "Suchen…"
+
+#: packages/documentsearch-extension/src/index.ts:248
 msgid "Find and Replace…"
 msgstr "Suchen und Ersetzen…"
 
-#: packages/documentsearch-extension/src/index.ts:203 packages/documentsearch-extension/src/index.ts:272
+#: packages/documentsearch-extension/src/index.ts:272
 msgid "Find Next"
 msgstr "Finde Nächste"
 
-#: packages/documentsearch-extension/src/index.ts:227 packages/documentsearch-extension/src/index.ts:287
+#: packages/documentsearch-extension/src/index.ts:287
 msgid "Find Previous"
 msgstr "Finde Vorherige"
 
 #: packages/documentsearch-extension/src/index.ts:302
 msgid "End Search"
 msgstr ""
 
-#: packages/documentsearch/src/searchoverlay.tsx:203 packages/documentsearch/src/searchview.tsx:260
-msgid "Replace All"
-msgstr "Alle ersetzen"
-
-#: packages/documentsearch/src/searchoverlay.tsx:321 packages/notebook/src/searchprovider.ts:222
-msgid "Search Cell Outputs"
-msgstr "Suche Zellausgaben"
-
-#: packages/documentsearch/src/searchoverlay.tsx:338
-msgid "Search Selected Cell(s)"
-msgstr "Ausgewählte Zelle(n) suchen"
-
 #: packages/documentsearch/src/searchview.tsx:169
 msgid "Match Case"
 msgstr ""
 
 #: packages/documentsearch/src/searchview.tsx:177
 msgid "Match Whole Word"
 msgstr ""
@@ -4834,14 +4382,18 @@
 msgid "Use Regular Expression"
 msgstr ""
 
 #: packages/documentsearch/src/searchview.tsx:230
 msgid "Preserve Case"
 msgstr ""
 
+#: packages/documentsearch/src/searchview.tsx:260
+msgid "Replace All"
+msgstr "Alle ersetzen"
+
 #: packages/documentsearch/src/searchview.tsx:280
 msgid "Previous Match"
 msgstr ""
 
 #: packages/documentsearch/src/searchview.tsx:291
 msgid "Next Match"
 msgstr ""
@@ -4854,105 +4406,57 @@
 msgid "Show Search Filters"
 msgstr "Suchfilter anzeigen"
 
 #: packages/documentsearch/src/searchview.tsx:637
 msgid "Toggle Replace"
 msgstr "Ersetzen umschalten"
 
-#: packages/extensionmanager-extension/src/index.ts:107 packages/extensionmanager-extension/src/index.ts:141
-msgid "Enable Extension Manager"
-msgstr "Erweiterungsmanager aktivieren"
-
-#: packages/extensionmanager-extension/src/index.ts:117 packages/extensionmanager-extension/src/index.ts:131 packages/extensionmanager-extension/src/index.ts:153 packages/extensionmanager-extension/src/index.ts:56 packages/extensionmanager-extension/src/index.ts:59
+#: packages/extensionmanager-extension/src/index.ts:131 packages/extensionmanager-extension/src/index.ts:153 packages/extensionmanager-extension/src/index.ts:59
 msgid "Extension Manager"
 msgstr "Erweiterungsmanager"
 
-#: packages/extensionmanager-extension/src/index.ts:143 packages/extensionmanager-extension/src/index.ts:177
+#: packages/extensionmanager-extension/src/index.ts:141
+msgid "Enable Extension Manager"
+msgstr "Erweiterungsmanager aktivieren"
+
+#: packages/extensionmanager-extension/src/index.ts:177
 msgid "Enable Extension Manager?"
 msgstr "Erweiterungsmanager aktivieren?"
 
-#: packages/extensionmanager-extension/src/index.ts:144 packages/extensionmanager-extension/src/index.ts:178
+#: packages/extensionmanager-extension/src/index.ts:178
 msgid "Thanks for trying out JupyterLab's extension manager.\n"
 "The JupyterLab development team is excited to have a robust\n"
 "third-party extension community.\n"
 "However, we cannot vouch for every extension,\n"
 "and some may introduce security risks.\n"
 "Do you want to continue?"
 msgstr "Danke, dass du den Erweiterungsmanager von JupyterLab ausprobierst.\n"
 "Das JupyterLab Entwicklungsteam freut sich über eine robuste\n"
 "Drittanbieter-Erweiterungsgemeinschaft.\n"
 "Wir können jedoch nicht für jede Erweiterung bürgen,\n"
 "und einige können Sicherheitsrisiken mit sich bringen.\n"
 "Möchten Sie fortfahren?"
 
-#: packages/extensionmanager-extension/src/index.ts:151 packages/extensionmanager-extension/src/index.ts:185 packages/extensionmanager/src/widget.tsx:161 packages/extensionmanager/src/widget.tsx:329 packages/extensionmanager/src/widget.tsx:807
+#: packages/extensionmanager-extension/src/index.ts:185 packages/extensionmanager/src/widget.tsx:161
 msgid "Disable"
 msgstr "Deaktivieren"
 
-#: packages/extensionmanager-extension/src/index.ts:152 packages/extensionmanager-extension/src/index.ts:186 packages/extensionmanager/src/widget.tsx:170 packages/extensionmanager/src/widget.tsx:338 packages/extensionmanager/src/widget.tsx:822
+#: packages/extensionmanager-extension/src/index.ts:186 packages/extensionmanager/src/widget.tsx:170
 msgid "Enable"
 msgstr "Aktivieren"
 
-#: packages/extensionmanager-extension/src/index.ts:61 packages/extensionmanager-extension/src/index.ts:68 packages/extensionmanager-extension/src/index.ts:89
+#: packages/extensionmanager-extension/src/index.ts:61
 msgid "Extension Manager section"
 msgstr "Abschnitt des Extension Manager"
 
-#: packages/extensionmanager/src/companions.tsx:137
-msgid "This package has indicated that it needs a corresponding server\n"
-"extension. Please contact your Administrator to update the server with\n"
-"one of the following commands:"
-msgstr ""
-
-#: packages/extensionmanager/src/companions.tsx:153
-msgid "This package has indicated that it needs a corresponding package for the kernel."
-msgstr "Dieses Paket hat angegeben, dass es ein entsprechendes Paket für den Kernel benötigt."
-
-#: packages/extensionmanager/src/companions.tsx:161
-msgid "The package <code>%1</code>, is required by the following kernels:"
-msgstr "Das Paket <code>%1</code> wird von den folgenden Kerneln benötigt:"
-
-#: packages/extensionmanager/src/companions.tsx:178
-msgid "This package has indicated that it needs a corresponding kernel\n"
-"package. Please contact your Administrator to update the server with\n"
-"one of the following commands:"
-msgstr "Dieses Paket hat angedeutet, dass es ein entsprechendes Kernel-Paket\n"
-"benötigt. Bitte kontaktiere deinen Administrator, um den Server mit\n"
-"einem der folgenden Befehle zu aktualisieren:"
-
-#: packages/extensionmanager/src/companions.tsx:196
-msgid "You should make sure that the indicated packages are installed before\n"
-"trying to use the extension. Do you want to continue with the extension\n"
-"installation?"
-msgstr "Du solltest sicherstellen, dass die angegebenen Pakete installiert sind, bevor du versuchst, die Erweiterung zu verwenden. Möchtest du mit der Installation der Erweiterung fortfahren?"
-
-#: packages/extensionmanager/src/companions.tsx:206
-msgid "Kernel and Server Companions"
-msgstr ""
-
-#: packages/extensionmanager/src/companions.tsx:208
-msgid "Kernel Companions"
-msgstr ""
-
-#: packages/extensionmanager/src/companions.tsx:210
-msgid "Server Companion"
-msgstr "Server-Begleiter"
-
-#: packages/extensionmanager/src/companions.tsx:219
-msgid "Install the JupyterLab extension."
-msgstr "Installiere die JupyterLab Erweiterung."
-
-#: packages/extensionmanager/src/dialog.tsx:23
-msgid "An error occurred installing <code>%1</code>."
-msgstr "Beim Installieren von <code>%1</code> ist ein Fehler aufgetreten."
-
-#: packages/extensionmanager/src/dialog.tsx:27 packages/extensionmanager/src/dialog.tsx:29
+#: packages/extensionmanager/src/dialog.tsx:27
 msgid "Error message:"
 msgstr "Fehlermeldung:"
 
-#: packages/extensionmanager/src/dialog.tsx:35 packages/extensionmanager/src/dialog.tsx:37
+#: packages/extensionmanager/src/dialog.tsx:35
 msgid "Extension Installation Error"
 msgstr "Fehler bei der Installation der Erweiterung"
 
 #: packages/extensionmanager/src/model.ts:505
 msgid "You will need to restart JupyterLab to apply the changes."
 msgstr ""
 
@@ -4980,35 +4484,23 @@
 msgid "This extension is approved by your security team."
 msgstr ""
 
 #: packages/extensionmanager/src/widget.tsx:133
 msgid "Update \"%1\" to \"%2\""
 msgstr "„%1“ auf „%2“ aktualisieren"
 
-#: packages/extensionmanager/src/widget.tsx:135
-msgid "A build is needed to include the latest changes"
-msgstr "Ein Build wird benötigt, um die neuesten Änderungen einzubinden"
-
-#: packages/extensionmanager/src/widget.tsx:138
-msgid "Rebuild"
-msgstr ""
-
-#: packages/extensionmanager/src/widget.tsx:141
-msgid "Ignore"
-msgstr "Ignorieren"
-
 #: packages/extensionmanager/src/widget.tsx:141
 msgid "Update to %1"
 msgstr "Auf %1 aktualisieren"
 
 #: packages/extensionmanager/src/widget.tsx:146
 msgid "Uninstall \"%1\""
 msgstr "„%1“ deinstallieren"
 
-#: packages/extensionmanager/src/widget.tsx:150 packages/extensionmanager/src/widget.tsx:320
+#: packages/extensionmanager/src/widget.tsx:150
 msgid "Uninstall"
 msgstr "Deinstallieren"
 
 #: packages/extensionmanager/src/widget.tsx:157
 msgid "Disable \"%1\""
 msgstr "„%1“ deaktivieren"
 
@@ -5016,82 +4508,52 @@
 msgid "Enable \"%1\""
 msgstr "„%1“ aktivieren"
 
 #: packages/extensionmanager/src/widget.tsx:178
 msgid "Install \"%1\""
 msgstr "„%1“ installieren"
 
-#: packages/extensionmanager/src/widget.tsx:182 packages/extensionmanager/src/widget.tsx:298
+#: packages/extensionmanager/src/widget.tsx:182
 msgid "Install"
 msgstr "Installieren"
 
-#: packages/extensionmanager/src/widget.tsx:193
-msgid "%1 (Developed by Project Jupyter)"
-msgstr "%1 (Entwickelt vom Projekt Jupyter)"
-
-#: packages/extensionmanager/src/widget.tsx:247
-msgid "%1 extension has been blockedExtensions since install. Please uninstall immediately and contact your blockedExtensions administrator."
-msgstr ""
-
-#: packages/extensionmanager/src/widget.tsx:251 packages/extensionmanager/src/widget.tsx:491
+#: packages/extensionmanager/src/widget.tsx:251
 msgid "No entries"
 msgstr "Keine Einträge"
 
-#: packages/extensionmanager/src/widget.tsx:263
-msgid "%1 extension has been removed from the allowedExtensions since installation. Please uninstall immediately and contact your allowedExtensions administrator."
-msgstr ""
-
-#: packages/extensionmanager/src/widget.tsx:311
-msgid "Update"
-msgstr "Aktualisieren"
-
 #: packages/extensionmanager/src/widget.tsx:350
 msgid "%1 Manager"
 msgstr ""
 
 #: packages/extensionmanager/src/widget.tsx:355
 msgid "Extension installation path: %1"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:363 packages/shortcuts-extension/src/components/TopNav.tsx:258
+#: packages/extensionmanager/src/widget.tsx:363
 msgid "Search"
 msgstr "Suchen"
 
-#: packages/extensionmanager/src/widget.tsx:365
-msgid "About"
-msgstr "Über"
-
 #: packages/extensionmanager/src/widget.tsx:379
 msgid "Error when performing an action."
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:380 packages/extensionmanager/src/widget.tsx:844
+#: packages/extensionmanager/src/widget.tsx:380
 msgid "Reason given:"
 msgstr "Angegebener Grund:"
 
-#: packages/extensionmanager/src/widget.tsx:384
-msgid "This is a prebuilt extension. To uninstall it, please\n"
-"    apply following instructions."
-msgstr ""
-
-#: packages/extensionmanager/src/widget.tsx:394
-msgid "This is a prebuilt extension. To uninstall it, please\n"
-"    read the user guide on:"
-msgstr ""
-
 #: packages/extensionmanager/src/widget.tsx:400
 msgid "The JupyterLab development team is excited to have a robust\n"
 "third-party extension community. However, we do not review\n"
 "third-party extensions, and some extensions may introduce security\n"
 "risks or contain malicious code that runs on your machine. Moreover in order\n"
 "to work, this panel needs to fetch data from web services. Do you agree to\n"
 "activate this feature?"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:413 packages/extensionmanager/src/widget.tsx:792
+#: packages/extensionmanager/src/widget.tsx:413
 msgid "Please read the privacy policy."
 msgstr ""
 
 #: packages/extensionmanager/src/widget.tsx:422
 msgid "This will withdraw your consent."
 msgstr ""
 
@@ -5103,362 +4565,314 @@
 msgid "No, disable"
 msgstr ""
 
 #: packages/extensionmanager/src/widget.tsx:471 packages/extensionmanager/src/widget.tsx:565
 msgid "Updating extensions list…"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:591 packages/extensionmanager/src/widget.tsx:952
+#: packages/extensionmanager/src/widget.tsx:591
 msgid "Search Results"
 msgstr "Suchergebnisse"
 
-#: packages/extensionmanager/src/widget.tsx:592 packages/extensionmanager/src/widget.tsx:953
+#: packages/extensionmanager/src/widget.tsx:592
 msgid "Discover"
 msgstr "Entdecken"
 
-#: packages/extensionmanager/src/widget.tsx:617 packages/extensionmanager/src/widget.tsx:776 packages/logconsole-extension/src/index.tsx:382 packages/logconsole-extension/src/index.tsx:393 packages/settingeditor/src/settingseditor.tsx:117 packages/settingeditor/src/settingseditor.tsx:122 packages/settingeditor/src/settingseditor.tsx:129 packages/settingeditor/src/settingseditor.tsx:134
+#: packages/extensionmanager/src/widget.tsx:617 packages/logconsole-extension/src/index.tsx:377 packages/settingeditor/src/settingseditor.tsx:122 packages/settingeditor/src/settingseditor.tsx:134
 msgid "Warning"
 msgstr "Warnung"
 
-#: packages/extensionmanager/src/widget.tsx:623 packages/extensionmanager/src/widget.tsx:899
+#: packages/extensionmanager/src/widget.tsx:623
 msgid "Installed"
 msgstr "Installiert"
 
 #: packages/extensionmanager/src/widget.tsx:636
 msgid "Refresh extensions list"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:722
-msgid "The extension manager is disabled. Please contact your system\n"
-"administrator to verify the listings configuration."
-msgstr ""
-
-#: packages/extensionmanager/src/widget.tsx:732
-msgid "Read more in the JupyterLab documentation."
-msgstr ""
-
-#: packages/extensionmanager/src/widget.tsx:780
-msgid "The JupyterLab development team is excited to have a robust\n"
-"third-party extension community. However, we do not review\n"
-"third-party extensions, and some extensions may introduce security\n"
-"risks or contain malicious code that runs on your machine. Moreover in order\n"
-"to work, this panel needs to fetch data from web services."
-msgstr ""
-
 #: packages/extensionmanager/src/widget.tsx:81
 msgid "%1 extension home page"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:832
-msgid "Updating extensions list"
-msgstr ""
-
-#: packages/extensionmanager/src/widget.tsx:839
-msgid "Error communicating with server extension. Consult the documentation\n"
-"            for how to ensure that it is enabled."
-msgstr ""
-
-#: packages/extensionmanager/src/widget.tsx:852
-msgid "The server has some missing requirements for installing extensions."
-msgstr ""
-
-#: packages/extensionmanager/src/widget.tsx:857
-msgid "Details:"
-msgstr ""
-
 #: packages/extensionmanager/src/widget.tsx:90
 msgid "Version: %1"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:907
-msgid "Refresh extension list"
-msgstr "Erweiterungsliste aktualisieren"
-
 #: packages/extensionmanager/src/widget.tsx:97
 msgid "%1 extension is not allowed anymore. Please uninstall it immediately or contact your administrator."
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1012 packages/filebrowser-extension/src/index.ts:1028 packages/filebrowser-extension/src/index.ts:1117 packages/filebrowser-extension/src/index.ts:747 packages/filebrowser-extension/src/index.ts:849 packages/filebrowser-extension/src/index.ts:926
-msgid "Open"
-msgstr "Öffnen"
+#: packages/filebrowser-extension/src/index.ts:1014
+msgid "Open from Path…"
+msgstr "Von Pfad öffnen …"
 
-#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:735 packages/filebrowser-extension/src/index.ts:737 packages/filebrowser-extension/src/index.ts:837 packages/filebrowser-extension/src/index.ts:839 packages/filebrowser-extension/src/index.ts:912 packages/filebrowser-extension/src/index.ts:914
+#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:837 packages/filebrowser-extension/src/index.ts:839
 msgid "Open %1"
 msgstr "%1 öffnen"
 
-#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:912
-msgid "Open from Path…"
-msgstr "Von Pfad öffnen …"
-
-#: packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:914
+#: packages/filebrowser-extension/src/index.ts:1016
 msgid "Open from path"
 msgstr "Von Pfad öffnen"
 
-#: packages/filebrowser-extension/src/index.ts:1025 packages/filebrowser-extension/src/index.ts:1130 packages/fileeditor-extension/src/commands.ts:866 packages/fileeditor-extension/src/commands.ts:974 packages/terminal-extension/src/index.ts:488 packages/terminal-extension/src/index.ts:512
-msgid "Paste"
-msgstr "Einfügen"
-
-#: packages/filebrowser-extension/src/index.ts:1025 packages/filebrowser-extension/src/index.ts:923
+#: packages/filebrowser-extension/src/index.ts:1025
 msgid "Path"
 msgstr "Pfad"
 
-#: packages/filebrowser-extension/src/index.ts:1027 packages/filebrowser-extension/src/index.ts:925
+#: packages/filebrowser-extension/src/index.ts:1027
 msgid "Open Path"
 msgstr "Pfad öffnen"
 
-#: packages/filebrowser-extension/src/index.ts:1038 packages/filebrowser-extension/src/index.ts:1143 packages/filebrowser/src/opendialog.ts:153 packages/filebrowser/src/opendialog.ts:156
+#: packages/filebrowser-extension/src/index.ts:1028 packages/filebrowser-extension/src/index.ts:1117 packages/filebrowser-extension/src/index.ts:849
+msgid "Open"
+msgstr "Öffnen"
+
+#: packages/filebrowser-extension/src/index.ts:1063
+msgid "Could not find path: %1"
+msgstr "Pfad konnte nicht gefunden werden: %1"
+
+#: packages/filebrowser-extension/src/index.ts:1065
+msgid "Cannot open"
+msgstr "Kann nicht geöffnet werden"
+
+#: packages/filebrowser-extension/src/index.ts:1130 packages/fileeditor-extension/src/commands.ts:974 packages/terminal-extension/src/index.ts:488
+msgid "Paste"
+msgstr "Einfügen"
+
+#: packages/filebrowser-extension/src/index.ts:1143 packages/filebrowser/src/opendialog.ts:153
 msgid "New Folder"
 msgstr "Neuer Ordner"
 
-#: packages/filebrowser-extension/src/index.ts:1050 packages/filebrowser-extension/src/index.ts:1155
+#: packages/filebrowser-extension/src/index.ts:1155
 msgid "New File"
 msgstr "Neue Datei"
 
-#: packages/filebrowser-extension/src/index.ts:1062 packages/filebrowser-extension/src/index.ts:1167 packages/fileeditor-extension/src/commands.ts:809 packages/fileeditor-extension/src/commands.ts:988
+#: packages/filebrowser-extension/src/index.ts:1167 packages/fileeditor-extension/src/commands.ts:809
 msgid "New Markdown File"
 msgstr "Neue Markdown-Datei"
 
-#: packages/filebrowser-extension/src/index.ts:1063 packages/filebrowser-extension/src/index.ts:957
-msgid "Could not find path: %1"
-msgstr "Pfad konnte nicht gefunden werden: %1"
-
-#: packages/filebrowser-extension/src/index.ts:1065 packages/filebrowser-extension/src/index.ts:959
-msgid "Cannot open"
-msgstr "Kann nicht geöffnet werden"
-
-#: packages/filebrowser-extension/src/index.ts:1074 packages/filebrowser-extension/src/index.ts:1179
+#: packages/filebrowser-extension/src/index.ts:1179
 msgid "Refresh the file browser."
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1075 packages/filebrowser-extension/src/index.ts:1180 packages/filebrowser/src/opendialog.ts:168 packages/filebrowser/src/opendialog.ts:171
+#: packages/filebrowser-extension/src/index.ts:1180 packages/filebrowser/src/opendialog.ts:168
 msgid "Refresh File List"
 msgstr "Dateiliste aktualisieren"
 
-#: packages/filebrowser-extension/src/index.ts:1108 packages/filebrowser-extension/src/index.ts:1220
+#: packages/filebrowser-extension/src/index.ts:1220
 msgid "Copy Path"
 msgstr "Pfad kopieren"
 
-#: packages/filebrowser-extension/src/index.ts:1120 packages/filebrowser-extension/src/index.ts:1232 packages/mainmenu-extension/src/index.ts:531 packages/mainmenu-extension/src/index.ts:536 packages/notebook-extension/src/index.ts:2332 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66
+#: packages/filebrowser-extension/src/index.ts:1232 packages/mainmenu-extension/src/index.ts:531 packages/notebook-extension/src/index.ts:2332 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66
 msgid "Shut Down Kernel"
 msgstr "Kernel herunterfahren"
 
-#: packages/filebrowser-extension/src/index.ts:1134 packages/launcher-extension/src/index.ts:59 packages/launcher-extension/src/index.ts:72 packages/ui-components/src/icon/widgets/tabbarsvg.ts:29 packages/ui-components/src/icon/widgets/tabbarsvg.ts:31
-msgid "New Launcher"
-msgstr "Neuer Launcher"
-
-#: packages/filebrowser-extension/src/index.ts:1145 packages/filebrowser-extension/src/index.ts:550
-msgid "Show Active File in File Browser"
-msgstr "Aktive Datei im Dateibrowser anzeigen"
-
-#: packages/filebrowser-extension/src/index.ts:1160 packages/filebrowser-extension/src/index.ts:1236
+#: packages/filebrowser-extension/src/index.ts:1236
 msgid "Show Last Modified Column"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1176 packages/filebrowser-extension/src/index.ts:1268
-msgid "Show Hidden Files"
-msgstr "Versteckte Dateien anzeigen"
-
-#: packages/filebrowser-extension/src/index.ts:1193 packages/filebrowser-extension/src/index.ts:1301
-msgid "Search on File Names"
-msgstr "Suche nach Dateinamen"
-
 #: packages/filebrowser-extension/src/index.ts:1252
 msgid "Show File Size Column"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1272 packages/filebrowser-extension/src/index.ts:1370
-msgid "No browser for path"
-msgstr "Kein Browser für den Pfad"
+#: packages/filebrowser-extension/src/index.ts:1268
+msgid "Show Hidden Files"
+msgstr "Versteckte Dateien anzeigen"
 
 #: packages/filebrowser-extension/src/index.ts:1285
 msgid "Show File Checkboxes"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:196 packages/filebrowser-extension/src/index.ts:443
-msgid "File Browser (%1)"
-msgstr "Dateibrowser (%1)"
+#: packages/filebrowser-extension/src/index.ts:1301
+msgid "Search on File Names"
+msgstr "Suche nach Dateinamen"
 
-#: packages/filebrowser-extension/src/index.ts:198 packages/filebrowser-extension/src/index.ts:445 packages/filebrowser-extension/src/index.ts:497 packages/filebrowser/src/browser.ts:75
-msgid "File Browser"
-msgstr "Dateibrowser"
+#: packages/filebrowser-extension/src/index.ts:1370
+msgid "No browser for path"
+msgstr "Kein Browser für den Pfad"
 
-#: packages/filebrowser-extension/src/index.ts:360 packages/filebrowser-extension/src/index.ts:389
+#: packages/filebrowser-extension/src/index.ts:389
 msgid "Copy Download Link"
 msgstr "Link zum Herunterladen kopieren"
 
-#: packages/filebrowser-extension/src/index.ts:396 packages/filebrowser-extension/src/index.ts:432
+#: packages/filebrowser-extension/src/index.ts:432
 msgid "File Browser Section"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:475 packages/filebrowser/src/browser.ts:101 packages/filebrowser/src/browser.ts:178
+#: packages/filebrowser-extension/src/index.ts:443
+msgid "File Browser (%1)"
+msgstr "Dateibrowser (%1)"
+
+#: packages/filebrowser-extension/src/index.ts:445 packages/filebrowser-extension/src/index.ts:497 packages/filebrowser/src/browser.ts:75
+msgid "File Browser"
+msgstr "Dateibrowser"
+
+#: packages/filebrowser-extension/src/index.ts:475
 msgid "Filter files by name"
 msgstr "Dateien nach Namen filtern"
 
 #: packages/filebrowser-extension/src/index.ts:508
 msgid "Open the file browser for the provided `path`."
 msgstr ""
 
 #: packages/filebrowser-extension/src/index.ts:540
 msgid "Hide the file browser."
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:549 packages/filebrowser-extension/src/index.ts:647
+#: packages/filebrowser-extension/src/index.ts:550
+msgid "Show Active File in File Browser"
+msgstr "Aktive Datei im Dateibrowser anzeigen"
+
+#: packages/filebrowser-extension/src/index.ts:647
 msgid "Copy Shareable Link"
 msgstr "Teilbarer Link kopieren"
 
-#: packages/filebrowser-extension/src/index.ts:670 packages/filebrowser-extension/src/index.ts:771
+#: packages/filebrowser-extension/src/index.ts:771
 msgid "Open in Simple Mode"
 msgstr "Im einfachen Modus öffnen"
 
-#: packages/filebrowser-extension/src/index.ts:735 packages/filebrowser-extension/src/index.ts:837
+#: packages/filebrowser-extension/src/index.ts:837
 msgid "Open from URL…"
 msgstr "Von URL öffnen…"
 
-#: packages/filebrowser-extension/src/index.ts:737 packages/filebrowser-extension/src/index.ts:839
+#: packages/filebrowser-extension/src/index.ts:839
 msgid "Open from URL"
 msgstr "Von URL öffnen"
 
-#: packages/filebrowser-extension/src/index.ts:744 packages/filebrowser-extension/src/index.ts:846
+#: packages/filebrowser-extension/src/index.ts:846
 msgid "URL"
 msgstr "URL"
 
-#: packages/filebrowser-extension/src/index.ts:746 packages/filebrowser-extension/src/index.ts:848
+#: packages/filebrowser-extension/src/index.ts:848
 msgid "Open URL"
 msgstr "URL öffnen"
 
-#: packages/filebrowser-extension/src/index.ts:765 packages/filebrowser-extension/src/index.ts:867
+#: packages/filebrowser-extension/src/index.ts:867
 msgid "Could not open URL: %1"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:767 packages/filebrowser-extension/src/index.ts:869
+#: packages/filebrowser-extension/src/index.ts:869
 msgid "Cannot fetch"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:780 packages/filebrowser-extension/src/index.ts:882 packages/filebrowser/src/upload.ts:51 packages/filebrowser/src/upload.ts:52
+#: packages/filebrowser-extension/src/index.ts:882 packages/filebrowser/src/upload.ts:52
 msgctxt "showErrorMessage"
 msgid "Upload Error"
 msgstr "Upload fehlgeschlagen"
 
-#: packages/filebrowser-extension/src/index.ts:832 packages/filebrowser-extension/src/index.ts:935 packages/fileeditor-extension/src/commands.ts:832 packages/fileeditor-extension/src/commands.ts:947 packages/terminal-extension/src/index.ts:463 packages/terminal-extension/src/index.ts:475
+#: packages/filebrowser-extension/src/index.ts:935 packages/fileeditor-extension/src/commands.ts:947 packages/terminal-extension/src/index.ts:463
 msgid "Copy"
 msgstr "Kopieren"
 
-#: packages/filebrowser-extension/src/index.ts:845 packages/filebrowser-extension/src/index.ts:948 packages/fileeditor-extension/src/commands.ts:791 packages/fileeditor-extension/src/commands.ts:913
+#: packages/filebrowser-extension/src/index.ts:948 packages/fileeditor-extension/src/commands.ts:913
 msgid "Cut"
 msgstr "Ausschneiden"
 
-#: packages/filebrowser-extension/src/index.ts:857 packages/filebrowser-extension/src/index.ts:960
+#: packages/filebrowser-extension/src/index.ts:960
 msgid "Duplicate"
 msgstr "Duplizieren"
 
 #: packages/filebrowser-extension/src/index.ts:964
 msgid "Update the file browser to display the provided `path`."
 msgstr ""
 
-#: packages/filebrowser/src/browser.ts:372 packages/filebrowser/src/browser.ts:400
+#: packages/filebrowser/src/browser.ts:372
 msgid "Directory not found"
 msgstr "Verzeichnis nicht gefunden"
 
-#: packages/filebrowser/src/browser.ts:373 packages/filebrowser/src/browser.ts:401 packages/filebrowser/src/model.ts:298 packages/filebrowser/src/model.ts:305
+#: packages/filebrowser/src/browser.ts:373 packages/filebrowser/src/model.ts:298
 msgid "Directory not found: \"%1\""
 msgstr "Verzeichnis nicht gefunden: \"%1\""
 
-#: packages/filebrowser/src/browser.ts:69 packages/filebrowser/src/browser.ts:81
+#: packages/filebrowser/src/browser.ts:69
 msgid "file browser"
 msgstr "Dateibrowser"
 
 #: packages/filebrowser/src/crumbs.ts:175 packages/filebrowser/src/crumbs.ts:194
 msgid "Open Error"
 msgstr "Fehler beim Öffnen"
 
 #: packages/filebrowser/src/crumbs.ts:302
 msgid "Move Error"
 msgstr "Fehler beim Verschieben"
 
-#: packages/filebrowser/src/listing.ts:1015 packages/filebrowser/src/listing.ts:1120
+#: packages/filebrowser/src/listing.ts:1120
 msgctxt "showErrorMessage"
 msgid "Open directory"
 msgstr "Verzeichnis öffnen"
 
-#: packages/filebrowser/src/listing.ts:1136 packages/filebrowser/src/listing.ts:1395
+#: packages/filebrowser/src/listing.ts:1395
 msgid "Error Uploading Folder"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:1137 packages/filebrowser/src/listing.ts:1396
+#: packages/filebrowser/src/listing.ts:1396
 msgid "Drag and Drop is currently not supported for folders"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:1256 packages/filebrowser/src/listing.ts:1515
+#: packages/filebrowser/src/listing.ts:1515
 msgctxt "showErrorMessage"
 msgid "Error while copying/moving files"
 msgstr "Fehler beim Kopieren/Verschieben von Dateien"
 
-#: packages/filebrowser/src/listing.ts:1495 packages/filebrowser/src/listing.ts:1814
+#: packages/filebrowser/src/listing.ts:1814
 msgctxt "showErrorMessage"
 msgid "Delete Failed"
 msgstr "Löschen fehlgeschlagen"
 
-#: packages/filebrowser/src/listing.ts:1529 packages/filebrowser/src/listing.ts:1877
+#: packages/filebrowser/src/listing.ts:1877
 msgctxt "showErrorMessage"
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:1553 packages/filebrowser/src/listing.ts:1896
+#: packages/filebrowser/src/listing.ts:1896
 msgctxt "showErrorMessage"
 msgid "Rename Error"
 msgstr "Fehler beim Umbenennen"
 
-#: packages/filebrowser/src/listing.ts:1880 packages/filebrowser/src/listing.ts:2260
+#: packages/filebrowser/src/listing.ts:2260
 msgid "Last Modified"
 msgstr "Zuletzt geändert"
 
-#: packages/filebrowser/src/listing.ts:2051 packages/filebrowser/src/listing.ts:2549
+#: packages/filebrowser/src/listing.ts:2261
+msgid "File Size"
+msgstr "Dateigröße"
+
+#: packages/filebrowser/src/listing.ts:2549
 msgid "Name: %1"
 msgstr "Name: %1"
 
-#: packages/filebrowser/src/listing.ts:2055 packages/filebrowser/src/listing.ts:2555
+#: packages/filebrowser/src/listing.ts:2555
 msgid "\n"
 "Size: %1"
 msgstr "\n"
 "Größe: %1"
 
-#: packages/filebrowser/src/listing.ts:2063 packages/filebrowser/src/listing.ts:2565
+#: packages/filebrowser/src/listing.ts:2565
 msgid "\n"
 "Path: %1"
 msgstr "\n"
 "Pfad: %1"
 
-#: packages/filebrowser/src/listing.ts:2070 packages/filebrowser/src/listing.ts:2572
+#: packages/filebrowser/src/listing.ts:2572
 msgid "\n"
 "Created: %1"
 msgstr "\n"
 "Erstellt: %1"
 
-#: packages/filebrowser/src/listing.ts:2076 packages/filebrowser/src/listing.ts:2578
+#: packages/filebrowser/src/listing.ts:2578
 msgid "\n"
 "Modified: %1"
 msgstr "\n"
 "Geändert: %1"
 
-#: packages/filebrowser/src/listing.ts:2081 packages/filebrowser/src/listing.ts:2583
+#: packages/filebrowser/src/listing.ts:2583
 msgid "\n"
 "Writable: %1"
 msgstr "\n"
 "Schreibbar: %1"
 
-#: packages/filebrowser/src/listing.ts:2151 packages/filebrowser/src/listing.ts:2687
-msgid "%1 Item"
-msgid_plural "%1 Items"
-msgstr[0] "%1 Element"
-msgstr[1] "%1 Elemente"
-
-#: packages/filebrowser/src/listing.ts:2261
-msgid "File Size"
-msgstr "Dateigröße"
-
 #: packages/filebrowser/src/listing.ts:2608
 msgid "Deselect directory \"%1\""
 msgstr ""
 
 #: packages/filebrowser/src/listing.ts:2609
 msgid "Select directory \"%1\""
 msgstr ""
@@ -5467,592 +4881,580 @@
 msgid "Deselect file \"%1\""
 msgstr "Datei „%1“ abwählen"
 
 #: packages/filebrowser/src/listing.ts:2613
 msgid "Select file \"%1\""
 msgstr "Datei „%1“ auswählen"
 
-#: packages/filebrowser/src/listing.ts:382 packages/filebrowser/src/listing.ts:396
+#: packages/filebrowser/src/listing.ts:2687
+msgid "%1 Item"
+msgid_plural "%1 Items"
+msgstr[0] "%1 Element"
+msgstr[1] "%1 Elemente"
+
+#: packages/filebrowser/src/listing.ts:396
 msgctxt "showErrorMessage"
 msgid "Paste Error"
 msgstr "Fehler beim Einfügen"
 
-#: packages/filebrowser/src/listing.ts:402 packages/filebrowser/src/listing.ts:416
+#: packages/filebrowser/src/listing.ts:416
 msgid "Are you sure you want to permanently delete: %1?"
 msgstr "Bist du sicher, dass du %1 endgültig löschen möchtest?"
 
-#: packages/filebrowser/src/listing.ts:406 packages/filebrowser/src/listing.ts:420
+#: packages/filebrowser/src/listing.ts:420
 msgid "Are you sure you want to permanently delete the %1 selected item?"
 msgid_plural "Are you sure you want to permanently delete the %1 selected items?"
 msgstr[0] ""
 msgstr[1] ""
 
-#: packages/filebrowser/src/listing.ts:448 packages/filebrowser/src/listing.ts:472
+#: packages/filebrowser/src/listing.ts:472
 msgctxt "showErrorMessage"
 msgid "Duplicate file"
 msgstr "Datei duplizieren"
 
-#: packages/filebrowser/src/listing.ts:488 packages/filebrowser/src/listing.ts:512
+#: packages/filebrowser/src/listing.ts:512
 msgctxt "showErrorMessage"
 msgid "Shut down kernel"
 msgstr "Kernel herunterfahren"
 
-#: packages/filebrowser/src/listing.ts:845 packages/filebrowser/src/listing.ts:908
-msgid "%1\n"
-"Kernel: %2"
-msgstr "%1\n"
-"Kernel: %2"
-
 #: packages/filebrowser/src/listing.ts:852
 msgid "Deselect all files and directories"
 msgstr "Alle Dateien und Verzeichnisse abwählen"
 
 #: packages/filebrowser/src/listing.ts:853
 msgid "Select all files and directories"
 msgstr "Alle Dateien und Verzeichnisse auswählen"
 
 #: packages/filebrowser/src/listing.ts:906
 msgid "unknown"
 msgstr "unbekannt"
 
-#: packages/filebrowser/src/model.ts:414 packages/filebrowser/src/model.ts:421
+#: packages/filebrowser/src/listing.ts:908
+msgid "%1\n"
+"Kernel: %2"
+msgstr "%1\n"
+"Kernel: %2"
+
+#: packages/filebrowser/src/model.ts:414
 msgid "Cannot upload file (>%1 MB). %2"
 msgstr ""
 
-#: packages/filebrowser/src/model.ts:443 packages/filebrowser/src/model.ts:450
+#: packages/filebrowser/src/model.ts:443
 msgid "Large file size warning"
 msgstr ""
 
-#: packages/filebrowser/src/model.ts:444 packages/filebrowser/src/model.ts:451
+#: packages/filebrowser/src/model.ts:444
 msgid "The file size is %1 MB. Do you still want to upload it?"
 msgstr ""
 
-#: packages/filebrowser/src/model.ts:450 packages/filebrowser/src/model.ts:457
+#: packages/filebrowser/src/model.ts:450
 msgid "Upload"
 msgstr "Hochladen"
 
-#: packages/filebrowser/src/model.ts:83 packages/filebrowser/src/model.ts:90
+#: packages/filebrowser/src/model.ts:83
 msgid "Files still uploading"
 msgstr "Dateien werden noch hochgeladen"
 
-#: packages/filebrowser/src/upload.ts:111 packages/filebrowser/src/upload.ts:117
+#: packages/filebrowser/src/upload.ts:117
 msgid "Upload Files"
 msgstr "Dateien hochladen"
 
-#: packages/filebrowser/src/uploadstatus.tsx:36 packages/filebrowser/src/uploadstatus.tsx:37
+#: packages/filebrowser/src/uploadstatus.tsx:37
 msgid "Uploading…"
 msgstr "Lade hoch…"
 
-#: packages/filebrowser/src/uploadstatus.tsx:95 packages/filebrowser/src/uploadstatus.tsx:96
+#: packages/filebrowser/src/uploadstatus.tsx:96
 msgid "Complete!"
 msgstr "Fertig!"
 
-#: packages/fileeditor-extension/src/commands.ts:1020 packages/fileeditor-extension/src/commands.ts:1034 packages/fileeditor-extension/src/commands.ts:1050 packages/fileeditor-extension/src/commands.ts:1100 packages/fileeditor-extension/src/commands.ts:1114 packages/fileeditor-extension/src/commands.ts:1130 packages/launcher/src/index.tsx:151 packages/launcher/src/index.tsx:161 packages/launcher/src/index.tsx:437 packages/launcher/src/widget.tsx:117 packages/launcher/src/widget.tsx:127 packages/launcher/src/widget.tsx:295 packages/terminal-extension/src/index.ts:271
+#: packages/fileeditor-extension/src/commands.ts:1100 packages/fileeditor-extension/src/commands.ts:1114 packages/fileeditor-extension/src/commands.ts:1130 packages/launcher/src/widget.tsx:117 packages/launcher/src/widget.tsx:127 packages/launcher/src/widget.tsx:295 packages/terminal-extension/src/index.ts:271
 msgid "Other"
 msgstr "Andere"
 
-#: packages/fileeditor-extension/src/commands.ts:1080 packages/fileeditor-extension/src/commands.ts:1104 packages/fileeditor-extension/src/commands.ts:1119 packages/fileeditor-extension/src/commands.ts:1134 packages/fileeditor-extension/src/commands.ts:1152 packages/fileeditor-extension/src/commands.ts:1160 packages/fileeditor-extension/src/commands.ts:1182 packages/fileeditor-extension/src/commands.ts:1197 packages/fileeditor-extension/src/commands.ts:1212 packages/fileeditor-extension/src/commands.ts:1230
+#: packages/fileeditor-extension/src/commands.ts:1160 packages/fileeditor-extension/src/commands.ts:1182 packages/fileeditor-extension/src/commands.ts:1197 packages/fileeditor-extension/src/commands.ts:1212 packages/fileeditor-extension/src/commands.ts:1230
 msgid "Text Editor"
 msgstr "Texteditor"
 
-#: packages/fileeditor-extension/src/commands.ts:1274 packages/fileeditor-extension/src/commands.ts:524 packages/fileeditor-extension/src/commands.ts:619
-msgid "Create Console for Editor"
-msgstr "Konsole für Editor erstellen"
-
-#: packages/fileeditor-extension/src/commands.ts:1292 packages/fileeditor-extension/src/commands.ts:595
-msgid "Run Code"
-msgstr "Code ausführen"
-
-#: packages/fileeditor-extension/src/commands.ts:1293 packages/fileeditor-extension/src/commands.ts:640 packages/fileeditor-extension/src/commands.ts:743
-msgid "Run All Code"
-msgstr "Gesamten Code ausführen"
-
-#: packages/fileeditor-extension/src/commands.ts:1295
-msgid "Restart Kernel and Run All Code"
-msgstr "Kernel neu starten und gesamten Code ausführen"
-
 #: packages/fileeditor-extension/src/commands.ts:1358
 msgid "Code Viewer"
 msgstr "Code-Betrachter"
 
 #: packages/fileeditor-extension/src/commands.ts:1377
 msgid "Open Code Viewer"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:279 packages/fileeditor-extension/src/commands.ts:297
+#: packages/fileeditor-extension/src/commands.ts:279
 msgid "Increase Text Editor Font Size"
 msgstr "Texteditor-Schriftgröße erhöhen"
 
-#: packages/fileeditor-extension/src/commands.ts:283 packages/fileeditor-extension/src/commands.ts:301
+#: packages/fileeditor-extension/src/commands.ts:283
 msgid "Decrease Text Editor Font Size"
 msgstr "Texteditor-Schriftgröße verringern"
 
-#: packages/fileeditor-extension/src/commands.ts:306 packages/fileeditor-extension/src/commands.ts:310 packages/mainmenu-extension/src/index.ts:574 packages/mainmenu-extension/src/index.ts:576 packages/notebook-extension/src/index.ts:2963
+#: packages/fileeditor-extension/src/commands.ts:306 packages/fileeditor-extension/src/commands.ts:310 packages/mainmenu-extension/src/index.ts:576 packages/notebook-extension/src/index.ts:2963
 msgid "Show Line Numbers"
 msgstr "Zeilennummern anzeigen"
 
 #: packages/fileeditor-extension/src/commands.ts:311
 msgid "Show the line numbers for the current file."
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:351 packages/fileeditor-extension/src/commands.ts:359
+#: packages/fileeditor-extension/src/commands.ts:351
 msgid "Word Wrap"
 msgstr "Zeilenumbruch"
 
-#: packages/fileeditor-extension/src/commands.ts:355 packages/mainmenu-extension/src/index.ts:600 packages/mainmenu-extension/src/index.ts:612
+#: packages/fileeditor-extension/src/commands.ts:355 packages/mainmenu-extension/src/index.ts:600
 msgid "Wrap Words"
 msgstr "Automatischer Zeilenumbruch"
 
 #: packages/fileeditor-extension/src/commands.ts:356
 msgid "Wrap words for the current file."
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:375 packages/fileeditor-extension/src/index.ts:102
-msgid "Spaces: %1"
-msgid_plural "Spaces: %1"
-msgstr[0] "Leerzeichen: %1"
-msgstr[1] "Leerzeichen: %1"
-
-#: packages/fileeditor-extension/src/commands.ts:381 packages/fileeditor-extension/src/commands.ts:384 packages/fileeditor-extension/src/index.ts:138 packages/fileeditor-extension/src/index.ts:95
-msgid "Indent with Tab"
-msgstr "Mit Tabulator einrücken"
-
 #: packages/fileeditor-extension/src/commands.ts:382 packages/fileeditor-extension/src/index.ts:145
 msgctxt "v4"
 msgid "Spaces: %1"
 msgstr "Leerzeichen: %1"
 
+#: packages/fileeditor-extension/src/commands.ts:384 packages/fileeditor-extension/src/index.ts:138
+msgid "Indent with Tab"
+msgstr "Mit Tabulator einrücken"
+
 #: packages/fileeditor-extension/src/commands.ts:429
 msgid "Change match brackets for the current file."
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:446
-msgid "Auto Close Brackets for Text Editor"
-msgstr "Klammern im Texteditor automatisch schließen"
-
 #: packages/fileeditor-extension/src/commands.ts:467
 msgid "Auto Close Brackets in Text Editor"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:472 packages/fileeditor-extension/src/commands.ts:495
+#: packages/fileeditor-extension/src/commands.ts:495
 msgid "Auto Close Brackets"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:499 packages/fileeditor-extension/src/commands.ts:601
-msgid "Replace Selection in Editor"
-msgstr "Auswahl im Editor ersetzen"
-
 #: packages/fileeditor-extension/src/commands.ts:510
 msgid "Editor Theme"
 msgstr ""
 
+#: packages/fileeditor-extension/src/commands.ts:538 packages/mainmenu-extension/src/index.ts:324
+msgid "Go to Line…"
+msgstr "Zur Zeile springen…"
+
 #: packages/fileeditor-extension/src/commands.ts:563
 msgid "Change editor language."
 msgstr ""
 
+#: packages/fileeditor-extension/src/commands.ts:601
+msgid "Replace Selection in Editor"
+msgstr "Auswahl im Editor ersetzen"
+
+#: packages/fileeditor-extension/src/commands.ts:619
+msgid "Create Console for Editor"
+msgstr "Konsole für Editor erstellen"
+
 #: packages/fileeditor-extension/src/commands.ts:640
 msgid "Restart Kernel"
 msgstr "Kernel neu starten"
 
-#: packages/fileeditor-extension/src/commands.ts:673 packages/fileeditor-extension/src/commands.ts:770
-msgid "Show Markdown Preview"
-msgstr "Markdown-Vorschau anzeigen"
-
 #: packages/fileeditor-extension/src/commands.ts:705
 msgid "Run Selected Code"
 msgstr "Ausgewählten Code ausführen"
 
-#: packages/fileeditor-extension/src/commands.ts:711 packages/fileeditor-extension/src/commands.ts:847 packages/mainmenu-extension/src/index.ts:264 packages/mainmenu-extension/src/index.ts:277 packages/notebook-extension/src/index.ts:3045
-msgid "Undo"
-msgstr "Rückgängig"
+#: packages/fileeditor-extension/src/commands.ts:743
+msgid "Run All Code"
+msgstr "Gesamten Code ausführen"
 
-#: packages/fileeditor-extension/src/commands.ts:749 packages/fileeditor-extension/src/commands.ts:878 packages/mainmenu-extension/src/index.ts:269 packages/mainmenu-extension/src/index.ts:288 packages/notebook-extension/src/index.ts:3031
-msgid "Redo"
-msgstr "Wiederholen"
+#: packages/fileeditor-extension/src/commands.ts:770
+msgid "Show Markdown Preview"
+msgstr "Markdown-Vorschau anzeigen"
 
-#: packages/fileeditor-extension/src/commands.ts:781 packages/fileeditor-extension/src/commands.ts:954
+#: packages/fileeditor-extension/src/commands.ts:781
 msgid "New Text File"
 msgstr "Neue Textdatei"
 
-#: packages/fileeditor-extension/src/commands.ts:783 packages/fileeditor-extension/src/commands.ts:956
+#: packages/fileeditor-extension/src/commands.ts:783
 msgid "Text File"
 msgstr "Textdatei"
 
-#: packages/fileeditor-extension/src/commands.ts:786 packages/fileeditor-extension/src/commands.ts:959
+#: packages/fileeditor-extension/src/commands.ts:786
 msgid "Create a new text file"
 msgstr "Eine neue Textdatei erstellen"
 
-#: packages/fileeditor-extension/src/commands.ts:811 packages/fileeditor-extension/src/commands.ts:990
+#: packages/fileeditor-extension/src/commands.ts:811
 msgid "Create a new markdown file"
 msgstr "Eine neue Markdown-Datei erstellen"
 
-#: packages/fileeditor-extension/src/commands.ts:891 packages/fileeditor-extension/src/commands.ts:992
+#: packages/fileeditor-extension/src/commands.ts:847 packages/mainmenu-extension/src/index.ts:277 packages/notebook-extension/src/index.ts:3045
+msgid "Undo"
+msgstr "Rückgängig"
+
+#: packages/fileeditor-extension/src/commands.ts:878 packages/mainmenu-extension/src/index.ts:288 packages/notebook-extension/src/index.ts:3031
+msgid "Redo"
+msgstr "Wiederholen"
+
+#: packages/fileeditor-extension/src/commands.ts:992
 msgid "Select All"
 msgstr "Alles auswählen"
 
-#: packages/fileeditor-extension/src/index.ts:210 packages/fileeditor-extension/src/index.ts:330
+#: packages/fileeditor-extension/src/index.ts:307
+msgid "Editor"
+msgstr "Editor"
+
+#: packages/fileeditor-extension/src/index.ts:330
 msgid "New Python File"
 msgstr "Neue Python-Datei"
 
-#: packages/fileeditor-extension/src/index.ts:211 packages/fileeditor-extension/src/index.ts:331
+#: packages/fileeditor-extension/src/index.ts:331
 msgid "Create a new Python file"
 msgstr "Neue Python-Datei erstellen"
 
-#: packages/fileeditor-extension/src/index.ts:222 packages/fileeditor-extension/src/index.ts:342
+#: packages/fileeditor-extension/src/index.ts:342
 msgid "New Julia File"
 msgstr "Neue Julia-Datei"
 
-#: packages/fileeditor-extension/src/index.ts:223 packages/fileeditor-extension/src/index.ts:343
+#: packages/fileeditor-extension/src/index.ts:343
 msgid "Create a new Julia file"
 msgstr "Neue Julia-Datei erstellen"
 
-#: packages/fileeditor-extension/src/index.ts:234 packages/fileeditor-extension/src/index.ts:354
+#: packages/fileeditor-extension/src/index.ts:354
 msgid "New R File"
 msgstr "Neue R-Datei"
 
-#: packages/fileeditor-extension/src/index.ts:235 packages/fileeditor-extension/src/index.ts:355
+#: packages/fileeditor-extension/src/index.ts:355
 msgid "Create a new R file"
 msgstr "Neue R-Datei erstellen"
 
-#: packages/fileeditor-extension/src/index.ts:307
-msgid "Editor"
-msgstr "Editor"
+#: packages/fileeditor/src/syntaxstatus.tsx:66
+msgid "Change text editor syntax highlighting"
+msgstr "Syntaxhervorhebung des Texteditors ändern"
 
-#: packages/fileeditor/src/tabspacestatus.tsx:48 packages/fileeditor/src/tabspacestatus.tsx:57
+#: packages/fileeditor/src/tabspacestatus.tsx:48
 msgid "Spaces"
 msgstr "Leerzeichen"
 
 #: packages/fileeditor/src/tabspacestatus.tsx:49
 msgid "Tab Indent"
 msgstr ""
 
 #: packages/fileeditor/src/tabspacestatus.tsx:58
 msgid "Change the indentation…"
 msgstr ""
 
-#: packages/fileeditor/src/tabspacestatus.tsx:58
-msgid "Tab Size"
-msgstr "Tabgröße"
-
-#: packages/fileeditor/src/tabspacestatus.tsx:63
-msgid "Change Tab indentation…"
-msgstr "Tab-Einrückung ändern…"
-
 #: packages/help-extension/src/index.tsx:124
 msgid "CONTRIBUTOR LIST"
 msgstr "MITWIRKENDENLISTE"
 
 #: packages/help-extension/src/index.tsx:132
 msgid "ABOUT PROJECT JUPYTER"
 msgstr "ÜBER PROJECT JUPYTER"
 
 #: packages/help-extension/src/index.tsx:138
 msgid "© 2015-2023 Project Jupyter Contributors"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:185
-msgid "Launch Classic Notebook"
-msgstr "Klassisches Notebook starten"
-
-#: packages/help-extension/src/index.tsx:186 packages/help-extension/src/index.tsx:215
+#: packages/help-extension/src/index.tsx:186
 msgid "Jupyter Forum"
 msgstr "Jupyter-Forum"
 
-#: packages/help-extension/src/index.tsx:223 packages/help-extension/src/index.tsx:250
+#: packages/help-extension/src/index.tsx:223
 msgid "JupyterLab Reference"
 msgstr "JupyterLab Referenz"
 
-#: packages/help-extension/src/index.tsx:227 packages/help-extension/src/index.tsx:254
+#: packages/help-extension/src/index.tsx:227
 msgid "JupyterLab FAQ"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:231 packages/help-extension/src/index.tsx:259
+#: packages/help-extension/src/index.tsx:231
 msgid "Jupyter Reference"
 msgstr "JupyterLab Referenz"
 
-#: packages/help-extension/src/index.tsx:235 packages/help-extension/src/index.tsx:263
+#: packages/help-extension/src/index.tsx:235
 msgid "Markdown Reference"
 msgstr "Markdown Referenz"
 
 #: packages/help-extension/src/index.tsx:268
 msgid "Open the provided `url` in a tab."
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:375 packages/help-extension/src/index.tsx:384
+#: packages/help-extension/src/index.tsx:384
 msgid "About the %1 Kernel"
 msgstr "Über den %1 Kernel"
 
-#: packages/help-extension/src/index.tsx:480 packages/help-extension/src/index.tsx:486
+#: packages/help-extension/src/index.tsx:480
 msgid "Download All Licenses as"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:481 packages/help-extension/src/index.tsx:487 packages/help-extension/src/licenses.tsx:438 packages/help-extension/src/licenses.tsx:441
+#: packages/help-extension/src/index.tsx:481 packages/help-extension/src/licenses.tsx:441
 msgid "Licenses"
 msgstr "Lizenzen"
 
-#: packages/help-extension/src/index.tsx:482 packages/help-extension/src/index.tsx:488
+#: packages/help-extension/src/index.tsx:482
 msgid "Refresh Licenses"
 msgstr "Lizenzen aktualisieren"
 
 #: packages/help-extension/src/index.tsx:93
 msgid "About %1"
 msgstr "Über %1"
 
 #: packages/help-extension/src/index.tsx:96
 msgid "Version %1"
 msgstr "Version %1"
 
-#: packages/help-extension/src/licenses.tsx:513 packages/help-extension/src/licenses.tsx:517
+#: packages/help-extension/src/licenses.tsx:517
 msgid "Filter Licenses By"
 msgstr "Lizenzen filtern nach"
 
-#: packages/help-extension/src/licenses.tsx:517 packages/help-extension/src/licenses.tsx:522 packages/help-extension/src/licenses.tsx:643 packages/help-extension/src/licenses.tsx:650
+#: packages/help-extension/src/licenses.tsx:522 packages/help-extension/src/licenses.tsx:650
 msgid "Package"
 msgstr "Paket"
 
-#: packages/help-extension/src/licenses.tsx:521 packages/help-extension/src/licenses.tsx:526 packages/help-extension/src/licenses.tsx:644 packages/help-extension/src/licenses.tsx:651
+#: packages/help-extension/src/licenses.tsx:526 packages/help-extension/src/licenses.tsx:651
 msgid "Version"
 msgstr "Version"
 
-#: packages/help-extension/src/licenses.tsx:525 packages/help-extension/src/licenses.tsx:530 packages/help-extension/src/licenses.tsx:645 packages/help-extension/src/licenses.tsx:652 packages/help-extension/src/licenses.tsx:712 packages/help-extension/src/licenses.tsx:719
+#: packages/help-extension/src/licenses.tsx:530 packages/help-extension/src/licenses.tsx:652 packages/help-extension/src/licenses.tsx:719
 msgid "License"
 msgstr "Lizenz"
 
-#: packages/help-extension/src/licenses.tsx:530 packages/help-extension/src/licenses.tsx:536
+#: packages/help-extension/src/licenses.tsx:536
 msgid "Distributions"
 msgstr "Distributionen"
 
-#: packages/help-extension/src/licenses.tsx:633 packages/help-extension/src/licenses.tsx:640
+#: packages/help-extension/src/licenses.tsx:640
 msgid "No Packages found"
 msgstr "Keine Pakete gefunden"
 
-#: packages/help-extension/src/licenses.tsx:707 packages/help-extension/src/licenses.tsx:714
+#: packages/help-extension/src/licenses.tsx:714
 msgid "No Package selected"
 msgstr "Keine Pakete ausgewählt"
 
-#: packages/help-extension/src/licenses.tsx:713 packages/help-extension/src/licenses.tsx:720
+#: packages/help-extension/src/licenses.tsx:720
 msgid "No License ID found"
 msgstr "Keine License ID gefunden"
 
-#: packages/help-extension/src/licenses.tsx:715 packages/help-extension/src/licenses.tsx:722
+#: packages/help-extension/src/licenses.tsx:722
 msgid "No License Text found"
 msgstr "Kein License Text gefunden"
 
-#: packages/htmlviewer-extension/src/index.tsx:102 packages/htmlviewer-extension/src/index.tsx:105
+#: packages/htmlviewer-extension/src/index.tsx:105
 msgid "HTML File"
 msgstr "HTML-Datei"
 
 #: packages/htmlviewer-extension/src/index.tsx:115
 msgid "HTML Viewer"
 msgstr "HTML-Betrachter"
 
-#: packages/htmlviewer-extension/src/index.tsx:155 packages/htmlviewer-extension/src/index.tsx:181
+#: packages/htmlviewer-extension/src/index.tsx:181
 msgid "Trust HTML File"
 msgstr "HTML-Datei vertrauen"
 
-#: packages/htmlviewer-extension/src/index.tsx:156 packages/htmlviewer-extension/src/index.tsx:182
+#: packages/htmlviewer-extension/src/index.tsx:182
 msgid "Whether the HTML file is trusted.\n"
 "    Trusting the file allows scripts to run in it,\n"
 "    which may result in security risks.\n"
 "    Only enable for files you trust."
 msgstr ""
 
-#: packages/htmlviewer/src/index.tsx:258 packages/htmlviewer/src/widget.tsx:240
+#: packages/htmlviewer/src/widget.tsx:240
 msgid "Rerender HTML Document"
 msgstr "HTML-Dokument erneut rendern"
 
-#: packages/htmlviewer/src/index.tsx:333 packages/htmlviewer/src/widget.tsx:315
+#: packages/htmlviewer/src/widget.tsx:315
 msgid "Whether the HTML file is trusted.\n"
 "Trusting the file allows scripts to run in it,\n"
 "which may result in security risks.\n"
 "Only enable for files you trust."
 msgstr "Ob die HTML-Datei vertrauenswürdig ist.\n"
 "Dadurch Skripte in der Datei ausgeführt werden,\n"
 "was zu Sicherheitsrisiken führen kann.\n"
 "Nur für Dateien aktivieren, denen du vertraust."
 
-#: packages/htmlviewer/src/index.tsx:339 packages/htmlviewer/src/widget.tsx:321
+#: packages/htmlviewer/src/widget.tsx:321
 msgid "Distrust HTML"
 msgstr "HTML misstrauen"
 
-#: packages/htmlviewer/src/index.tsx:340 packages/htmlviewer/src/widget.tsx:322
+#: packages/htmlviewer/src/widget.tsx:322
 msgid "Trust HTML"
 msgstr "HTML vertrauen"
 
-#: packages/hub-extension/src/index.ts:154 packages/hub-extension/src/index.ts:166
+#: packages/hub-extension/src/index.ts:166
 msgid "Server unavailable or unreachable"
 msgstr "Server nicht verfügbar oder nicht erreichbar"
 
-#: packages/hub-extension/src/index.ts:155 packages/hub-extension/src/index.ts:167
+#: packages/hub-extension/src/index.ts:167
 msgid "Your server at %1 is not running.\n"
 "Would you like to restart it?"
 msgstr ""
 
-#: packages/hub-extension/src/index.ts:160 packages/hub-extension/src/index.ts:172
+#: packages/hub-extension/src/index.ts:172
 msgid "Restart"
 msgstr "Neu starten"
 
-#: packages/hub-extension/src/index.ts:66 packages/hub-extension/src/index.ts:67
+#: packages/hub-extension/src/index.ts:67
 msgid "Restart Server"
 msgstr "Server neu starten"
 
-#: packages/hub-extension/src/index.ts:67 packages/hub-extension/src/index.ts:68
+#: packages/hub-extension/src/index.ts:68
 msgid "Request that the Hub restart this server"
 msgstr ""
 
-#: packages/hub-extension/src/index.ts:74 packages/hub-extension/src/index.ts:75
+#: packages/hub-extension/src/index.ts:75
 msgid "Hub Control Panel"
 msgstr "Hub-Kontrollzentrum"
 
-#: packages/hub-extension/src/index.ts:75 packages/hub-extension/src/index.ts:76
+#: packages/hub-extension/src/index.ts:76
 msgid "Open the Hub control panel in a new browser tab"
 msgstr ""
 
-#: packages/hub-extension/src/index.ts:82 packages/hub-extension/src/index.ts:83 packages/mainmenu-extension/src/index.ts:443 packages/mainmenu-extension/src/index.ts:450
+#: packages/hub-extension/src/index.ts:83 packages/mainmenu-extension/src/index.ts:443
 msgid "Log Out"
 msgstr "Abmelden"
 
-#: packages/hub-extension/src/index.ts:83 packages/hub-extension/src/index.ts:84
+#: packages/hub-extension/src/index.ts:84
 msgid "Log out of the Hub"
 msgstr "Vom Hub abmelden"
 
-#: packages/hub-extension/src/index.ts:91 packages/hub-extension/src/index.ts:92
+#: packages/hub-extension/src/index.ts:92
 msgid "Hub"
 msgstr ""
 
 #: packages/imageviewer-extension/src/index.ts:128
 msgid "Image (Text)"
 msgstr ""
 
-#: packages/imageviewer-extension/src/index.ts:158 packages/imageviewer-extension/src/index.ts:161
+#: packages/imageviewer-extension/src/index.ts:161
 msgid "Image Viewer"
 msgstr "Bildbetrachter"
 
-#: packages/imageviewer-extension/src/index.ts:199 packages/imageviewer-extension/src/index.ts:202
+#: packages/imageviewer-extension/src/index.ts:202
 msgid "Zoom In"
 msgstr "Hineinzoomen"
 
-#: packages/imageviewer-extension/src/index.ts:205 packages/imageviewer-extension/src/index.ts:208
+#: packages/imageviewer-extension/src/index.ts:208
 msgid "Zoom Out"
 msgstr "Herauszoomen"
 
-#: packages/imageviewer-extension/src/index.ts:211 packages/imageviewer-extension/src/index.ts:214
+#: packages/imageviewer-extension/src/index.ts:214
 msgid "Reset Image"
 msgstr "Bild zurücksetzen"
 
-#: packages/imageviewer-extension/src/index.ts:217 packages/imageviewer-extension/src/index.ts:220
+#: packages/imageviewer-extension/src/index.ts:220
 msgid "Rotate Clockwise"
 msgstr "Im Uhrzeigersinn drehen"
 
-#: packages/imageviewer-extension/src/index.ts:223 packages/imageviewer-extension/src/index.ts:226
+#: packages/imageviewer-extension/src/index.ts:226
 msgid "Rotate Counterclockwise"
 msgstr "Gegen den Uhrzeigersinn drehen"
 
-#: packages/imageviewer-extension/src/index.ts:229 packages/imageviewer-extension/src/index.ts:232
+#: packages/imageviewer-extension/src/index.ts:232
 msgid "Flip image horizontally"
 msgstr "Bild horizontal spiegeln"
 
-#: packages/imageviewer-extension/src/index.ts:235 packages/imageviewer-extension/src/index.ts:238
+#: packages/imageviewer-extension/src/index.ts:238
 msgid "Flip image vertically"
 msgstr "Bild vertikal spiegeln"
 
-#: packages/imageviewer-extension/src/index.ts:241 packages/imageviewer-extension/src/index.ts:244
+#: packages/imageviewer-extension/src/index.ts:244
 msgid "Invert Colors"
 msgstr "Farben invertieren"
 
-#: packages/inspector-extension/src/index.ts:105 packages/inspector-extension/src/index.ts:136 packages/inspector-extension/src/index.ts:57
+#: packages/inspector-extension/src/index.ts:106 packages/inspector-extension/src/index.ts:137
 msgid "Show Contextual Help"
 msgstr "Kontextbezogene Hilfe anzeigen"
 
-#: packages/inspector-extension/src/index.ts:126
+#: packages/inspector-extension/src/index.ts:127
 msgid "Hide Contextual Help"
 msgstr ""
 
-#: packages/inspector-extension/src/index.ts:59 packages/inspector-extension/src/index.ts:91
+#: packages/inspector-extension/src/index.ts:60
 msgid "Live updating code documentation from the active kernel"
 msgstr "Live-Update der Code-Dokumentation vom aktiven Kernel"
 
-#: packages/inspector-extension/src/index.ts:62
+#: packages/inspector-extension/src/index.ts:63
 msgid "Contextual Help"
 msgstr ""
 
-#: packages/inspector/src/inspector.ts:51 packages/inspector/src/inspector.ts:52
+#: packages/inspector/src/inspector.ts:52
 msgid "Click on a function to see documentation."
 msgstr "Klicke auf eine Funktion, um die Dokumentation anzuzeigen."
 
 #: packages/javascript-extension/src/index.ts:41
 msgid "Are you sure that you want to run arbitrary Javascript within your JupyterLab session?"
 msgstr ""
 
-#: packages/javascript-extension/src/index.ts:45 packages/rendermime/src/renderers.ts:66 packages/rendermime/src/renderers.ts:70
+#: packages/javascript-extension/src/index.ts:45 packages/rendermime/src/renderers.ts:66
 msgid "Run"
 msgstr "Ausführen"
 
-#: packages/json-extension/src/component.tsx:63 packages/json-extension/src/component.tsx:78
+#: packages/json-extension/src/component.tsx:78
 msgid "Filter…"
 msgstr ""
 
-#: packages/launcher-extension/src/index.ts:103 packages/launcher-extension/src/index.ts:148 packages/launcher-extension/src/index.ts:76 packages/launcher-extension/src/index.ts:94
+#: packages/launcher-extension/src/index.ts:148 packages/launcher-extension/src/index.ts:94
 msgid "Launcher"
 msgstr "Starter"
 
-#: packages/launcher/src/index.tsx:411 packages/launcher/src/widget.tsx:272
+#: packages/launcher-extension/src/index.ts:72 packages/ui-components/src/icon/widgets/tabbarsvg.ts:31
+msgid "New Launcher"
+msgstr "Neuer Launcher"
+
+#: packages/launcher/src/widget.tsx:272
 msgctxt "Error"
 msgid "Launcher Error"
 msgstr "Launcher-Fehler"
 
-#: packages/logconsole-extension/src/index.tsx:142 packages/logconsole-extension/src/index.tsx:143 packages/logconsole/src/widget.ts:389
+#: packages/logconsole-extension/src/index.tsx:136 packages/logconsole/src/widget.ts:389
 msgid "Log Console"
 msgstr "Protokollkonsole"
 
-#: packages/logconsole-extension/src/index.tsx:191 packages/logconsole-extension/src/index.tsx:200
+#: packages/logconsole-extension/src/index.tsx:193
 msgid "Show Log Console"
 msgstr "Protokollkonsole anzeigen"
 
-#: packages/logconsole-extension/src/index.tsx:211 packages/logconsole-extension/src/index.tsx:220
+#: packages/logconsole-extension/src/index.tsx:213
 msgid "Add Checkpoint"
 msgstr "Kontrollpunkt hinzufügen"
 
-#: packages/logconsole-extension/src/index.tsx:220 packages/logconsole-extension/src/index.tsx:229
+#: packages/logconsole-extension/src/index.tsx:222
 msgid "Clear Log"
 msgstr "Protokoll leeren"
 
-#: packages/logconsole-extension/src/index.tsx:236 packages/logconsole-extension/src/index.tsx:246
+#: packages/logconsole-extension/src/index.tsx:239
 msgid "Set Log Level to %1"
 msgstr "Protokollierungsstufe auf %1 festlegen"
 
-#: packages/logconsole-extension/src/index.tsx:247
+#: packages/logconsole-extension/src/index.tsx:240
 msgid "Set log level to `level`."
 msgstr ""
 
-#: packages/logconsole-extension/src/index.tsx:366 packages/logconsole-extension/src/index.tsx:377
+#: packages/logconsole-extension/src/index.tsx:361
 msgid "Log Level:"
 msgstr "Protokollierungsstufe:"
 
-#: packages/logconsole-extension/src/index.tsx:374 packages/logconsole-extension/src/index.tsx:385
+#: packages/logconsole-extension/src/index.tsx:369
 msgid "Log level"
 msgstr "Protokollierungsstufe"
 
-#: packages/logconsole-extension/src/index.tsx:380 packages/logconsole-extension/src/index.tsx:391
+#: packages/logconsole-extension/src/index.tsx:375
 msgid "Critical"
 msgstr "Kritisch"
 
-#: packages/logconsole-extension/src/index.tsx:383 packages/logconsole-extension/src/index.tsx:394
+#: packages/logconsole-extension/src/index.tsx:378
 msgid "Info"
 msgstr ""
 
-#: packages/logconsole-extension/src/index.tsx:384 packages/logconsole-extension/src/index.tsx:395
+#: packages/logconsole-extension/src/index.tsx:379
 msgid "Debug"
 msgstr ""
 
-#: packages/logconsole-extension/src/status.tsx:29 packages/logconsole-extension/src/status.tsx:30
+#: packages/logconsole-extension/src/status.tsx:29
 msgid "%1 new messages, %2 log entries for %3"
 msgstr "%1 neue Nachrichten, %2 Logeinträge für %3"
 
-#: packages/logconsole-extension/src/status.tsx:36 packages/logconsole-extension/src/status.tsx:37
+#: packages/logconsole-extension/src/status.tsx:36
 msgid "%1 log entries for %2"
 msgstr "%1 Protokolleinträge für %2"
 
 #: packages/logconsole/src/widget.ts:390
 msgid "Log: %1"
 msgstr "Protokoll: %1"
 
@@ -6064,15 +5466,15 @@
 msgid "No log messages."
 msgstr "Keine Protokollmeldungen."
 
 #: packages/lsp-extension/src/index.ts:257
 msgid "Language servers"
 msgstr ""
 
-#: packages/lsp-extension/src/index.ts:276 packages/mainmenu-extension/src/index.ts:549 packages/mainmenu-extension/src/index.ts:552 packages/running-extension/src/kernels.ts:40 packages/running-extension/src/kernels.ts:67 packages/running/src/index.tsx:222 packages/running/src/index.tsx:357 packages/terminal-extension/src/index.ts:303 packages/terminal-extension/src/index.ts:323
+#: packages/lsp-extension/src/index.ts:276 packages/mainmenu-extension/src/index.ts:549 packages/running-extension/src/kernels.ts:67 packages/running/src/index.tsx:357 packages/terminal-extension/src/index.ts:323
 msgid "Shut Down All"
 msgstr "Alles herunterfahren"
 
 #: packages/lsp-extension/src/index.ts:277
 msgid "Are you sure you want to permanently shut down all running language servers?"
 msgstr ""
 
@@ -6096,574 +5498,326 @@
 msgid "Add server"
 msgstr ""
 
 #: packages/lsp/src/adapters/adapter.ts:455 packages/lsp/src/adapters/adapter.ts:473
 msgid "Message from "
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:185 packages/mainmenu-extension/src/index.ts:193
+#: packages/mainmenu-extension/src/index.ts:193
 msgid "Open Edit Menu"
 msgstr "Bearbeitungs Menü öffen"
 
-#: packages/mainmenu-extension/src/index.ts:189 packages/mainmenu-extension/src/index.ts:197
+#: packages/mainmenu-extension/src/index.ts:197
 msgid "Open File Menu"
 msgstr "Datei Menü öffen"
 
-#: packages/mainmenu-extension/src/index.ts:193 packages/mainmenu-extension/src/index.ts:201
+#: packages/mainmenu-extension/src/index.ts:201
 msgid "Open Kernel Menu"
 msgstr "Kernel Menü öffen"
 
-#: packages/mainmenu-extension/src/index.ts:197 packages/mainmenu-extension/src/index.ts:205
+#: packages/mainmenu-extension/src/index.ts:205
 msgid "Open Run Menu"
 msgstr "Ausführungs Menü öffen"
 
-#: packages/mainmenu-extension/src/index.ts:201 packages/mainmenu-extension/src/index.ts:209
+#: packages/mainmenu-extension/src/index.ts:209
 msgid "Open View Menu"
 msgstr "Anzeige Menü öffnen"
 
-#: packages/mainmenu-extension/src/index.ts:205 packages/mainmenu-extension/src/index.ts:213
+#: packages/mainmenu-extension/src/index.ts:213
 msgid "Open Settings Menu"
 msgstr "Einstellungs Menü öffnen"
 
-#: packages/mainmenu-extension/src/index.ts:209 packages/mainmenu-extension/src/index.ts:217
+#: packages/mainmenu-extension/src/index.ts:217
 msgid "Open Tabs Menu"
 msgstr "Tabs Menü öffnen"
 
-#: packages/mainmenu-extension/src/index.ts:213 packages/mainmenu-extension/src/index.ts:221
+#: packages/mainmenu-extension/src/index.ts:221
 msgid "Open Help Menu"
 msgstr "Hilfe Menü öffnen"
 
-#: packages/mainmenu-extension/src/index.ts:217 packages/mainmenu-extension/src/index.ts:225
+#: packages/mainmenu-extension/src/index.ts:225
 msgid "Open First Menu"
 msgstr "Erstes Menü öffnen"
 
-#: packages/mainmenu-extension/src/index.ts:237 packages/mainmenu-extension/src/index.ts:245
+#: packages/mainmenu-extension/src/index.ts:245
 msgid "Kernel Operations"
 msgstr "Kernel Optionen"
 
-#: packages/mainmenu-extension/src/index.ts:282 packages/mainmenu-extension/src/index.ts:301
+#: packages/mainmenu-extension/src/index.ts:301
 msgid "Clear"
 msgstr "Leeren"
 
-#: packages/mainmenu-extension/src/index.ts:298 packages/mainmenu-extension/src/index.ts:312
+#: packages/mainmenu-extension/src/index.ts:312
 msgid "Clear All"
 msgstr "Alle entfernen"
 
-#: packages/mainmenu-extension/src/index.ts:341
-msgid "Close and Shutdown"
-msgstr "Schließen und herunterfahren"
-
-#: packages/mainmenu-extension/src/index.ts:352 packages/notebook-extension/src/index.ts:1735
+#: packages/mainmenu-extension/src/index.ts:352
 msgid "Close and Shut Down"
 msgstr "Schließen und Herunterfahren"
 
-#: packages/mainmenu-extension/src/index.ts:368 packages/mainmenu-extension/src/index.ts:371
+#: packages/mainmenu-extension/src/index.ts:368
 msgid "New Console for Activity"
 msgstr "Neue Konsole für Aktivität"
 
-#: packages/mainmenu-extension/src/index.ts:376 packages/mainmenu-extension/src/index.ts:383
+#: packages/mainmenu-extension/src/index.ts:376
 msgid "Shut down JupyterLab"
 msgstr "JupyterLab herunterfahren"
 
-#: packages/mainmenu-extension/src/index.ts:381 packages/mainmenu-extension/src/index.ts:388
+#: packages/mainmenu-extension/src/index.ts:381
 msgid "Shutdown confirmation"
 msgstr "Herunterfahrbestätigung"
 
-#: packages/mainmenu-extension/src/index.ts:382 packages/mainmenu-extension/src/index.ts:389
+#: packages/mainmenu-extension/src/index.ts:382
 msgid "Please confirm you want to shut down JupyterLab."
 msgstr "Bitte bestätige, dass du JupyterLab herunterfahren möchtest."
 
-#: packages/mainmenu-extension/src/index.ts:414 packages/mainmenu-extension/src/index.ts:421
+#: packages/mainmenu-extension/src/index.ts:414
 msgid "You have shut down the Jupyter server. You can now close this tab."
 msgstr "Du hast den Jupyter-Server heruntergefahren. Du kannst diesen Tab nun schließen."
 
-#: packages/mainmenu-extension/src/index.ts:418 packages/mainmenu-extension/src/index.ts:425
+#: packages/mainmenu-extension/src/index.ts:418
 msgid "To use JupyterLab again, you will need to relaunch it."
 msgstr "Um JupyterLab erneut nutzen zu können, musst du es neu starten."
 
-#: packages/mainmenu-extension/src/index.ts:425 packages/mainmenu-extension/src/index.ts:432
+#: packages/mainmenu-extension/src/index.ts:425
 msgid "Server stopped"
 msgstr "Server gestoppt"
 
-#: packages/mainmenu-extension/src/index.ts:444 packages/mainmenu-extension/src/index.ts:451
+#: packages/mainmenu-extension/src/index.ts:444
 msgid "Log out of JupyterLab"
 msgstr "Aus JupyterLab abmelden"
 
-#: packages/mainmenu-extension/src/index.ts:482 packages/mainmenu-extension/src/index.ts:483 packages/notebook-extension/src/index.ts:3081
+#: packages/mainmenu-extension/src/index.ts:482 packages/notebook-extension/src/index.ts:3081
 msgid "Reconnect to Kernel"
 msgstr "Erneut mit Kernel verbinden"
 
 #: packages/mainmenu-extension/src/index.ts:507
 msgid "Restart Kernel and Clear…"
 msgstr "Kernel neu starten und leeren…"
 
 #: packages/mainmenu-extension/src/index.ts:532
 msgid "Shut down kernel"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:539 packages/mainmenu-extension/src/index.ts:542
+#: packages/mainmenu-extension/src/index.ts:539
 msgid "Shut Down All Kernels…"
 msgstr "Alle Kernel herunterfahren…"
 
-#: packages/mainmenu-extension/src/index.ts:545 packages/mainmenu-extension/src/index.ts:548
+#: packages/mainmenu-extension/src/index.ts:545
 msgid "Shut Down All?"
 msgstr "Alles herunterfahren?"
 
-#: packages/mainmenu-extension/src/index.ts:546 packages/mainmenu-extension/src/index.ts:549
+#: packages/mainmenu-extension/src/index.ts:546
 msgid "Shut down all kernels?"
 msgstr "Alle Kernel herunterfahren?"
 
-#: packages/mainmenu-extension/src/index.ts:622 packages/mainmenu-extension/src/index.ts:623 packages/mainmenu-extension/src/index.ts:645 packages/mainmenu-extension/src/index.ts:654
+#: packages/mainmenu-extension/src/index.ts:622 packages/mainmenu-extension/src/index.ts:623
 msgid "Run Selected"
 msgstr "Ausgewählte ausführen"
 
-#: packages/mainmenu-extension/src/index.ts:636 packages/mainmenu-extension/src/index.ts:637 packages/mainmenu-extension/src/index.ts:663 packages/mainmenu-extension/src/index.ts:679
+#: packages/mainmenu-extension/src/index.ts:636 packages/mainmenu-extension/src/index.ts:637
 msgid "Run All"
 msgstr "Alle ausführen"
 
-#: packages/mainmenu-extension/src/index.ts:648 packages/mainmenu-extension/src/index.ts:649 packages/mainmenu-extension/src/index.ts:699 packages/mainmenu-extension/src/index.ts:715
+#: packages/mainmenu-extension/src/index.ts:648 packages/mainmenu-extension/src/index.ts:649
 msgid "Restart Kernel and Run All"
 msgstr "Kernel neu starten und alle ausführen"
 
 #: packages/mainmenu-extension/src/index.ts:677
 msgid "Activate a widget by its `id`."
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:694 packages/mainmenu-extension/src/index.ts:774
+#: packages/mainmenu-extension/src/index.ts:694
 msgid "Activate Previously Used Tab"
 msgstr "Zuletzt benutzten Tab aktivieren"
 
-#: packages/mainmenu-extension/src/index.ts:771 packages/mainmenu-extension/src/index.ts:943
+#: packages/mainmenu-extension/src/index.ts:771
 msgid "Menu customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr ""
 
-#: packages/markdownviewer-extension/src/index.ts:117 packages/markdownviewer-extension/src/index.ts:138 packages/markdownviewer-extension/src/index.ts:143
+#: packages/markdownviewer-extension/src/index.ts:117 packages/markdownviewer-extension/src/index.ts:143
 msgid "Markdown Preview"
 msgstr "Markdown Vorschau"
 
-#: packages/markdownviewer-extension/src/index.ts:173 packages/markdownviewer-extension/src/index.ts:178
+#: packages/markdownviewer-extension/src/index.ts:178
 msgid "Show Markdown Editor"
 msgstr "Markdown-Editor anzeigen"
 
 #: packages/metadataform/src/metadataform.ts:54
 msgid "No metadata."
 msgstr "Keine Metadaten."
 
-#: packages/notebook-extension/src/index.ts:1012 packages/notebook-extension/src/index.ts:1335 packages/notebook-extension/src/index.ts:2705
+#: packages/notebook-extension/src/index.ts:1113
+msgid "Notebook Tools"
+msgstr "Notebook-Werkzeuge"
+
+#: packages/notebook-extension/src/index.ts:1265
+msgid "Create New View for Cell Output"
+msgstr ""
+
+#: packages/notebook-extension/src/index.ts:1335
 msgid "New Console for Notebook"
 msgstr "Neue Konsole für Notebook"
 
-#: packages/notebook-extension/src/index.ts:1030 packages/notebook-extension/src/index.ts:1353
+#: packages/notebook-extension/src/index.ts:1353
 msgid "Run Selected Text or Current Line in Console"
 msgstr "Ausgewählten Text oder aktuelle Zeile in der Konsole ausführen"
 
-#: packages/notebook-extension/src/index.ts:1113 packages/notebook-extension/src/index.ts:783
-msgid "Notebook Tools"
-msgstr "Notebook-Werkzeuge"
-
-#: packages/notebook-extension/src/index.ts:1190 packages/notebook-extension/src/index.ts:1517
+#: packages/notebook-extension/src/index.ts:1517
 msgid "Copy Output to Clipboard"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1265
-msgid "Create New View for Cell Output"
-msgstr ""
-
-#: packages/notebook-extension/src/index.ts:1283 packages/notebook-extension/src/index.ts:1673
+#: packages/notebook-extension/src/index.ts:1673
 msgid "Auto Close Brackets for All Notebook Cell Types"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1290 packages/notebook-extension/src/index.ts:1682
+#: packages/notebook-extension/src/index.ts:1682
 msgid "Set side-by-side ratio"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1293 packages/notebook-extension/src/index.ts:1685
+#: packages/notebook-extension/src/index.ts:1685
 msgid "Width of the output in side-by-side mode"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1480 packages/notebook-extension/src/index.ts:1900
+#: packages/notebook-extension/src/index.ts:1900
 msgid "New Notebook"
 msgstr "Neues Notebook"
 
-#: packages/notebook-extension/src/index.ts:1484 packages/notebook-extension/src/index.ts:1904
+#: packages/notebook-extension/src/index.ts:1904
 msgid "Create a new notebook"
 msgstr "Neues Notebook erstellen"
 
-#: packages/notebook-extension/src/index.ts:1617 packages/notebook-extension/src/index.ts:2728
-msgid "Run Selected Cells"
-msgstr "Ausgewählte Zellen ausführen"
-
-#: packages/notebook-extension/src/index.ts:1630
-msgid "Run Selected Cells and Do not Advance"
-msgstr ""
-
-#: packages/notebook-extension/src/index.ts:1643
-msgid "Run Selected Cells and Insert Below"
-msgstr "Ausgewählte Zellen ausführen und neue unterhalb einfügen"
-
-#: packages/notebook-extension/src/index.ts:1656 packages/notebook-extension/src/index.ts:2239 packages/notebook-extension/src/index.ts:2730
-msgid "Run All Cells"
-msgstr "Alle Zellen ausführen"
-
-#: packages/notebook-extension/src/index.ts:1669 packages/notebook-extension/src/index.ts:2258
-msgid "Run All Above Selected Cell"
-msgstr "Alles oberhalb der ausgewählten Zelle ausführen"
-
-#: packages/notebook-extension/src/index.ts:1689 packages/notebook-extension/src/index.ts:2283
-msgid "Run Selected Cell and All Below"
-msgstr "Ausgewählte Zelle und alles darunter ausführen"
-
-#: packages/notebook-extension/src/index.ts:1710 packages/notebook-extension/src/index.ts:2309
-msgid "Render All Markdown Cells"
-msgstr "Alle Markdown Zellen ausführen"
-
-#: packages/notebook-extension/src/index.ts:1746 packages/notebook-extension/src/index.ts:2356
-msgid "Shut down the notebook?"
-msgstr "Notebook herunterfahren?"
-
-#: packages/notebook-extension/src/index.ts:1760 packages/notebook-extension/src/index.ts:2372
-msgid "Trust Notebook"
-msgstr "Notebook vertrauen"
-
-#: packages/notebook-extension/src/index.ts:1771 packages/notebook-extension/src/index.ts:2684
-msgid "Restart Kernel and Clear All Outputs…"
-msgstr "Kernel neu starten und alle Ausgaben löschen…"
-
-#: packages/notebook-extension/src/index.ts:1786 packages/notebook-extension/src/index.ts:2396
-msgid "Restart Kernel and Run up to Selected Cell…"
-msgstr "Kernel neu starten und bis zur ausgewählten Zelle ausführen…"
-
-#: packages/notebook-extension/src/index.ts:1810 packages/notebook-extension/src/index.ts:2414 packages/notebook-extension/src/index.ts:2733
-msgid "Restart Kernel and Run All Cells…"
-msgstr "Kernel neu starten und alle Zellen ausführen…"
-
-#: packages/notebook-extension/src/index.ts:1830 packages/notebook-extension/src/index.ts:2635
-msgid "Clear All Outputs"
-msgstr "Alle Ausgaben löschen"
-
-#: packages/notebook-extension/src/index.ts:1841
-msgid "Clear Outputs"
-msgstr "Ausgaben löschen"
-
-#: packages/notebook-extension/src/index.ts:1869 packages/notebook-extension/src/index.ts:2470
-msgid "Change to Code Cell Type"
-msgstr "Wechsel zu Code Zellen-Typ"
-
-#: packages/notebook-extension/src/index.ts:1880 packages/notebook-extension/src/index.ts:2481
-msgid "Change to Markdown Cell Type"
-msgstr "Wechsel zu Markdown Zellen-Typ"
-
-#: packages/notebook-extension/src/index.ts:1891 packages/notebook-extension/src/index.ts:2492
-msgid "Change to Raw Cell Type"
-msgstr "Wechsel zu Raw Zellen-Typ"
-
-#: packages/notebook-extension/src/index.ts:1902
-msgid "Cut Cells"
-msgstr "Zellen ausschneiden"
-
-#: packages/notebook-extension/src/index.ts:1903 packages/notebook/src/default-toolbar.tsx:140 packages/notebook/src/default-toolbar.tsx:141
-msgid "Cut the selected cells"
-msgstr "Markierte Zellen ausschneiden"
-
-#: packages/notebook-extension/src/index.ts:1915
-msgid "Copy Cells"
-msgstr "Zellen kopieren"
-
-#: packages/notebook-extension/src/index.ts:1916 packages/notebook/src/default-toolbar.tsx:160 packages/notebook/src/default-toolbar.tsx:161
-msgid "Copy the selected cells"
-msgstr "Markierte Zellen kopieren"
-
-#: packages/notebook-extension/src/index.ts:1928
-msgid "Paste Cells Below"
-msgstr "Zellen unterhalb einfügen"
-
-#: packages/notebook-extension/src/index.ts:1929 packages/notebook/src/default-toolbar.tsx:180 packages/notebook/src/default-toolbar.tsx:181
-msgid "Paste cells from the clipboard"
-msgstr "Zellen aus der Zwischenablage einfügen"
-
-#: packages/notebook-extension/src/index.ts:1941
-msgid "Paste Cells Above"
-msgstr "Zellen oberhalb einfügen"
-
-#: packages/notebook-extension/src/index.ts:1952
-msgid "Duplicate Cells Below"
-msgstr ""
-
-#: packages/notebook-extension/src/index.ts:1953
-msgid "Copy the selected cells and paste them below the selection"
-msgstr ""
-
-#: packages/notebook-extension/src/index.ts:1967
-msgid "Paste Cells and Replace"
-msgstr "Zellen einfügen und ersetzen"
-
-#: packages/notebook-extension/src/index.ts:1978
-msgid "Delete Cells"
-msgstr "Zelle löschen"
-
-#: packages/notebook-extension/src/index.ts:1989 packages/notebook-extension/src/index.ts:2682
-msgid "Split Cell"
-msgstr "Zelle teilen"
-
-#: packages/notebook-extension/src/index.ts:2000 packages/notebook-extension/src/index.ts:2693
-msgid "Merge Selected Cells"
-msgstr "Ausgewählte Zellen zusammenführen"
-
-#: packages/notebook-extension/src/index.ts:2011 packages/notebook-extension/src/index.ts:2704
-msgid "Merge Cell Above"
-msgstr ""
-
-#: packages/notebook-extension/src/index.ts:2022 packages/notebook-extension/src/index.ts:2715
-msgid "Merge Cell Below"
-msgstr ""
-
-#: packages/notebook-extension/src/index.ts:2033 packages/notebook-extension/src/index.ts:2726
-msgid "Insert Cell Above"
-msgstr "Zellen oberhalb einfügen"
-
-#: packages/notebook-extension/src/index.ts:2045 packages/notebook-extension/src/index.ts:2739
-msgid "Insert Cell Below"
-msgstr "Zellen unterhalb einfügen"
-
-#: packages/notebook-extension/src/index.ts:2046 packages/notebook-extension/src/index.ts:2740 packages/notebook/src/default-toolbar.tsx:120 packages/notebook/src/default-toolbar.tsx:121
-msgid "Insert a cell below"
-msgstr ""
-
-#: packages/notebook-extension/src/index.ts:2058 packages/notebook-extension/src/index.ts:2752
-msgid "Select Cell Above"
-msgstr "Zellen oberhalb auswählen"
-
-#: packages/notebook-extension/src/index.ts:2069 packages/notebook-extension/src/index.ts:2763
-msgid "Select Cell Below"
-msgstr "Zellen unterhalb auswählen"
-
-#: packages/notebook-extension/src/index.ts:2080 packages/notebook-extension/src/index.ts:2821
-msgid "Extend Selection Above"
-msgstr "Auswahl nach oben erweitern"
-
-#: packages/notebook-extension/src/index.ts:2091 packages/notebook-extension/src/index.ts:2832
-msgid "Extend Selection to Top"
-msgstr "Auswahl bis zum Anfang erweitern"
-
-#: packages/notebook-extension/src/index.ts:2102 packages/notebook-extension/src/index.ts:2843
-msgid "Extend Selection Below"
-msgstr "Auswahl nach unten erweitern"
-
-#: packages/notebook-extension/src/index.ts:2113 packages/notebook-extension/src/index.ts:2854
-msgid "Extend Selection to Bottom"
-msgstr "Auswahl bis zum Ende erweitern"
-
-#: packages/notebook-extension/src/index.ts:2124 packages/notebook-extension/src/index.ts:2865
-msgid "Select All Cells"
-msgstr "Alle Zellen auswählen"
-
-#: packages/notebook-extension/src/index.ts:2135 packages/notebook-extension/src/index.ts:2876
-msgid "Deselect All Cells"
-msgstr "Alle Zellen abwählen"
-
-#: packages/notebook-extension/src/index.ts:2146
-msgid "Move Cells Up"
-msgstr "Zellen nach oben verschieben"
-
-#: packages/notebook-extension/src/index.ts:2158
-msgid "Move Cells Down"
-msgstr "Zellen nach unten verschieben"
-
 #: packages/notebook-extension/src/index.ts:2158
 msgid "Run Selected Cell"
 msgid_plural "Run Selected Cells"
 msgstr[0] ""
 msgstr[1] ""
 
 #: packages/notebook-extension/src/index.ts:2166
 msgid "Run this cell and advance"
 msgid_plural "Run these %1 cells and advance"
 msgstr[0] ""
 msgstr[1] ""
 
-#: packages/notebook-extension/src/index.ts:2170
-msgid "Toggle All Line Numbers"
-msgstr "Alle Zeilennummern umschalten"
-
-#: packages/notebook-extension/src/index.ts:2181 packages/notebook-extension/src/index.ts:2987
-msgid "Enter Command Mode"
-msgstr "Befehlsmodus aktivieren"
-
 #: packages/notebook-extension/src/index.ts:2191
 msgid "Run Selected Cell and Do not Advance"
 msgid_plural "Run Selected Cells and Do not Advance"
 msgstr[0] ""
 msgstr[1] ""
 
-#: packages/notebook-extension/src/index.ts:2192 packages/notebook-extension/src/index.ts:2998
-msgid "Enter Edit Mode"
-msgstr "Bearbeitungsmodus aktivieren"
-
-#: packages/notebook-extension/src/index.ts:2203 packages/notebook-extension/src/index.ts:3009
-msgid "Undo Cell Operation"
-msgstr "Zellenoperation rückgängig machen"
-
-#: packages/notebook-extension/src/index.ts:2214 packages/notebook-extension/src/index.ts:3020
-msgid "Redo Cell Operation"
-msgstr "Zellenoperation wiederholen"
-
 #: packages/notebook-extension/src/index.ts:2216
 msgid "Run Selected Cell and Insert Below"
 msgid_plural "Run Selected Cells and Insert Below"
 msgstr[0] ""
 msgstr[1] ""
 
 #: packages/notebook-extension/src/index.ts:2239
-msgid "Reconnect To Kernel"
-msgstr "Verbindung zum Kernel wiederherstellen"
+msgid "Run All Cells"
+msgstr "Alle Zellen ausführen"
 
 #: packages/notebook-extension/src/index.ts:2240
 msgid "Run all cells"
 msgstr "Alle Zellen ausführen"
 
-#: packages/notebook-extension/src/index.ts:2256 packages/notebook-extension/src/index.ts:3098
-msgid "Change to Heading 1"
-msgstr "In Überschrift 1 ändern"
-
-#: packages/notebook-extension/src/index.ts:2267 packages/notebook-extension/src/index.ts:3109
-msgid "Change to Heading 2"
-msgstr "In Überschrift 2 ändern"
-
-#: packages/notebook-extension/src/index.ts:2278 packages/notebook-extension/src/index.ts:3120
-msgid "Change to Heading 3"
-msgstr "In Überschrift 3 ändern"
-
-#: packages/notebook-extension/src/index.ts:2289 packages/notebook-extension/src/index.ts:3131
-msgid "Change to Heading 4"
-msgstr "In Überschrift 4 ändern"
-
-#: packages/notebook-extension/src/index.ts:2300 packages/notebook-extension/src/index.ts:3142
-msgid "Change to Heading 5"
-msgstr ""
-
-#: packages/notebook-extension/src/index.ts:2311 packages/notebook-extension/src/index.ts:3153
-msgid "Change to Heading 6"
-msgstr ""
-
-#: packages/notebook-extension/src/index.ts:2322 packages/notebook-extension/src/index.ts:3164
-msgid "Collapse Selected Code"
-msgstr "Asugewählten Code reduzieren"
+#: packages/notebook-extension/src/index.ts:2258
+msgid "Run All Above Selected Cell"
+msgstr "Alles oberhalb der ausgewählten Zelle ausführen"
 
-#: packages/notebook-extension/src/index.ts:2333 packages/notebook-extension/src/index.ts:3175
-msgid "Expand Selected Code"
-msgstr "Asugewählten Code erweitern"
+#: packages/notebook-extension/src/index.ts:2283
+msgid "Run Selected Cell and All Below"
+msgstr "Ausgewählte Zelle und alles darunter ausführen"
 
-#: packages/notebook-extension/src/index.ts:2344 packages/notebook-extension/src/index.ts:3186
-msgid "Collapse All Code"
-msgstr "Gesamten Code reduzieren"
+#: packages/notebook-extension/src/index.ts:2309
+msgid "Render All Markdown Cells"
+msgstr "Alle Markdown Zellen ausführen"
 
 #: packages/notebook-extension/src/index.ts:2345
 msgid "Close and Shut Down Notebook"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2355 packages/notebook-extension/src/index.ts:3197
-msgid "Expand All Code"
-msgstr "Gesamten Code erweitern"
-
-#: packages/notebook-extension/src/index.ts:2366 packages/notebook-extension/src/index.ts:3208
-msgid "Collapse Selected Outputs"
-msgstr "Ausgewählte Ausgaben reduzieren"
+#: packages/notebook-extension/src/index.ts:2356
+msgid "Shut down the notebook?"
+msgstr "Notebook herunterfahren?"
 
-#: packages/notebook-extension/src/index.ts:2377 packages/notebook-extension/src/index.ts:3219
-msgid "Expand Selected Outputs"
-msgstr "Ausgewählte Ausgaben erweitern"
+#: packages/notebook-extension/src/index.ts:2372
+msgid "Trust Notebook"
+msgstr "Notebook vertrauen"
 
 #: packages/notebook-extension/src/index.ts:2383
 msgid "Restart Kernel and Clear Outputs of All Cells…"
 msgstr ""
 
 #: packages/notebook-extension/src/index.ts:2384
 msgid "Restart the kernel and clear all outputs of all cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2388 packages/notebook-extension/src/index.ts:3230
-msgid "Collapse All Outputs"
-msgstr "Alle Ausgaben reduzieren"
+#: packages/notebook-extension/src/index.ts:2396
+msgid "Restart Kernel and Run up to Selected Cell…"
+msgstr "Kernel neu starten und bis zur ausgewählten Zelle ausführen…"
 
-#: packages/notebook-extension/src/index.ts:2400 packages/notebook-extension/src/index.ts:3242
-msgid "Render Side-by-Side"
-msgstr ""
+#: packages/notebook-extension/src/index.ts:2414
+msgid "Restart Kernel and Run All Cells…"
+msgstr "Kernel neu starten und alle Zellen ausführen…"
 
 #: packages/notebook-extension/src/index.ts:2415
 msgid "Restart the kernel and run all cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2422 packages/notebook-extension/src/index.ts:3264
-msgid "Expand All Outputs"
-msgstr "Alle Ausgaben erweitern"
-
 #: packages/notebook-extension/src/index.ts:2428
 msgid "Clear Outputs of All Cells"
 msgstr ""
 
 #: packages/notebook-extension/src/index.ts:2429
 msgid "Clear all outputs of all cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2433 packages/notebook-extension/src/index.ts:3275
-msgid "Enable Scrolling for Outputs"
-msgstr "Scrollen für Ausgaben aktivieren"
-
 #: packages/notebook-extension/src/index.ts:2440
 msgid "Clear Cell Output"
 msgstr ""
 
 #: packages/notebook-extension/src/index.ts:2441
 msgid "Clear outputs for the selected cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2444 packages/notebook-extension/src/index.ts:3286
-msgid "Disable Scrolling for Outputs"
-msgstr "Scrollen für Ausgaben deaktivieren"
+#: packages/notebook-extension/src/index.ts:2470
+msgid "Change to Code Cell Type"
+msgstr "Wechsel zu Code Zellen-Typ"
 
-#: packages/notebook-extension/src/index.ts:2455 packages/notebook-extension/src/index.ts:3297
-msgid "Select current running or last run cell"
-msgstr "Aktuelle laufende oder zuletzt ausgeführte Zelle auswählen"
+#: packages/notebook-extension/src/index.ts:2481
+msgid "Change to Markdown Cell Type"
+msgstr "Wechsel zu Markdown Zellen-Typ"
 
-#: packages/notebook-extension/src/index.ts:2466 packages/notebook-extension/src/index.ts:3308
-msgid "Replace Selection in Notebook Cell"
-msgstr "Auswahl in Notebook Zelle ersetzen"
+#: packages/notebook-extension/src/index.ts:2492
+msgid "Change to Raw Cell Type"
+msgstr "Wechsel zu Raw Zellen-Typ"
 
 #: packages/notebook-extension/src/index.ts:2505
 msgid "Cut Cell"
 msgid_plural "Cut Cells"
 msgstr[0] "Zelle ausschneiden"
 msgstr[1] "Zellen ausschneiden"
 
 #: packages/notebook-extension/src/index.ts:2513
 msgid "Cut this cell"
 msgid_plural "Cut these %1 cells"
 msgstr[0] "Diese Zelle ausschneiden"
 msgstr[1] "Diese %1 Zellen ausschneiden"
 
-#: packages/notebook-extension/src/index.ts:2514 packages/notebook-extension/src/index.ts:3399 packages/notebook-extension/src/index.ts:572 packages/notebook-extension/src/index.ts:657
-msgid "Notebook Operations"
-msgstr "Notebook Operationen"
-
 #: packages/notebook-extension/src/index.ts:2532
 msgid "Copy Cell"
 msgid_plural "Copy Cells"
 msgstr[0] "Zelle kopieren"
 msgstr[1] "Zellen kopieren"
 
 #: packages/notebook-extension/src/index.ts:2540
 msgid "Copy this cell"
 msgid_plural "Copy these %1 cells"
 msgstr[0] "Diese Zelle kopieren"
 msgstr[1] "Diese %1 Zellen kopieren"
 
-#: packages/notebook-extension/src/index.ts:2550 packages/notebook-extension/src/index.ts:3435
-msgid "Notebook Cell Operations"
-msgstr "Notebook Zellen Operationen"
-
 #: packages/notebook-extension/src/index.ts:2559
 msgid "Paste Cell Below"
 msgid_plural "Paste Cells Below"
 msgstr[0] "Zelle unterhalb einfügen"
 msgstr[1] "Zellen unterhalb einfügen"
 
 #: packages/notebook-extension/src/index.ts:2567 packages/notebook-extension/src/index.ts:2594
@@ -6686,60 +5840,72 @@
 
 #: packages/notebook-extension/src/index.ts:2620
 msgid "Create a duplicate of this cell below"
 msgid_plural "Create duplicates of %1 cells below"
 msgstr[0] ""
 msgstr[1] ""
 
-#: packages/notebook-extension/src/index.ts:2633
-msgid "Clear Output"
-msgstr "Ausgaben löschen"
-
 #: packages/notebook-extension/src/index.ts:2639
 msgid "Paste Cell and Replace"
 msgid_plural "Paste Cells and Replace"
 msgstr[0] ""
 msgstr[1] ""
 
-#: packages/notebook-extension/src/index.ts:2649
-msgid "Close and Shutdown Notebook"
-msgstr ""
-
-#: packages/notebook-extension/src/index.ts:2653
-msgid "Shut down the Notebook?"
-msgstr ""
-
 #: packages/notebook-extension/src/index.ts:2657
 msgid "Delete Cell"
 msgid_plural "Delete Cells"
 msgstr[0] "Zelle löschen"
 msgstr[1] "Zellen löschen"
 
 #: packages/notebook-extension/src/index.ts:2665
 msgid "Delete this cell"
 msgid_plural "Delete these %1 cells"
 msgstr[0] "Diese Zelle löschen"
 msgstr[1] "Diese %1 Zellen löschen"
 
-#: packages/notebook-extension/src/index.ts:2727
-msgid "Insert a cell above"
+#: packages/notebook-extension/src/index.ts:2682
+msgid "Split Cell"
+msgstr "Zelle teilen"
+
+#: packages/notebook-extension/src/index.ts:2693
+msgid "Merge Selected Cells"
+msgstr "Ausgewählte Zellen zusammenführen"
+
+#: packages/notebook-extension/src/index.ts:2704
+msgid "Merge Cell Above"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2729 packages/notebook/src/default-toolbar.tsx:200 packages/notebook/src/default-toolbar.tsx:207
-msgid "Run the selected cells and advance"
+#: packages/notebook-extension/src/index.ts:2715
+msgid "Merge Cell Below"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2731
-msgid "Run the all notebook cells"
+#: packages/notebook-extension/src/index.ts:2726
+msgid "Insert Cell Above"
+msgstr "Zellen oberhalb einfügen"
+
+#: packages/notebook-extension/src/index.ts:2727
+msgid "Insert a cell above"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2735 packages/notebook/src/default-toolbar.tsx:227 packages/notebook/src/default-toolbar.tsx:238
-msgid "Restart the kernel, then re-run the whole notebook"
+#: packages/notebook-extension/src/index.ts:2739
+msgid "Insert Cell Below"
+msgstr "Zellen unterhalb einfügen"
+
+#: packages/notebook-extension/src/index.ts:2740 packages/notebook/src/default-toolbar.tsx:121
+msgid "Insert a cell below"
 msgstr ""
 
+#: packages/notebook-extension/src/index.ts:2752
+msgid "Select Cell Above"
+msgstr "Zellen oberhalb auswählen"
+
+#: packages/notebook-extension/src/index.ts:2763
+msgid "Select Cell Below"
+msgstr "Zellen unterhalb auswählen"
+
 #: packages/notebook-extension/src/index.ts:2773
 msgid "Insert Heading Above Current Heading"
 msgstr ""
 
 #: packages/notebook-extension/src/index.ts:2784
 msgid "Insert Heading Below Current Heading"
 msgstr ""
@@ -6748,44 +5914,44 @@
 msgid "Select Heading Above or Collapse Heading"
 msgstr ""
 
 #: packages/notebook-extension/src/index.ts:2808
 msgid "Select Heading Below or Expand Heading"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2870 packages/notebook-extension/src/index.ts:3680 packages/notebook-extension/src/index.ts:757
-msgid "PDF"
-msgstr ""
+#: packages/notebook-extension/src/index.ts:2821
+msgid "Extend Selection Above"
+msgstr "Auswahl nach oben erweitern"
 
-#: packages/notebook-extension/src/index.ts:2871 packages/notebook-extension/src/index.ts:3681
-msgid "ReStructured Text"
-msgstr "ReStructuredText"
+#: packages/notebook-extension/src/index.ts:2832
+msgid "Extend Selection to Top"
+msgstr "Auswahl bis zum Anfang erweitern"
 
-#: packages/notebook-extension/src/index.ts:2872 packages/notebook-extension/src/index.ts:3682
-msgid "Executable Script"
-msgstr "Ausführbares Skript"
+#: packages/notebook-extension/src/index.ts:2843
+msgid "Extend Selection Below"
+msgstr "Auswahl nach unten erweitern"
 
-#: packages/notebook-extension/src/index.ts:2873 packages/notebook-extension/src/index.ts:3683
-msgid "Reveal.js Slides"
-msgstr ""
+#: packages/notebook-extension/src/index.ts:2854
+msgid "Extend Selection to Bottom"
+msgstr "Auswahl bis zum Ende erweitern"
+
+#: packages/notebook-extension/src/index.ts:2865
+msgid "Select All Cells"
+msgstr "Alle Zellen auswählen"
+
+#: packages/notebook-extension/src/index.ts:2876
+msgid "Deselect All Cells"
+msgstr "Alle Zellen abwählen"
 
 #: packages/notebook-extension/src/index.ts:2889
 msgid "Move Cell Up"
 msgid_plural "Move Cells Up"
 msgstr[0] ""
 msgstr[1] ""
 
-#: packages/notebook-extension/src/index.ts:2891 packages/notebook-extension/src/index.ts:3737
-msgid "For Notebook: %1"
-msgstr "Für Notebook: %1"
-
-#: packages/notebook-extension/src/index.ts:2892 packages/notebook-extension/src/index.ts:3738
-msgid "For Notebook:"
-msgstr "Für Notebook:"
-
 #: packages/notebook-extension/src/index.ts:2897
 msgid "Move this cell up"
 msgid_plural "Move these %1 cells up"
 msgstr[0] ""
 msgstr[1] ""
 
 #: packages/notebook-extension/src/index.ts:2909
@@ -6804,14 +5970,106 @@
 msgstr[0] ""
 msgstr[1] ""
 
 #: packages/notebook-extension/src/index.ts:2946
 msgid "Notebook cell shifted down successfully"
 msgstr ""
 
+#: packages/notebook-extension/src/index.ts:2987
+msgid "Enter Command Mode"
+msgstr "Befehlsmodus aktivieren"
+
+#: packages/notebook-extension/src/index.ts:2998
+msgid "Enter Edit Mode"
+msgstr "Bearbeitungsmodus aktivieren"
+
+#: packages/notebook-extension/src/index.ts:3009
+msgid "Undo Cell Operation"
+msgstr "Zellenoperation rückgängig machen"
+
+#: packages/notebook-extension/src/index.ts:3020
+msgid "Redo Cell Operation"
+msgstr "Zellenoperation wiederholen"
+
+#: packages/notebook-extension/src/index.ts:3098
+msgid "Change to Heading 1"
+msgstr "In Überschrift 1 ändern"
+
+#: packages/notebook-extension/src/index.ts:3109
+msgid "Change to Heading 2"
+msgstr "In Überschrift 2 ändern"
+
+#: packages/notebook-extension/src/index.ts:3120
+msgid "Change to Heading 3"
+msgstr "In Überschrift 3 ändern"
+
+#: packages/notebook-extension/src/index.ts:3131
+msgid "Change to Heading 4"
+msgstr "In Überschrift 4 ändern"
+
+#: packages/notebook-extension/src/index.ts:3142
+msgid "Change to Heading 5"
+msgstr ""
+
+#: packages/notebook-extension/src/index.ts:3153
+msgid "Change to Heading 6"
+msgstr ""
+
+#: packages/notebook-extension/src/index.ts:3164
+msgid "Collapse Selected Code"
+msgstr "Asugewählten Code reduzieren"
+
+#: packages/notebook-extension/src/index.ts:3175
+msgid "Expand Selected Code"
+msgstr "Asugewählten Code erweitern"
+
+#: packages/notebook-extension/src/index.ts:3186
+msgid "Collapse All Code"
+msgstr "Gesamten Code reduzieren"
+
+#: packages/notebook-extension/src/index.ts:3197
+msgid "Expand All Code"
+msgstr "Gesamten Code erweitern"
+
+#: packages/notebook-extension/src/index.ts:3208
+msgid "Collapse Selected Outputs"
+msgstr "Ausgewählte Ausgaben reduzieren"
+
+#: packages/notebook-extension/src/index.ts:3219
+msgid "Expand Selected Outputs"
+msgstr "Ausgewählte Ausgaben erweitern"
+
+#: packages/notebook-extension/src/index.ts:3230
+msgid "Collapse All Outputs"
+msgstr "Alle Ausgaben reduzieren"
+
+#: packages/notebook-extension/src/index.ts:3242
+msgid "Render Side-by-Side"
+msgstr ""
+
+#: packages/notebook-extension/src/index.ts:3264
+msgid "Expand All Outputs"
+msgstr "Alle Ausgaben erweitern"
+
+#: packages/notebook-extension/src/index.ts:3275
+msgid "Enable Scrolling for Outputs"
+msgstr "Scrollen für Ausgaben aktivieren"
+
+#: packages/notebook-extension/src/index.ts:3286
+msgid "Disable Scrolling for Outputs"
+msgstr "Scrollen für Ausgaben deaktivieren"
+
+#: packages/notebook-extension/src/index.ts:3297
+msgid "Select current running or last run cell"
+msgstr "Aktuelle laufende oder zuletzt ausgeführte Zelle auswählen"
+
+#: packages/notebook-extension/src/index.ts:3308
+msgid "Replace Selection in Notebook Cell"
+msgstr "Auswahl in Notebook Zelle ersetzen"
+
 #: packages/notebook-extension/src/index.ts:3320
 msgid "Toggle Collapse Notebook Heading"
 msgstr ""
 
 #: packages/notebook-extension/src/index.ts:3330 packages/toc-extension/src/index.ts:141
 msgid "Collapse All Headings"
 msgstr "Alle Überschriften einklappen"
@@ -6820,266 +6078,245 @@
 msgid "Expand All Headings"
 msgstr "Alle Überschriften ausklappen"
 
 #: packages/notebook-extension/src/index.ts:3349
 msgid "Select and Run Cell(s) for this Heading"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:504 packages/notebook-extension/src/index.ts:573
-msgid "Save and Export Notebook: %1"
-msgstr "Notebook speichern und exportieren: %1"
+#: packages/notebook-extension/src/index.ts:3399 packages/notebook-extension/src/index.ts:657
+msgid "Notebook Operations"
+msgstr "Notebook Operationen"
 
-#: packages/notebook-extension/src/index.ts:569
-msgid "Save and Export Notebook to the given `format`."
+#: packages/notebook-extension/src/index.ts:3435
+msgid "Notebook Cell Operations"
+msgstr "Notebook Zellen Operationen"
+
+#: packages/notebook-extension/src/index.ts:3680
+msgid "PDF"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:758
-msgid "Slides"
-msgstr "Folien"
+#: packages/notebook-extension/src/index.ts:3681
+msgid "ReStructured Text"
+msgstr "ReStructuredText"
 
-#: packages/notebook-extension/src/index.ts:759
-msgid "Script"
-msgstr "Skript"
+#: packages/notebook-extension/src/index.ts:3682
+msgid "Executable Script"
+msgstr "Ausführbares Skript"
 
-#: packages/notebook-extension/src/index.ts:761
-msgid "Custom"
+#: packages/notebook-extension/src/index.ts:3683
+msgid "Reveal.js Slides"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:943
-msgid "Create New View for Output"
+#: packages/notebook-extension/src/index.ts:3737
+msgid "For Notebook: %1"
+msgstr "Für Notebook: %1"
+
+#: packages/notebook-extension/src/index.ts:3738
+msgid "For Notebook:"
+msgstr "Für Notebook:"
+
+#: packages/notebook-extension/src/index.ts:569
+msgid "Save and Export Notebook to the given `format`."
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:1881 packages/notebook/src/actions.tsx:2026
+#: packages/notebook-extension/src/index.ts:573
+msgid "Save and Export Notebook: %1"
+msgstr "Notebook speichern und exportieren: %1"
+
+#: packages/notebook/src/actions.tsx:2032
 msgid "A trusted Jupyter notebook may execute hidden malicious code when you open it."
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:1885
-msgid "Selecting trust will re-render this notebook in a trusted state."
+#: packages/notebook/src/actions.tsx:2036
+msgid "Selecting \"Trust\" will re-render this notebook in a trusted state."
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:1889 packages/notebook/src/actions.tsx:2034
+#: packages/notebook/src/actions.tsx:2040
 msgid "For more information, see"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:1895 packages/notebook/src/actions.tsx:2040
+#: packages/notebook/src/actions.tsx:2046
 msgid "the Jupyter security documentation"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:1902 packages/notebook/src/actions.tsx:2048
+#: packages/notebook/src/actions.tsx:2054
 msgid "Notebook is already trusted"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:1909 packages/notebook/src/actions.tsx:2055
+#: packages/notebook/src/actions.tsx:2061
 msgid "Trust this notebook?"
 msgstr "Diesem Notebook vertrauen?"
 
-#: packages/notebook/src/actions.tsx:1978
-msgid "Notebook is still rendering and has for now (%1) remaining cells to render.\n\n"
-"Please wait for the complete rendering before invoking that action."
-msgstr ""
-
-#: packages/notebook/src/actions.tsx:2030
-msgid "Selecting \"Trust\" will re-render this notebook in a trusted state."
-msgstr ""
-
-#: packages/notebook/src/actions.tsx:2058
+#: packages/notebook/src/actions.tsx:2064
 msgid "Trust"
 msgstr "Vertrauen"
 
-#: packages/notebook/src/actions.tsx:2150 packages/notebook/src/actions.tsx:2273
+#: packages/notebook/src/actions.tsx:2279
 msgid "Kernel Terminating"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2151 packages/notebook/src/actions.tsx:2274
+#: packages/notebook/src/actions.tsx:2280
 msgid "The kernel for %1 appears to be terminating. You can not run any cell for now."
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2161 packages/notebook/src/actions.tsx:2284
+#: packages/notebook/src/actions.tsx:2290
 msgid "Cell not executed due to pending input"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2162 packages/notebook/src/actions.tsx:2285
+#: packages/notebook/src/actions.tsx:2291
 msgid "The cell has not been executed to avoid kernel deadlock as there is another pending input! Submit your pending input and try again."
 msgstr ""
 
-#: packages/notebook/src/default-toolbar.tsx:355 packages/notebook/src/default-toolbar.tsx:374
+#: packages/notebook/src/default-toolbar.tsx:141
+msgid "Cut the selected cells"
+msgstr "Markierte Zellen ausschneiden"
+
+#: packages/notebook/src/default-toolbar.tsx:161
+msgid "Copy the selected cells"
+msgstr "Markierte Zellen kopieren"
+
+#: packages/notebook/src/default-toolbar.tsx:181
+msgid "Paste cells from the clipboard"
+msgstr "Zellen aus der Zwischenablage einfügen"
+
+#: packages/notebook/src/default-toolbar.tsx:207
+msgid "Run the selected cells and advance"
+msgstr ""
+
+#: packages/notebook/src/default-toolbar.tsx:238
+msgid "Restart the kernel, then re-run the whole notebook"
+msgstr ""
+
+#: packages/notebook/src/default-toolbar.tsx:374
 msgid "Cell type"
 msgstr "Zellentyp"
 
-#: packages/notebook/src/default-toolbar.tsx:356 packages/notebook/src/default-toolbar.tsx:375
+#: packages/notebook/src/default-toolbar.tsx:375
 msgid "Select the cell type"
 msgstr ""
 
-#: packages/notebook/src/default-toolbar.tsx:359 packages/notebook/src/default-toolbar.tsx:378
+#: packages/notebook/src/default-toolbar.tsx:378
 msgid "Code"
 msgstr "Code"
 
-#: packages/notebook/src/default-toolbar.tsx:361 packages/notebook/src/default-toolbar.tsx:380
+#: packages/notebook/src/default-toolbar.tsx:380
 msgid "Raw"
 msgstr "Roh"
 
-#: packages/notebook/src/default-toolbar.tsx:86 packages/notebook/src/default-toolbar.tsx:87
+#: packages/notebook/src/default-toolbar.tsx:87
 msgid "Save the notebook contents and create checkpoint"
 msgstr "Speichern des Notebook-Inhalts und Erstellen eines Kontrollpunkts"
 
-#: packages/notebook/src/executionindicator.tsx:127 packages/notebook/src/executionindicator.tsx:129 packages/notebook/src/executionindicator.tsx:145 packages/notebook/src/executionindicator.tsx:147
+#: packages/notebook/src/executionindicator.tsx:129 packages/notebook/src/executionindicator.tsx:147
 msgid "Elapsed time: %1 second"
 msgid_plural "Elapsed time: %1 seconds"
 msgstr[0] "Vergangene Zeit: %1 Sekunde"
 msgstr[1] "Vergangene Zeit: %1 Sekunden"
 
-#: packages/notebook/src/executionindicator.tsx:138 packages/notebook/src/executionindicator.tsx:140
+#: packages/notebook/src/executionindicator.tsx:140
 msgid "Executed %1 cell"
 msgid_plural "Executed %1 cells"
 msgstr[0] "%1 Zelle ausgeführt"
 msgstr[1] "%1 Zellen ausgeführt"
 
 #: packages/notebook/src/executionindicator.tsx:71
 msgid "Kernel status"
 msgstr "Kernel-Status"
 
-#: packages/notebook/src/executionindicator.tsx:73 packages/notebook/src/executionindicator.tsx:75
+#: packages/notebook/src/executionindicator.tsx:75
 msgid "Kernel status: %1"
 msgstr "Kernel-Status: %1"
 
-#: packages/notebook/src/model.ts:350 packages/notebook/src/model.ts:354
+#: packages/notebook/src/model.ts:354
 msgid "This notebook has been converted from an older notebook format (v%1)\n"
 "to the current notebook format (v%2).\n"
 "The next time you save this notebook, the current notebook format (v%2) will be used.\n"
 "'Older versions of Jupyter may not be able to read the new format.' To preserve the original format version,\n"
 "close the notebook without saving it."
 msgstr ""
 
-#: packages/notebook/src/model.ts:360 packages/notebook/src/model.ts:364
+#: packages/notebook/src/model.ts:364
 msgid "This notebook has been converted from an newer notebook format (v%1)\n"
 "to the current notebook format (v%2).\n"
 "The next time you save this notebook, the current notebook format (v%2) will be used.\n"
 "Some features of the original notebook may not be available.' To preserve the original format version,\n"
 "close the notebook without saving it."
 msgstr "Dieses Notebook wurde von einem neueren Notebookformat (v%1)\n"
 "in das aktuelle Notebookformat (v%2) konvertiert.\n"
 "Wenn du dieses Notebook das nächste Mal speicherst, wird das aktuelle Notebookformat (v%2) verwendet.\n"
 "Möglicherweise sind einige Funktionen des ursprünglichen Notebooks nicht verfügbar. Um die ursprüngliche Formatversion beizubehalten, schließe das Notebook ohne es zu speichern."
 
-#: packages/notebook/src/model.ts:371 packages/notebook/src/model.ts:375
+#: packages/notebook/src/model.ts:375
 msgid "Notebook converted"
 msgstr "Notizbuch konvertiert"
 
-#: packages/notebook/src/modestatus.tsx:24 packages/notebook/src/modestatus.tsx:29
+#: packages/notebook/src/modestatus.tsx:29
 msgid "Mode: %1"
 msgstr "Modus: %1"
 
-#: packages/notebook/src/modestatus.tsx:66 packages/notebook/src/modestatus.tsx:71 packages/shortcuts-extension/src/components/TopNav.tsx:181 packages/shortcuts-extension/src/components/TopNav.tsx:273
+#: packages/notebook/src/modestatus.tsx:71 packages/shortcuts-extension/src/components/TopNav.tsx:181
 msgid "Command"
 msgstr "Befehl"
 
-#: packages/notebook/src/modestatus.tsx:67 packages/notebook/src/modestatus.tsx:72 packages/shortcuts-extension/src/components/ShortcutItem.tsx:61 packages/shortcuts-extension/src/components/ShortcutItem.tsx:80
+#: packages/notebook/src/modestatus.tsx:72 packages/shortcuts-extension/src/components/ShortcutItem.tsx:61
 msgid "Edit"
 msgstr "Editieren"
 
-#: packages/notebook/src/modestatus.tsx:78 packages/notebook/src/modestatus.tsx:83
+#: packages/notebook/src/modestatus.tsx:83
 msgid "Notebook is in %1 mode"
 msgstr "Notizbuch ist im %1 Modus"
 
 #: packages/notebook/src/notebookfooter.ts:24
 msgid "Click to add a cell."
 msgstr ""
 
-#: packages/notebook/src/notebooktools.ts:614
-msgid "Notebook Metadata"
-msgstr ""
-
-#: packages/notebook/src/notebooktools.ts:650
-msgid "Cell Metadata"
-msgstr "Zellen-Metadaten"
-
-#: packages/notebook/src/notebooktools.ts:78
-msgid "Advanced Tools"
-msgstr "Erweiterte Werkzeuge"
-
-#: packages/notebook/src/notebooktools.ts:918
-msgid "Slide Type"
-msgstr ""
-
-#: packages/notebook/src/notebooktools.ts:921
-msgid "Slide"
-msgstr "Folie"
-
-#: packages/notebook/src/notebooktools.ts:922
-msgid "Sub-Slide"
-msgstr "Unter-Folie"
-
-#: packages/notebook/src/notebooktools.ts:923
-msgid "Fragment"
-msgstr ""
-
-#: packages/notebook/src/notebooktools.ts:924
-msgid "Skip"
-msgstr "Überspringen"
-
-#: packages/notebook/src/notebooktools.ts:925
-msgid "Notes"
-msgstr "Notizen"
-
-#: packages/notebook/src/notebooktools.ts:963
-msgid "Raw NBConvert Format"
-msgstr "Raw-NBConvert-Format"
-
-#: packages/notebook/src/panel.ts:208 packages/notebook/src/panel.ts:214
+#: packages/notebook/src/panel.ts:229
 msgid "Kernel Restarting"
 msgstr ""
 
-#: packages/notebook/src/panel.ts:209 packages/notebook/src/panel.ts:215
+#: packages/notebook/src/panel.ts:230
 msgid "The kernel for %1 appears to have died. It will restart automatically."
 msgstr ""
 
-#: packages/notebook/src/searchprovider.ts:223
+#: packages/notebook/src/searchprovider.ts:226
+msgid "Search Cell Outputs"
+msgstr "Suche Zellausgaben"
+
+#: packages/notebook/src/searchprovider.ts:227
 msgid "Search in the cell outputs."
 msgstr ""
 
-#: packages/notebook/src/searchprovider.ts:230
+#: packages/notebook/src/searchprovider.ts:234
 msgid "Search in %1 Selected Cell"
 msgid_plural "Search in %1 Selected Cells"
 msgstr[0] ""
 msgstr[1] ""
 
-#: packages/notebook/src/searchprovider.ts:235
+#: packages/notebook/src/searchprovider.ts:239
 msgid "Search in %1 Selected Line"
 msgid_plural "Search in %1 Selected Lines"
 msgstr[0] ""
 msgstr[1] ""
 
-#: packages/notebook/src/searchprovider.ts:240
+#: packages/notebook/src/searchprovider.ts:244
 msgid "Search only in the selected cells or text (depending on edit/command mode)."
 msgstr ""
 
-#: packages/notebook/src/searchprovider.ts:500
+#: packages/notebook/src/searchprovider.ts:510
 msgid "Searching outputs is expensive and requires to first rendered all outputs. Are you sure you want to search in the cell outputs?"
 msgstr ""
 
-#: packages/notebook/src/truststatus.tsx:21
-msgid "Notebook trusted: %1 of %2 cells trusted."
-msgstr "Notebook vertrauenswürdig: %1 von %2 Zellen vertrauenswürdig."
-
-#: packages/notebook/src/truststatus.tsx:30
-msgid "Active cell trusted: %1 of %2 cells trusted."
-msgstr "Aktive Zelle vertrauenswürdig: %1 von %2 Zellen vertrauenswürdig."
-
 #: packages/notebook/src/truststatus.tsx:30
 msgid "Notebook trusted: %1 of %2 code cells trusted."
 msgstr ""
 
 #: packages/notebook/src/truststatus.tsx:36
 msgid "Active cell trusted: %1 of %2 code cells trusted."
 msgstr ""
 
-#: packages/notebook/src/truststatus.tsx:39
-msgid "Notebook not trusted: %1 of %2 cells trusted."
-msgstr "Notebook nicht vertrauenswürdig: %1 von %2 Zellen vertrauenswürdig."
-
 #: packages/notebook/src/truststatus.tsx:42
 msgid "Notebook not trusted: %1 of %2 code cells trusted."
 msgstr ""
 
 #: packages/notebook/src/widget.ts:439
 msgid "The notebook is empty. Click the + button on the toolbar to add a new cell."
 msgstr ""
@@ -7092,35 +6329,35 @@
 msgid "Toggle output scrolling"
 msgstr ""
 
 #: packages/outputarea/src/widget.ts:605
 msgid "Javascript Error: %1"
 msgstr "Javascript-Fehler: %1"
 
-#: packages/property-inspector/src/index.ts:170 packages/property-inspector/src/index.ts:189
+#: packages/property-inspector/src/index.ts:189
 msgid "No properties to inspect."
 msgstr "Keine Eigenschaften zu inspizieren."
 
-#: packages/rendermime-extension/src/index.ts:58 packages/rendermime-extension/src/index.ts:67
+#: packages/rendermime-extension/src/index.ts:67
 msgid "Handle Local Link"
 msgstr ""
 
-#: packages/rendermime/src/renderers.ts:62 packages/rendermime/src/renderers.ts:66
+#: packages/rendermime/src/renderers.ts:62
 msgid "This HTML output contains inline scripts. Are you sure that you want to run arbitrary Javascript within your JupyterLab session?"
 msgstr ""
 
-#: packages/rendermime/src/widgets.ts:420 packages/rendermime/src/widgets.ts:428
+#: packages/rendermime/src/widgets.ts:428
 msgid "JavaScript output is disabled in JupyterLab"
 msgstr ""
 
-#: packages/running-extension/src/index.ts:54 packages/running-extension/src/index.ts:66
+#: packages/running-extension/src/index.ts:66
 msgid "Running Terminals and Kernels"
 msgstr "Laufende Terminals und Kernel"
 
-#: packages/running-extension/src/index.ts:57 packages/running-extension/src/index.ts:69
+#: packages/running-extension/src/index.ts:69
 msgid "Running Sessions section"
 msgstr ""
 
 #: packages/running-extension/src/index.ts:86
 msgid "Sessions and Tabs"
 msgstr ""
 
@@ -7129,116 +6366,86 @@
 msgstr ""
 
 #: packages/running-extension/src/kernels.ts:250
 msgid "%1\n"
 "Path: %2"
 msgstr ""
 
-#: packages/running-extension/src/kernels.ts:30 packages/running-extension/src/kernels.ts:49
+#: packages/running-extension/src/kernels.ts:49
 msgid "Kernels"
 msgstr "Kernel"
 
-#: packages/running-extension/src/kernels.ts:41 packages/running-extension/src/kernels.ts:68
+#: packages/running-extension/src/kernels.ts:68
 msgid "Are you sure you want to permanently shut down all running kernels?"
 msgstr ""
 
 #: packages/running-extension/src/kernels.ts:77
 msgid "New Console for Kernel"
 msgstr ""
 
-#: packages/running-extension/src/kernels.ts:80
-msgid "Path: %1\n"
-"Kernel: %2"
-msgstr "Pfad: %1\n"
-"Kernel: %2"
-
 #: packages/running-extension/src/kernels.ts:88
 msgid "New Notebook for Kernel"
 msgstr ""
 
-#: packages/running-extension/src/opentabs.ts:70 packages/running-extension/src/opentabs.ts:71
+#: packages/running-extension/src/opentabs.ts:70
 msgid "Open Tabs"
 msgstr "Offene Tabs"
 
-#: packages/running-extension/src/opentabs.ts:87 packages/running-extension/src/opentabs.ts:88
+#: packages/running-extension/src/opentabs.ts:87
 msgid "Close All"
 msgstr "Alle schließen"
 
-#: packages/running-extension/src/opentabs.ts:88 packages/running-extension/src/opentabs.ts:89
+#: packages/running-extension/src/opentabs.ts:88
 msgid "Are you sure you want to close all open tabs?"
 msgstr ""
 
-#: packages/running/src/index.tsx:288 packages/running/src/index.tsx:443
+#: packages/running/src/index.tsx:443
 msgid "Refresh List"
 msgstr "Liste aktualisieren"
 
-#: packages/settingeditor-extension/src/index.ts:141 packages/settingeditor-extension/src/index.ts:145
+#: packages/settingeditor-extension/src/index.ts:145
 msgid "JSON Settings Editor"
 msgstr ""
 
-#: packages/settingeditor-extension/src/index.ts:148 packages/settingeditor-extension/src/index.ts:152 packages/settingeditor-extension/src/index.ts:183 packages/settingeditor-extension/src/index.ts:187 packages/settingeditor-extension/src/index.ts:312 packages/settingeditor-extension/src/index.ts:319 packages/settingeditor/src/jsonsettingeditor.tsx:67 packages/settingeditor/src/pluginlist.tsx:455 packages/settingeditor/src/pluginlist.tsx:467
+#: packages/settingeditor-extension/src/index.ts:152 packages/settingeditor-extension/src/index.ts:187 packages/settingeditor-extension/src/index.ts:319 packages/settingeditor/src/pluginlist.tsx:467
 msgid "Settings"
 msgstr "Einstellungen"
 
-#: packages/settingeditor-extension/src/index.ts:177 packages/settingeditor-extension/src/index.ts:302 packages/settingeditor-extension/src/index.ts:309 packages/settingeditor-extension/src/index.ts:315
-msgid "Advanced Settings Editor"
-msgstr "Editor für erweiterte Einstellungen"
-
 #: packages/settingeditor-extension/src/index.ts:181
 msgid "Settings Editor"
 msgstr ""
 
-#: packages/settingeditor-extension/src/index.ts:308
-msgid "Advanced JSON Settings Editor"
-msgstr ""
+#: packages/settingeditor-extension/src/index.ts:309 packages/settingeditor-extension/src/index.ts:315
+msgid "Advanced Settings Editor"
+msgstr "Editor für erweiterte Einstellungen"
 
-#: packages/settingeditor-extension/src/index.ts:322 packages/settingeditor-extension/src/index.ts:329
+#: packages/settingeditor-extension/src/index.ts:329
 msgid "Revert User Settings"
 msgstr "Benutzereinstellungen zurücksetzen"
 
-#: packages/settingeditor-extension/src/index.ts:329 packages/settingeditor-extension/src/index.ts:336
+#: packages/settingeditor-extension/src/index.ts:336
 msgid "Save User Settings"
 msgstr "Benutzereinstellungen speichern"
 
 #: packages/settingeditor/src/InstructionsPlaceholder.tsx:21
 msgid "No Plugin Selected"
 msgstr ""
 
-#: packages/settingeditor/src/InstructionsPlaceholder.tsx:23 packages/settingeditor/src/jsonsettingeditor.tsx:71
+#: packages/settingeditor/src/InstructionsPlaceholder.tsx:23
 msgid "Select a plugin from the list to view and edit its preferences."
 msgstr "Wähle eine Erweiterung aus der Liste aus, um ihre Einstellungen anzuzeigen und zu bearbeiten."
 
-#: packages/settingeditor/src/SettingsFormEditor.tsx:158
-msgid "Move Up"
-msgstr "Nach oben verschieben"
-
-#: packages/settingeditor/src/SettingsFormEditor.tsx:165
-msgid "Move Down"
-msgstr "Nach unten verschieben"
-
-#: packages/settingeditor/src/SettingsFormEditor.tsx:166 packages/settingeditor/src/SettingsFormEditor.tsx:441
+#: packages/settingeditor/src/SettingsFormEditor.tsx:172
 msgid "Error saving settings."
 msgstr ""
 
-#: packages/settingeditor/src/SettingsFormEditor.tsx:172 packages/settingeditor/src/SettingsFormEditor.tsx:348 packages/ui-components/src/components/form.tsx:183 packages/ui-components/src/components/form.tsx:570
-msgid "Remove"
-msgstr "Entfernen"
-
-#: packages/settingeditor/src/SettingsFormEditor.tsx:183 packages/settingeditor/src/SettingsFormEditor.tsx:225 packages/shortcuts-extension/src/components/ShortcutItem.tsx:416 packages/shortcuts-extension/src/components/ShortcutItem.tsx:432 packages/shortcuts-extension/src/components/ShortcutItem.tsx:66 packages/shortcuts-extension/src/components/ShortcutItem.tsx:71 packages/shortcuts-extension/src/components/ShortcutItem.tsx:85 packages/shortcuts-extension/src/components/ShortcutItem.tsx:90 packages/ui-components/src/components/form.tsx:212
-msgid "Add"
-msgstr "Hinzufügen"
-
-#: packages/settingeditor/src/SettingsFormEditor.tsx:197 packages/settingeditor/src/SettingsFormEditor.tsx:485
+#: packages/settingeditor/src/SettingsFormEditor.tsx:205
 msgid "Restore to Defaults"
 msgstr ""
 
-#: packages/settingeditor/src/SettingsFormEditor.tsx:356 packages/ui-components/src/components/form.tsx:580
-msgid "Default: %1"
-msgstr "Standard: %1"
-
 #: packages/settingeditor/src/inspector.ts:114
 msgid "additional property error"
 msgstr ""
 
 #: packages/settingeditor/src/inspector.ts:115
 msgid "`%1` is not a valid property"
 msgstr ""
@@ -7259,131 +6466,135 @@
 msgid "Any errors will be listed here"
 msgstr "Alle Fehler werden hier aufgelistet"
 
 #: packages/settingeditor/src/inspector.ts:90
 msgid "No errors found"
 msgstr "Keine Fehler gefunden"
 
-#: packages/settingeditor/src/plugineditor.ts:129 packages/settingeditor/src/plugineditor.ts:134
+#: packages/settingeditor/src/plugineditor.ts:129
 msgid "You have unsaved changes."
 msgstr "Du hast nicht gespeicherte Änderungen."
 
-#: packages/settingeditor/src/plugineditor.ts:130 packages/settingeditor/src/plugineditor.ts:135
+#: packages/settingeditor/src/plugineditor.ts:130
 msgid "Do you want to leave without saving?"
 msgstr ""
 
-#: packages/settingeditor/src/plugineditor.ts:255 packages/settingeditor/src/plugineditor.ts:257
+#: packages/settingeditor/src/plugineditor.ts:255
 msgid "Your changes were not saved."
 msgstr "Ihre Änderungen wurden nicht gespeichert."
 
-#: packages/settingeditor/src/pluginlist.tsx:442 packages/settingeditor/src/pluginlist.tsx:454 packages/shortcuts-extension/src/components/TopNav.tsx:167
+#: packages/settingeditor/src/pluginlist.tsx:454 packages/shortcuts-extension/src/components/TopNav.tsx:167
 msgid "Search…"
 msgstr "Suchen…"
 
-#: packages/settingeditor/src/pluginlist.tsx:449 packages/settingeditor/src/pluginlist.tsx:461
+#: packages/settingeditor/src/pluginlist.tsx:461
 msgid "Modified"
 msgstr "Geändert"
 
-#: packages/settingeditor/src/pluginlist.tsx:461 packages/settingeditor/src/pluginlist.tsx:473
+#: packages/settingeditor/src/pluginlist.tsx:473
 msgid "No items match your search."
 msgstr ""
 
-#: packages/settingeditor/src/raweditor.ts:368 packages/settingeditor/src/raweditor.ts:377
+#: packages/settingeditor/src/raweditor.ts:368
 msgid "System Defaults"
 msgstr "System-Standardeinstellungen"
 
-#: packages/settingeditor/src/raweditor.ts:409 packages/settingeditor/src/raweditor.ts:418
+#: packages/settingeditor/src/raweditor.ts:409
 msgid "User Preferences"
 msgstr "Benutzereinstellungen"
 
-#: packages/settingeditor/src/settingseditor.tsx:118 packages/settingeditor/src/settingseditor.tsx:123
+#: packages/settingeditor/src/settingseditor.tsx:123
 msgid "Unsaved changes due to validation error. Continue without saving?"
 msgstr ""
 
-#: packages/settingeditor/src/settingseditor.tsx:130 packages/settingeditor/src/settingseditor.tsx:135
+#: packages/settingeditor/src/settingseditor.tsx:135
 msgid "Some changes have not been saved. Continue without saving?"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutInput.tsx:445 packages/shortcuts-extension/src/components/ShortcutInput.tsx:451
+#: packages/shortcuts-extension/src/components/ShortcutInput.tsx:445
 msgid "press keys"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:218 packages/shortcuts-extension/src/components/ShortcutItem.tsx:241
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:218
 msgid "Shortcut already in use by %1. Overwrite it?"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:260 packages/shortcuts-extension/src/components/ShortcutItem.tsx:281 packages/shortcuts-extension/src/components/ShortcutItem.tsx:76 packages/shortcuts-extension/src/components/ShortcutItem.tsx:95
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:260 packages/shortcuts-extension/src/components/ShortcutItem.tsx:76
 msgid "Reset"
 msgstr "Zurücksetzen"
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:332 packages/shortcuts-extension/src/components/ShortcutItem.tsx:348
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:332
 msgid "or"
 msgstr "oder"
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:51 packages/shortcuts-extension/src/components/ShortcutItem.tsx:70
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:416 packages/shortcuts-extension/src/components/ShortcutItem.tsx:66 packages/shortcuts-extension/src/components/ShortcutItem.tsx:71 packages/ui-components/src/components/form.tsx:212
+msgid "Add"
+msgstr "Hinzufügen"
+
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:51
 msgid "Edit First"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:52 packages/shortcuts-extension/src/components/ShortcutItem.tsx:57 packages/shortcuts-extension/src/components/ShortcutItem.tsx:62 packages/shortcuts-extension/src/components/ShortcutItem.tsx:71 packages/shortcuts-extension/src/components/ShortcutItem.tsx:76 packages/shortcuts-extension/src/components/ShortcutItem.tsx:81
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:52 packages/shortcuts-extension/src/components/ShortcutItem.tsx:57 packages/shortcuts-extension/src/components/ShortcutItem.tsx:62
 msgid "Edit existing shortcut"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:56 packages/shortcuts-extension/src/components/ShortcutItem.tsx:75
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:56
 msgid "Edit Second"
 msgstr "Zweite bearbeiten"
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:67 packages/shortcuts-extension/src/components/ShortcutItem.tsx:86
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:67
 msgid "Add new shortcut"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:72 packages/shortcuts-extension/src/components/ShortcutItem.tsx:91
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:72
 msgid "Add another shortcut"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:77 packages/shortcuts-extension/src/components/ShortcutItem.tsx:96
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:77
 msgid "Reset shortcut back to default"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:126 packages/shortcuts-extension/src/components/TopNav.tsx:207
+#: packages/shortcuts-extension/src/components/TopNav.tsx:126
 msgid "Toggle Selectors"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:127 packages/shortcuts-extension/src/components/TopNav.tsx:208
+#: packages/shortcuts-extension/src/components/TopNav.tsx:127
 msgid "Toggle command selectors"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:136 packages/shortcuts-extension/src/components/TopNav.tsx:149 packages/shortcuts-extension/src/components/TopNav.tsx:171 packages/shortcuts-extension/src/components/TopNav.tsx:217 packages/shortcuts-extension/src/components/TopNav.tsx:92
+#: packages/shortcuts-extension/src/components/TopNav.tsx:136 packages/shortcuts-extension/src/components/TopNav.tsx:92
 msgid "Reset All"
 msgstr "Alle zurücksetzen"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:137 packages/shortcuts-extension/src/components/TopNav.tsx:218
+#: packages/shortcuts-extension/src/components/TopNav.tsx:137
 msgid "Reset all shortcuts"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:142 packages/shortcuts-extension/src/components/TopNav.tsx:164 packages/shortcuts-extension/src/components/TopNav.tsx:85
-msgid "Hide Selectors"
-msgstr ""
-
-#: packages/shortcuts-extension/src/components/TopNav.tsx:143 packages/shortcuts-extension/src/components/TopNav.tsx:165 packages/shortcuts-extension/src/components/TopNav.tsx:86
-msgid "Show Selectors"
-msgstr ""
-
-#: packages/shortcuts-extension/src/components/TopNav.tsx:180 packages/shortcuts-extension/src/components/TopNav.tsx:272
+#: packages/shortcuts-extension/src/components/TopNav.tsx:180
 msgid "Category"
 msgstr "Kategorie"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:183 packages/shortcuts-extension/src/components/TopNav.tsx:275
+#: packages/shortcuts-extension/src/components/TopNav.tsx:183
 msgid "Shortcut"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:187 packages/shortcuts-extension/src/components/TopNav.tsx:279
+#: packages/shortcuts-extension/src/components/TopNav.tsx:187
 msgid "Selectors"
 msgstr "Selektoren"
 
-#: packages/shortcuts-extension/src/index.ts:136 packages/shortcuts-extension/src/index.ts:143
+#: packages/shortcuts-extension/src/components/TopNav.tsx:85
+msgid "Hide Selectors"
+msgstr ""
+
+#: packages/shortcuts-extension/src/components/TopNav.tsx:86
+msgid "Show Selectors"
+msgstr ""
+
+#: packages/shortcuts-extension/src/index.ts:143
 msgid "Note: To disable a system default shortcut,\n"
 "copy it to User Preferences and add the\n"
 "\"disabled\" key, for example:\n"
 "{\n"
 "    \"command\": \"application:activate-next-tab\",\n"
 "    \"keys\": [\n"
 "        \"Ctrl Shift ]\"\n"
@@ -7392,52 +6603,44 @@
 "    \"disabled\": true\n"
 "}\n\n"
 "List of commands followed by keyboard shortcuts:\n"
 "%1\n\n"
 "List of keyboard shortcuts:"
 msgstr ""
 
-#: packages/statusbar-extension/src/index.ts:52 packages/statusbar-extension/src/index.ts:78
+#: packages/statusbar-extension/src/index.ts:52
 msgid "Show Status Bar"
 msgstr "Statusleiste anzeigen"
 
-#: packages/statusbar/src/defaults/kernelStatus.tsx:126
-msgid "No Kernel!"
-msgstr "Kein Kernel!"
-
-#: packages/terminal-extension/src/index.ts:103 packages/terminal-extension/src/index.ts:350 packages/terminal-extension/src/index.ts:99 packages/terminal/src/widget.ts:102 packages/terminal/src/widget.ts:74
+#: packages/terminal-extension/src/index.ts:103 packages/terminal-extension/src/index.ts:350 packages/terminal/src/widget.ts:102
 msgid "Terminal"
 msgstr "Terminal"
 
-#: packages/terminal-extension/src/index.ts:187 packages/terminal-extension/src/index.ts:191
+#: packages/terminal-extension/src/index.ts:191
 msgctxt "menu"
 msgid "Terminal Theme"
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:192 packages/terminal-extension/src/index.ts:196 packages/terminal-extension/src/index.ts:251 packages/terminal-extension/src/index.ts:534 packages/terminal-extension/src/index.ts:544
+#: packages/terminal-extension/src/index.ts:196 packages/terminal-extension/src/index.ts:251 packages/terminal-extension/src/index.ts:534
 msgid "Inherit"
 msgstr "Vererben"
 
-#: packages/terminal-extension/src/index.ts:200 packages/terminal-extension/src/index.ts:204 packages/terminal-extension/src/index.ts:258 packages/terminal-extension/src/index.ts:535 packages/terminal-extension/src/index.ts:545
+#: packages/terminal-extension/src/index.ts:204 packages/terminal-extension/src/index.ts:258 packages/terminal-extension/src/index.ts:535
 msgid "Light"
 msgstr "Hell"
 
-#: packages/terminal-extension/src/index.ts:206 packages/terminal-extension/src/index.ts:210 packages/terminal-extension/src/index.ts:263 packages/terminal-extension/src/index.ts:536 packages/terminal-extension/src/index.ts:546
+#: packages/terminal-extension/src/index.ts:210 packages/terminal-extension/src/index.ts:263 packages/terminal-extension/src/index.ts:536
 msgid "Dark"
 msgstr "Dunkel"
 
-#: packages/terminal-extension/src/index.ts:228 packages/terminal-extension/src/index.ts:492
-msgid "Shutdown Terminal"
-msgstr "Terminal herunterfahren"
-
-#: packages/terminal-extension/src/index.ts:296 packages/terminal-extension/src/index.ts:316
+#: packages/terminal-extension/src/index.ts:316
 msgid "Terminals"
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:304 packages/terminal-extension/src/index.ts:324
+#: packages/terminal-extension/src/index.ts:324
 msgid "Are you sure you want to permanently shut down all running terminals?"
 msgstr "Bist du sicher, dass du alle laufenden Terminals herunterfahren möchtest?"
 
 #: packages/terminal-extension/src/index.ts:350
 msgid "New Terminal"
 msgstr "Neues Terminal"
 
@@ -7445,110 +6648,82 @@
 msgid "Start a new terminal session"
 msgstr "Eine neue Terminal-Sitzung starten"
 
 #: packages/terminal-extension/src/index.ts:389
 msgid "Open a terminal by its `name`."
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:407 packages/terminal-extension/src/index.ts:415
+#: packages/terminal-extension/src/index.ts:407
 msgid "Refresh Terminal"
 msgstr "Terminal aktualisieren"
 
-#: packages/terminal-extension/src/index.ts:408 packages/terminal-extension/src/index.ts:416
+#: packages/terminal-extension/src/index.ts:408
 msgid "Refresh the current terminal session"
 msgstr "Aktualisiere die aktuelle Terminal-Sitzung"
 
-#: packages/terminal-extension/src/index.ts:506 packages/terminal-extension/src/index.ts:516
+#: packages/terminal-extension/src/index.ts:492
+msgid "Shutdown Terminal"
+msgstr "Terminal herunterfahren"
+
+#: packages/terminal-extension/src/index.ts:506
 msgid "Increase Terminal Font Size"
 msgstr "Terminal-Schriftgröße erhöhen"
 
-#: packages/terminal-extension/src/index.ts:520 packages/terminal-extension/src/index.ts:530
+#: packages/terminal-extension/src/index.ts:520
 msgid "Decrease Terminal Font Size"
 msgstr "Terminal-Schriftgröße verringern"
 
 #: packages/terminal-extension/src/index.ts:542
 msgid "Set terminal theme to the provided `theme`."
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:550 packages/terminal-extension/src/index.ts:557
+#: packages/terminal-extension/src/index.ts:550
 msgid "Use Terminal Theme: %1"
 msgstr "Verwende Terminal-Theme: %1"
 
-#: packages/terminal-extension/src/index.ts:553 packages/terminal-extension/src/index.ts:560
+#: packages/terminal-extension/src/index.ts:553
 msgid "Set the terminal theme"
 msgstr "Terminal-Theme festlegen"
 
-#: packages/terminal/src/widget.ts:110 packages/terminal/src/widget.ts:345
+#: packages/terminal/src/widget.ts:345
 msgid "Terminal %1"
 msgstr "Terminal %1"
 
-#: packages/theme-dark-extension/src/index.ts:30 packages/theme-dark-extension/src/index.ts:31
+#: packages/theme-dark-extension/src/index.ts:31
 msgid "JupyterLab Dark"
 msgstr "JupyterLab Dunkel"
 
-#: packages/theme-light-extension/src/index.ts:30 packages/theme-light-extension/src/index.ts:31
+#: packages/theme-light-extension/src/index.ts:31
 msgid "JupyterLab Light"
 msgstr "JupyterLab Hell"
 
 #: packages/toc-extension/src/index.ts:113
 msgid "Show output headings"
 msgstr ""
 
-#: packages/toc-extension/src/index.ts:127 packages/toc-extension/src/index.ts:77 packages/toc-extension/src/index.ts:83 packages/toc/src/panel.ts:28 packages/toc/src/panel.ts:79 packages/toc/src/toc.tsx:130
+#: packages/toc-extension/src/index.ts:127 packages/toc-extension/src/index.ts:77 packages/toc/src/panel.ts:28 packages/toc/src/panel.ts:79
 msgid "Table of Contents"
 msgstr "Inhaltsverzeichnis"
 
-#: packages/toc-extension/src/index.ts:129
-msgid "Run Cell(s)"
-msgstr ""
-
 #: packages/toc-extension/src/index.ts:242
 msgid "More actions…"
 msgstr ""
 
-#: packages/toc-extension/src/index.ts:80 packages/toc-extension/src/index.ts:86
+#: packages/toc-extension/src/index.ts:80
 msgid "Table of Contents section"
 msgstr ""
 
 #: packages/toc-extension/src/index.ts:83
 msgid "Show first-level heading number"
 msgstr ""
 
 #: packages/toc-extension/src/index.ts:97
 msgid "Show heading number in the document"
 msgstr ""
 
-#: packages/toc/src/generators/markdown/toolbar_generator.tsx:64 packages/toc/src/generators/markdown/toolbar_generator.tsx:65 packages/toc/src/generators/notebook/toolbar_generator.tsx:214 packages/toc/src/generators/notebook/toolbar_generator.tsx:215
-msgid "Toggle Auto-Numbering"
-msgstr "Auto-Nummerierung umschalten"
-
-#: packages/toc/src/generators/notebook/tagstool/index.tsx:217
-msgid "No Tags Available"
-msgstr "Keine Tags verfügbar"
-
-#: packages/toc/src/generators/notebook/tagstool/index.tsx:224
-msgid "Clear Filters"
-msgstr "Filter löschen"
-
-#: packages/toc/src/generators/notebook/tagstool/index.tsx:255 packages/toc/src/generators/notebook/tagstool/index.tsx:256 packages/toc/src/generators/notebook/tagstool/index.tsx:258 packages/toc/src/generators/notebook/tagstool/index.tsx:266 packages/toc/src/generators/notebook/tagstool/index.tsx:267 packages/toc/src/generators/notebook/tagstool/index.tsx:271
-msgid "Select All Cells With Current Tags"
-msgstr ""
-
-#: packages/toc/src/generators/notebook/toolbar_generator.tsx:182 packages/toc/src/generators/notebook/toolbar_generator.tsx:183
-msgid "Toggle Code Cells"
-msgstr "Code-Zellen umschalten"
-
-#: packages/toc/src/generators/notebook/toolbar_generator.tsx:198 packages/toc/src/generators/notebook/toolbar_generator.tsx:199
-msgid "Toggle Markdown Text Cells"
-msgstr "Markdown Textzellen umschalten"
-
-#: packages/toc/src/generators/notebook/toolbar_generator.tsx:230 packages/toc/src/generators/notebook/toolbar_generator.tsx:231
-msgid "Show Tags Menu"
-msgstr "Tags-Menü anzeigen"
-
 #: packages/toc/src/panel.ts:32
 msgid "No Headings"
 msgstr ""
 
 #: packages/toc/src/panel.ts:33
 msgid "The table of contents shows headings in notebooks and supported files."
 msgstr ""
@@ -7557,23 +6732,23 @@
 msgid "Open the tooltip"
 msgstr ""
 
 #: packages/tooltip-extension/src/index.ts:56
 msgid "Dismiss the tooltip"
 msgstr ""
 
-#: packages/translation-extension/src/index.ts:132 packages/translation-extension/src/index.ts:141
+#: packages/translation-extension/src/index.ts:141
 msgid "Change interface language?"
 msgstr "Interfacesprache ändern?"
 
-#: packages/translation-extension/src/index.ts:133 packages/translation-extension/src/index.ts:142
+#: packages/translation-extension/src/index.ts:142
 msgid "After changing the interface language to %1, you will need to reload JupyterLab to see the changes."
 msgstr ""
 
-#: packages/translation-extension/src/index.ts:139 packages/translation-extension/src/index.ts:148
+#: packages/translation-extension/src/index.ts:148
 msgid "Change and reload"
 msgstr ""
 
 #: packages/translation-extension/src/index.ts:175
 msgid "Display Languages"
 msgstr ""
 
@@ -7581,14 +6756,22 @@
 msgid "Move down"
 msgstr ""
 
 #: packages/ui-components/src/components/form.tsx:146
 msgid "Move up"
 msgstr ""
 
+#: packages/ui-components/src/components/form.tsx:183 packages/ui-components/src/components/form.tsx:570
+msgid "Remove"
+msgstr "Entfernen"
+
+#: packages/ui-components/src/components/form.tsx:580
+msgid "Default: %1"
+msgstr "Standard: %1"
+
 #: packages/ui-components/src/components/sidepanel.ts:118
 msgid "side panel actions"
 msgstr ""
 
 #: packages/ui-components/src/components/sidepanel.ts:41
 msgid "side panel content"
 msgstr ""
```

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_git.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_git.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_lsp.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_lsp.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_search_replace.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_search_replace.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_spreadsheet_editor.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_spreadsheet_editor.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_tour.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_tour.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_widgets.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupyterlab_widgets.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupytext.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/jupytext.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/notebook.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/notebook.po`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: de\n"
 "X-Crowdin-File: /main/extensions/notebook/locale/notebook.pot\n"
 "X-Crowdin-File-ID: 231\n"
 "Language-Team: German\n"
 "Language: de_DE\n"
-"PO-Revision-Date: 2023-04-30 17:13\n"
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
 msgstr "Umbenennen…"
 
 #: packages/application-extension/src/index.ts:481
 msgid "Show Header"
 msgstr "Kopfzeile anzeigen"
 
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
 msgstr "Linke Seitenleiste"
 
-#: packages/application-extension/src/index.ts:691
+#: packages/application-extension/src/index.ts:698
 msgid "Right Sidebar"
 msgstr "Rechte Seitenleiste"
 
-#: packages/application-extension/src/index.ts:880
+#: packages/application-extension/src/index.ts:887
 msgid "Toggle Zen Mode"
 msgstr "Zen-Modus umschalten"
 
-#: packages/application/src/shell.ts:196 packages/application/src/shell.ts:200
+#: packages/application/src/shell.ts:203 packages/application/src/shell.ts:207
 msgid "Collapse %1 side panel"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:116
+#: packages/help-extension/src/index.tsx:114
 msgid "Version: %1"
 msgstr "Version: %1"
 
-#: packages/help-extension/src/index.tsx:117
+#: packages/help-extension/src/index.tsx:115
 msgid "© 2021-2023 Jupyter Notebook Contributors"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:133 packages/help-extension/src/index.tsx:215
+#: packages/help-extension/src/index.tsx:131
 msgid "Dismiss"
 msgstr "Verwerfen"
 
-#: packages/help-extension/src/index.tsx:174 packages/help-extension/src/index.tsx:79 packages/lab-extension/src/index.ts:162
+#: packages/help-extension/src/index.tsx:77 packages/lab-extension/src/index.ts:178
 msgid "Help"
 msgstr "Hilfe"
 
-#: packages/help-extension/src/index.tsx:177 packages/help-extension/src/index.tsx:182
-msgid "Keyboard Shortcuts"
-msgstr ""
-
-#: packages/help-extension/src/index.tsx:191
-msgid "Name"
-msgstr "Name"
-
-#: packages/help-extension/src/index.tsx:192
-msgid "Shortcut"
-msgstr ""
-
-#: packages/help-extension/src/index.tsx:82
+#: packages/help-extension/src/index.tsx:80
 msgid "About %1"
 msgstr "Über %1"
 
-#: packages/help-extension/src/index.tsx:94
+#: packages/help-extension/src/index.tsx:92
 msgid "JUPYTER NOTEBOOK ON GITHUB"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:95
+#: packages/help-extension/src/index.tsx:93
 msgid "CONTRIBUTOR LIST"
 msgstr ""
 
-#: packages/lab-extension/src/index.ts:117 packages/lab-extension/src/index.ts:126
-msgid "Open With %1"
-msgstr "Mit %1 öffnen"
+#: packages/lab-extension/src/index.ts:131
+msgid "Notebook"
+msgstr ""
+
+#: packages/lab-extension/src/index.ts:132 packages/lab-extension/src/index.ts:142
+msgid "Open in %1"
+msgstr ""
+
+#: packages/lab-extension/src/index.ts:141
+msgid "JupyterLab"
+msgstr ""
 
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

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/retrolab.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/retrolab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/spellchecker.po` & `jupyterlab_language_pack_de_de-4.0.post0/jupyterlab_language_pack_de_DE/locale/de_DE/LC_MESSAGES/spellchecker.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/.gitignore` & `jupyterlab_language_pack_de_de-4.0.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/LICENSE.txt` & `jupyterlab_language_pack_de_de-4.0.post0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/pyproject.toml` & `jupyterlab_language_pack_de_de-4.0.post0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 keywords = ["jupyterlab", "language", "language pack", "localization"]
 dynamic = ["version"]
 
 [project.entry-points."jupyterlab.languagepack"]
 de_DE = "jupyterlab_language_pack_de_DE"
 
-[projects.urls]
+[project.urls]
 homepage = "https://github.com/jupyterlab/language-packs"
 
 [tool.hatch.build]
 artifacts = [
     "CONTRIBUTORS.md"
 ]
```

### Comparing `jupyterlab_language_pack_de_de-3.6.post3/PKG-INFO` & `jupyterlab_language_pack_de_de-4.0.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: jupyterlab-language-pack-de-DE
-Version: 3.6.post3
+Version: 4.0.post0
 Summary: JupyterLab German (Germany) Language Pack
+Project-URL: homepage, https://github.com/jupyterlab/language-packs
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2023 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

