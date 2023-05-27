# Comparing `tmp/jupyterlab_language_pack_ja_jp-3.6.post3.tar.gz` & `tmp/jupyterlab_language_pack_ja_jp-4.0.post0.tar.gz`

## Comparing `jupyterlab_language_pack_ja_jp-3.6.post3.tar` & `jupyterlab_language_pack_ja_jp-4.0.post0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/.copier-answers.yml
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/CONTRIBUTORS.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/dask_labextension.po
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyter_archive.po
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyter_collaboration.po
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyter_resource_usage.po
--rw-r--r--   0        0        0   303477 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab.po
--rw-r--r--   0        0        0    96103 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_git.po
--rw-r--r--   0        0        0    42484 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_lsp.po
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_search_replace.po
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_tour.po
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_widgets.po
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupytext.po
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/notebook.po
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/retrolab.po
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/spellchecker.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/LICENSE.txt
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/README.md
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/pyproject.toml
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-3.6.post3/PKG-INFO
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/.copier-answers.yml
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/dask_labextension.po
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyter_archive.po
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyter_collaboration.po
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyter_resource_usage.po
+-rw-r--r--   0        0        0   222164 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab.po
+-rw-r--r--   0        0        0    96103 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_git.po
+-rw-r--r--   0        0        0    42484 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_lsp.po
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_search_replace.po
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_tour.po
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_widgets.po
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupytext.po
+-rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/notebook.po
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/retrolab.po
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/spellchecker.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/LICENSE.txt
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/README.md
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/pyproject.toml
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ja_jp-4.0.post0/PKG-INFO
```

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/CONTRIBUTORS.md` & `jupyterlab_language_pack_ja_jp-4.0.post0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/dask_labextension.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/dask_labextension.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyter_archive.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyter_archive.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyter_resource_usage.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyter_resource_usage.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab.po`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: ja\n"
 "X-Crowdin-File: /main/jupyterlab/locale/jupyterlab.pot\n"
 "X-Crowdin-File-ID: 191\n"
 "Language-Team: Japanese\n"
 "Language: ja_JP\n"
-"PO-Revision-Date: 2023-04-28 15:38\n"
+"PO-Revision-Date: 2023-05-21 14:18\n"
 
 #: /examples/federated/md_package/schema/plugin.json:/description /packages/markdownviewer-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Markdown viewer settings."
 msgstr "Markdown ビューアの設定。"
 
 #: /examples/federated/md_package/schema/plugin.json:/jupyter.lab.setting-icon-label /packages/markdownviewer-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
@@ -27,27 +27,27 @@
 #: /examples/federated/md_package/schema/plugin.json:/properties/fontFamily/description /packages/markdownviewer-extension/schema/plugin.json:/properties/fontFamily/description
 msgctxt "settings"
 msgid "The font family used to render markdown.\n"
 "If `null`, value from current theme is used."
 msgstr "Markdownのレンダリングに使用する行の高さ。\n"
 "`null`の場合、現在のテーマの値が使用される。"
 
-#: /examples/federated/md_package/schema/plugin.json:/properties/fontFamily/title /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/fontFamily/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/fontFamily/title /packages/markdownviewer-extension/schema/plugin.json:/properties/fontFamily/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/fontFamily/title
+#: /examples/federated/md_package/schema/plugin.json:/properties/fontFamily/title /packages/markdownviewer-extension/schema/plugin.json:/properties/fontFamily/title
 msgctxt "settings"
 msgid "Font Family"
 msgstr "フォントの種類"
 
 #: /examples/federated/md_package/schema/plugin.json:/properties/fontSize/description /packages/markdownviewer-extension/schema/plugin.json:/properties/fontSize/description
 msgctxt "settings"
 msgid "The size in pixel of the font used to render markdown.\n"
 "If `null`, value from current theme is used."
 msgstr "マークダウンの表示に使用されるフォントのピクセルサイズ。\n"
 "「null」の場合、現在のテーマの値が使用されます。"
 
-#: /examples/federated/md_package/schema/plugin.json:/properties/fontSize/title /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/fontSize/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/fontSize/title /packages/markdownviewer-extension/schema/plugin.json:/properties/fontSize/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/fontSize/title
+#: /examples/federated/md_package/schema/plugin.json:/properties/fontSize/title /packages/markdownviewer-extension/schema/plugin.json:/properties/fontSize/title
 msgctxt "settings"
 msgid "Font Size"
 msgstr "フォントサイズ"
 
 #: /examples/federated/md_package/schema/plugin.json:/properties/hideFrontMatter/description /packages/markdownviewer-extension/schema/plugin.json:/properties/hideFrontMatter/description
 msgctxt "settings"
 msgid "Whether to hide YAML front matter.\n"
@@ -67,15 +67,15 @@
 #: /examples/federated/md_package/schema/plugin.json:/properties/lineHeight/description /packages/markdownviewer-extension/schema/plugin.json:/properties/lineHeight/description
 msgctxt "settings"
 msgid "The line height used to render markdown.\n"
 "If `null`, value from current theme is used."
 msgstr "マークダウンの表示に使用される行の高さ。\n"
 "「null」の場合、現在のテーマの値が使用されます。"
 
-#: /examples/federated/md_package/schema/plugin.json:/properties/lineHeight/title /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/lineHeight/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/lineHeight/title /packages/markdownviewer-extension/schema/plugin.json:/properties/lineHeight/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/lineHeight/title
+#: /examples/federated/md_package/schema/plugin.json:/properties/lineHeight/title /packages/markdownviewer-extension/schema/plugin.json:/properties/lineHeight/title
 msgctxt "settings"
 msgid "Line Height"
 msgstr "行の高さ"
 
 #: /examples/federated/md_package/schema/plugin.json:/properties/lineWidth/description /packages/markdownviewer-extension/schema/plugin.json:/properties/lineWidth/description
 msgctxt "settings"
 msgid "The text line width expressed in CSS ch units.\n"
@@ -284,58 +284,29 @@
 "}。"
 
 #: /packages/application-extension/schema/shell.json:/properties/layout/title
 msgctxt "settings"
 msgid "Customize shell widget positioning"
 msgstr "シェルウィジェットの位置をカスタマイズする"
 
-#: /packages/application-extension/schema/shell.json:/properties/startMode/description /packages/statusbar-extension/schema/plugin.json:/properties/startMode/description
+#: /packages/application-extension/schema/shell.json:/properties/startMode/description
 msgctxt "settings"
 msgid "The mode under which JupyterLab should start. If empty, the mode will be imposed by the URL"
 msgstr "JupyterLabが起動するモード。空の場合、モードはURLによって設定されます。"
 
 #: /packages/application-extension/schema/shell.json:/properties/startMode/title
 msgctxt "settings"
 msgid "Start mode: ``, `single` or `multiple`"
 msgstr "起動モード: ``, `single` または `multiple`"
 
 #: /packages/application-extension/schema/shell.json:/title
 msgctxt "schema"
 msgid "JupyterLab Shell"
 msgstr "JupyterLabシェル"
 
-#: /packages/application-extension/schema/sidebar.json:/description
-msgctxt "schema"
-msgid "Sidebar layout settings."
-msgstr "サイドバーのレイアウト設定。"
-
-#: /packages/application-extension/schema/sidebar.json:/jupyter.lab.setting-icon-label
-msgctxt "settings"
-msgid "Sidebar"
-msgstr "サイドバー"
-
-#: /packages/application-extension/schema/sidebar.json:/properties/overrides/description
-msgctxt "settings"
-msgid "Overrides for where to show sidebar items\n"
-"e.g., {\"jp-debugger-sidebar\": \"left\"}\n"
-"You can also change this by right-clicking the sidebar icons."
-msgstr "サイドバーアイテムを表示する位置の設定\n"
-"例: {\"jp-debugger-sidebar\": \"left\"}\n"
-"サイドバーのアイコンを右クリックして、変更することもできます。"
-
-#: /packages/application-extension/schema/sidebar.json:/properties/overrides/title
-msgctxt "settings"
-msgid "Overrides"
-msgstr "アイテム表示位置"
-
-#: /packages/application-extension/schema/sidebar.json:/title
-msgctxt "schema"
-msgid "Sidebar"
-msgstr "サイドバー"
-
 #: /packages/application-extension/schema/top-bar.json:/definitions/toolbarItem/properties/disabled/title /packages/cell-toolbar-extension/schema/plugin.json:/definitions/toolbarItem/properties/disabled/title /packages/csvviewer-extension/schema/csv.json:/definitions/toolbarItem/properties/disabled/title /packages/csvviewer-extension/schema/tsv.json:/definitions/toolbarItem/properties/disabled/title /packages/filebrowser-extension/schema/widget.json:/definitions/toolbarItem/properties/disabled/title /packages/fileeditor-extension/schema/plugin.json:/definitions/toolbarItem/properties/disabled/title /packages/htmlviewer-extension/schema/plugin.json:/definitions/toolbarItem/properties/disabled/title /packages/notebook-extension/schema/panel.json:/definitions/toolbarItem/properties/disabled/title
 msgctxt "settings"
 msgid "Whether the item is ignored or not"
 msgstr "メニューが無効かどうか"
 
 #: /packages/application-extension/schema/top-bar.json:/definitions/toolbarItem/properties/icon/description /packages/cell-toolbar-extension/schema/plugin.json:/definitions/toolbarItem/properties/icon/description /packages/csvviewer-extension/schema/csv.json:/definitions/toolbarItem/properties/icon/description /packages/csvviewer-extension/schema/tsv.json:/definitions/toolbarItem/properties/icon/description /packages/filebrowser-extension/schema/widget.json:/definitions/toolbarItem/properties/icon/description /packages/fileeditor-extension/schema/plugin.json:/definitions/toolbarItem/properties/icon/description /packages/htmlviewer-extension/schema/plugin.json:/definitions/toolbarItem/properties/icon/description /packages/notebook-extension/schema/panel.json:/definitions/toolbarItem/properties/icon/description
 msgctxt "settings"
@@ -614,159 +585,38 @@
 msgstr ""
 
 #: /packages/celltags-extension/schema/plugin.json:/title /packages/notebook-extension/schema/tools.json:/title
 msgctxt "schema"
 msgid "Common tools"
 msgstr ""
 
-#: /packages/codemirror-extension/schema/commands.json:/description /packages/codemirror-extension/schema/plugin.json:/description
+#: /packages/codemirror-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Text editor settings for all CodeMirror editors."
 msgstr "すべてのCodeMirrorエディタのテキストエディタの設定。"
 
-#: /packages/codemirror-extension/schema/commands.json:/jupyter.lab.menus/main[0]/items[1]/submenu/label /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[1]/items[1]/submenu/label
-msgctxt "menu"
-msgid "Text Editor Syntax Highlighting"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/jupyter.lab.menus/main[1]/items[0]/submenu/label
-msgctxt "menu"
-msgid "Text Editor Key Map"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/jupyter.lab.menus/main[1]/items[1]/submenu/label /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[2]/items[5]/submenu/label
-msgctxt "menu"
-msgid "Text Editor Theme"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/jupyter.lab.setting-icon-label /packages/codemirror-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
-msgctxt "settings"
-msgid "CodeMirror"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/keyMap/description
-msgctxt "settings"
-msgid "Configures the keymap to use"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/keyMap/title
-msgctxt "settings"
-msgid "Key Map"
-msgstr "キーマップ"
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/lineWiseCopyCut/description /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWiseCopyCut/description /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWiseCopyCut/description
-msgctxt "settings"
-msgid "When enabled, which is the default, doing copy or cut when there is no selection will copy or cut the whole lines that have cursors on them."
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/lineWiseCopyCut/title /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWiseCopyCut/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWiseCopyCut/title
-msgctxt "settings"
-msgid "Line-wise Ctrl-C"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/scrollPastEnd/description
-msgctxt "settings"
-msgid "Whether to scroll past the end of text document"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/scrollPastEnd/title /packages/fileeditor-extension/schema/plugin.json:/properties/scrollPastEnd/title
-msgctxt "settings"
-msgid "Scroll behavior"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/selectionPointer/description
-msgctxt "settings"
-msgid "Control the mouse cursor appearance when hovering over the selection. Value is boolean or string, e.g. 'pointer'."
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/selectionPointer/oneOf[0]/title
-msgctxt "settings"
-msgid "Use default"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/selectionPointer/oneOf[1]/title
-msgctxt "settings"
-msgid "Cursor pointer name"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/selectionPointer/title
-msgctxt "settings"
-msgid "Selection Pointer"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/styleActiveLine/description
-msgctxt "settings"
-msgid "Highlight active line. Value is boolean, or { nonEmpty: boolean }."
-msgstr ""
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
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/styleSelectedText/title
-msgctxt "settings"
-msgid "Style Selected Text"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/theme/description
-msgctxt "settings"
-msgid "CSS file defining the corresponding\n"
-".cm-s-[name] styles is loaded"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/properties/theme/title /packages/terminal-extension/schema/plugin.json:/properties/theme/title
+#: /packages/codemirror-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
-msgid "Theme"
-msgstr ""
-
-#: /packages/codemirror-extension/schema/commands.json:/title /packages/codemirror-extension/schema/plugin.json:/title
-msgctxt "schema"
 msgid "CodeMirror"
 msgstr ""
 
 #: /packages/codemirror-extension/schema/plugin.json:/properties/defaultConfig/description
 msgctxt "settings"
 msgid "Base configuration used by all CodeMirror editors."
 msgstr ""
 
 #: /packages/codemirror-extension/schema/plugin.json:/properties/defaultConfig/title
 msgctxt "settings"
 msgid "Default editor configuration"
 msgstr ""
 
-#: /packages/completer-extension/schema/consoles.json:/description /packages/console-extension/schema/completer.json:/description
-msgctxt "schema"
-msgid "Console completer settings."
-msgstr "コンソール入力補完設定。"
-
-#: /packages/completer-extension/schema/consoles.json:/title /packages/console-extension/schema/completer.json:/title
-msgctxt "schema"
-msgid "Console Completer"
-msgstr "コンソール入力補完"
-
-#: /packages/completer-extension/schema/files.json:/description /packages/fileeditor-extension/schema/completer.json:/description
-msgctxt "schema"
-msgid "File editor completer settings."
-msgstr "ファイルエディタ入力補完設定。"
-
-#: /packages/completer-extension/schema/files.json:/title /packages/fileeditor-extension/schema/completer.json:/title
+#: /packages/codemirror-extension/schema/plugin.json:/title
 msgctxt "schema"
-msgid "File Editor Completer"
-msgstr "ファイルエディタ入力補完"
+msgid "CodeMirror"
+msgstr ""
 
 #: /packages/completer-extension/schema/manager.json:/description
 msgctxt "schema"
 msgid "Code Completion settings."
 msgstr ""
 
 #: /packages/completer-extension/schema/manager.json:/jupyter.lab.setting-icon-label
@@ -815,94 +665,34 @@
 msgstr ""
 
 #: /packages/completer-extension/schema/manager.json:/title
 msgctxt "schema"
 msgid "Code Completion"
 msgstr ""
 
-#: /packages/completer-extension/schema/notebooks.json:/description /packages/notebook-extension/schema/completer.json:/description
+#: /packages/console-extension/schema/completer.json:/description
 msgctxt "schema"
-msgid "Notebook completer settings."
-msgstr "Notebook入力補完設定。"
+msgid "Console completer settings."
+msgstr "コンソール入力補完設定。"
 
-#: /packages/completer-extension/schema/notebooks.json:/title /packages/notebook-extension/schema/completer.json:/title
+#: /packages/console-extension/schema/completer.json:/title
 msgctxt "schema"
-msgid "Notebook Completer"
-msgstr "Notebook入力補完"
+msgid "Console Completer"
+msgstr "コンソール入力補完"
 
 #: /packages/console-extension/schema/foreign.json:/description
 msgctxt "schema"
 msgid "Code Console Foreign plugin settings."
 msgstr ""
 
 #: /packages/console-extension/schema/foreign.json:/title
 msgctxt "schema"
 msgid "Code Console Foreign plugin"
 msgstr ""
 
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/autoClosingBrackets/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/autoClosingBrackets/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/autoClosingBrackets/title
-msgctxt "settings"
-msgid "Auto Closing Brackets"
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/codeFolding/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/codeFolding/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/codeFolding/title
-msgctxt "settings"
-msgid "Code Folding"
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/cursorBlinkRate/description /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/cursorBlinkRate/description /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/cursorBlinkRate/description
-msgctxt "settings"
-msgid "Half-period in milliseconds used for cursor blinking. The default blink rate is 530ms. By setting this to zero, blinking can be disabled. A negative value hides the cursor entirely."
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/cursorBlinkRate/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/cursorBlinkRate/title
-msgctxt "settings"
-msgid "Cursor Blinking Rate"
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/insertSpaces/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/insertSpaces/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/insertSpaces/title
-msgctxt "settings"
-msgid "Insert Spaces"
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/lineNumbers/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/lineNumbers/title
-msgctxt "settings"
-msgid "Show Line Numbers"
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWrap/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/lineWrap/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWrap/title
-msgctxt "settings"
-msgid "Line Wrap"
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/matchBrackets/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/matchBrackets/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/matchBrackets/title
-msgctxt "settings"
-msgid "Match Brackets"
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/readOnly/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/readOnly/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/readOnly/title
-msgctxt "settings"
-msgid "Read Only"
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/rulers/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/rulers/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/rulers/title
-msgctxt "settings"
-msgid "Rulers"
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/tabSize/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/tabSize/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/tabSize/title
-msgctxt "settings"
-msgid "Tab Size"
-msgstr "タブサイズ"
-
-#: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/wordWrapColumn/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/wordWrapColumn/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/wordWrapColumn/title
-msgctxt "settings"
-msgid "Word Wrap Column"
-msgstr ""
-
 #: /packages/console-extension/schema/tracker.json:/description
 msgctxt "schema"
 msgid "Code Console settings."
 msgstr "コード コンソールの設定。"
 
 #: /packages/console-extension/schema/tracker.json:/jupyter.lab.menus/main[1]/items[1]/submenu/label
 msgctxt "menu"
@@ -923,19 +713,14 @@
 #: /packages/console-extension/schema/tracker.json:/properties/interactionMode/title
 msgctxt "settings"
 msgid "Interaction mode"
 msgstr ""
 
 #: /packages/console-extension/schema/tracker.json:/properties/promptCellConfig/description
 msgctxt "settings"
-msgid "The configuration for all prompt cells."
-msgstr ""
-
-#: /packages/console-extension/schema/tracker.json:/properties/promptCellConfig/description
-msgctxt "settings"
 msgid "The configuration for all prompt cells; it will override the CodeMirror default configuration."
 msgstr ""
 
 #: /packages/console-extension/schema/tracker.json:/properties/promptCellConfig/title
 msgctxt "settings"
 msgid "Prompt Cell Configuration"
 msgstr ""
@@ -1194,61 +979,25 @@
 msgstr ""
 
 #: /packages/extensionmanager-extension/schema/plugin.json:/properties/disclaimed/title
 msgctxt "settings"
 msgid "Disclaimed Status"
 msgstr ""
 
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
 msgstr ""
 
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
 msgstr "拡張機能マネージャ"
 
 #: /packages/filebrowser-extension/schema/browser.json:/description
 msgctxt "schema"
@@ -1298,19 +1047,14 @@
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showFileSizeColumn/title
 msgctxt "settings"
 msgid "Show file size column"
 msgstr ""
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showHiddenFiles/description
 msgctxt "settings"
-msgid "Whether to show hidden files"
-msgstr ""
-
-#: /packages/filebrowser-extension/schema/browser.json:/properties/showHiddenFiles/description
-msgctxt "settings"
 msgid "Whether to show hidden files. The server parameter `ContentsManager.allow_hidden` must be set to `True` to display hidden files."
 msgstr ""
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showHiddenFiles/title
 msgctxt "settings"
 msgid "Show hidden files"
 msgstr ""
@@ -1402,53 +1146,51 @@
 msgstr ""
 
 #: /packages/filebrowser-extension/schema/widget.json:/title
 msgctxt "schema"
 msgid "File Browser Widget"
 msgstr ""
 
-#: /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/cursorBlinkRate/title
-msgctxt "settings"
-msgid "Cursor blinking rate"
-msgstr "カーソル点滅周期"
-
-#: /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/lineNumbers/title
-msgctxt "settings"
-msgid "Line Numbers"
-msgstr "行番号"
+#: /packages/fileeditor-extension/schema/completer.json:/description
+msgctxt "schema"
+msgid "File editor completer settings."
+msgstr "ファイルエディタ入力補完設定。"
 
-#: /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/showTrailingSpace/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/showTrailingSpace/title
-msgctxt "settings"
-msgid "Show Trailing Space"
-msgstr "末尾の空白を表示"
+#: /packages/fileeditor-extension/schema/completer.json:/title
+msgctxt "schema"
+msgid "File Editor Completer"
+msgstr "ファイルエディタ入力補完"
 
 #: /packages/fileeditor-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Text editor settings."
 msgstr "テキストエディタの設定。"
 
-#: /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[1]/items[1]/submenu/label /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[2]/items[1]/submenu/label
+#: /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[1]/items[1]/submenu/label
+msgctxt "menu"
+msgid "Text Editor Syntax Highlighting"
+msgstr ""
+
+#: /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[2]/items[1]/submenu/label
 msgctxt "menu"
 msgid "Text Editor Indentation"
 msgstr "テキストエディタのインデント"
 
+#: /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.menus/main[2]/items[5]/submenu/label
+msgctxt "menu"
+msgid "Text Editor Theme"
+msgstr ""
+
 #: /packages/fileeditor-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "Editor"
 msgstr "エディタ"
 
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
@@ -1456,14 +1198,19 @@
 msgstr "エディタ設定"
 
 #: /packages/fileeditor-extension/schema/plugin.json:/properties/scrollPastEnd/description
 msgctxt "settings"
 msgid "Whether to scroll past the end of text document."
 msgstr ""
 
+#: /packages/fileeditor-extension/schema/plugin.json:/properties/scrollPastEnd/title
+msgctxt "settings"
+msgid "Scroll behavior"
+msgstr ""
+
 #: /packages/fileeditor-extension/schema/plugin.json:/properties/toolbar/description
 msgctxt "settings"
 msgid "Note: To disable a toolbar item,\n"
 "copy it to User Preferences and add the\n"
 "\"disabled\" key. Toolbar description:"
 msgstr ""
 
@@ -1540,20 +1287,20 @@
 msgstr ""
 
 #: /packages/htmlviewer-extension/schema/plugin.json:/title
 msgctxt "schema"
 msgid "HTML Viewer"
 msgstr "HTMLビュワー"
 
-#: /packages/hub-extension/schema/menu.json:/description /packages/hub-extension/schema/plugin.json:/description
+#: /packages/hub-extension/schema/menu.json:/description
 msgctxt "schema"
 msgid "JupyterHub settings."
 msgstr "JupyterHubの設定。"
 
-#: /packages/hub-extension/schema/menu.json:/title /packages/hub-extension/schema/plugin.json:/title
+#: /packages/hub-extension/schema/menu.json:/title
 msgctxt "schema"
 msgid "JupyterHub"
 msgstr ""
 
 #: /packages/imageviewer-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Image viewer settings."
@@ -1853,14 +1600,24 @@
 msgstr ""
 
 #: /packages/metadataform-extension/schema/metadataforms.json:/title
 msgctxt "schema"
 msgid "Metadata Form"
 msgstr ""
 
+#: /packages/notebook-extension/schema/completer.json:/description
+msgctxt "schema"
+msgid "Notebook completer settings."
+msgstr "Notebook入力補完設定。"
+
+#: /packages/notebook-extension/schema/completer.json:/title
+msgctxt "schema"
+msgid "Notebook Completer"
+msgstr "Notebook入力補完"
+
 #: /packages/notebook-extension/schema/export.json:/description
 msgctxt "schema"
 msgid "Notebook Export settings."
 msgstr "Notebookエキスポート設定。"
 
 #: /packages/notebook-extension/schema/export.json:/jupyter.lab.menus/main[0]/items[1]/submenu/label
 msgctxt "menu"
@@ -1936,19 +1693,14 @@
 #: /packages/notebook-extension/schema/tracker.json:/properties/autoStartDefaultKernel/title
 msgctxt "settings"
 msgid "Automatically Start Preferred Kernel"
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/codeCellConfig/description
 msgctxt "settings"
-msgid "The configuration for all code cells."
-msgstr ""
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/codeCellConfig/description
-msgctxt "settings"
 msgid "The configuration for all code cells; it will override the CodeMirror default configuration."
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/codeCellConfig/title
 msgctxt "settings"
 msgid "Code Cell Configuration"
 msgstr ""
@@ -1969,24 +1721,14 @@
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
@@ -2011,19 +1753,14 @@
 #: /packages/notebook-extension/schema/tracker.json:/properties/kernelStatus/title
 msgctxt "settings"
 msgid "Kernel status icon configuration"
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/markdownCellConfig/description
 msgctxt "settings"
-msgid "The configuration for all markdown cells."
-msgstr ""
-
-#: /packages/notebook-extension/schema/tracker.json:/properties/markdownCellConfig/description
-msgctxt "settings"
 msgid "The configuration for all markdown cells; it will override the CodeMirror default configuration."
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/markdownCellConfig/title
 msgctxt "settings"
 msgid "Markdown Cell Configuration"
 msgstr ""
@@ -2034,61 +1771,26 @@
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
-msgstr ""
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
@@ -2099,34 +1801,14 @@
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/recordTiming/title
 msgctxt "settings"
 msgid "Recording timing"
 msgstr ""
 
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
@@ -2191,15 +1873,15 @@
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
 
@@ -2279,19 +1961,14 @@
 msgstr "ステータスバーの設定。"
 
 #: /packages/statusbar-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "Status Bar"
 msgstr "ステータスバー"
 
-#: /packages/statusbar-extension/schema/plugin.json:/properties/startMode/title
-msgctxt "settings"
-msgid "Start mode: ``, `single`or `multiple`"
-msgstr ""
-
 #: /packages/statusbar-extension/schema/plugin.json:/properties/visible/description
 msgctxt "settings"
 msgid "Whether to show status bar or not"
 msgstr ""
 
 #: /packages/statusbar-extension/schema/plugin.json:/properties/visible/title
 msgctxt "settings"
@@ -2404,74 +2081,44 @@
 msgstr ""
 
 #: /packages/terminal-extension/schema/plugin.json:/properties/theme/description
 msgctxt "settings"
 msgid "The theme for the terminal."
 msgstr ""
 
+#: /packages/terminal-extension/schema/plugin.json:/properties/theme/title
+msgctxt "settings"
+msgid "Theme"
+msgstr ""
+
 #: /packages/terminal-extension/schema/plugin.json:/title
 msgctxt "schema"
 msgid "Terminal"
 msgstr "ターミナル"
 
-#: /packages/toc-extension/schema/plugin.json:/description
+#: /packages/toc-extension/schema/registry.json:/description
 msgctxt "schema"
-msgid "Table of contents settings."
-msgstr "目次の設定。"
+msgid "Default table of contents settings."
+msgstr ""
 
-#: /packages/toc-extension/schema/plugin.json:/jupyter.lab.setting-icon-label /packages/toc-extension/schema/registry.json:/jupyter.lab.setting-icon-label
+#: /packages/toc-extension/schema/registry.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "Table of Contents"
 msgstr "目次"
 
-#: /packages/toc-extension/schema/plugin.json:/properties/includeOutput/description
+#: /packages/toc-extension/schema/registry.json:/properties/includeOutput/description
 msgctxt "settings"
-msgid "Whether to include cell output in headings"
+msgid "Whether to include cell output in headings or not."
 msgstr ""
 
-#: /packages/toc-extension/schema/plugin.json:/properties/includeOutput/title /packages/toc-extension/schema/registry.json:/properties/includeOutput/title
+#: /packages/toc-extension/schema/registry.json:/properties/includeOutput/title
 msgctxt "settings"
 msgid "Include cell output in headings"
 msgstr ""
 
-#: /packages/toc-extension/schema/plugin.json:/properties/numberingH1/description
-msgctxt "settings"
-msgid "Whether to number first-level headings"
-msgstr ""
-
-#: /packages/toc-extension/schema/plugin.json:/properties/numberingH1/title
-msgctxt "settings"
-msgid "Enable h1 numbering"
-msgstr ""
-
-#: /packages/toc-extension/schema/plugin.json:/properties/syncCollapseState/description
-msgctxt "settings"
-msgid "If set to true, when a header is collapsed in the table of contents the corresponding section in the notebook is collapsed as well and vice versa."
-msgstr ""
-
-#: /packages/toc-extension/schema/plugin.json:/properties/syncCollapseState/title /packages/toc-extension/schema/registry.json:/properties/syncCollapseState/title
-msgctxt "settings"
-msgid "Synchronize collapse state"
-msgstr ""
-
-#: /packages/toc-extension/schema/plugin.json:/title /packages/toc-extension/schema/registry.json:/title
-msgctxt "schema"
-msgid "Table of Contents"
-msgstr "目次"
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
@@ -2494,14 +2141,24 @@
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
+msgstr "目次"
+
 #: /packages/tooltip-extension/schema/consoles.json:/description
 msgctxt "schema"
 msgid "Console tooltip settings."
 msgstr "コンソールのツールチップの設定。"
 
 #: /packages/tooltip-extension/schema/consoles.json:/title
 msgctxt "schema"
@@ -2574,110 +2231,110 @@
 msgstr ""
 
 #: /packages/translation-extension/schema/plugin.json:/title
 msgctxt "schema"
 msgid "Language"
 msgstr "言語"
 
-#: packages/application-extension/src/index.tsx:1078 packages/application-extension/src/index.tsx:1083 packages/application-extension/src/index.tsx:933
+#: packages/application-extension/src/index.tsx:1078 packages/application-extension/src/index.tsx:1083
 msgid "Property Inspector"
 msgstr "プロパティインスペクタ"
 
-#: packages/application-extension/src/index.tsx:111 packages/application-extension/src/index.tsx:132 packages/apputils-extension/src/index.ts:308 packages/apputils-extension/src/index.ts:319 packages/documentsearch-extension/src/index.ts:254 packages/documentsearch-extension/src/index.ts:258 packages/documentsearch-extension/src/index.ts:262 packages/documentsearch-extension/src/index.ts:326 packages/logconsole-extension/src/index.tsx:242 packages/logconsole-extension/src/index.tsx:253 packages/mainmenu-extension/src/index.ts:228 packages/mainmenu-extension/src/index.ts:232 packages/mainmenu-extension/src/index.ts:236 packages/mainmenu-extension/src/index.ts:240 packages/mainmenu-extension/src/index.ts:242 packages/mainmenu-extension/src/index.ts:250 packages/statusbar-extension/src/index.ts:48 packages/statusbar-extension/src/index.ts:74
-msgid "Main Area"
-msgstr "メインエリア"
-
-#: packages/application-extension/src/index.tsx:115 packages/application-extension/src/index.tsx:136
-msgid "Shift+Right Click for Browser Menu"
-msgstr "Shift+右クリックでブラウザメニュー"
-
-#: packages/application-extension/src/index.tsx:1171 packages/statusbar-extension/src/index.ts:381
+#: packages/application-extension/src/index.tsx:1171
 msgid "Simple Interface (%1)"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:1173 packages/application-extension/src/index.tsx:340 packages/application-extension/src/index.tsx:385 packages/statusbar-extension/src/index.ts:383
+#: packages/application-extension/src/index.tsx:1173 packages/application-extension/src/index.tsx:385
 msgid "Simple Interface"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:1181 packages/statusbar-extension/src/index.ts:391
+#: packages/application-extension/src/index.tsx:1181
 msgid "Simple"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:1208 packages/application-extension/src/index.tsx:1402
-msgid "Switch Sidebar Side"
-msgstr "サイドバーの左右を切り替え"
-
-#: packages/application-extension/src/index.tsx:1220 packages/application-extension/src/index.tsx:791 packages/application-extension/src/index.tsx:989 packages/apputils/src/toolbar/factory.ts:28 packages/apputils/src/toolbar/factory.ts:33 packages/extensionmanager/src/model.ts:504 packages/extensionmanager/src/model.ts:526 packages/mainmenu-extension/src/index.ts:770 packages/mainmenu-extension/src/index.ts:942
+#: packages/application-extension/src/index.tsx:1220 packages/application-extension/src/index.tsx:791 packages/apputils/src/toolbar/factory.ts:33 packages/extensionmanager/src/model.ts:504 packages/extensionmanager/src/model.ts:526 packages/mainmenu-extension/src/index.ts:770
 msgid "Information"
 msgstr "情報"
 
-#: packages/application-extension/src/index.tsx:1221 packages/application-extension/src/index.tsx:990
+#: packages/application-extension/src/index.tsx:1221
 msgid "Context menu customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:1226 packages/application-extension/src/index.tsx:797 packages/application-extension/src/index.tsx:995 packages/apputils/src/toolbar/factory.ts:34 packages/apputils/src/toolbar/factory.ts:39 packages/docmanager-extension/src/index.tsx:654 packages/docmanager-extension/src/index.tsx:739 packages/docprovider/src/yprovider.ts:135 packages/mainmenu-extension/src/index.ts:776 packages/mainmenu-extension/src/index.ts:948
+#: packages/application-extension/src/index.tsx:1226 packages/application-extension/src/index.tsx:797 packages/apputils/src/toolbar/factory.ts:39 packages/docmanager-extension/src/index.tsx:739 packages/mainmenu-extension/src/index.ts:776
 msgid "Reload"
 msgstr "再読込"
 
-#: packages/application-extension/src/index.tsx:200 packages/application-extension/src/index.tsx:205
+#: packages/application-extension/src/index.tsx:132 packages/apputils-extension/src/index.ts:319 packages/documentsearch-extension/src/index.ts:326 packages/logconsole-extension/src/index.tsx:246 packages/mainmenu-extension/src/index.ts:236 packages/mainmenu-extension/src/index.ts:240 packages/mainmenu-extension/src/index.ts:250 packages/statusbar-extension/src/index.ts:48
+msgid "Main Area"
+msgstr "メインエリア"
+
+#: packages/application-extension/src/index.tsx:136
+msgid "Shift+Right Click for Browser Menu"
+msgstr "Shift+右クリックでブラウザメニュー"
+
+#: packages/application-extension/src/index.tsx:1402
+msgid "Switch Sidebar Side"
+msgstr "サイドバーの左右を切り替え"
+
+#: packages/application-extension/src/index.tsx:205
 msgid "Close Tab"
 msgstr "タブを閉じる"
 
-#: packages/application-extension/src/index.tsx:214 packages/application-extension/src/index.tsx:219
+#: packages/application-extension/src/index.tsx:219
 msgid "Close All Other Tabs"
 msgstr "他のすべてのタブを閉じる"
 
-#: packages/application-extension/src/index.tsx:234 packages/application-extension/src/index.tsx:239
+#: packages/application-extension/src/index.tsx:239
 msgid "Close Tabs to Right"
 msgstr "右側のタブをすべて閉じる"
 
-#: packages/application-extension/src/index.tsx:249 packages/application-extension/src/index.tsx:254
+#: packages/application-extension/src/index.tsx:254
 msgid "Activate Next Tab"
 msgstr "右のタブをアクティブにする"
 
-#: packages/application-extension/src/index.tsx:256 packages/application-extension/src/index.tsx:261
+#: packages/application-extension/src/index.tsx:261
 msgid "Activate Previous Tab"
 msgstr "左のタブをアクティブにする"
 
-#: packages/application-extension/src/index.tsx:263 packages/application-extension/src/index.tsx:268
+#: packages/application-extension/src/index.tsx:268
 msgid "Activate Next Tab Bar"
 msgstr "右のタブバーをアクティブにする"
 
-#: packages/application-extension/src/index.tsx:270 packages/application-extension/src/index.tsx:275
+#: packages/application-extension/src/index.tsx:275
 msgid "Activate Previous Tab Bar"
 msgstr "左のタブバーをアクティブにする"
 
-#: packages/application-extension/src/index.tsx:277 packages/application-extension/src/index.tsx:282
+#: packages/application-extension/src/index.tsx:282
 msgid "Close All Tabs"
 msgstr "すべてのタブを閉じる"
 
-#: packages/application-extension/src/index.tsx:284 packages/application-extension/src/index.tsx:300
-msgid "Show Left Sidebar"
-msgstr "左のサイドバーを表示"
-
 #: packages/application-extension/src/index.tsx:289
 msgid "Show Header"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:300 packages/application-extension/src/index.tsx:316
+#: packages/application-extension/src/index.tsx:300
+msgid "Show Left Sidebar"
+msgstr "左のサイドバーを表示"
+
+#: packages/application-extension/src/index.tsx:316
 msgid "Show Right Sidebar"
 msgstr "右のサイドバーを表示"
 
-#: packages/application-extension/src/index.tsx:316 packages/application-extension/src/index.tsx:354
-msgid "Presentation Mode"
-msgstr "プレゼンテーションモード"
-
 #: packages/application-extension/src/index.tsx:334
 msgid "Show Right Activity Bar"
 msgstr ""
 
 #: packages/application-extension/src/index.tsx:335
 msgid "Show Left Activity Bar"
 msgstr ""
 
+#: packages/application-extension/src/index.tsx:354
+msgid "Presentation Mode"
+msgstr "プレゼンテーションモード"
+
 #: packages/application-extension/src/index.tsx:365
 msgid "Set %1 mode."
 msgstr ""
 
 #: packages/application-extension/src/index.tsx:366
 msgid "Set the layout `mode`."
 msgstr ""
@@ -2686,530 +2343,526 @@
 msgid "The layout `mode` can be \"single-document\" or \"multiple-document\"."
 msgstr ""
 
 #: packages/application-extension/src/index.tsx:397
 msgid "Reset Default Layout"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:431 packages/application-extension/src/index.tsx:527
+#: packages/application-extension/src/index.tsx:527
 msgid "Error Registering Plugins"
 msgstr "プラグインの登録でエラーが発生"
 
-#: packages/application-extension/src/index.tsx:481 packages/application-extension/src/index.tsx:577 packages/extensionmanager/src/build-helper.tsx:27
+#: packages/application-extension/src/index.tsx:577
 msgid "Build Complete"
 msgstr "ビルド完了"
 
-#: packages/application-extension/src/index.tsx:484 packages/application-extension/src/index.tsx:580 packages/extensionmanager/src/build-helper.tsx:30
+#: packages/application-extension/src/index.tsx:580
 msgid "Build successfully completed, reload page?"
 msgstr "ビルドが正常に完了しました。ページを再読み込みしますか?"
 
-#: packages/application-extension/src/index.tsx:486 packages/application-extension/src/index.tsx:582 packages/extensionmanager/src/build-helper.tsx:32
+#: packages/application-extension/src/index.tsx:582
 msgid "You will lose any unsaved changes."
 msgstr "保存されていない変更は全て失なわれます。"
 
-#: packages/application-extension/src/index.tsx:491 packages/application-extension/src/index.tsx:587 packages/extensionmanager/src/build-helper.tsx:37
+#: packages/application-extension/src/index.tsx:587
 msgid "Reload Without Saving"
 msgstr "保存せずに再読み込み"
 
-#: packages/application-extension/src/index.tsx:494 packages/application-extension/src/index.tsx:590 packages/extensionmanager/src/build-helper.tsx:40
+#: packages/application-extension/src/index.tsx:590
 msgid "Save and Reload"
 msgstr "保存して再読み込み"
 
-#: packages/application-extension/src/index.tsx:507 packages/application-extension/src/index.tsx:603 packages/extensionmanager/src/build-helper.tsx:53
+#: packages/application-extension/src/index.tsx:603
 msgid "Save Failed"
 msgstr "保存に失敗しました"
 
-#: packages/application-extension/src/index.tsx:516 packages/application-extension/src/index.tsx:612 packages/extensionmanager/src/build-helper.tsx:63
+#: packages/application-extension/src/index.tsx:612
 msgid "Build Failed"
 msgstr "ビルドに失敗しました"
 
-#: packages/application-extension/src/index.tsx:534 packages/application-extension/src/index.tsx:630
+#: packages/application-extension/src/index.tsx:630
 msgid "JupyterLab build is suggested:"
 msgstr "JupyterLabビルドが提案されています:"
 
-#: packages/application-extension/src/index.tsx:541 packages/application-extension/src/index.tsx:637
+#: packages/application-extension/src/index.tsx:637
 msgid "Build Recommended"
 msgstr "推奨ビルド"
 
-#: packages/application-extension/src/index.tsx:545 packages/application-extension/src/index.tsx:641
+#: packages/application-extension/src/index.tsx:641
 msgid "Build"
 msgstr "ビルド"
 
-#: packages/application-extension/src/index.tsx:608 packages/application-extension/src/index.tsx:707
+#: packages/application-extension/src/index.tsx:707
 msgid "Are you sure you want to exit JupyterLab?\n\n"
 "Any unsaved changes will be lost."
 msgstr "JupyterLabを終了してもよろしいですか？\n\n"
 "保存されていない変更はすべて失われます。"
 
-#: packages/application-extension/src/index.tsx:781 packages/application-extension/src/index.tsx:925
+#: packages/application-extension/src/index.tsx:792
+msgid "User layout customization has changed. You may need to reload JupyterLab to see the changes."
+msgstr ""
+
+#: packages/application-extension/src/index.tsx:925
 msgid "The path: %1 was not found. JupyterLab redirected to: %2"
 msgstr "パス: %1 が見つかりませんでした。JupyterLabは %2 にリダイレクトされます。"
 
-#: packages/application-extension/src/index.tsx:790 packages/application-extension/src/index.tsx:934
+#: packages/application-extension/src/index.tsx:934
 msgid "Path Not Found"
 msgstr "パスが見つかりません"
 
-#: packages/application-extension/src/index.tsx:792
-msgid "User layout customization has changed. You may need to reload JupyterLab to see the changes."
-msgstr ""
-
 #: packages/application/src/connectionlost.ts:19
 msgid "Server Connection Error"
 msgstr "サーバー接続のエラー"
 
 #: packages/application/src/connectionlost.ts:20
 msgid "A connection to the Jupyter server could not be established.\n"
 "JupyterLab will continue trying to reconnect.\n"
 "Check your network connection or Jupyter server configuration.\n"
 msgstr "Jupyterサーバへ接続できません。JupyterLabは引き続き接続を試みます。ネットワーク接続とJupyterサーバの設定を確認してください。\n"
 
-#: packages/application/src/shell.ts:253 packages/application/src/shell.ts:698
+#: packages/application/src/shell.ts:713
 msgid "main"
 msgstr ""
 
-#: packages/application/src/shell.ts:288 packages/application/src/shell.ts:292 packages/application/src/shell.ts:701 packages/application/src/shell.ts:705
+#: packages/application/src/shell.ts:716 packages/application/src/shell.ts:720
 msgid "main sidebar"
 msgstr ""
 
-#: packages/application/src/shell.ts:301 packages/application/src/shell.ts:305 packages/application/src/shell.ts:709 packages/application/src/shell.ts:713
+#: packages/application/src/shell.ts:724 packages/application/src/shell.ts:728
 msgid "alternate sidebar"
 msgstr ""
 
 #: packages/application/src/utils.ts:148
 msgid "%1 and %2"
 msgstr ""
 
-#: packages/apputils-extension/src/announcements.ts:102 packages/apputils-extension/src/announcements.ts:95
+#: packages/apputils-extension/src/announcements.ts:102
 msgid "Would you like to receive official Jupyter news?\n"
 "Please read the privacy policy."
 msgstr ""
 
-#: packages/apputils-extension/src/announcements.ts:103 packages/apputils-extension/src/announcements.ts:110
+#: packages/apputils-extension/src/announcements.ts:110
 msgid "Open privacy policy"
 msgstr ""
 
-#: packages/apputils-extension/src/announcements.ts:109 packages/apputils-extension/src/announcements.ts:116
+#: packages/apputils-extension/src/announcements.ts:116
 msgid "Privacy policies"
 msgstr ""
 
-#: packages/apputils-extension/src/announcements.ts:119 packages/apputils-extension/src/announcements.ts:126 packages/extensionmanager/src/widget.tsx:434
+#: packages/apputils-extension/src/announcements.ts:126 packages/extensionmanager/src/widget.tsx:434
 msgid "Yes"
 msgstr ""
 
-#: packages/apputils-extension/src/announcements.ts:136 packages/apputils-extension/src/announcements.ts:143 packages/extensionmanager/src/widget.tsx:424
+#: packages/apputils-extension/src/announcements.ts:143 packages/extensionmanager/src/widget.tsx:424
 msgid "No"
 msgstr ""
 
-#: packages/apputils-extension/src/announcements.ts:171 packages/apputils-extension/src/announcements.ts:178
+#: packages/apputils-extension/src/announcements.ts:180
 msgid "Hide"
 msgstr ""
 
-#: packages/apputils-extension/src/announcements.ts:172 packages/apputils-extension/src/announcements.ts:179
+#: packages/apputils-extension/src/announcements.ts:181
 msgid "Never show this notification again."
 msgstr ""
 
-#: packages/apputils-extension/src/announcements.ts:232 packages/apputils-extension/src/announcements.ts:239
+#: packages/apputils-extension/src/announcements.ts:243
 msgid "Do not check for updates"
 msgstr ""
 
-#: packages/apputils-extension/src/announcements.ts:233 packages/apputils-extension/src/announcements.ts:240
+#: packages/apputils-extension/src/announcements.ts:244
 msgid "If pressed, you will not be prompted if a new JupyterLab version is found."
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:210 packages/apputils-extension/src/index.ts:219
+#: packages/apputils-extension/src/index.ts:219
 msgid "Loading…"
 msgstr "読み込み中…"
 
-#: packages/apputils-extension/src/index.ts:211 packages/apputils-extension/src/index.ts:220
+#: packages/apputils-extension/src/index.ts:220
 msgid "The loading screen is taking a long time.\n"
 "Would you like to clear the workspace or keep waiting?"
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:214 packages/apputils-extension/src/index.ts:223
+#: packages/apputils-extension/src/index.ts:223
 msgid "Keep Waiting"
 msgstr "お待ちください"
 
-#: packages/apputils-extension/src/index.ts:215 packages/apputils-extension/src/index.ts:224
+#: packages/apputils-extension/src/index.ts:224
 msgid "Clear Workspace"
 msgstr "ワークスペースのクリア"
 
-#: packages/apputils-extension/src/index.ts:280 packages/apputils-extension/src/index.ts:290
+#: packages/apputils-extension/src/index.ts:290
 msgid "Print…"
 msgstr "印刷…"
 
-#: packages/apputils-extension/src/index.ts:310 packages/apputils-extension/src/index.ts:321
+#: packages/apputils-extension/src/index.ts:321
 msgid "Show Header Above Content"
 msgstr ""
 
 #: packages/apputils-extension/src/index.ts:429
 msgid "Load state for the current workspace."
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:477 packages/apputils-extension/src/index.ts:493
+#: packages/apputils-extension/src/index.ts:493
 msgid "Reset Application State"
 msgstr "アプリケーションの状態をリセット"
 
 #: packages/apputils-extension/src/index.ts:504
 msgid "Reset state when loading for the workspace."
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:568 packages/apputils-extension/src/index.ts:595
+#: packages/apputils-extension/src/index.ts:595
 msgid "Run First Enabled Command"
 msgstr "最初の有効化されたコマンドを実行"
 
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
 msgstr "ヘルプ"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:156 packages/apputils-extension/src/notificationplugin.tsx:160 packages/apputils-extension/src/notificationplugin.tsx:347 packages/apputils-extension/src/notificationplugin.tsx:351
+#: packages/apputils-extension/src/notificationplugin.tsx:166 packages/apputils-extension/src/notificationplugin.tsx:353
 msgid "%1 notification"
 msgid_plural "%1 notifications"
 msgstr[0] ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:157 packages/apputils-extension/src/notificationplugin.tsx:161 packages/apputils-extension/src/notificationplugin.tsx:348 packages/apputils-extension/src/notificationplugin.tsx:352
+#: packages/apputils-extension/src/notificationplugin.tsx:167 packages/apputils-extension/src/notificationplugin.tsx:354
 msgid "No notifications"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:166 packages/apputils-extension/src/notificationplugin.tsx:170
+#: packages/apputils-extension/src/notificationplugin.tsx:176
 msgid "Dismiss all notifications"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:173 packages/apputils-extension/src/notificationplugin.tsx:177
+#: packages/apputils-extension/src/notificationplugin.tsx:183
 msgid "Hide notifications"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:218 packages/apputils-extension/src/notificationplugin.tsx:222
+#: packages/apputils-extension/src/notificationplugin.tsx:229
 msgid "Dismiss notification"
 msgstr ""
 
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
 msgstr ""
 
-#: packages/apputils-extension/src/palette.ts:141 packages/apputils-extension/src/palette.ts:142
+#: packages/apputils-extension/src/palette.ts:141
 msgid "Commands (%1)"
 msgstr "コマンド (%1)"
 
-#: packages/apputils-extension/src/palette.ts:143 packages/apputils-extension/src/palette.ts:144 packages/apputils-extension/src/palette.ts:208 packages/apputils-extension/src/palette.ts:209
+#: packages/apputils-extension/src/palette.ts:143 packages/apputils-extension/src/palette.ts:208
 msgid "Commands"
 msgstr "コマンド"
 
-#: packages/apputils-extension/src/palette.ts:159 packages/apputils-extension/src/palette.ts:160
+#: packages/apputils-extension/src/palette.ts:159
 msgid "Activate Command Palette"
 msgstr "コマンドパレットを有効にする"
 
-#: packages/apputils-extension/src/palette.ts:162 packages/apputils-extension/src/palette.ts:163 packages/extensionmanager/src/widget.tsx:742
+#: packages/apputils-extension/src/palette.ts:162
 msgid "SEARCH"
 msgstr "検索"
 
 #: packages/apputils-extension/src/palette.ts:42
 msgid "Command Palette"
 msgstr "コマンドパレット"
 
 #: packages/apputils-extension/src/shortcuts.tsx:183
 msgid "Keyboard Shortcuts"
 msgstr ""
 
-#: packages/apputils-extension/src/shortcuts.tsx:187 packages/docmanager/src/widgetmanager.ts:397 packages/docmanager/src/widgetmanager.ts:399 packages/filebrowser/src/listing.ts:1140 packages/filebrowser/src/listing.ts:1399 packages/running-extension/src/opentabs.ts:86 packages/running-extension/src/opentabs.ts:87
+#: packages/apputils-extension/src/shortcuts.tsx:187 packages/docmanager/src/widgetmanager.ts:397 packages/filebrowser/src/listing.ts:1399 packages/running-extension/src/opentabs.ts:86
 msgid "Close"
 msgstr ""
 
-#: packages/apputils-extension/src/themesplugins.ts:103 packages/apputils-extension/src/themesplugins.ts:131
-msgid "Theme Scrollbars"
-msgstr "テーマのスクロールバー"
-
-#: packages/apputils-extension/src/themesplugins.ts:110 packages/apputils-extension/src/themesplugins.ts:138
-msgid "waiting for fonts"
-msgstr ""
-
 #: packages/apputils-extension/src/themesplugins.ts:112
 msgid "Switch to the provided `theme`."
 msgstr ""
 
-#: packages/apputils-extension/src/themesplugins.ts:117 packages/apputils-extension/src/themesplugins.ts:89
+#: packages/apputils-extension/src/themesplugins.ts:117
 msgid "Use Theme: %1"
 msgstr "テーマを使用: %1"
 
-#: packages/apputils-extension/src/themesplugins.ts:121 packages/apputils-extension/src/themesplugins.ts:149
+#: packages/apputils-extension/src/themesplugins.ts:131
+msgid "Theme Scrollbars"
+msgstr "テーマのスクロールバー"
+
+#: packages/apputils-extension/src/themesplugins.ts:138
+msgid "waiting for fonts"
+msgstr ""
+
+#: packages/apputils-extension/src/themesplugins.ts:149
 msgid "Increase Code Font Size"
 msgstr "コードのフォントサイズを大きくする"
 
-#: packages/apputils-extension/src/themesplugins.ts:123 packages/apputils-extension/src/themesplugins.ts:151
+#: packages/apputils-extension/src/themesplugins.ts:151
 msgid "Increase Content Font Size"
 msgstr "内容のフォントサイズを大きくする"
 
-#: packages/apputils-extension/src/themesplugins.ts:125 packages/apputils-extension/src/themesplugins.ts:153
+#: packages/apputils-extension/src/themesplugins.ts:153
 msgid "Increase UI Font Size"
 msgstr "UIのフォントサイズを大きくする"
 
-#: packages/apputils-extension/src/themesplugins.ts:127 packages/apputils-extension/src/themesplugins.ts:155 packages/fileeditor-extension/src/commands.ts:280 packages/fileeditor-extension/src/commands.ts:298
+#: packages/apputils-extension/src/themesplugins.ts:155 packages/fileeditor-extension/src/commands.ts:280
 msgid "Increase Font Size"
 msgstr "フォントを大きく"
 
-#: packages/apputils-extension/src/themesplugins.ts:137 packages/apputils-extension/src/themesplugins.ts:165
+#: packages/apputils-extension/src/themesplugins.ts:165
 msgid "Decrease Code Font Size"
 msgstr "コードのフォントサイズを小さくする"
 
-#: packages/apputils-extension/src/themesplugins.ts:139 packages/apputils-extension/src/themesplugins.ts:167
+#: packages/apputils-extension/src/themesplugins.ts:167
 msgid "Decrease Content Font Size"
 msgstr "内容のフォントサイズを小さくする"
 
-#: packages/apputils-extension/src/themesplugins.ts:141 packages/apputils-extension/src/themesplugins.ts:169
+#: packages/apputils-extension/src/themesplugins.ts:169
 msgid "Decrease UI Font Size"
 msgstr "UIのフォントサイズを小さくする"
 
-#: packages/apputils-extension/src/themesplugins.ts:143 packages/apputils-extension/src/themesplugins.ts:171 packages/fileeditor-extension/src/commands.ts:284 packages/fileeditor-extension/src/commands.ts:302
+#: packages/apputils-extension/src/themesplugins.ts:171 packages/fileeditor-extension/src/commands.ts:284
 msgid "Decrease Font Size"
 msgstr "フォントサイズを小さく"
 
-#: packages/apputils-extension/src/themesplugins.ts:202 packages/apputils-extension/src/themesplugins.ts:231 packages/codemirror/src/extension.ts:851
+#: packages/apputils-extension/src/themesplugins.ts:231 packages/codemirror/src/extension.ts:851
 msgid "Theme"
 msgstr "テーマ"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:181 packages/apputils-extension/src/workspacesplugin.ts:189
+#: packages/apputils-extension/src/workspacesplugin.ts:181
 msgid "Workspace loader"
 msgstr "ワークスペース ローダ"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:266 packages/apputils-extension/src/workspacesplugin.ts:272 packages/apputils-extension/src/workspacesplugin.ts:274 packages/apputils-extension/src/workspacesplugin.ts:280 packages/docmanager/src/widgetmanager.ts:436 packages/docmanager/src/widgetmanager.ts:438 packages/docregistry/src/context.ts:1019 packages/docregistry/src/context.ts:1035 packages/docregistry/src/context.ts:1042 packages/docregistry/src/context.ts:1101 packages/docregistry/src/context.ts:1108
+#: packages/apputils-extension/src/workspacesplugin.ts:266 packages/apputils-extension/src/workspacesplugin.ts:272 packages/docmanager/src/widgetmanager.ts:436 packages/docregistry/src/context.ts:1019
 msgid "Save"
 msgstr "保存"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:268 packages/apputils-extension/src/workspacesplugin.ts:276 packages/apputils-extension/src/workspacesplugin.ts:79 packages/apputils-extension/src/workspacesplugin.ts:82
+#: packages/apputils-extension/src/workspacesplugin.ts:268 packages/apputils-extension/src/workspacesplugin.ts:79
 msgid "Save Current Workspace As…"
 msgstr "現在のワークスペースを別名で保存…"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:278 packages/apputils/src/dialog.tsx:763 packages/apputils/src/dialog.tsx:862 packages/apputils/src/sessioncontext.tsx:1292 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:625 packages/debugger-extension/src/index.ts:696 packages/debugger/src/panels/breakpoints/index.ts:66 packages/docmanager-extension/src/index.tsx:1015 packages/docmanager-extension/src/index.tsx:653 packages/docmanager-extension/src/index.tsx:703 packages/docmanager-extension/src/index.tsx:994 packages/docmanager/src/dialogs.ts:115 packages/docmanager/src/dialogs.ts:52 packages/docmanager/src/widgetmanager.ts:444 packages/extensionmanager/src/companions.tsx:216 packages/filebrowser/src/listing.ts:415 packages/filebrowser/src/listing.ts:429 packages/filebrowser/src/model.ts:449 packages/filebrowser/src/model.ts:456 packages/filebrowser/src/opendialog.ts:87 packages/notebook/src/actions.tsx:1911 packages/notebook/src/searchprovider.ts:504 packages/running/src/index.tsx:232 packages/settingeditor/src/plugineditor.ts:132 packages/settingeditor/src/plugineditor.ts:137 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/shortcuts-extension/src/components/ShortcutItem.tsx:247 packages/translation-extension/src/index.ts:138 packages/translation-extension/src/index.ts:147
-msgid "Cancel"
-msgstr "キャンセル"
-
-#: packages/apputils-extension/src/workspacesplugin.ts:72 packages/apputils-extension/src/workspacesplugin.ts:75
+#: packages/apputils-extension/src/workspacesplugin.ts:72
 msgid "JupyterLab workspace File"
 msgstr "JupyterLab ワークスペースファイル"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:93 packages/apputils-extension/src/workspacesplugin.ts:96
+#: packages/apputils-extension/src/workspacesplugin.ts:93
 msgid "Save Current Workspace"
 msgstr "現在のワークスペースを保存"
 
-#: packages/apputils/src/dialog.tsx:47 packages/help-extension/src/index.tsx:153 packages/help-extension/src/index.tsx:395 packages/help-extension/src/index.tsx:404 packages/hub-extension/src/index.ts:161 packages/hub-extension/src/index.ts:173 packages/lsp/src/adapters/adapter.ts:470 packages/mainmenu-extension/src/index.ts:548 packages/mainmenu-extension/src/index.ts:551
+#: packages/apputils/src/dialog.tsx:47 packages/help-extension/src/index.tsx:153 packages/help-extension/src/index.tsx:404 packages/hub-extension/src/index.ts:173 packages/lsp/src/adapters/adapter.ts:470 packages/mainmenu-extension/src/index.ts:548
 msgid "Dismiss"
 msgstr "閉じる"
 
-#: packages/apputils/src/dialog.tsx:763 packages/docmanager-extension/src/index.tsx:642 packages/docmanager-extension/src/index.tsx:687 packages/docmanager-extension/src/index.tsx:750 packages/docmanager-extension/src/index.tsx:761 packages/docmanager-extension/src/index.tsx:874 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:508 packages/extensionmanager/src/model.ts:531 packages/notebook/src/actions.tsx:1903 packages/notebook/src/actions.tsx:1912 packages/notebook/src/actions.tsx:1984 packages/notebook/src/actions.tsx:2155 packages/notebook/src/actions.tsx:2165 packages/notebook/src/default-toolbar.tsx:70 packages/notebook/src/model.ts:373 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:213 packages/notebook/src/panel.ts:219 packages/notebook/src/searchprovider.ts:505 packages/settingeditor/src/plugineditor.ts:133 packages/settingeditor/src/plugineditor.ts:138
+#: packages/apputils/src/dialog.tsx:763 packages/apputils/src/dialog.tsx:862 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:696 packages/filebrowser/src/listing.ts:429 packages/filebrowser/src/model.ts:449 packages/notebook/src/searchprovider.ts:514 packages/settingeditor/src/plugineditor.ts:132 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/translation-extension/src/index.ts:147
+msgid "Cancel"
+msgstr "キャンセル"
+
+#: packages/apputils/src/dialog.tsx:763 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:508 packages/extensionmanager/src/model.ts:531 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:234 packages/notebook/src/searchprovider.ts:515 packages/settingeditor/src/plugineditor.ts:133
 msgid "Ok"
 msgstr ""
 
-#: packages/apputils/src/kernelstatuses.ts:17 packages/apputils/src/kernelstatuses.tsx:29
+#: packages/apputils/src/kernelstatuses.tsx:210 packages/apputils/src/sessioncontext.tsx:1746 packages/apputils/src/sessioncontext.tsx:631
+msgid "No Kernel"
+msgstr "カーネルがありません"
+
+#: packages/apputils/src/kernelstatuses.tsx:29
 msgid "Unknown"
 msgstr "不定"
 
-#: packages/apputils/src/kernelstatuses.ts:18 packages/apputils/src/kernelstatuses.tsx:30
+#: packages/apputils/src/kernelstatuses.tsx:30
 msgid "Starting"
 msgstr "開始中"
 
-#: packages/apputils/src/kernelstatuses.ts:19 packages/apputils/src/kernelstatuses.tsx:31
+#: packages/apputils/src/kernelstatuses.tsx:31
 msgid "Idle"
 msgstr "アイドル"
 
-#: packages/apputils/src/kernelstatuses.ts:20 packages/apputils/src/kernelstatuses.tsx:32
+#: packages/apputils/src/kernelstatuses.tsx:32
 msgid "Busy"
 msgstr "実行中"
 
-#: packages/apputils/src/kernelstatuses.ts:21 packages/apputils/src/kernelstatuses.tsx:33
+#: packages/apputils/src/kernelstatuses.tsx:33
 msgid "Terminating"
 msgstr "終了中"
 
-#: packages/apputils/src/kernelstatuses.ts:22 packages/apputils/src/kernelstatuses.tsx:34
+#: packages/apputils/src/kernelstatuses.tsx:34
 msgid "Restarting"
 msgstr "再起動中"
 
-#: packages/apputils/src/kernelstatuses.ts:23 packages/apputils/src/kernelstatuses.tsx:35
+#: packages/apputils/src/kernelstatuses.tsx:35
 msgid "Autorestarting"
 msgstr "自動実行中"
 
-#: packages/apputils/src/kernelstatuses.ts:24 packages/apputils/src/kernelstatuses.tsx:36
+#: packages/apputils/src/kernelstatuses.tsx:36
 msgid "Dead"
 msgstr "停止"
 
-#: packages/apputils/src/kernelstatuses.ts:25 packages/apputils/src/kernelstatuses.tsx:37
+#: packages/apputils/src/kernelstatuses.tsx:37
 msgid "Connected"
 msgstr "接続済み"
 
-#: packages/apputils/src/kernelstatuses.ts:26 packages/apputils/src/kernelstatuses.tsx:38
+#: packages/apputils/src/kernelstatuses.tsx:38
 msgid "Connecting"
 msgstr "接続中"
 
-#: packages/apputils/src/kernelstatuses.ts:27 packages/apputils/src/kernelstatuses.tsx:39
+#: packages/apputils/src/kernelstatuses.tsx:39
 msgid "Disconnected"
 msgstr "切断"
 
-#: packages/apputils/src/kernelstatuses.ts:28 packages/apputils/src/kernelstatuses.tsx:40
+#: packages/apputils/src/kernelstatuses.tsx:40
 msgid "Initializing"
 msgstr "初期化中"
 
-#: packages/apputils/src/kernelstatuses.tsx:210 packages/apputils/src/sessioncontext.tsx:1689 packages/apputils/src/sessioncontext.tsx:1746 packages/apputils/src/sessioncontext.tsx:613 packages/apputils/src/sessioncontext.tsx:631 packages/statusbar/src/defaults/kernelStatus.tsx:185
-msgid "No Kernel"
-msgstr "カーネルがありません"
-
-#: packages/apputils/src/kernelstatuses.tsx:62 packages/statusbar/src/defaults/kernelStatus.tsx:36
+#: packages/apputils/src/kernelstatuses.tsx:62
 msgid "Change kernel for %1"
 msgstr "%1 のカーネルを変更"
 
 #: packages/apputils/src/mainareawidget.ts:47
 msgid "notebook content"
 msgstr ""
 
 #: packages/apputils/src/mainareawidget.ts:50
 msgid "notebook actions"
 msgstr ""
 
-#: packages/apputils/src/runningSessions.tsx:115 packages/statusbar/src/defaults/runningSessions.tsx:111
+#: packages/apputils/src/runningSessions.tsx:115
 msgid "%1 Terminals, %2 Kernel sessions"
 msgstr "%1 ターミナル, %2 カーネルセッション"
 
-#: packages/apputils/src/sessioncontext.tsx:1019 packages/apputils/src/sessioncontext.tsx:1051
+#: packages/apputils/src/sessioncontext.tsx:1051
 msgid "Error Starting Kernel"
 msgstr "カーネルの起動エラー"
 
-#: packages/apputils/src/sessioncontext.tsx:1298 packages/apputils/src/sessioncontext.tsx:1341 packages/filebrowser/src/opendialog.ts:83 packages/filebrowser/src/opendialog.ts:89
+#: packages/apputils/src/sessioncontext.tsx:1341 packages/filebrowser/src/opendialog.ts:83
 msgid "Select"
 msgstr "選択"
 
-#: packages/apputils/src/sessioncontext.tsx:1302 packages/apputils/src/sessioncontext.tsx:1348
+#: packages/apputils/src/sessioncontext.tsx:1348
 msgid "Select Kernel"
 msgstr "カーネルを選択"
 
 #: packages/apputils/src/sessioncontext.tsx:1353
 msgid "Always start the preferred kernel"
 msgstr ""
 
 #: packages/apputils/src/sessioncontext.tsx:1354
 msgid "Remember my choice and always start the preferred kernel"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1355 packages/apputils/src/sessioncontext.tsx:1415
+#: packages/apputils/src/sessioncontext.tsx:1415
 msgid "Restart Kernel?"
 msgstr "カーネルを再起動しますか？"
 
-#: packages/apputils/src/sessioncontext.tsx:1356
-msgid "Do you want to restart the current kernel? All variables will be lost."
-msgstr "現在のカーネルを再起動しますか？変数はすべて失われます。"
-
-#: packages/apputils/src/sessioncontext.tsx:1410 packages/apputils/src/sessioncontext.tsx:1473
-msgid "Select kernel for:"
-msgstr "次のカーネルを選択:"
-
 #: packages/apputils/src/sessioncontext.tsx:1416
 msgid "Do you want to restart the kernel of %1? All variables will be lost."
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1550 packages/apputils/src/sessioncontext.tsx:1607
+#: packages/apputils/src/sessioncontext.tsx:1473
+msgid "Select kernel for:"
+msgstr "次のカーネルを選択:"
+
+#: packages/apputils/src/sessioncontext.tsx:1607
 msgid "Start Preferred Kernel"
 msgstr "優先するカーネルを起動"
 
-#: packages/apputils/src/sessioncontext.tsx:1565 packages/apputils/src/sessioncontext.tsx:1622
+#: packages/apputils/src/sessioncontext.tsx:1622
 msgid "Start Other Kernel"
 msgstr "他のカーネルを起動"
 
-#: packages/apputils/src/sessioncontext.tsx:1622 packages/apputils/src/sessioncontext.tsx:1679
+#: packages/apputils/src/sessioncontext.tsx:1679
 msgid "Use Kernel from Preferred Session"
 msgstr "優先するセッションのカーネルを使用する"
 
-#: packages/apputils/src/sessioncontext.tsx:1637 packages/apputils/src/sessioncontext.tsx:1694
+#: packages/apputils/src/sessioncontext.tsx:1694
 msgid "Use Kernel from Other Session"
 msgstr "他のセッションのカーネルを使用する"
 
-#: packages/apputils/src/sessioncontext.tsx:1687 packages/apputils/src/sessioncontext.tsx:1744
+#: packages/apputils/src/sessioncontext.tsx:1744
 msgid "Use No Kernel"
 msgstr "カーネルを使用しない"
 
-#: packages/apputils/src/sessioncontext.tsx:1711 packages/apputils/src/sessioncontext.tsx:1768
+#: packages/apputils/src/sessioncontext.tsx:1768
 msgid "Path:"
 msgstr "パス:"
 
-#: packages/apputils/src/sessioncontext.tsx:1712 packages/apputils/src/sessioncontext.tsx:1769
+#: packages/apputils/src/sessioncontext.tsx:1769
 msgid "Name:"
 msgstr "名前:"
 
-#: packages/apputils/src/sessioncontext.tsx:1713 packages/apputils/src/sessioncontext.tsx:1770
+#: packages/apputils/src/sessioncontext.tsx:1770
 msgid "Kernel Name:"
 msgstr "カーネル名:"
 
-#: packages/apputils/src/sessioncontext.tsx:1714 packages/apputils/src/sessioncontext.tsx:1771
+#: packages/apputils/src/sessioncontext.tsx:1771
 msgid "Kernel Id:"
 msgstr "カーネルID:"
 
-#: packages/apputils/src/thememanager.ts:362 packages/apputils/src/thememanager.ts:371 packages/apputils/src/thememanager.ts:373
+#: packages/apputils/src/thememanager.ts:371
 msgid "Neither theme %1 nor default %2 loaded."
 msgstr "テーマ %1 もデフォルトテーマ %2 も読み込まれていません。"
 
-#: packages/apputils/src/thememanager.ts:446 packages/apputils/src/thememanager.ts:455 packages/apputils/src/thememanager.ts:457
+#: packages/apputils/src/thememanager.ts:455
 msgid "Error Loading Theme"
 msgstr "テーマの読み込みエラー"
 
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
 msgstr "カーネルを切り替え"
 
-#: packages/apputils/src/toolbar/widget.tsx:1314 packages/apputils/src/toolbar/widget.tsx:208
+#: packages/apputils/src/toolbar/widget.tsx:208
 msgid "Kernel %1"
 msgstr "カーネル %1"
 
-#: packages/apputils/src/toolbar/widget.tsx:56 packages/apputils/src/toolbar/widget.tsx:610 packages/mainmenu-extension/src/index.ts:469 packages/mainmenu-extension/src/index.ts:472 packages/notebook-extension/src/index.ts:2453
+#: packages/apputils/src/toolbar/widget.tsx:56 packages/mainmenu-extension/src/index.ts:469 packages/notebook-extension/src/index.ts:2453
 msgid "Interrupt the kernel"
 msgstr "カーネルを中断"
 
-#: packages/apputils/src/toolbar/widget.tsx:635 packages/apputils/src/toolbar/widget.tsx:80 packages/mainmenu-extension/src/index.ts:494 packages/notebook-extension/src/index.ts:2321
+#: packages/apputils/src/toolbar/widget.tsx:80 packages/mainmenu-extension/src/index.ts:494 packages/notebook-extension/src/index.ts:2321
 msgid "Restart the kernel"
 msgstr "カーネルを再起動"
 
 #: packages/cells/src/placeholder.ts:85
 msgid "Click to expand"
 msgstr ""
 
@@ -3230,70 +2883,42 @@
 msgid_plural "%1 cells hidden"
 msgstr[0] ""
 
 #: packages/cells/src/widget.ts:2338
 msgid "Raw Cell Content"
 msgstr ""
 
-#: packages/celltags-extension/src/celltag.tsx:211 packages/celltags/src/addwidget.ts:159 packages/celltags/src/addwidget.ts:31
+#: packages/celltags-extension/src/celltag.tsx:211
 msgid "Add Tag"
 msgstr "タグの追加"
 
-#: packages/celltags/src/tool.ts:200
-msgid "Cell Tags"
-msgstr ""
-
-#: packages/codeeditor/src/jsoneditor.ts:315 packages/codeeditor/src/jsoneditor.ts:327 packages/codeeditor/src/jsoneditor.ts:78
+#: packages/codeeditor/src/jsoneditor.ts:315
 msgid "No data!"
 msgstr "データがありません!"
 
-#: packages/codeeditor/src/jsoneditor.ts:58 packages/codeeditor/src/jsoneditor.ts:59
+#: packages/codeeditor/src/jsoneditor.ts:59
 msgid "Revert changes to data"
 msgstr "データの変更を元に戻す"
 
-#: packages/codeeditor/src/jsoneditor.ts:63 packages/codeeditor/src/jsoneditor.ts:64
+#: packages/codeeditor/src/jsoneditor.ts:64
 msgid "Commit changes to data"
 msgstr "データに変更を反映させる"
 
-#: packages/codeeditor/src/lineCol.tsx:131 packages/statusbar/src/defaults/lineCol.tsx:133
+#: packages/codeeditor/src/lineCol.tsx:131
 msgid "Go to line number between 1 and %1"
 msgstr "1 から %1 の行番号に移動"
 
-#: packages/codeeditor/src/lineCol.tsx:229 packages/statusbar/src/defaults/lineCol.tsx:231
+#: packages/codeeditor/src/lineCol.tsx:229
 msgid "Ln %1, Col %2"
 msgstr ""
 
-#: packages/codeeditor/src/lineCol.tsx:230 packages/statusbar/src/defaults/lineCol.tsx:232
+#: packages/codeeditor/src/lineCol.tsx:230
 msgid "Go to line number…"
 msgstr "行番号に移動…"
 
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
-msgstr "検索…"
-
-#: packages/codemirror-extension/src/index.ts:342 packages/fileeditor-extension/src/commands.ts:538 packages/mainmenu-extension/src/index.ts:313 packages/mainmenu-extension/src/index.ts:324
-msgid "Go to Line…"
-msgstr "行へ移動…"
-
-#: packages/codemirror/src/editor.ts:1144
-msgid "Code Editor out of Sync"
-msgstr "コードエディタが同期していません"
-
-#: packages/codemirror/src/editor.ts:1145
-msgid "Please open your browser JavaScript console for bug report instructions"
-msgstr "バグレポートの手順については、ブラウザのJavaScriptコンソールを開いてください"
-
 #: packages/codemirror/src/extension.ts:608
 msgid "Auto Closing Brackets"
 msgstr ""
 
 #: packages/codemirror/src/extension.ts:617
 msgid "Code Folding"
 msgstr ""
@@ -3322,23 +2947,23 @@
 msgid "Indentation unit"
 msgstr ""
 
 #: packages/codemirror/src/extension.ts:675
 msgid "The indentation is a `Tab` or the number of spaces. This defaults to 4 spaces."
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:702 packages/fileeditor-extension/src/commands.ts:329
+#: packages/codemirror/src/extension.ts:702
 msgid "Line Numbers"
 msgstr "行番号"
 
 #: packages/codemirror/src/extension.ts:711
 msgid "Line Wrap"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:720 packages/fileeditor-extension/src/commands.ts:420 packages/fileeditor-extension/src/commands.ts:421 packages/fileeditor-extension/src/commands.ts:428 packages/mainmenu-extension/src/index.ts:588 packages/mainmenu-extension/src/index.ts:593
+#: packages/codemirror/src/extension.ts:720 packages/fileeditor-extension/src/commands.ts:421 packages/fileeditor-extension/src/commands.ts:428 packages/mainmenu-extension/src/index.ts:588
 msgid "Match Brackets"
 msgstr "括弧を一致させる"
 
 #: packages/codemirror/src/extension.ts:733
 msgid "Rectangular selection"
 msgstr ""
 
@@ -3422,19 +3047,19 @@
 msgid "Go to line"
 msgstr ""
 
 #: packages/codemirror/src/extension.ts:878
 msgid "go"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:879 packages/documentsearch/src/searchoverlay.tsx:124 packages/documentsearch/src/searchview.tsx:154 packages/documentsearch/src/searchview.tsx:159
+#: packages/codemirror/src/extension.ts:879 packages/documentsearch/src/searchview.tsx:154 packages/documentsearch/src/searchview.tsx:159
 msgid "Find"
 msgstr "検索"
 
-#: packages/codemirror/src/extension.ts:880 packages/documentsearch/src/searchoverlay.tsx:173 packages/documentsearch/src/searchoverlay.tsx:191 packages/documentsearch/src/searchview.tsx:217 packages/documentsearch/src/searchview.tsx:221 packages/documentsearch/src/searchview.tsx:248
+#: packages/codemirror/src/extension.ts:880 packages/documentsearch/src/searchview.tsx:217 packages/documentsearch/src/searchview.tsx:221 packages/documentsearch/src/searchview.tsx:248
 msgid "Replace"
 msgstr "置換"
 
 #: packages/codemirror/src/extension.ts:881
 msgid "next"
 msgstr ""
 
@@ -3674,15 +3299,15 @@
 msgid "Swift"
 msgstr ""
 
 #: packages/codemirror/src/language.ts:1477
 msgid "sTeX"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1486 packages/notebook-extension/src/index.ts:2868 packages/notebook-extension/src/index.ts:3678
+#: packages/codemirror/src/language.ts:1486 packages/notebook-extension/src/index.ts:3678
 msgid "LaTeX"
 msgstr ""
 
 #: packages/codemirror/src/language.ts:1497
 msgid "SystemVerilog"
 msgstr ""
 
@@ -3786,15 +3411,15 @@
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
 
@@ -3810,15 +3435,15 @@
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
 
@@ -4042,211 +3667,179 @@
 msgid "HTTP"
 msgstr ""
 
 #: packages/codemirror/src/language.ts:996
 msgid "IDL"
 msgstr ""
 
-#: packages/codemirror/src/syntaxstatus.tsx:66 packages/fileeditor/src/syntaxstatus.tsx:66
-msgid "Change text editor syntax highlighting"
-msgstr "テキストエディタのシンタックスハイライトを変更"
-
-#: packages/collaboration-extension/src/index.ts:163
-msgid "User info"
-msgstr ""
-
-#: packages/collaboration-extension/src/index.ts:164
-msgid "User information"
-msgstr ""
-
-#: packages/collaboration-extension/src/index.ts:176
-msgid "Online Collaborators"
+#: packages/codemirror/src/theme.ts:215
+msgid "codemirror"
 msgstr ""
 
-#: packages/console-extension/src/foreign.ts:65 packages/console-extension/src/foreign.ts:66 packages/console-extension/src/index.ts:155 packages/console-extension/src/index.ts:203 packages/console-extension/src/index.ts:262 packages/console-extension/src/index.ts:311 packages/console-extension/src/index.ts:483 packages/console-extension/src/index.ts:530 packages/console/src/panel.ts:331 packages/console/src/panel.ts:333 packages/launcher/src/index.tsx:150 packages/launcher/src/index.tsx:155 packages/launcher/src/widget.tsx:116 packages/launcher/src/widget.tsx:121
+#: packages/console-extension/src/foreign.ts:66 packages/console-extension/src/index.ts:262 packages/console-extension/src/index.ts:311 packages/console-extension/src/index.ts:530 packages/console/src/panel.ts:333 packages/launcher/src/widget.tsx:116 packages/launcher/src/widget.tsx:121
 msgid "Console"
 msgstr "コンソール"
 
-#: packages/console-extension/src/foreign.ts:79 packages/console-extension/src/foreign.ts:80
+#: packages/console-extension/src/foreign.ts:80
 msgid "Show All Kernel Activity"
 msgstr "すべてのカーネルのアクティビティを表示"
 
-#: packages/console-extension/src/index.ts:418 packages/console-extension/src/index.ts:464
+#: packages/console-extension/src/index.ts:464
 msgid "Auto Close Brackets for Code Console Prompt"
 msgstr "コードコンソールプロンプトで括弧を自動で閉じる"
 
-#: packages/console-extension/src/index.ts:472 packages/console-extension/src/index.ts:519
-msgid "New Console"
-msgstr "新規コンソール"
-
 #: packages/console-extension/src/index.ts:490
 msgid "Open a console for the provided `path`."
 msgstr ""
 
-#: packages/console-extension/src/index.ts:507 packages/console-extension/src/index.ts:554
+#: packages/console-extension/src/index.ts:519
+msgid "New Console"
+msgstr "新規コンソール"
+
+#: packages/console-extension/src/index.ts:554
 msgid "Clear Console Cells"
 msgstr "コンソールのセルを消去"
 
-#: packages/console-extension/src/index.ts:519 packages/console-extension/src/index.ts:566
+#: packages/console-extension/src/index.ts:566
 msgid "Run Cell (unforced)"
 msgstr "セルを実行 (未強制)"
 
-#: packages/console-extension/src/index.ts:531 packages/console-extension/src/index.ts:578
+#: packages/console-extension/src/index.ts:578
 msgid "Run Cell (forced)"
 msgstr "セルの実行 (強制)"
 
-#: packages/console-extension/src/index.ts:543 packages/console-extension/src/index.ts:590
+#: packages/console-extension/src/index.ts:590
 msgid "Insert Line Break"
 msgstr "改行を挿入"
 
-#: packages/console-extension/src/index.ts:555 packages/console-extension/src/index.ts:602
+#: packages/console-extension/src/index.ts:602
 msgid "Replace Selection in Console"
 msgstr "コンソールで選択範囲を置き換え"
 
-#: packages/console-extension/src/index.ts:568 packages/console-extension/src/index.ts:615 packages/mainmenu-extension/src/index.ts:468 packages/mainmenu-extension/src/index.ts:471 packages/notebook-extension/src/index.ts:1852 packages/notebook-extension/src/index.ts:2452
+#: packages/console-extension/src/index.ts:615 packages/mainmenu-extension/src/index.ts:468 packages/notebook-extension/src/index.ts:2452
 msgid "Interrupt Kernel"
 msgstr "カーネルを中断"
 
-#: packages/console-extension/src/index.ts:583 packages/console-extension/src/index.ts:630 packages/mainmenu-extension/src/index.ts:493 packages/notebook-extension/src/index.ts:1724 packages/notebook-extension/src/index.ts:2320
+#: packages/console-extension/src/index.ts:630 packages/mainmenu-extension/src/index.ts:493 packages/notebook-extension/src/index.ts:2320
 msgid "Restart Kernel…"
 msgstr "カーネルを再起動…"
 
-#: packages/console-extension/src/index.ts:598 packages/console-extension/src/index.ts:654
+#: packages/console-extension/src/index.ts:642 packages/lsp-extension/src/index.ts:275 packages/mainmenu-extension/src/index.ts:375 packages/mainmenu-extension/src/index.ts:385 packages/running/src/index.tsx:161 packages/terminal-extension/src/index.ts:322
+msgid "Shut Down"
+msgstr "シャットダウン"
+
+#: packages/console-extension/src/index.ts:654
 msgid "Close and Shut Down…"
 msgstr "閉じてシャットダウン…"
 
-#: packages/console-extension/src/index.ts:605 packages/console-extension/src/index.ts:661
+#: packages/console-extension/src/index.ts:661
 msgid "Shut down the console?"
 msgstr "コンソールをシャットダウンしますか?"
 
-#: packages/console-extension/src/index.ts:606 packages/console-extension/src/index.ts:662 packages/console-extension/src/index.ts:685 packages/notebook-extension/src/index.ts:1747 packages/notebook-extension/src/index.ts:2357 packages/notebook-extension/src/index.ts:2654
+#: packages/console-extension/src/index.ts:662 packages/notebook-extension/src/index.ts:2357
 msgid "Are you sure you want to close \"%1\"?"
 msgstr "\"%1\" を閉じてもよろしいですか?"
 
-#: packages/console-extension/src/index.ts:642 packages/lsp-extension/src/index.ts:275 packages/mainmenu-extension/src/index.ts:375 packages/mainmenu-extension/src/index.ts:382 packages/mainmenu-extension/src/index.ts:385 packages/mainmenu-extension/src/index.ts:392 packages/running-extension/src/kernels.ts:39 packages/running/src/index.tsx:142 packages/running/src/index.tsx:161 packages/terminal-extension/src/index.ts:302 packages/terminal-extension/src/index.ts:322
-msgid "Shut Down"
-msgstr "シャットダウン"
-
-#: packages/console-extension/src/index.ts:646 packages/console-extension/src/index.ts:705 packages/mainmenu-extension/src/index.ts:519 packages/mainmenu-extension/src/index.ts:530 packages/notebook-extension/src/index.ts:2225 packages/notebook-extension/src/index.ts:3059
-msgid "Change Kernel…"
-msgstr "カーネルを変更…"
-
-#: packages/console-extension/src/index.ts:681
-msgid "Shutdown Console"
-msgstr "コンソールをシャットダウン"
-
 #: packages/console-extension/src/index.ts:684
 msgid "Inject some code in a console."
 msgstr ""
 
-#: packages/console-extension/src/index.ts:684
-msgid "Shut down the Console?"
-msgstr "コンソールをシャットダウンしますか?"
-
-#: packages/console-extension/src/index.ts:706
-msgid "Restart Kernel and Clear Console"
-msgstr "カーネルを再起動してコンソールをクリア"
+#: packages/console-extension/src/index.ts:705 packages/mainmenu-extension/src/index.ts:519 packages/notebook-extension/src/index.ts:3059
+msgid "Change Kernel…"
+msgstr "カーネルを変更…"
 
 #: packages/console-extension/src/index.ts:717 packages/mainmenu-extension/src/index.ts:754 packages/notebook-extension/src/index.ts:3070
 msgid "Get Kernel"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:737
-msgid "Run Cell"
-msgstr "セルを実行"
-
-#: packages/console-extension/src/index.ts:744
-msgid "Clear Console Cell"
-msgstr "コンソールのセルを消去"
-
-#: packages/console-extension/src/index.ts:757 packages/console-extension/src/index.ts:799
+#: packages/console-extension/src/index.ts:799
 msgid "Execute with Shift+Enter"
 msgstr "Shift+Enter で実行"
 
-#: packages/console-extension/src/index.ts:758 packages/console-extension/src/index.ts:800
+#: packages/console-extension/src/index.ts:800
 msgid "Execute with Enter"
 msgstr "Enter で実行"
 
 #: packages/console-extension/src/index.ts:844 packages/fileeditor-extension/src/commands.ts:1005 packages/notebook-extension/src/index.ts:1974
 msgid "Display the completion helper."
 msgstr ""
 
 #: packages/console-extension/src/index.ts:855 packages/fileeditor-extension/src/commands.ts:1016 packages/notebook-extension/src/index.ts:1984
 msgid "Select the completion suggestion."
 msgstr ""
 
-#: packages/console/src/panel.ts:314 packages/console/src/panel.ts:316
+#: packages/console/src/panel.ts:316
 msgid "Name: %1\n"
 msgstr "名前: %1\n"
 
-#: packages/console/src/panel.ts:315 packages/console/src/panel.ts:317
+#: packages/console/src/panel.ts:317
 msgid "Directory: %1\n"
 msgstr "ディレクトリ: %1\n"
 
-#: packages/console/src/panel.ts:316 packages/console/src/panel.ts:318
+#: packages/console/src/panel.ts:318
 msgid "Kernel: %1"
 msgstr "カーネル: %1"
 
-#: packages/console/src/panel.ts:319 packages/console/src/panel.ts:321
+#: packages/console/src/panel.ts:321
 msgid "\n"
 "Connected: %1"
 msgstr "\n"
 "接続: %1"
 
-#: packages/console/src/panel.ts:326 packages/console/src/panel.ts:328
+#: packages/console/src/panel.ts:328
 msgid "\n"
 "Last Execution: %1"
 msgstr "\n"
 "最後の実行: %1"
 
-#: packages/console/src/panel.ts:66 packages/console/src/panel.ts:67
+#: packages/console/src/panel.ts:66
 msgid "Console %1"
 msgstr "コンソール %1"
 
 #: packages/csvviewer-extension/src/index.ts:134
 msgid "CSV Viewer"
 msgstr ""
 
-#: packages/csvviewer-extension/src/index.ts:212 packages/csvviewer-extension/src/index.ts:219 packages/csvviewer-extension/src/index.ts:362 packages/csvviewer-extension/src/index.ts:369 packages/csvviewer-extension/src/index.ts:92
+#: packages/csvviewer-extension/src/index.ts:212 packages/csvviewer-extension/src/index.ts:219 packages/csvviewer-extension/src/index.ts:362 packages/csvviewer-extension/src/index.ts:369
 msgid "Go to Line"
 msgstr "行へ移動"
 
 #: packages/csvviewer-extension/src/index.ts:284
 msgid "TSV Viewer"
 msgstr ""
 
-#: packages/csvviewer/src/toolbar.ts:119 packages/csvviewer/src/toolbar.ts:133
+#: packages/csvviewer/src/toolbar.ts:119
 msgid "tab"
 msgstr "タブ"
 
-#: packages/csvviewer/src/toolbar.ts:120 packages/csvviewer/src/toolbar.ts:134
+#: packages/csvviewer/src/toolbar.ts:120
 msgid "pipe"
 msgstr "パイプ (\"|\")"
 
-#: packages/csvviewer/src/toolbar.ts:121 packages/csvviewer/src/toolbar.ts:135
+#: packages/csvviewer/src/toolbar.ts:121
 msgid "hash"
 msgstr "ハッシュ (\"#\")"
 
-#: packages/csvviewer/src/toolbar.ts:127 packages/csvviewer/src/toolbar.ts:141
+#: packages/csvviewer/src/toolbar.ts:127
 msgid "Delimiter: "
 msgstr "区切り文字: "
 
-#: packages/debugger-extension/src/index.ts:192 packages/debugger-extension/src/index.ts:193 packages/debugger-extension/src/index.ts:214 packages/debugger-extension/src/index.ts:215
+#: packages/debugger-extension/src/index.ts:214 packages/debugger-extension/src/index.ts:215
 msgid "Restart Kernel and Debug…"
 msgstr "カーネル再起動し、デバッグ…"
 
-#: packages/debugger-extension/src/index.ts:339 packages/debugger-extension/src/index.ts:340 packages/debugger-extension/src/index.ts:373 packages/debugger-extension/src/index.ts:374
+#: packages/debugger-extension/src/index.ts:373 packages/debugger-extension/src/index.ts:374
 msgid "Inspect Variable"
 msgstr "変数を調べる"
 
-#: packages/debugger-extension/src/index.ts:403 packages/debugger-extension/src/index.ts:440
+#: packages/debugger-extension/src/index.ts:440
 msgid "Render Variable"
 msgstr "変数の表示"
 
-#: packages/debugger-extension/src/index.ts:404 packages/debugger-extension/src/index.ts:441
+#: packages/debugger-extension/src/index.ts:441
 msgid "Render variable according to its mime type"
 msgstr "MIMEタイプに応じて変数を表示する"
 
 #: packages/debugger-extension/src/index.ts:518
 msgid "Copy to Clipboard"
 msgstr ""
 
@@ -4258,241 +3851,221 @@
 msgid "Copy Variable to Globals"
 msgstr ""
 
 #: packages/debugger-extension/src/index.ts:537
 msgid "Copy variable to globals scope"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:616 packages/debugger-extension/src/index.ts:617 packages/debugger-extension/src/index.ts:623 packages/debugger-extension/src/index.ts:687 packages/debugger-extension/src/index.ts:688 packages/debugger-extension/src/index.ts:694
+#: packages/debugger-extension/src/index.ts:687 packages/debugger-extension/src/index.ts:688 packages/debugger-extension/src/index.ts:694
 msgid "Evaluate Code"
 msgstr "コード評価"
 
-#: packages/debugger-extension/src/index.ts:624 packages/debugger-extension/src/index.ts:695
+#: packages/debugger-extension/src/index.ts:695
 msgid "Evaluate"
 msgstr "評価"
 
-#: packages/debugger-extension/src/index.ts:653 packages/debugger-extension/src/index.ts:658 packages/debugger-extension/src/index.ts:728 packages/debugger-extension/src/index.ts:733
+#: packages/debugger-extension/src/index.ts:728 packages/debugger-extension/src/index.ts:733
 msgid "Continue"
 msgstr "続行"
 
-#: packages/debugger-extension/src/index.ts:654 packages/debugger-extension/src/index.ts:659 packages/debugger-extension/src/index.ts:729 packages/debugger-extension/src/index.ts:734
+#: packages/debugger-extension/src/index.ts:729 packages/debugger-extension/src/index.ts:734
 msgid "Pause"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:678 packages/debugger-extension/src/index.ts:679 packages/debugger-extension/src/index.ts:753 packages/debugger-extension/src/index.ts:754
+#: packages/debugger-extension/src/index.ts:753 packages/debugger-extension/src/index.ts:754
 msgid "Terminate"
 msgstr "停止"
 
-#: packages/debugger-extension/src/index.ts:689 packages/debugger-extension/src/index.ts:690 packages/debugger-extension/src/index.ts:764 packages/debugger-extension/src/index.ts:765
+#: packages/debugger-extension/src/index.ts:764 packages/debugger-extension/src/index.ts:765
 msgid "Next"
 msgstr "次へ"
 
-#: packages/debugger-extension/src/index.ts:699 packages/debugger-extension/src/index.ts:700 packages/debugger-extension/src/index.ts:774 packages/debugger-extension/src/index.ts:775
+#: packages/debugger-extension/src/index.ts:774 packages/debugger-extension/src/index.ts:775
 msgid "Step In"
 msgstr "ステップイン"
 
-#: packages/debugger-extension/src/index.ts:709 packages/debugger-extension/src/index.ts:710 packages/debugger-extension/src/index.ts:784 packages/debugger-extension/src/index.ts:785
+#: packages/debugger-extension/src/index.ts:784 packages/debugger-extension/src/index.ts:785
 msgid "Step Out"
 msgstr "ステップアウト"
 
-#: packages/debugger-extension/src/index.ts:719 packages/debugger-extension/src/index.ts:727
-msgid "Enable / Disable pausing on exceptions"
-msgstr "例外での一時停止の有効/無効"
-
-#: packages/debugger-extension/src/index.ts:724
-msgid "Disable pausing on exceptions"
-msgstr "例外での一時停止の無効"
-
-#: packages/debugger-extension/src/index.ts:725
-msgid "Enable pausing on exceptions"
-msgstr "例外での一時停止の有効"
-
-#: packages/debugger-extension/src/index.ts:726
-msgid "Kernel does not support pausing on exceptions."
-msgstr "カーネルは、例外での一時停止をサポートしていません。"
+#: packages/debugger-extension/src/index.ts:811
+msgid "Select a filter for breakpoints on exception"
+msgstr ""
 
-#: packages/debugger-extension/src/index.ts:775 packages/debugger-extension/src/index.ts:859
+#: packages/debugger-extension/src/index.ts:859
 msgid "Debugger section"
 msgstr "デバッガセクション"
 
-#: packages/debugger-extension/src/index.ts:780 packages/debugger-extension/src/index.ts:861 packages/debugger-extension/src/index.ts:873
+#: packages/debugger-extension/src/index.ts:861 packages/debugger-extension/src/index.ts:873
 msgid "Debugger"
 msgstr "デバッガ"
 
-#: packages/debugger-extension/src/index.ts:811
-msgid "Select a filter for breakpoints on exception"
+#: packages/debugger-extension/src/index.ts:866
+msgid "Debugger Panel"
 msgstr ""
 
-#: packages/debugger/src/handler.ts:39 packages/debugger/src/handler.ts:57
+#: packages/debugger/src/handler.ts:39
 msgid "Enable Debugger"
 msgstr "デバッガ有効"
 
-#: packages/debugger/src/handler.ts:41 packages/debugger/src/handler.ts:59
+#: packages/debugger/src/handler.ts:41
 msgid "Disable Debugger"
 msgstr "デバッガ無効"
 
-#: packages/debugger/src/handler.ts:42 packages/debugger/src/handler.ts:60
+#: packages/debugger/src/handler.ts:42
 msgid "Select a kernel that supports debugging to enable debugger"
 msgstr "デバッグをサポートするカーネルを選択して、デバッガーを有効にします"
 
-#: packages/debugger/src/panels/breakpoints/header.ts:25 packages/debugger/src/panels/breakpoints/index.ts:28 packages/debugger/src/panels/breakpoints/index.ts:39
+#: packages/debugger/src/panels/breakpoints/index.ts:28
 msgid "Breakpoints"
 msgstr "ブレークポイント"
 
 #: packages/debugger/src/panels/breakpoints/index.ts:38
 msgid "Pause on exception filter"
 msgstr ""
 
-#: packages/debugger/src/panels/breakpoints/index.ts:51 packages/debugger/src/panels/breakpoints/index.ts:62 packages/debugger/src/panels/breakpoints/index.ts:63 packages/debugger/src/panels/breakpoints/index.ts:74
+#: packages/debugger/src/panels/breakpoints/index.ts:51 packages/debugger/src/panels/breakpoints/index.ts:63
 msgid "Remove All Breakpoints"
 msgstr "すべてのブレークポイントを削除する"
 
-#: packages/debugger/src/panels/breakpoints/index.ts:52 packages/debugger/src/panels/breakpoints/index.ts:63
+#: packages/debugger/src/panels/breakpoints/index.ts:52
 msgid "Are you sure you want to remove all breakpoints?"
 msgstr "全てのブレークポイントを削除して良いですか？"
 
-#: packages/debugger/src/panels/breakpoints/index.ts:54 packages/debugger/src/panels/breakpoints/index.ts:65
+#: packages/debugger/src/panels/breakpoints/index.ts:54
 msgid "Remove breakpoints"
 msgstr "ブレークポイントの削除"
 
-#: packages/debugger/src/panels/callstack/header.ts:25 packages/debugger/src/panels/callstack/index.ts:27
+#: packages/debugger/src/panels/callstack/index.ts:27
 msgid "Callstack"
 msgstr "コールスタック"
 
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
 msgstr "ソース"
 
-#: packages/debugger/src/panels/sources/index.ts:48 packages/debugger/src/panels/sources/index.tsx:42
+#: packages/debugger/src/panels/sources/index.tsx:42
 msgid "Open in the Main Area"
 msgstr "メインエリアで開く"
 
 #: packages/debugger/src/panels/variables/gridpanel.ts:218
 msgid "Type"
 msgstr ""
 
 #: packages/debugger/src/panels/variables/gridpanel.ts:218
 msgid "Value"
 msgstr ""
 
-#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:1878 packages/filebrowser/src/listing.ts:2258
+#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:2258
 msgid "Name"
 msgstr "名前"
 
-#: packages/debugger/src/panels/variables/header.ts:25 packages/debugger/src/panels/variables/index.ts:33
+#: packages/debugger/src/panels/variables/index.ts:33
 msgid "Variables"
 msgstr "変数"
 
 #: packages/debugger/src/panels/variables/index.ts:78
 msgid "Tree View"
 msgstr ""
 
 #: packages/debugger/src/panels/variables/index.ts:85
 msgid "Table View"
 msgstr ""
 
-#: packages/debugger/src/panels/variables/mimerenderer.ts:53 packages/debugger/src/panels/variables/mimerenderer.ts:58
+#: packages/debugger/src/panels/variables/mimerenderer.ts:58
 msgid "The variable is undefined in the active context."
 msgstr ""
 
-#: packages/debugger/src/panels/variables/scope.tsx:51 packages/debugger/src/panels/variables/scope.tsx:53
+#: packages/debugger/src/panels/variables/scope.tsx:51
 msgid "Scope"
 msgstr "スコープ"
 
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
+msgstr "%1 の新しいビュー"
+
+#: packages/docmanager-extension/src/index.tsx:1084
+msgid "Rename%1…"
+msgstr "%1の名前変更…"
+
+#: packages/docmanager-extension/src/index.tsx:1098
+msgid "Duplicate %1"
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:1113
 msgid "Delete %1"
 msgstr "%1 を削除"
 
-#: packages/docmanager-extension/src/index.tsx:1009 packages/docmanager-extension/src/index.tsx:1030 packages/docmanager-extension/src/index.tsx:1141
-msgid "Show in File Browser"
-msgstr "ファイルブラウザで表示"
-
-#: packages/docmanager-extension/src/index.tsx:1012 packages/docmanager-extension/src/index.tsx:1016 packages/docmanager-extension/src/index.tsx:1123 packages/docmanager-extension/src/index.tsx:1127 packages/docmanager-extension/src/index.tsx:991 packages/docmanager-extension/src/index.tsx:995 packages/filebrowser-extension/src/index.ts:819 packages/filebrowser-extension/src/index.ts:922 packages/filebrowser/src/listing.ts:412 packages/filebrowser/src/listing.ts:416 packages/filebrowser/src/listing.ts:426 packages/filebrowser/src/listing.ts:430
+#: packages/docmanager-extension/src/index.tsx:1123 packages/docmanager-extension/src/index.tsx:1127 packages/filebrowser-extension/src/index.ts:922 packages/filebrowser/src/listing.ts:426 packages/filebrowser/src/listing.ts:430
 msgid "Delete"
 msgstr "削除"
 
-#: packages/docmanager-extension/src/index.tsx:1013 packages/docmanager-extension/src/index.tsx:1124 packages/docmanager-extension/src/index.tsx:992
+#: packages/docmanager-extension/src/index.tsx:1124
 msgid "Are you sure you want to delete %1"
 msgstr "%1 を削除してもよろしいですか?"
 
-#: packages/docmanager-extension/src/index.tsx:1060 packages/docmanager-extension/src/index.tsx:943 packages/docmanager-extension/src/index.tsx:964
-msgid "New View for %1"
-msgstr "%1 の新しいビュー"
+#: packages/docmanager-extension/src/index.tsx:1141
+msgid "Show in File Browser"
+msgstr "ファイルブラウザで表示"
 
-#: packages/docmanager-extension/src/index.tsx:1075 packages/docmanager-extension/src/index.tsx:1096
-msgid "Are you sure you want to revert the %1 to the latest checkpoint? "
-msgstr "%1 を最新のチェックポイントに戻してもよろしいですか? "
+#: packages/docmanager-extension/src/index.tsx:1207
+msgid "Are you sure you want to revert the %1 to checkpoint? "
+msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1081 packages/docmanager-extension/src/index.tsx:1102 packages/docmanager-extension/src/index.tsx:1213
+#: packages/docmanager-extension/src/index.tsx:1213
 msgid "This cannot be undone."
 msgstr "この操作は元に戻すことができません。"
 
-#: packages/docmanager-extension/src/index.tsx:1084 packages/docmanager-extension/src/index.tsx:967 packages/docmanager-extension/src/index.tsx:988
-msgid "Rename%1…"
-msgstr "%1の名前変更…"
-
-#: packages/docmanager-extension/src/index.tsx:1088 packages/docmanager-extension/src/index.tsx:1109 packages/docmanager-extension/src/index.tsx:1220
+#: packages/docmanager-extension/src/index.tsx:1220
 msgid "The checkpoint was last updated at: "
 msgstr "チェックポイントの最終更新日時: "
 
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
@@ -4507,183 +4080,179 @@
 "}\n\n"
 "もし存在しないファイルタイプやビューワーを指定したり、ビューワーが指定されたファイルタイプを開けない場合は、この上書き設定は動作しません。\n\n"
 "利用可能なビューワー:\n"
 "%1\n\n"
 "利用可能なファイルタイプ:\n"
 "%2"
 
-#: packages/docmanager-extension/src/index.tsx:395 packages/docmanager-extension/src/index.tsx:474 packages/filebrowser-extension/src/index.ts:343 packages/filebrowser-extension/src/index.ts:367
+#: packages/docmanager-extension/src/index.tsx:474 packages/filebrowser-extension/src/index.ts:367
 msgid "Download"
 msgstr "ダウンロード"
 
-#: packages/docmanager-extension/src/index.tsx:396 packages/docmanager-extension/src/index.tsx:475
+#: packages/docmanager-extension/src/index.tsx:475
 msgid "Download the file to your computer"
 msgstr "ファイルをあなたのコンピュータにダウンロード"
 
-#: packages/docmanager-extension/src/index.tsx:404 packages/docmanager-extension/src/index.tsx:483
+#: packages/docmanager-extension/src/index.tsx:483
 msgid "Cannot Download"
 msgstr "ダウンロードできません"
 
-#: packages/docmanager-extension/src/index.tsx:405 packages/docmanager-extension/src/index.tsx:484 packages/docmanager-extension/src/index.tsx:641 packages/docmanager-extension/src/index.tsx:686 packages/docmanager-extension/src/index.tsx:726 packages/docmanager-extension/src/index.tsx:749 packages/docmanager-extension/src/index.tsx:771 packages/docmanager-extension/src/index.tsx:844 packages/docmanager-extension/src/index.tsx:873 packages/docmanager-extension/src/index.tsx:968
+#: packages/docmanager-extension/src/index.tsx:484 packages/docmanager-extension/src/index.tsx:726 packages/docmanager-extension/src/index.tsx:771 packages/docmanager-extension/src/index.tsx:844 packages/docmanager-extension/src/index.tsx:968
 msgid "No context found for current widget!"
 msgstr "現在のウィジェットにコンテキストが見つかりませんでした!"
 
-#: packages/docmanager-extension/src/index.tsx:414 packages/docmanager-extension/src/index.tsx:493 packages/docmanager-extension/src/index.tsx:550 packages/docmanager-extension/src/index.tsx:634 packages/filebrowser-extension/src/index.ts:1074 packages/filebrowser-extension/src/index.ts:1200 packages/filebrowser-extension/src/index.ts:566 packages/filebrowser-extension/src/index.ts:790 packages/filebrowser-extension/src/index.ts:892 packages/filebrowser-extension/src/index.ts:968 packages/htmlviewer-extension/src/index.tsx:180 packages/htmlviewer-extension/src/index.tsx:206
+#: packages/docmanager-extension/src/index.tsx:493 packages/docmanager-extension/src/index.tsx:634 packages/filebrowser-extension/src/index.ts:1074 packages/filebrowser-extension/src/index.ts:566 packages/filebrowser-extension/src/index.ts:892 packages/htmlviewer-extension/src/index.tsx:206
 msgid "File Operations"
 msgstr "ファイル操作"
 
-#: packages/docmanager-extension/src/index.tsx:461 packages/docmanager-extension/src/index.tsx:542 packages/filebrowser-extension/src/index.ts:671 packages/filebrowser-extension/src/index.ts:772
+#: packages/docmanager-extension/src/index.tsx:542 packages/filebrowser-extension/src/index.ts:772
 msgid "Open in New Browser Tab"
 msgstr "新規ブラウザタブで開く"
 
-#: packages/docmanager-extension/src/index.tsx:587 packages/docmanager-extension/src/index.tsx:670 packages/filebrowser/src/browser.ts:236 packages/filebrowser/src/browser.ts:282 packages/filebrowser/src/browser.ts:312 packages/logconsole-extension/src/index.tsx:381 packages/logconsole-extension/src/index.tsx:392
+#: packages/docmanager-extension/src/index.tsx:670 packages/filebrowser/src/browser.ts:236 packages/logconsole-extension/src/index.tsx:376
 msgid "Error"
 msgstr "エラー"
 
-#: packages/docmanager-extension/src/index.tsx:625 packages/docmanager-extension/src/index.tsx:647 packages/docmanager-extension/src/index.tsx:710 packages/docmanager-extension/src/index.tsx:732
+#: packages/docmanager-extension/src/index.tsx:704
+msgid "Open the provided `path`."
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:710 packages/docmanager-extension/src/index.tsx:732
 msgid "Reload %1 from Disk"
 msgstr "ディスクから %1 を再読み込み"
 
-#: packages/docmanager-extension/src/index.tsx:629 packages/docmanager-extension/src/index.tsx:714
+#: packages/docmanager-extension/src/index.tsx:714
 msgid "Reload contents from disk"
 msgstr "ディスクから内容を再読み込み"
 
-#: packages/docmanager-extension/src/index.tsx:640 packages/docmanager-extension/src/index.tsx:725
+#: packages/docmanager-extension/src/index.tsx:725
 msgid "Cannot Reload"
 msgstr "再読み込みできません"
 
-#: packages/docmanager-extension/src/index.tsx:648 packages/docmanager-extension/src/index.tsx:733
+#: packages/docmanager-extension/src/index.tsx:733
 msgid "Are you sure you want to reload the %1 from the disk?"
 msgstr "ディスクから %1 を再読み込みしてもよろしいですか?"
 
-#: packages/docmanager-extension/src/index.tsx:671
-msgid "Revert %1 to Checkpoint"
-msgstr "%1 をチェックポイントに戻す"
+#: packages/docmanager-extension/src/index.tsx:756
+msgid "Revert %1 to Checkpoint…"
+msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:675 packages/docmanager-extension/src/index.tsx:760
+#: packages/docmanager-extension/src/index.tsx:760
 msgid "Revert contents to previous checkpoint"
 msgstr "内容を前のチェックポイントに戻す"
 
-#: packages/docmanager-extension/src/index.tsx:685 packages/docmanager-extension/src/index.tsx:770
+#: packages/docmanager-extension/src/index.tsx:770
 msgid "Cannot Revert"
 msgstr "元に戻すことができません"
 
-#: packages/docmanager-extension/src/index.tsx:700 packages/docmanager-extension/src/index.tsx:793
-msgid "Revert %1 to checkpoint"
-msgstr "%1 をチェックポイントに戻す"
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
+msgstr "%1 をチェックポイントに戻す"
+
+#: packages/docmanager-extension/src/index.tsx:797 packages/docregistry/src/context.ts:805
 msgid "Revert"
 msgstr "元に戻す"
 
-#: packages/docmanager-extension/src/index.tsx:725 packages/docmanager-extension/src/index.tsx:820
+#: packages/docmanager-extension/src/index.tsx:820
 msgid "In collaborative mode, the document is saved automatically after every change"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:731 packages/docmanager-extension/src/index.tsx:826
+#: packages/docmanager-extension/src/index.tsx:826
 msgid "Save and create checkpoint"
 msgstr "保存してチェックポイントを作成"
 
-#: packages/docmanager-extension/src/index.tsx:737 packages/docmanager-extension/src/index.tsx:832
+#: packages/docmanager-extension/src/index.tsx:832
 msgid "Save %1"
 msgstr "%1 を保存"
 
-#: packages/docmanager-extension/src/index.tsx:748 packages/docmanager-extension/src/index.tsx:759 packages/docmanager-extension/src/index.tsx:843 packages/docmanager-extension/src/index.tsx:854 packages/docmanager-extension/src/index.tsx:872 packages/docmanager-extension/src/index.tsx:967 packages/notebook/src/default-toolbar.tsx:68
+#: packages/docmanager-extension/src/index.tsx:843 packages/docmanager-extension/src/index.tsx:854 packages/docmanager-extension/src/index.tsx:967 packages/notebook/src/default-toolbar.tsx:68
 msgid "Cannot Save"
 msgstr "保存できません"
 
-#: packages/docmanager-extension/src/index.tsx:756
-msgid "Revert %1 to Checkpoint…"
-msgstr ""
-
-#: packages/docmanager-extension/src/index.tsx:760 packages/docmanager-extension/src/index.tsx:855 packages/notebook/src/default-toolbar.tsx:69
+#: packages/docmanager-extension/src/index.tsx:855 packages/notebook/src/default-toolbar.tsx:69
 msgid "Document is read-only"
 msgstr "ドキュメントは読み取り専用です"
 
-#: packages/docmanager-extension/src/index.tsx:775 packages/docmanager-extension/src/index.tsx:870
+#: packages/docmanager-extension/src/index.tsx:870
 msgid "Rename file"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:776 packages/docmanager-extension/src/index.tsx:871 packages/docmanager/src/dialogs.ts:53 packages/docmanager/src/dialogs.ts:57 packages/filebrowser-extension/src/index.ts:1087 packages/filebrowser-extension/src/index.ts:1197
+#: packages/docmanager-extension/src/index.tsx:871 packages/docmanager/src/dialogs.ts:57 packages/filebrowser-extension/src/index.ts:1197
 msgid "Rename"
 msgstr "名前を変更"
 
-#: packages/docmanager-extension/src/index.tsx:777 packages/docmanager-extension/src/index.tsx:872
+#: packages/docmanager-extension/src/index.tsx:872
 msgid "File name"
 msgstr "ファイル名"
 
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
 msgstr "すべて保存"
 
-#: packages/docmanager-extension/src/index.tsx:840 packages/docmanager-extension/src/index.tsx:935
+#: packages/docmanager-extension/src/index.tsx:935
 msgid "Save all open documents"
 msgstr "開いているすべてのドキュメントを保存"
 
-#: packages/docmanager-extension/src/index.tsx:863 packages/docmanager-extension/src/index.tsx:958
+#: packages/docmanager-extension/src/index.tsx:958
 msgid "Save %1 As…"
 msgstr "%1 を別名で保存…"
 
-#: packages/docmanager-extension/src/index.tsx:864 packages/docmanager-extension/src/index.tsx:959
+#: packages/docmanager-extension/src/index.tsx:959
 msgid "Save with new path"
 msgstr "新しいパスに保存"
 
-#: packages/docmanager-extension/src/index.tsx:883 packages/docmanager-extension/src/index.tsx:904 packages/docmanager-extension/src/index.tsx:999
+#: packages/docmanager-extension/src/index.tsx:999
 msgid "Autosave Documents"
 msgstr "ドキュメントの自動保存"
 
-#: packages/docmanager/src/dialogs.ts:112 packages/docmanager/src/dialogs.ts:114
+#: packages/docmanager/src/dialogs.ts:114
 msgid "Overwrite file?"
 msgstr "ファイルを上書きしますか?"
 
-#: packages/docmanager/src/dialogs.ts:113 packages/docmanager/src/dialogs.ts:115
+#: packages/docmanager/src/dialogs.ts:115
 msgid "\"%1\" already exists, overwrite?"
 msgstr "\"%1\" は既に存在します。上書きしますか?"
 
-#: packages/docmanager/src/dialogs.ts:116 packages/docmanager/src/dialogs.ts:118 packages/docregistry/src/context.ts:809 packages/docregistry/src/context.ts:845 packages/docregistry/src/context.ts:853 packages/docregistry/src/context.ts:865 packages/docregistry/src/context.ts:876 packages/docregistry/src/context.ts:887 packages/docregistry/src/context.ts:888 packages/docregistry/src/context.ts:898 packages/docregistry/src/context.ts:910 packages/docregistry/src/context.ts:921 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutInput.tsx:499 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231 packages/shortcuts-extension/src/components/ShortcutItem.tsx:254
+#: packages/docmanager/src/dialogs.ts:118 packages/docregistry/src/context.ts:809 packages/docregistry/src/context.ts:845 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231
 msgid "Overwrite"
 msgstr "上書き"
 
-#: packages/docmanager/src/dialogs.ts:180 packages/docmanager/src/dialogs.ts:182
+#: packages/docmanager/src/dialogs.ts:182
 msgid "File Path"
 msgstr "ファイルパス"
 
-#: packages/docmanager/src/dialogs.ts:185 packages/docmanager/src/dialogs.ts:187
+#: packages/docmanager/src/dialogs.ts:187
 msgid "New Name"
 msgstr "新規名称"
 
-#: packages/docmanager/src/dialogs.ts:48 packages/docmanager/src/dialogs.ts:52
+#: packages/docmanager/src/dialogs.ts:52
 msgid "Rename File"
 msgstr "ファイル名を変更"
 
-#: packages/docmanager/src/dialogs.ts:61 packages/docmanager/src/dialogs.ts:65 packages/filebrowser/src/listing.ts:1527 packages/filebrowser/src/listing.ts:1875
+#: packages/docmanager/src/dialogs.ts:65 packages/filebrowser/src/listing.ts:1875
 msgid "Rename Error"
 msgstr "名称変更エラー"
 
-#: packages/docmanager/src/dialogs.ts:63 packages/docmanager/src/dialogs.ts:67
+#: packages/docmanager/src/dialogs.ts:67
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr "\"%1\" はファイルの有効な名前ではありません。名前は1文字以上で、\"/\"、\"\\\"、または\":\"を含めることはできません。"
 
 #: packages/docmanager/src/savingstatus.tsx:58
 msgid "Saving completed"
 msgstr ""
 
@@ -4709,180 +4278,160 @@
 msgid "Last Saved: %1\n"
 msgstr "最後に保存: %1\n"
 
 #: packages/docmanager/src/widgetmanager.ts:306
 msgid "Last Checkpoint: %1"
 msgstr "最後のチェックポイント: %1"
 
-#: packages/docmanager/src/widgetmanager.ts:397 packages/docmanager/src/widgetmanager.ts:399
+#: packages/docmanager/src/widgetmanager.ts:397
 msgid "Close and save"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:404 packages/docmanager/src/widgetmanager.ts:406
+#: packages/docmanager/src/widgetmanager.ts:404
 msgid "Close without saving"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:409 packages/docmanager/src/widgetmanager.ts:411 packages/notebook/src/searchprovider.ts:499
+#: packages/docmanager/src/widgetmanager.ts:409 packages/notebook/src/searchprovider.ts:509
 msgid "Confirmation"
 msgstr ""
 
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
 msgstr "別名で保存"
 
-#: packages/docmanager/src/widgetmanager.ts:439 packages/docmanager/src/widgetmanager.ts:441
+#: packages/docmanager/src/widgetmanager.ts:439
 msgid "Save your work"
 msgstr "作業内容の保存"
 
-#: packages/docmanager/src/widgetmanager.ts:440 packages/docmanager/src/widgetmanager.ts:442
+#: packages/docmanager/src/widgetmanager.ts:440
 msgid "Save changes in \"%1\" before closing?"
 msgstr "閉じる前に \"%1\" の変更を保存しますか?"
 
-#: packages/docmanager/src/widgetmanager.ts:443 packages/docmanager/src/widgetmanager.ts:445
+#: packages/docmanager/src/widgetmanager.ts:443
 msgid "Discard"
 msgstr "破棄する"
 
-#: packages/docprovider/src/yprovider.ts:131
-msgid "Session expired"
-msgstr ""
-
-#: packages/docprovider/src/yprovider.ts:132
-msgid "The document session expired. You need to reload this browser tab."
-msgstr ""
-
 #: packages/docregistry/src/context.ts:1021
 msgid "Save File As…"
 msgstr ""
 
-#: packages/docregistry/src/context.ts:1037 packages/docregistry/src/context.ts:1103
-msgid "Save File As.."
-msgstr "別名でファイルを保存.."
-
-#: packages/docregistry/src/context.ts:631 packages/docregistry/src/context.ts:642 packages/docregistry/src/context.ts:665 packages/docregistry/src/context.ts:894 packages/docregistry/src/context.ts:958
+#: packages/docregistry/src/context.ts:631 packages/docregistry/src/context.ts:894
 msgid "File Save Error for %1"
 msgstr "%1 のファイル保存エラー"
 
-#: packages/docregistry/src/context.ts:686 packages/docregistry/src/context.ts:695 packages/docregistry/src/context.ts:709 packages/docregistry/src/context.ts:744 packages/docregistry/src/context.ts:767
+#: packages/docregistry/src/context.ts:695
 msgid "File Load Error for %1"
 msgstr "%1 のファイル読み込みエラー"
 
-#: packages/docregistry/src/context.ts:798 packages/docregistry/src/context.ts:845 packages/docregistry/src/context.ts:868
+#: packages/docregistry/src/context.ts:798
 msgid "\"%1\" has changed on disk since the last time it was opened or saved.\n"
 "Do you want to overwrite the file on disk with the version open here,\n"
 "or load the version on disk (revert)?"
 msgstr ""
 
-#: packages/docregistry/src/context.ts:814 packages/docregistry/src/context.ts:857 packages/docregistry/src/context.ts:880
+#: packages/docregistry/src/context.ts:814
 msgid "File Changed"
 msgstr "ファイルが変更されました"
 
-#: packages/docregistry/src/context.ts:840 packages/docregistry/src/context.ts:882 packages/docregistry/src/context.ts:905
+#: packages/docregistry/src/context.ts:840
 msgid "\"%1\" already exists. Do you want to replace it?"
 msgstr "\"%1\" は既に存在します。置き換えますか?"
 
-#: packages/docregistry/src/context.ts:849 packages/docregistry/src/context.ts:890 packages/docregistry/src/context.ts:913
+#: packages/docregistry/src/context.ts:849
 msgid "File Overwrite?"
 msgstr "ファイルを上書きしますか?"
 
-#: packages/docregistry/src/mimedocument.ts:174 packages/docregistry/src/mimedocument.ts:70 packages/markdownviewer/src/widget.ts:201 packages/markdownviewer/src/widget.ts:211
+#: packages/docregistry/src/mimedocument.ts:174 packages/docregistry/src/mimedocument.ts:70 packages/markdownviewer/src/widget.ts:211
 msgid "Renderer Failure: %1"
 msgstr "レンダラーの失敗: %1"
 
-#: packages/docregistry/src/registry.ts:1287 packages/docregistry/src/registry.ts:1352
+#: packages/docregistry/src/registry.ts:1287
 msgid "default"
 msgstr "デフォルト"
 
-#: packages/docregistry/src/registry.ts:1310 packages/docregistry/src/registry.ts:1375
+#: packages/docregistry/src/registry.ts:1310
 msgid "Text"
 msgstr "テキスト"
 
-#: packages/docregistry/src/registry.ts:1333 packages/docregistry/src/registry.ts:1398 packages/launcher/src/index.tsx:149 packages/launcher/src/index.tsx:154 packages/launcher/src/widget.tsx:115 packages/launcher/src/widget.tsx:120 packages/notebook-extension/src/index.ts:1210 packages/notebook-extension/src/index.ts:1482 packages/notebook-extension/src/index.ts:1519 packages/notebook-extension/src/index.ts:1902 packages/notebook-extension/src/index.ts:1938 packages/notebook-extension/src/index.ts:760
+#: packages/docregistry/src/registry.ts:1333 packages/launcher/src/widget.tsx:115 packages/launcher/src/widget.tsx:120 packages/notebook-extension/src/index.ts:1210 packages/notebook-extension/src/index.ts:1902 packages/notebook-extension/src/index.ts:1938
 msgid "Notebook"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1358 packages/docregistry/src/registry.ts:1423
+#: packages/docregistry/src/registry.ts:1358
 msgid "Directory"
 msgstr "ディレクトリ"
 
-#: packages/docregistry/src/registry.ts:1385 packages/docregistry/src/registry.ts:1450 packages/fileeditor-extension/src/commands.ts:810 packages/fileeditor-extension/src/commands.ts:989
+#: packages/docregistry/src/registry.ts:1385 packages/fileeditor-extension/src/commands.ts:810
 msgid "Markdown File"
 msgstr "Markdownファイル"
 
-#: packages/docregistry/src/registry.ts:1392 packages/docregistry/src/registry.ts:1457
+#: packages/docregistry/src/registry.ts:1392
 msgid "PDF File"
 msgstr "PDFファイル"
 
-#: packages/docregistry/src/registry.ts:1399 packages/docregistry/src/registry.ts:1464 packages/fileeditor-extension/src/index.ts:209 packages/fileeditor-extension/src/index.ts:329
+#: packages/docregistry/src/registry.ts:1399 packages/fileeditor-extension/src/index.ts:329
 msgid "Python File"
 msgstr "Pythonファイル"
 
-#: packages/docregistry/src/registry.ts:1406 packages/docregistry/src/registry.ts:1471
+#: packages/docregistry/src/registry.ts:1406
 msgid "JSON File"
 msgstr "JSONファイル"
 
-#: packages/docregistry/src/registry.ts:1413 packages/docregistry/src/registry.ts:1478 packages/fileeditor-extension/src/index.ts:221 packages/fileeditor-extension/src/index.ts:341
+#: packages/docregistry/src/registry.ts:1413 packages/fileeditor-extension/src/index.ts:341
 msgid "Julia File"
 msgstr "Juliaファイル"
 
-#: packages/docregistry/src/registry.ts:1420 packages/docregistry/src/registry.ts:1485
+#: packages/docregistry/src/registry.ts:1420
 msgid "CSV File"
 msgstr "CSVファイル"
 
-#: packages/docregistry/src/registry.ts:1427 packages/docregistry/src/registry.ts:1492
+#: packages/docregistry/src/registry.ts:1427
 msgid "TSV File"
 msgstr "TSVファイル"
 
-#: packages/docregistry/src/registry.ts:1434 packages/docregistry/src/registry.ts:1499 packages/fileeditor-extension/src/index.ts:233 packages/fileeditor-extension/src/index.ts:353
+#: packages/docregistry/src/registry.ts:1434 packages/fileeditor-extension/src/index.ts:353
 msgid "R File"
 msgstr "Rファイル"
 
-#: packages/docregistry/src/registry.ts:1441 packages/docregistry/src/registry.ts:1506
+#: packages/docregistry/src/registry.ts:1441
 msgid "YAML File"
 msgstr "YAMLファイル"
 
-#: packages/docregistry/src/registry.ts:1448 packages/docregistry/src/registry.ts:1456 packages/docregistry/src/registry.ts:1464 packages/docregistry/src/registry.ts:1472 packages/docregistry/src/registry.ts:1480 packages/docregistry/src/registry.ts:1488 packages/docregistry/src/registry.ts:1496 packages/docregistry/src/registry.ts:1513 packages/docregistry/src/registry.ts:1521 packages/docregistry/src/registry.ts:1529 packages/docregistry/src/registry.ts:1537 packages/docregistry/src/registry.ts:1545 packages/docregistry/src/registry.ts:1553 packages/docregistry/src/registry.ts:1561 packages/imageviewer-extension/src/index.ts:119
+#: packages/docregistry/src/registry.ts:1448 packages/docregistry/src/registry.ts:1456 packages/docregistry/src/registry.ts:1464 packages/docregistry/src/registry.ts:1472 packages/docregistry/src/registry.ts:1480 packages/docregistry/src/registry.ts:1488 packages/docregistry/src/registry.ts:1496 packages/imageviewer-extension/src/index.ts:119
 msgid "Image"
 msgstr "画像"
 
-#: packages/documentsearch-extension/src/index.ts:183 packages/documentsearch-extension/src/index.ts:248
+#: packages/documentsearch-extension/src/index.ts:229 packages/fileeditor-extension/src/commands.ts:525
+msgid "Find…"
+msgstr "検索…"
+
+#: packages/documentsearch-extension/src/index.ts:248
 msgid "Find and Replace…"
 msgstr "検索と置換…"
 
-#: packages/documentsearch-extension/src/index.ts:203 packages/documentsearch-extension/src/index.ts:272
+#: packages/documentsearch-extension/src/index.ts:272
 msgid "Find Next"
 msgstr "次を検索"
 
-#: packages/documentsearch-extension/src/index.ts:227 packages/documentsearch-extension/src/index.ts:287
+#: packages/documentsearch-extension/src/index.ts:287
 msgid "Find Previous"
 msgstr "前を検索"
 
 #: packages/documentsearch-extension/src/index.ts:302
 msgid "End Search"
 msgstr ""
 
-#: packages/documentsearch/src/searchoverlay.tsx:203 packages/documentsearch/src/searchview.tsx:260
-msgid "Replace All"
-msgstr "すべてを置換"
-
-#: packages/documentsearch/src/searchoverlay.tsx:321 packages/notebook/src/searchprovider.ts:222
-msgid "Search Cell Outputs"
-msgstr ""
-
-#: packages/documentsearch/src/searchoverlay.tsx:338
-msgid "Search Selected Cell(s)"
-msgstr ""
-
 #: packages/documentsearch/src/searchview.tsx:169
 msgid "Match Case"
 msgstr ""
 
 #: packages/documentsearch/src/searchview.tsx:177
 msgid "Match Whole Word"
 msgstr ""
@@ -4891,14 +4440,18 @@
 msgid "Use Regular Expression"
 msgstr ""
 
 #: packages/documentsearch/src/searchview.tsx:230
 msgid "Preserve Case"
 msgstr ""
 
+#: packages/documentsearch/src/searchview.tsx:260
+msgid "Replace All"
+msgstr "すべてを置換"
+
 #: packages/documentsearch/src/searchview.tsx:280
 msgid "Previous Match"
 msgstr ""
 
 #: packages/documentsearch/src/searchview.tsx:291
 msgid "Next Match"
 msgstr ""
@@ -4911,101 +4464,55 @@
 msgid "Show Search Filters"
 msgstr ""
 
 #: packages/documentsearch/src/searchview.tsx:637
 msgid "Toggle Replace"
 msgstr ""
 
-#: packages/extensionmanager-extension/src/index.ts:107 packages/extensionmanager-extension/src/index.ts:141
-msgid "Enable Extension Manager"
-msgstr "拡張機能マネージャを有効にする"
-
-#: packages/extensionmanager-extension/src/index.ts:117 packages/extensionmanager-extension/src/index.ts:131 packages/extensionmanager-extension/src/index.ts:153 packages/extensionmanager-extension/src/index.ts:56 packages/extensionmanager-extension/src/index.ts:59
+#: packages/extensionmanager-extension/src/index.ts:131 packages/extensionmanager-extension/src/index.ts:153 packages/extensionmanager-extension/src/index.ts:59
 msgid "Extension Manager"
 msgstr "拡張機能マネージャ"
 
-#: packages/extensionmanager-extension/src/index.ts:143 packages/extensionmanager-extension/src/index.ts:177
+#: packages/extensionmanager-extension/src/index.ts:141
+msgid "Enable Extension Manager"
+msgstr "拡張機能マネージャを有効にする"
+
+#: packages/extensionmanager-extension/src/index.ts:177
 msgid "Enable Extension Manager?"
 msgstr "拡張機能マネージャを有効にしますか?"
 
-#: packages/extensionmanager-extension/src/index.ts:144 packages/extensionmanager-extension/src/index.ts:178
+#: packages/extensionmanager-extension/src/index.ts:178
 msgid "Thanks for trying out JupyterLab's extension manager.\n"
 "The JupyterLab development team is excited to have a robust\n"
 "third-party extension community.\n"
 "However, we cannot vouch for every extension,\n"
 "and some may introduce security risks.\n"
 "Do you want to continue?"
 msgstr "JupyterLabの拡張機能マネージャをお試しいただきありがとうございます。\n"
 "JupyterLab開発チームは拡張機能開発をおこなう力強いサードパーティコミュニティの存在を嬉しく思います。\n"
 "しかし、我々は全ての拡張機能の動作を保証することはできず、場合によってはセキュリティリスクをもたらす可能性もあります。\n"
 "続けますか?"
 
-#: packages/extensionmanager-extension/src/index.ts:151 packages/extensionmanager-extension/src/index.ts:185 packages/extensionmanager/src/widget.tsx:161 packages/extensionmanager/src/widget.tsx:329 packages/extensionmanager/src/widget.tsx:807
+#: packages/extensionmanager-extension/src/index.ts:185 packages/extensionmanager/src/widget.tsx:161
 msgid "Disable"
 msgstr "無効にする"
 
-#: packages/extensionmanager-extension/src/index.ts:152 packages/extensionmanager-extension/src/index.ts:186 packages/extensionmanager/src/widget.tsx:170 packages/extensionmanager/src/widget.tsx:338 packages/extensionmanager/src/widget.tsx:822
+#: packages/extensionmanager-extension/src/index.ts:186 packages/extensionmanager/src/widget.tsx:170
 msgid "Enable"
 msgstr "有効にする"
 
-#: packages/extensionmanager-extension/src/index.ts:61 packages/extensionmanager-extension/src/index.ts:68 packages/extensionmanager-extension/src/index.ts:89
+#: packages/extensionmanager-extension/src/index.ts:61
 msgid "Extension Manager section"
 msgstr ""
 
-#: packages/extensionmanager/src/companions.tsx:137
-msgid "This package has indicated that it needs a corresponding server\n"
-"extension. Please contact your Administrator to update the server with\n"
-"one of the following commands:"
-msgstr "このパッケージは対応するサーバ機能拡張が必要であることを示しています。以下のコマンドの中のいずれかでサーバをアップデートするようシステム管理者に問い合わせてください。"
-
-#: packages/extensionmanager/src/companions.tsx:153
-msgid "This package has indicated that it needs a corresponding package for the kernel."
-msgstr "このパッケージは、カーネルに対応するパッケージが必要であることを示しています。"
-
-#: packages/extensionmanager/src/companions.tsx:161
-msgid "The package <code>%1</code>, is required by the following kernels:"
-msgstr "パッケージ <code>%1</code>は以下のカーネルで必要です:"
-
-#: packages/extensionmanager/src/companions.tsx:178
-msgid "This package has indicated that it needs a corresponding kernel\n"
-"package. Please contact your Administrator to update the server with\n"
-"one of the following commands:"
-msgstr "このパッケージは対応するカーネルパッケージが必要であることを示しています。以下のコマンドの中のいずれかでサーバをアップデートするようシステム管理者に問い合わせてください。"
-
-#: packages/extensionmanager/src/companions.tsx:196
-msgid "You should make sure that the indicated packages are installed before\n"
-"trying to use the extension. Do you want to continue with the extension\n"
-"installation?"
-msgstr "この拡張機能を使うにはあらかじめ指定されたパッケージがインストールされている必要があります。拡張機能のインストールを続けますか?"
-
-#: packages/extensionmanager/src/companions.tsx:206
-msgid "Kernel and Server Companions"
-msgstr "カーネルおよびサーバー コンパニオン"
-
-#: packages/extensionmanager/src/companions.tsx:208
-msgid "Kernel Companions"
-msgstr "カーネル コンパニオン"
-
-#: packages/extensionmanager/src/companions.tsx:210
-msgid "Server Companion"
-msgstr "サーバー コンパニオン"
-
-#: packages/extensionmanager/src/companions.tsx:219
-msgid "Install the JupyterLab extension."
-msgstr "JupyterLab 拡張機能をインストールします。"
-
-#: packages/extensionmanager/src/dialog.tsx:23
-msgid "An error occurred installing <code>%1</code>."
-msgstr "<code>%1</code> のインストール中にエラーが発生しました。"
-
-#: packages/extensionmanager/src/dialog.tsx:27 packages/extensionmanager/src/dialog.tsx:29
+#: packages/extensionmanager/src/dialog.tsx:27
 msgid "Error message:"
 msgstr "エラーメッセージ:"
 
-#: packages/extensionmanager/src/dialog.tsx:35 packages/extensionmanager/src/dialog.tsx:37
+#: packages/extensionmanager/src/dialog.tsx:35
 msgid "Extension Installation Error"
 msgstr "拡張機能のインストールエラー"
 
 #: packages/extensionmanager/src/model.ts:505
 msgid "You will need to restart JupyterLab to apply the changes."
 msgstr ""
 
@@ -5033,35 +4540,23 @@
 msgid "This extension is approved by your security team."
 msgstr ""
 
 #: packages/extensionmanager/src/widget.tsx:133
 msgid "Update \"%1\" to \"%2\""
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:135
-msgid "A build is needed to include the latest changes"
-msgstr "最新の変更を含めるためにビルドが必要です"
-
-#: packages/extensionmanager/src/widget.tsx:138
-msgid "Rebuild"
-msgstr "リビルド"
-
-#: packages/extensionmanager/src/widget.tsx:141
-msgid "Ignore"
-msgstr "無視する"
-
 #: packages/extensionmanager/src/widget.tsx:141
 msgid "Update to %1"
 msgstr ""
 
 #: packages/extensionmanager/src/widget.tsx:146
 msgid "Uninstall \"%1\""
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:150 packages/extensionmanager/src/widget.tsx:320
+#: packages/extensionmanager/src/widget.tsx:150
 msgid "Uninstall"
 msgstr "アンインストール"
 
 #: packages/extensionmanager/src/widget.tsx:157
 msgid "Disable \"%1\""
 msgstr ""
 
@@ -5069,84 +4564,52 @@
 msgid "Enable \"%1\""
 msgstr ""
 
 #: packages/extensionmanager/src/widget.tsx:178
 msgid "Install \"%1\""
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:182 packages/extensionmanager/src/widget.tsx:298
+#: packages/extensionmanager/src/widget.tsx:182
 msgid "Install"
 msgstr "インストール"
 
-#: packages/extensionmanager/src/widget.tsx:193
-msgid "%1 (Developed by Project Jupyter)"
-msgstr "%1 (Project Jupyterによって開発)"
-
-#: packages/extensionmanager/src/widget.tsx:247
-msgid "%1 extension has been blockedExtensions since install. Please uninstall immediately and contact your blockedExtensions administrator."
-msgstr "%1 拡張機能はインストール後にblockedExtensionsとなりました。直ちにアンインストールし、blockedExtensionsの管理者に連絡してください。"
-
-#: packages/extensionmanager/src/widget.tsx:251 packages/extensionmanager/src/widget.tsx:491
+#: packages/extensionmanager/src/widget.tsx:251
 msgid "No entries"
 msgstr "エントリーがありません"
 
-#: packages/extensionmanager/src/widget.tsx:263
-msgid "%1 extension has been removed from the allowedExtensions since installation. Please uninstall immediately and contact your allowedExtensions administrator."
-msgstr "%1 拡張機能はインストール後にallowedExtensionsから削除されました。直ちにアンインストールし、allowedExtensionsの管理者に連絡してください。"
-
-#: packages/extensionmanager/src/widget.tsx:311
-msgid "Update"
-msgstr "アップデート"
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
 msgstr "検索"
 
-#: packages/extensionmanager/src/widget.tsx:365
-msgid "About"
-msgstr ""
-
 #: packages/extensionmanager/src/widget.tsx:379
 msgid "Error when performing an action."
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:380 packages/extensionmanager/src/widget.tsx:844
+#: packages/extensionmanager/src/widget.tsx:380
 msgid "Reason given:"
 msgstr "理由:"
 
-#: packages/extensionmanager/src/widget.tsx:384
-msgid "This is a prebuilt extension. To uninstall it, please\n"
-"    apply following instructions."
-msgstr "これはビルド済みの拡張機能です。 アンインストールするには、\n"
-"  次の手順を行います。"
-
-#: packages/extensionmanager/src/widget.tsx:394
-msgid "This is a prebuilt extension. To uninstall it, please\n"
-"    read the user guide on:"
-msgstr "これはビルド済みの拡張機能です。 アンインストールするには、\n"
-"  ユーザー ガイドをお読みください。:"
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
 
@@ -5158,362 +4621,314 @@
 msgid "No, disable"
 msgstr ""
 
 #: packages/extensionmanager/src/widget.tsx:471 packages/extensionmanager/src/widget.tsx:565
 msgid "Updating extensions list…"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:591 packages/extensionmanager/src/widget.tsx:952
+#: packages/extensionmanager/src/widget.tsx:591
 msgid "Search Results"
 msgstr "検索結果"
 
-#: packages/extensionmanager/src/widget.tsx:592 packages/extensionmanager/src/widget.tsx:953
+#: packages/extensionmanager/src/widget.tsx:592
 msgid "Discover"
 msgstr "見つける"
 
-#: packages/extensionmanager/src/widget.tsx:617 packages/extensionmanager/src/widget.tsx:776 packages/logconsole-extension/src/index.tsx:382 packages/logconsole-extension/src/index.tsx:393 packages/settingeditor/src/settingseditor.tsx:117 packages/settingeditor/src/settingseditor.tsx:122 packages/settingeditor/src/settingseditor.tsx:129 packages/settingeditor/src/settingseditor.tsx:134
+#: packages/extensionmanager/src/widget.tsx:617 packages/logconsole-extension/src/index.tsx:377 packages/settingeditor/src/settingseditor.tsx:122 packages/settingeditor/src/settingseditor.tsx:134
 msgid "Warning"
 msgstr "警告"
 
-#: packages/extensionmanager/src/widget.tsx:623 packages/extensionmanager/src/widget.tsx:899
+#: packages/extensionmanager/src/widget.tsx:623
 msgid "Installed"
 msgstr "インストール済み"
 
 #: packages/extensionmanager/src/widget.tsx:636
 msgid "Refresh extensions list"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:722
-msgid "The extension manager is disabled. Please contact your system\n"
-"administrator to verify the listings configuration."
-msgstr "拡張機能マネージャーが無効になっています。リスト表示の設定を確認するには、システム\n"
-"管理者に問い合わせてください。"
-
-#: packages/extensionmanager/src/widget.tsx:732
-msgid "Read more in the JupyterLab documentation."
-msgstr "JupyterLabのドキュメントで詳細をご覧ください。"
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
-msgstr "拡張機能のリストを更新しています"
-
-#: packages/extensionmanager/src/widget.tsx:839
-msgid "Error communicating with server extension. Consult the documentation\n"
-"            for how to ensure that it is enabled."
-msgstr "サーバー拡張機能との通信中にエラーが発生しました。有効にする方法についてはドキュメントを参照してください。"
-
-#: packages/extensionmanager/src/widget.tsx:852
-msgid "The server has some missing requirements for installing extensions."
-msgstr "サーバにおいて拡張機能をインストールするためのいくつかの要件が不足しています。"
-
-#: packages/extensionmanager/src/widget.tsx:857
-msgid "Details:"
-msgstr "詳細:"
-
 #: packages/extensionmanager/src/widget.tsx:90
 msgid "Version: %1"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:907
-msgid "Refresh extension list"
-msgstr "拡張機能リストを更新"
-
 #: packages/extensionmanager/src/widget.tsx:97
 msgid "%1 extension is not allowed anymore. Please uninstall it immediately or contact your administrator."
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1012 packages/filebrowser-extension/src/index.ts:1028 packages/filebrowser-extension/src/index.ts:1117 packages/filebrowser-extension/src/index.ts:747 packages/filebrowser-extension/src/index.ts:849 packages/filebrowser-extension/src/index.ts:926
-msgid "Open"
-msgstr "開く"
+#: packages/filebrowser-extension/src/index.ts:1014
+msgid "Open from Path…"
+msgstr "パスから開く…"
 
-#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:735 packages/filebrowser-extension/src/index.ts:737 packages/filebrowser-extension/src/index.ts:837 packages/filebrowser-extension/src/index.ts:839 packages/filebrowser-extension/src/index.ts:912 packages/filebrowser-extension/src/index.ts:914
+#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:837 packages/filebrowser-extension/src/index.ts:839
 msgid "Open %1"
 msgstr "%1を開く"
 
-#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:912
-msgid "Open from Path…"
-msgstr "パスから開く…"
-
-#: packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:914
+#: packages/filebrowser-extension/src/index.ts:1016
 msgid "Open from path"
 msgstr "パスから開く"
 
-#: packages/filebrowser-extension/src/index.ts:1025 packages/filebrowser-extension/src/index.ts:1130 packages/fileeditor-extension/src/commands.ts:866 packages/fileeditor-extension/src/commands.ts:974 packages/terminal-extension/src/index.ts:488 packages/terminal-extension/src/index.ts:512
-msgid "Paste"
-msgstr "貼り付け"
-
-#: packages/filebrowser-extension/src/index.ts:1025 packages/filebrowser-extension/src/index.ts:923
+#: packages/filebrowser-extension/src/index.ts:1025
 msgid "Path"
 msgstr "パス"
 
-#: packages/filebrowser-extension/src/index.ts:1027 packages/filebrowser-extension/src/index.ts:925
+#: packages/filebrowser-extension/src/index.ts:1027
 msgid "Open Path"
 msgstr "パスを開く"
 
-#: packages/filebrowser-extension/src/index.ts:1038 packages/filebrowser-extension/src/index.ts:1143 packages/filebrowser/src/opendialog.ts:153 packages/filebrowser/src/opendialog.ts:156
+#: packages/filebrowser-extension/src/index.ts:1028 packages/filebrowser-extension/src/index.ts:1117 packages/filebrowser-extension/src/index.ts:849
+msgid "Open"
+msgstr "開く"
+
+#: packages/filebrowser-extension/src/index.ts:1063
+msgid "Could not find path: %1"
+msgstr "パスが見つかりません: %1"
+
+#: packages/filebrowser-extension/src/index.ts:1065
+msgid "Cannot open"
+msgstr "開けません"
+
+#: packages/filebrowser-extension/src/index.ts:1130 packages/fileeditor-extension/src/commands.ts:974 packages/terminal-extension/src/index.ts:488
+msgid "Paste"
+msgstr "貼り付け"
+
+#: packages/filebrowser-extension/src/index.ts:1143 packages/filebrowser/src/opendialog.ts:153
 msgid "New Folder"
 msgstr "新規フォルダ"
 
-#: packages/filebrowser-extension/src/index.ts:1050 packages/filebrowser-extension/src/index.ts:1155
+#: packages/filebrowser-extension/src/index.ts:1155
 msgid "New File"
 msgstr "新規ファイル"
 
-#: packages/filebrowser-extension/src/index.ts:1062 packages/filebrowser-extension/src/index.ts:1167 packages/fileeditor-extension/src/commands.ts:809 packages/fileeditor-extension/src/commands.ts:988
+#: packages/filebrowser-extension/src/index.ts:1167 packages/fileeditor-extension/src/commands.ts:809
 msgid "New Markdown File"
 msgstr "新規Markdownファイル"
 
-#: packages/filebrowser-extension/src/index.ts:1063 packages/filebrowser-extension/src/index.ts:957
-msgid "Could not find path: %1"
-msgstr "パスが見つかりません: %1"
-
-#: packages/filebrowser-extension/src/index.ts:1065 packages/filebrowser-extension/src/index.ts:959
-msgid "Cannot open"
-msgstr "開けません"
-
-#: packages/filebrowser-extension/src/index.ts:1074 packages/filebrowser-extension/src/index.ts:1179
+#: packages/filebrowser-extension/src/index.ts:1179
 msgid "Refresh the file browser."
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1075 packages/filebrowser-extension/src/index.ts:1180 packages/filebrowser/src/opendialog.ts:168 packages/filebrowser/src/opendialog.ts:171
+#: packages/filebrowser-extension/src/index.ts:1180 packages/filebrowser/src/opendialog.ts:168
 msgid "Refresh File List"
 msgstr "ファイル一覧を更新"
 
-#: packages/filebrowser-extension/src/index.ts:1108 packages/filebrowser-extension/src/index.ts:1220
+#: packages/filebrowser-extension/src/index.ts:1220
 msgid "Copy Path"
 msgstr "パスをコピー"
 
-#: packages/filebrowser-extension/src/index.ts:1120 packages/filebrowser-extension/src/index.ts:1232 packages/mainmenu-extension/src/index.ts:531 packages/mainmenu-extension/src/index.ts:536 packages/notebook-extension/src/index.ts:2332 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66
+#: packages/filebrowser-extension/src/index.ts:1232 packages/mainmenu-extension/src/index.ts:531 packages/notebook-extension/src/index.ts:2332 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66
 msgid "Shut Down Kernel"
 msgstr "カーネルをシャットダウン"
 
-#: packages/filebrowser-extension/src/index.ts:1134 packages/launcher-extension/src/index.ts:59 packages/launcher-extension/src/index.ts:72 packages/ui-components/src/icon/widgets/tabbarsvg.ts:29 packages/ui-components/src/icon/widgets/tabbarsvg.ts:31
-msgid "New Launcher"
-msgstr "新規ランチャー"
-
-#: packages/filebrowser-extension/src/index.ts:1145 packages/filebrowser-extension/src/index.ts:550
-msgid "Show Active File in File Browser"
-msgstr "ファイルブラウザでアクティブなファイルを表示"
-
-#: packages/filebrowser-extension/src/index.ts:1160 packages/filebrowser-extension/src/index.ts:1236
+#: packages/filebrowser-extension/src/index.ts:1236
 msgid "Show Last Modified Column"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1176 packages/filebrowser-extension/src/index.ts:1268
-msgid "Show Hidden Files"
-msgstr ""
-
-#: packages/filebrowser-extension/src/index.ts:1193 packages/filebrowser-extension/src/index.ts:1301
-msgid "Search on File Names"
-msgstr "ファイル名で検索"
-
 #: packages/filebrowser-extension/src/index.ts:1252
 msgid "Show File Size Column"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1272 packages/filebrowser-extension/src/index.ts:1370
-msgid "No browser for path"
-msgstr "パスのブラウザがありません"
+#: packages/filebrowser-extension/src/index.ts:1268
+msgid "Show Hidden Files"
+msgstr ""
 
 #: packages/filebrowser-extension/src/index.ts:1285
 msgid "Show File Checkboxes"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:196 packages/filebrowser-extension/src/index.ts:443
-msgid "File Browser (%1)"
-msgstr "ファイルブラウザ (%1)"
+#: packages/filebrowser-extension/src/index.ts:1301
+msgid "Search on File Names"
+msgstr "ファイル名で検索"
 
-#: packages/filebrowser-extension/src/index.ts:198 packages/filebrowser-extension/src/index.ts:445 packages/filebrowser-extension/src/index.ts:497 packages/filebrowser/src/browser.ts:75
-msgid "File Browser"
-msgstr "ファイルブラウザ"
+#: packages/filebrowser-extension/src/index.ts:1370
+msgid "No browser for path"
+msgstr "パスのブラウザがありません"
 
-#: packages/filebrowser-extension/src/index.ts:360 packages/filebrowser-extension/src/index.ts:389
+#: packages/filebrowser-extension/src/index.ts:389
 msgid "Copy Download Link"
 msgstr "ダウンロードのリンクをコピー"
 
-#: packages/filebrowser-extension/src/index.ts:396 packages/filebrowser-extension/src/index.ts:432
+#: packages/filebrowser-extension/src/index.ts:432
 msgid "File Browser Section"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:475 packages/filebrowser/src/browser.ts:101 packages/filebrowser/src/browser.ts:178
+#: packages/filebrowser-extension/src/index.ts:443
+msgid "File Browser (%1)"
+msgstr "ファイルブラウザ (%1)"
+
+#: packages/filebrowser-extension/src/index.ts:445 packages/filebrowser-extension/src/index.ts:497 packages/filebrowser/src/browser.ts:75
+msgid "File Browser"
+msgstr "ファイルブラウザ"
+
+#: packages/filebrowser-extension/src/index.ts:475
 msgid "Filter files by name"
 msgstr "名前でファイルをフィルタ"
 
 #: packages/filebrowser-extension/src/index.ts:508
 msgid "Open the file browser for the provided `path`."
 msgstr ""
 
 #: packages/filebrowser-extension/src/index.ts:540
 msgid "Hide the file browser."
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:549 packages/filebrowser-extension/src/index.ts:647
+#: packages/filebrowser-extension/src/index.ts:550
+msgid "Show Active File in File Browser"
+msgstr "ファイルブラウザでアクティブなファイルを表示"
+
+#: packages/filebrowser-extension/src/index.ts:647
 msgid "Copy Shareable Link"
 msgstr "共有可能なリンクをコピー"
 
-#: packages/filebrowser-extension/src/index.ts:670 packages/filebrowser-extension/src/index.ts:771
+#: packages/filebrowser-extension/src/index.ts:771
 msgid "Open in Simple Mode"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:735 packages/filebrowser-extension/src/index.ts:837
+#: packages/filebrowser-extension/src/index.ts:837
 msgid "Open from URL…"
 msgstr "URLから開く…"
 
-#: packages/filebrowser-extension/src/index.ts:737 packages/filebrowser-extension/src/index.ts:839
+#: packages/filebrowser-extension/src/index.ts:839
 msgid "Open from URL"
 msgstr "URLから開く"
 
-#: packages/filebrowser-extension/src/index.ts:744 packages/filebrowser-extension/src/index.ts:846
+#: packages/filebrowser-extension/src/index.ts:846
 msgid "URL"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:746 packages/filebrowser-extension/src/index.ts:848
+#: packages/filebrowser-extension/src/index.ts:848
 msgid "Open URL"
 msgstr "URLを開く"
 
-#: packages/filebrowser-extension/src/index.ts:765 packages/filebrowser-extension/src/index.ts:867
+#: packages/filebrowser-extension/src/index.ts:867
 msgid "Could not open URL: %1"
 msgstr "URLから開く…"
 
-#: packages/filebrowser-extension/src/index.ts:767 packages/filebrowser-extension/src/index.ts:869
+#: packages/filebrowser-extension/src/index.ts:869
 msgid "Cannot fetch"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:780 packages/filebrowser-extension/src/index.ts:882 packages/filebrowser/src/upload.ts:51 packages/filebrowser/src/upload.ts:52
+#: packages/filebrowser-extension/src/index.ts:882 packages/filebrowser/src/upload.ts:52
 msgctxt "showErrorMessage"
 msgid "Upload Error"
 msgstr "アップロードのエラー"
 
-#: packages/filebrowser-extension/src/index.ts:832 packages/filebrowser-extension/src/index.ts:935 packages/fileeditor-extension/src/commands.ts:832 packages/fileeditor-extension/src/commands.ts:947 packages/terminal-extension/src/index.ts:463 packages/terminal-extension/src/index.ts:475
+#: packages/filebrowser-extension/src/index.ts:935 packages/fileeditor-extension/src/commands.ts:947 packages/terminal-extension/src/index.ts:463
 msgid "Copy"
 msgstr "コピー"
 
-#: packages/filebrowser-extension/src/index.ts:845 packages/filebrowser-extension/src/index.ts:948 packages/fileeditor-extension/src/commands.ts:791 packages/fileeditor-extension/src/commands.ts:913
+#: packages/filebrowser-extension/src/index.ts:948 packages/fileeditor-extension/src/commands.ts:913
 msgid "Cut"
 msgstr "切り取り"
 
-#: packages/filebrowser-extension/src/index.ts:857 packages/filebrowser-extension/src/index.ts:960
+#: packages/filebrowser-extension/src/index.ts:960
 msgid "Duplicate"
 msgstr "複製"
 
 #: packages/filebrowser-extension/src/index.ts:964
 msgid "Update the file browser to display the provided `path`."
 msgstr ""
 
-#: packages/filebrowser/src/browser.ts:372 packages/filebrowser/src/browser.ts:400
+#: packages/filebrowser/src/browser.ts:372
 msgid "Directory not found"
 msgstr "ディレクトリが見つかりません"
 
-#: packages/filebrowser/src/browser.ts:373 packages/filebrowser/src/browser.ts:401 packages/filebrowser/src/model.ts:298 packages/filebrowser/src/model.ts:305
+#: packages/filebrowser/src/browser.ts:373 packages/filebrowser/src/model.ts:298
 msgid "Directory not found: \"%1\""
 msgstr "ディレクトリが見つかりません: \"%1\""
 
-#: packages/filebrowser/src/browser.ts:69 packages/filebrowser/src/browser.ts:81
+#: packages/filebrowser/src/browser.ts:69
 msgid "file browser"
 msgstr ""
 
 #: packages/filebrowser/src/crumbs.ts:175 packages/filebrowser/src/crumbs.ts:194
 msgid "Open Error"
 msgstr "開く際にエラー"
 
 #: packages/filebrowser/src/crumbs.ts:302
 msgid "Move Error"
 msgstr "移動の際にエラー"
 
-#: packages/filebrowser/src/listing.ts:1015 packages/filebrowser/src/listing.ts:1120
+#: packages/filebrowser/src/listing.ts:1120
 msgctxt "showErrorMessage"
 msgid "Open directory"
 msgstr "ディレクトリを開く"
 
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
 msgstr "ファイルのコピー/移動中にエラー"
 
-#: packages/filebrowser/src/listing.ts:1495 packages/filebrowser/src/listing.ts:1814
+#: packages/filebrowser/src/listing.ts:1814
 msgctxt "showErrorMessage"
 msgid "Delete Failed"
 msgstr "削除に失敗"
 
-#: packages/filebrowser/src/listing.ts:1529 packages/filebrowser/src/listing.ts:1877
+#: packages/filebrowser/src/listing.ts:1877
 msgctxt "showErrorMessage"
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr "\"%1\" はファイルの有効な名前ではありません。名前は1文字以上で、\"/\"、\"\\\"、または\":\"を含めることはできません。"
 
-#: packages/filebrowser/src/listing.ts:1553 packages/filebrowser/src/listing.ts:1896
+#: packages/filebrowser/src/listing.ts:1896
 msgctxt "showErrorMessage"
 msgid "Rename Error"
 msgstr "名称変更エラー"
 
-#: packages/filebrowser/src/listing.ts:1880 packages/filebrowser/src/listing.ts:2260
+#: packages/filebrowser/src/listing.ts:2260
 msgid "Last Modified"
 msgstr "最終更新"
 
-#: packages/filebrowser/src/listing.ts:2051 packages/filebrowser/src/listing.ts:2549
+#: packages/filebrowser/src/listing.ts:2261
+msgid "File Size"
+msgstr ""
+
+#: packages/filebrowser/src/listing.ts:2549
 msgid "Name: %1"
 msgstr "名前: %1"
 
-#: packages/filebrowser/src/listing.ts:2055 packages/filebrowser/src/listing.ts:2555
+#: packages/filebrowser/src/listing.ts:2555
 msgid "\n"
 "Size: %1"
 msgstr "\n"
 "サイズ: %1"
 
-#: packages/filebrowser/src/listing.ts:2063 packages/filebrowser/src/listing.ts:2565
+#: packages/filebrowser/src/listing.ts:2565
 msgid "\n"
 "Path: %1"
 msgstr "\n"
 "パス: %1"
 
-#: packages/filebrowser/src/listing.ts:2070 packages/filebrowser/src/listing.ts:2572
+#: packages/filebrowser/src/listing.ts:2572
 msgid "\n"
 "Created: %1"
 msgstr "\n"
 "作成: %1"
 
-#: packages/filebrowser/src/listing.ts:2076 packages/filebrowser/src/listing.ts:2578
+#: packages/filebrowser/src/listing.ts:2578
 msgid "\n"
 "Modified: %1"
 msgstr "\n"
 "修正: %1"
 
-#: packages/filebrowser/src/listing.ts:2081 packages/filebrowser/src/listing.ts:2583
+#: packages/filebrowser/src/listing.ts:2583
 msgid "\n"
 "Writable: %1"
 msgstr "\n"
 "書き込み可能: %1"
 
-#: packages/filebrowser/src/listing.ts:2151 packages/filebrowser/src/listing.ts:2687
-msgid "%1 Item"
-msgid_plural "%1 Items"
-msgstr[0] "%1 項目"
-
-#: packages/filebrowser/src/listing.ts:2261
-msgid "File Size"
-msgstr ""
-
 #: packages/filebrowser/src/listing.ts:2608
 msgid "Deselect directory \"%1\""
 msgstr ""
 
 #: packages/filebrowser/src/listing.ts:2609
 msgid "Select directory \"%1\""
 msgstr ""
@@ -5522,588 +4937,576 @@
 msgid "Deselect file \"%1\""
 msgstr ""
 
 #: packages/filebrowser/src/listing.ts:2613
 msgid "Select file \"%1\""
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:382 packages/filebrowser/src/listing.ts:396
+#: packages/filebrowser/src/listing.ts:2687
+msgid "%1 Item"
+msgid_plural "%1 Items"
+msgstr[0] "%1 項目"
+
+#: packages/filebrowser/src/listing.ts:396
 msgctxt "showErrorMessage"
 msgid "Paste Error"
 msgstr "貼り付けのエラー"
 
-#: packages/filebrowser/src/listing.ts:402 packages/filebrowser/src/listing.ts:416
+#: packages/filebrowser/src/listing.ts:416
 msgid "Are you sure you want to permanently delete: %1?"
 msgstr "%1を完全に削除してもよろしいですか?"
 
-#: packages/filebrowser/src/listing.ts:406 packages/filebrowser/src/listing.ts:420
+#: packages/filebrowser/src/listing.ts:420
 msgid "Are you sure you want to permanently delete the %1 selected item?"
 msgid_plural "Are you sure you want to permanently delete the %1 selected items?"
 msgstr[0] "選択した項目 %1 を完全に削除してもよろしいですか?"
 
-#: packages/filebrowser/src/listing.ts:448 packages/filebrowser/src/listing.ts:472
+#: packages/filebrowser/src/listing.ts:472
 msgctxt "showErrorMessage"
 msgid "Duplicate file"
 msgstr "重複したファイル"
 
-#: packages/filebrowser/src/listing.ts:488 packages/filebrowser/src/listing.ts:512
+#: packages/filebrowser/src/listing.ts:512
 msgctxt "showErrorMessage"
 msgid "Shut down kernel"
 msgstr "カーネルをシャットダウンします"
 
-#: packages/filebrowser/src/listing.ts:845 packages/filebrowser/src/listing.ts:908
-msgid "%1\n"
-"Kernel: %2"
-msgstr "%1\n"
-"カーネル: %2"
-
 #: packages/filebrowser/src/listing.ts:852
 msgid "Deselect all files and directories"
 msgstr ""
 
 #: packages/filebrowser/src/listing.ts:853
 msgid "Select all files and directories"
 msgstr ""
 
 #: packages/filebrowser/src/listing.ts:906
 msgid "unknown"
 msgstr ""
 
-#: packages/filebrowser/src/model.ts:414 packages/filebrowser/src/model.ts:421
+#: packages/filebrowser/src/listing.ts:908
+msgid "%1\n"
+"Kernel: %2"
+msgstr "%1\n"
+"カーネル: %2"
+
+#: packages/filebrowser/src/model.ts:414
 msgid "Cannot upload file (>%1 MB). %2"
 msgstr "ファイル (>%1 MB) をアップロードできません。 %2"
 
-#: packages/filebrowser/src/model.ts:443 packages/filebrowser/src/model.ts:450
+#: packages/filebrowser/src/model.ts:443
 msgid "Large file size warning"
 msgstr "大きなファイルサイズの警告"
 
-#: packages/filebrowser/src/model.ts:444 packages/filebrowser/src/model.ts:451
+#: packages/filebrowser/src/model.ts:444
 msgid "The file size is %1 MB. Do you still want to upload it?"
 msgstr "ファイルサイズは %1 MB です。それでもアップロードしますか?"
 
-#: packages/filebrowser/src/model.ts:450 packages/filebrowser/src/model.ts:457
+#: packages/filebrowser/src/model.ts:450
 msgid "Upload"
 msgstr "アップロード"
 
-#: packages/filebrowser/src/model.ts:83 packages/filebrowser/src/model.ts:90
+#: packages/filebrowser/src/model.ts:83
 msgid "Files still uploading"
 msgstr "ファイルをアップロード中"
 
-#: packages/filebrowser/src/upload.ts:111 packages/filebrowser/src/upload.ts:117
+#: packages/filebrowser/src/upload.ts:117
 msgid "Upload Files"
 msgstr "ファイルのアップロード"
 
-#: packages/filebrowser/src/uploadstatus.tsx:36 packages/filebrowser/src/uploadstatus.tsx:37
+#: packages/filebrowser/src/uploadstatus.tsx:37
 msgid "Uploading…"
 msgstr "アップロード中…"
 
-#: packages/filebrowser/src/uploadstatus.tsx:95 packages/filebrowser/src/uploadstatus.tsx:96
+#: packages/filebrowser/src/uploadstatus.tsx:96
 msgid "Complete!"
 msgstr "完了!"
 
-#: packages/fileeditor-extension/src/commands.ts:1020 packages/fileeditor-extension/src/commands.ts:1034 packages/fileeditor-extension/src/commands.ts:1050 packages/fileeditor-extension/src/commands.ts:1100 packages/fileeditor-extension/src/commands.ts:1114 packages/fileeditor-extension/src/commands.ts:1130 packages/launcher/src/index.tsx:151 packages/launcher/src/index.tsx:161 packages/launcher/src/index.tsx:437 packages/launcher/src/widget.tsx:117 packages/launcher/src/widget.tsx:127 packages/launcher/src/widget.tsx:295 packages/terminal-extension/src/index.ts:271
+#: packages/fileeditor-extension/src/commands.ts:1100 packages/fileeditor-extension/src/commands.ts:1114 packages/fileeditor-extension/src/commands.ts:1130 packages/launcher/src/widget.tsx:117 packages/launcher/src/widget.tsx:127 packages/launcher/src/widget.tsx:295 packages/terminal-extension/src/index.ts:271
 msgid "Other"
 msgstr "その他"
 
-#: packages/fileeditor-extension/src/commands.ts:1080 packages/fileeditor-extension/src/commands.ts:1104 packages/fileeditor-extension/src/commands.ts:1119 packages/fileeditor-extension/src/commands.ts:1134 packages/fileeditor-extension/src/commands.ts:1152 packages/fileeditor-extension/src/commands.ts:1160 packages/fileeditor-extension/src/commands.ts:1182 packages/fileeditor-extension/src/commands.ts:1197 packages/fileeditor-extension/src/commands.ts:1212 packages/fileeditor-extension/src/commands.ts:1230
+#: packages/fileeditor-extension/src/commands.ts:1160 packages/fileeditor-extension/src/commands.ts:1182 packages/fileeditor-extension/src/commands.ts:1197 packages/fileeditor-extension/src/commands.ts:1212 packages/fileeditor-extension/src/commands.ts:1230
 msgid "Text Editor"
 msgstr "テキストエディタ"
 
-#: packages/fileeditor-extension/src/commands.ts:1274 packages/fileeditor-extension/src/commands.ts:524 packages/fileeditor-extension/src/commands.ts:619
-msgid "Create Console for Editor"
-msgstr "エディターのコンソールを作成"
-
-#: packages/fileeditor-extension/src/commands.ts:1292 packages/fileeditor-extension/src/commands.ts:595
-msgid "Run Code"
-msgstr "コードを実行"
-
-#: packages/fileeditor-extension/src/commands.ts:1293 packages/fileeditor-extension/src/commands.ts:640 packages/fileeditor-extension/src/commands.ts:743
-msgid "Run All Code"
-msgstr "すべてのコードを実行"
-
-#: packages/fileeditor-extension/src/commands.ts:1295
-msgid "Restart Kernel and Run All Code"
-msgstr "カーネルを再起動してすべてのコードを実行"
-
 #: packages/fileeditor-extension/src/commands.ts:1358
 msgid "Code Viewer"
 msgstr ""
 
 #: packages/fileeditor-extension/src/commands.ts:1377
 msgid "Open Code Viewer"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:279 packages/fileeditor-extension/src/commands.ts:297
+#: packages/fileeditor-extension/src/commands.ts:279
 msgid "Increase Text Editor Font Size"
 msgstr "テキストエディタのフォントサイズを大きく"
 
-#: packages/fileeditor-extension/src/commands.ts:283 packages/fileeditor-extension/src/commands.ts:301
+#: packages/fileeditor-extension/src/commands.ts:283
 msgid "Decrease Text Editor Font Size"
 msgstr "テキストエディタのフォントサイズを小さくする"
 
-#: packages/fileeditor-extension/src/commands.ts:306 packages/fileeditor-extension/src/commands.ts:310 packages/mainmenu-extension/src/index.ts:574 packages/mainmenu-extension/src/index.ts:576 packages/notebook-extension/src/index.ts:2963
+#: packages/fileeditor-extension/src/commands.ts:306 packages/fileeditor-extension/src/commands.ts:310 packages/mainmenu-extension/src/index.ts:576 packages/notebook-extension/src/index.ts:2963
 msgid "Show Line Numbers"
 msgstr "行番号を表示"
 
 #: packages/fileeditor-extension/src/commands.ts:311
 msgid "Show the line numbers for the current file."
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:351 packages/fileeditor-extension/src/commands.ts:359
+#: packages/fileeditor-extension/src/commands.ts:351
 msgid "Word Wrap"
 msgstr "文字列折り返し"
 
-#: packages/fileeditor-extension/src/commands.ts:355 packages/mainmenu-extension/src/index.ts:600 packages/mainmenu-extension/src/index.ts:612
+#: packages/fileeditor-extension/src/commands.ts:355 packages/mainmenu-extension/src/index.ts:600
 msgid "Wrap Words"
 msgstr "文字列の折り返し"
 
 #: packages/fileeditor-extension/src/commands.ts:356
 msgid "Wrap words for the current file."
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:375 packages/fileeditor-extension/src/index.ts:102
-msgid "Spaces: %1"
-msgid_plural "Spaces: %1"
-msgstr[0] "スペース: %1"
-
-#: packages/fileeditor-extension/src/commands.ts:381 packages/fileeditor-extension/src/commands.ts:384 packages/fileeditor-extension/src/index.ts:138 packages/fileeditor-extension/src/index.ts:95
-msgid "Indent with Tab"
-msgstr "タブによるインデント"
-
 #: packages/fileeditor-extension/src/commands.ts:382 packages/fileeditor-extension/src/index.ts:145
 msgctxt "v4"
 msgid "Spaces: %1"
 msgstr ""
 
+#: packages/fileeditor-extension/src/commands.ts:384 packages/fileeditor-extension/src/index.ts:138
+msgid "Indent with Tab"
+msgstr "タブによるインデント"
+
 #: packages/fileeditor-extension/src/commands.ts:429
 msgid "Change match brackets for the current file."
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:446
-msgid "Auto Close Brackets for Text Editor"
-msgstr "テキストエディターにて括弧を自動的に閉じる"
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
-msgstr "エディターにて選択範囲を置換する"
-
 #: packages/fileeditor-extension/src/commands.ts:510
 msgid "Editor Theme"
 msgstr ""
 
+#: packages/fileeditor-extension/src/commands.ts:538 packages/mainmenu-extension/src/index.ts:324
+msgid "Go to Line…"
+msgstr "行へ移動…"
+
 #: packages/fileeditor-extension/src/commands.ts:563
 msgid "Change editor language."
 msgstr ""
 
+#: packages/fileeditor-extension/src/commands.ts:601
+msgid "Replace Selection in Editor"
+msgstr "エディターにて選択範囲を置換する"
+
+#: packages/fileeditor-extension/src/commands.ts:619
+msgid "Create Console for Editor"
+msgstr "エディターのコンソールを作成"
+
 #: packages/fileeditor-extension/src/commands.ts:640
 msgid "Restart Kernel"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:673 packages/fileeditor-extension/src/commands.ts:770
-msgid "Show Markdown Preview"
-msgstr "マークダウンのプレビューを表示"
-
 #: packages/fileeditor-extension/src/commands.ts:705
 msgid "Run Selected Code"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:711 packages/fileeditor-extension/src/commands.ts:847 packages/mainmenu-extension/src/index.ts:264 packages/mainmenu-extension/src/index.ts:277 packages/notebook-extension/src/index.ts:3045
-msgid "Undo"
-msgstr "元に戻す"
+#: packages/fileeditor-extension/src/commands.ts:743
+msgid "Run All Code"
+msgstr "すべてのコードを実行"
 
-#: packages/fileeditor-extension/src/commands.ts:749 packages/fileeditor-extension/src/commands.ts:878 packages/mainmenu-extension/src/index.ts:269 packages/mainmenu-extension/src/index.ts:288 packages/notebook-extension/src/index.ts:3031
-msgid "Redo"
-msgstr "やり直す"
+#: packages/fileeditor-extension/src/commands.ts:770
+msgid "Show Markdown Preview"
+msgstr "マークダウンのプレビューを表示"
 
-#: packages/fileeditor-extension/src/commands.ts:781 packages/fileeditor-extension/src/commands.ts:954
+#: packages/fileeditor-extension/src/commands.ts:781
 msgid "New Text File"
 msgstr "新規テキストファイル"
 
-#: packages/fileeditor-extension/src/commands.ts:783 packages/fileeditor-extension/src/commands.ts:956
+#: packages/fileeditor-extension/src/commands.ts:783
 msgid "Text File"
 msgstr "テキストファイル"
 
-#: packages/fileeditor-extension/src/commands.ts:786 packages/fileeditor-extension/src/commands.ts:959
+#: packages/fileeditor-extension/src/commands.ts:786
 msgid "Create a new text file"
 msgstr "新しいテキストファイルを作成"
 
-#: packages/fileeditor-extension/src/commands.ts:811 packages/fileeditor-extension/src/commands.ts:990
+#: packages/fileeditor-extension/src/commands.ts:811
 msgid "Create a new markdown file"
 msgstr "新しいmarkdownファイルを作成"
 
-#: packages/fileeditor-extension/src/commands.ts:891 packages/fileeditor-extension/src/commands.ts:992
+#: packages/fileeditor-extension/src/commands.ts:847 packages/mainmenu-extension/src/index.ts:277 packages/notebook-extension/src/index.ts:3045
+msgid "Undo"
+msgstr "元に戻す"
+
+#: packages/fileeditor-extension/src/commands.ts:878 packages/mainmenu-extension/src/index.ts:288 packages/notebook-extension/src/index.ts:3031
+msgid "Redo"
+msgstr "やり直す"
+
+#: packages/fileeditor-extension/src/commands.ts:992
 msgid "Select All"
 msgstr "すべてを選択"
 
-#: packages/fileeditor-extension/src/index.ts:210 packages/fileeditor-extension/src/index.ts:330
+#: packages/fileeditor-extension/src/index.ts:307
+msgid "Editor"
+msgstr ""
+
+#: packages/fileeditor-extension/src/index.ts:330
 msgid "New Python File"
 msgstr "新規Pythonファイル"
 
-#: packages/fileeditor-extension/src/index.ts:211 packages/fileeditor-extension/src/index.ts:331
+#: packages/fileeditor-extension/src/index.ts:331
 msgid "Create a new Python file"
 msgstr "新しいPythonファイルを作成"
 
-#: packages/fileeditor-extension/src/index.ts:222 packages/fileeditor-extension/src/index.ts:342
+#: packages/fileeditor-extension/src/index.ts:342
 msgid "New Julia File"
 msgstr "新規Juliaファイル"
 
-#: packages/fileeditor-extension/src/index.ts:223 packages/fileeditor-extension/src/index.ts:343
+#: packages/fileeditor-extension/src/index.ts:343
 msgid "Create a new Julia file"
 msgstr "新しいJuliaファイルを作成"
 
-#: packages/fileeditor-extension/src/index.ts:234 packages/fileeditor-extension/src/index.ts:354
+#: packages/fileeditor-extension/src/index.ts:354
 msgid "New R File"
 msgstr "新規Rファイル"
 
-#: packages/fileeditor-extension/src/index.ts:235 packages/fileeditor-extension/src/index.ts:355
+#: packages/fileeditor-extension/src/index.ts:355
 msgid "Create a new R file"
 msgstr "新しいRファイルを作成"
 
-#: packages/fileeditor-extension/src/index.ts:307
-msgid "Editor"
-msgstr ""
+#: packages/fileeditor/src/syntaxstatus.tsx:66
+msgid "Change text editor syntax highlighting"
+msgstr "テキストエディタのシンタックスハイライトを変更"
 
-#: packages/fileeditor/src/tabspacestatus.tsx:48 packages/fileeditor/src/tabspacestatus.tsx:57
+#: packages/fileeditor/src/tabspacestatus.tsx:48
 msgid "Spaces"
 msgstr "スペース"
 
 #: packages/fileeditor/src/tabspacestatus.tsx:49
 msgid "Tab Indent"
 msgstr ""
 
 #: packages/fileeditor/src/tabspacestatus.tsx:58
 msgid "Change the indentation…"
 msgstr ""
 
-#: packages/fileeditor/src/tabspacestatus.tsx:58
-msgid "Tab Size"
-msgstr "タブのサイズ"
-
-#: packages/fileeditor/src/tabspacestatus.tsx:63
-msgid "Change Tab indentation…"
-msgstr "タブのインデントを変更…"
-
 #: packages/help-extension/src/index.tsx:124
 msgid "CONTRIBUTOR LIST"
 msgstr "コントリビューターのリスト"
 
 #: packages/help-extension/src/index.tsx:132
 msgid "ABOUT PROJECT JUPYTER"
 msgstr "PROJECT JUPYTER について"
 
 #: packages/help-extension/src/index.tsx:138
 msgid "© 2015-2023 Project Jupyter Contributors"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:185
-msgid "Launch Classic Notebook"
-msgstr "Classic Notebook を起動する"
-
-#: packages/help-extension/src/index.tsx:186 packages/help-extension/src/index.tsx:215
+#: packages/help-extension/src/index.tsx:186
 msgid "Jupyter Forum"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:223 packages/help-extension/src/index.tsx:250
+#: packages/help-extension/src/index.tsx:223
 msgid "JupyterLab Reference"
 msgstr "JupyterLab リファレンス"
 
-#: packages/help-extension/src/index.tsx:227 packages/help-extension/src/index.tsx:254
+#: packages/help-extension/src/index.tsx:227
 msgid "JupyterLab FAQ"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:231 packages/help-extension/src/index.tsx:259
+#: packages/help-extension/src/index.tsx:231
 msgid "Jupyter Reference"
 msgstr "Jupyter リファレンス"
 
-#: packages/help-extension/src/index.tsx:235 packages/help-extension/src/index.tsx:263
+#: packages/help-extension/src/index.tsx:235
 msgid "Markdown Reference"
 msgstr "Markdown リファレンス"
 
 #: packages/help-extension/src/index.tsx:268
 msgid "Open the provided `url` in a tab."
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:375 packages/help-extension/src/index.tsx:384
+#: packages/help-extension/src/index.tsx:384
 msgid "About the %1 Kernel"
 msgstr "%1 カーネルについて"
 
-#: packages/help-extension/src/index.tsx:480 packages/help-extension/src/index.tsx:486
+#: packages/help-extension/src/index.tsx:480
 msgid "Download All Licenses as"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:481 packages/help-extension/src/index.tsx:487 packages/help-extension/src/licenses.tsx:438 packages/help-extension/src/licenses.tsx:441
+#: packages/help-extension/src/index.tsx:481 packages/help-extension/src/licenses.tsx:441
 msgid "Licenses"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:482 packages/help-extension/src/index.tsx:488
+#: packages/help-extension/src/index.tsx:482
 msgid "Refresh Licenses"
 msgstr ""
 
 #: packages/help-extension/src/index.tsx:93
 msgid "About %1"
 msgstr "%1 について"
 
 #: packages/help-extension/src/index.tsx:96
 msgid "Version %1"
 msgstr "バージョン %1"
 
-#: packages/help-extension/src/licenses.tsx:513 packages/help-extension/src/licenses.tsx:517
+#: packages/help-extension/src/licenses.tsx:517
 msgid "Filter Licenses By"
 msgstr ""
 
-#: packages/help-extension/src/licenses.tsx:517 packages/help-extension/src/licenses.tsx:522 packages/help-extension/src/licenses.tsx:643 packages/help-extension/src/licenses.tsx:650
+#: packages/help-extension/src/licenses.tsx:522 packages/help-extension/src/licenses.tsx:650
 msgid "Package"
 msgstr ""
 
-#: packages/help-extension/src/licenses.tsx:521 packages/help-extension/src/licenses.tsx:526 packages/help-extension/src/licenses.tsx:644 packages/help-extension/src/licenses.tsx:651
+#: packages/help-extension/src/licenses.tsx:526 packages/help-extension/src/licenses.tsx:651
 msgid "Version"
 msgstr ""
 
-#: packages/help-extension/src/licenses.tsx:525 packages/help-extension/src/licenses.tsx:530 packages/help-extension/src/licenses.tsx:645 packages/help-extension/src/licenses.tsx:652 packages/help-extension/src/licenses.tsx:712 packages/help-extension/src/licenses.tsx:719
+#: packages/help-extension/src/licenses.tsx:530 packages/help-extension/src/licenses.tsx:652 packages/help-extension/src/licenses.tsx:719
 msgid "License"
 msgstr ""
 
-#: packages/help-extension/src/licenses.tsx:530 packages/help-extension/src/licenses.tsx:536
+#: packages/help-extension/src/licenses.tsx:536
 msgid "Distributions"
 msgstr ""
 
-#: packages/help-extension/src/licenses.tsx:633 packages/help-extension/src/licenses.tsx:640
+#: packages/help-extension/src/licenses.tsx:640
 msgid "No Packages found"
 msgstr ""
 
-#: packages/help-extension/src/licenses.tsx:707 packages/help-extension/src/licenses.tsx:714
+#: packages/help-extension/src/licenses.tsx:714
 msgid "No Package selected"
 msgstr ""
 
-#: packages/help-extension/src/licenses.tsx:713 packages/help-extension/src/licenses.tsx:720
+#: packages/help-extension/src/licenses.tsx:720
 msgid "No License ID found"
 msgstr ""
 
-#: packages/help-extension/src/licenses.tsx:715 packages/help-extension/src/licenses.tsx:722
+#: packages/help-extension/src/licenses.tsx:722
 msgid "No License Text found"
 msgstr ""
 
-#: packages/htmlviewer-extension/src/index.tsx:102 packages/htmlviewer-extension/src/index.tsx:105
+#: packages/htmlviewer-extension/src/index.tsx:105
 msgid "HTML File"
 msgstr "HTMLファイル"
 
 #: packages/htmlviewer-extension/src/index.tsx:115
 msgid "HTML Viewer"
 msgstr ""
 
-#: packages/htmlviewer-extension/src/index.tsx:155 packages/htmlviewer-extension/src/index.tsx:181
+#: packages/htmlviewer-extension/src/index.tsx:181
 msgid "Trust HTML File"
 msgstr "HTMLファイルを信用する"
 
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
 msgstr "HTMLドキュメントを再表示"
 
-#: packages/htmlviewer/src/index.tsx:333 packages/htmlviewer/src/widget.tsx:315
+#: packages/htmlviewer/src/widget.tsx:315
 msgid "Whether the HTML file is trusted.\n"
 "Trusting the file allows scripts to run in it,\n"
 "which may result in security risks.\n"
 "Only enable for files you trust."
 msgstr "そのHTMLファイルを信用するか否か。該当ファイル内のスクリプト実行を許容するものであり、セキュリティリスクをもたらす可能性があります。ファイルを信用できる時のみ有効にしてください。"
 
-#: packages/htmlviewer/src/index.tsx:339 packages/htmlviewer/src/widget.tsx:321
+#: packages/htmlviewer/src/widget.tsx:321
 msgid "Distrust HTML"
 msgstr "HTMLを信用しない"
 
-#: packages/htmlviewer/src/index.tsx:340 packages/htmlviewer/src/widget.tsx:322
+#: packages/htmlviewer/src/widget.tsx:322
 msgid "Trust HTML"
 msgstr "HTMLを信用する"
 
-#: packages/hub-extension/src/index.ts:154 packages/hub-extension/src/index.ts:166
+#: packages/hub-extension/src/index.ts:166
 msgid "Server unavailable or unreachable"
 msgstr ""
 
-#: packages/hub-extension/src/index.ts:155 packages/hub-extension/src/index.ts:167
+#: packages/hub-extension/src/index.ts:167
 msgid "Your server at %1 is not running.\n"
 "Would you like to restart it?"
 msgstr "%1 のサーバーが動作していません。\n"
 "再起動しますか?"
 
-#: packages/hub-extension/src/index.ts:160 packages/hub-extension/src/index.ts:172
+#: packages/hub-extension/src/index.ts:172
 msgid "Restart"
 msgstr "再起動"
 
-#: packages/hub-extension/src/index.ts:66 packages/hub-extension/src/index.ts:67
+#: packages/hub-extension/src/index.ts:67
 msgid "Restart Server"
 msgstr "サーバーを再起動"
 
-#: packages/hub-extension/src/index.ts:67 packages/hub-extension/src/index.ts:68
+#: packages/hub-extension/src/index.ts:68
 msgid "Request that the Hub restart this server"
 msgstr "ハブがこのサーバーを再起動するようリクエスト"
 
-#: packages/hub-extension/src/index.ts:74 packages/hub-extension/src/index.ts:75
+#: packages/hub-extension/src/index.ts:75
 msgid "Hub Control Panel"
 msgstr "Hub コントロールパネル"
 
-#: packages/hub-extension/src/index.ts:75 packages/hub-extension/src/index.ts:76
+#: packages/hub-extension/src/index.ts:76
 msgid "Open the Hub control panel in a new browser tab"
 msgstr "新しいブラウザタブでHubコントロールパネルを開く"
 
-#: packages/hub-extension/src/index.ts:82 packages/hub-extension/src/index.ts:83 packages/mainmenu-extension/src/index.ts:443 packages/mainmenu-extension/src/index.ts:450
+#: packages/hub-extension/src/index.ts:83 packages/mainmenu-extension/src/index.ts:443
 msgid "Log Out"
 msgstr "ログアウト"
 
-#: packages/hub-extension/src/index.ts:83 packages/hub-extension/src/index.ts:84
+#: packages/hub-extension/src/index.ts:84
 msgid "Log out of the Hub"
 msgstr "Hub からログアウト"
 
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
 msgstr "画像ビューア"
 
-#: packages/imageviewer-extension/src/index.ts:199 packages/imageviewer-extension/src/index.ts:202
+#: packages/imageviewer-extension/src/index.ts:202
 msgid "Zoom In"
 msgstr "ズームイン"
 
-#: packages/imageviewer-extension/src/index.ts:205 packages/imageviewer-extension/src/index.ts:208
+#: packages/imageviewer-extension/src/index.ts:208
 msgid "Zoom Out"
 msgstr "ズームアウト"
 
-#: packages/imageviewer-extension/src/index.ts:211 packages/imageviewer-extension/src/index.ts:214
+#: packages/imageviewer-extension/src/index.ts:214
 msgid "Reset Image"
 msgstr "画像をリセット"
 
-#: packages/imageviewer-extension/src/index.ts:217 packages/imageviewer-extension/src/index.ts:220
+#: packages/imageviewer-extension/src/index.ts:220
 msgid "Rotate Clockwise"
 msgstr "時計回りに回転"
 
-#: packages/imageviewer-extension/src/index.ts:223 packages/imageviewer-extension/src/index.ts:226
+#: packages/imageviewer-extension/src/index.ts:226
 msgid "Rotate Counterclockwise"
 msgstr "反時計回りに回転"
 
-#: packages/imageviewer-extension/src/index.ts:229 packages/imageviewer-extension/src/index.ts:232
+#: packages/imageviewer-extension/src/index.ts:232
 msgid "Flip image horizontally"
 msgstr "画像を横方向に反転"
 
-#: packages/imageviewer-extension/src/index.ts:235 packages/imageviewer-extension/src/index.ts:238
+#: packages/imageviewer-extension/src/index.ts:238
 msgid "Flip image vertically"
 msgstr "画像を垂直方向に反転"
 
-#: packages/imageviewer-extension/src/index.ts:241 packages/imageviewer-extension/src/index.ts:244
+#: packages/imageviewer-extension/src/index.ts:244
 msgid "Invert Colors"
 msgstr "色を反転"
 
-#: packages/inspector-extension/src/index.ts:105 packages/inspector-extension/src/index.ts:136 packages/inspector-extension/src/index.ts:57
+#: packages/inspector-extension/src/index.ts:106 packages/inspector-extension/src/index.ts:137
 msgid "Show Contextual Help"
 msgstr "コンテキストヘルプを表示"
 
-#: packages/inspector-extension/src/index.ts:126
+#: packages/inspector-extension/src/index.ts:127
 msgid "Hide Contextual Help"
 msgstr ""
 
-#: packages/inspector-extension/src/index.ts:59 packages/inspector-extension/src/index.ts:91
+#: packages/inspector-extension/src/index.ts:60
 msgid "Live updating code documentation from the active kernel"
 msgstr "アクティブなカーネルからコードドキュメントをライブ更新する"
 
-#: packages/inspector-extension/src/index.ts:62
+#: packages/inspector-extension/src/index.ts:63
 msgid "Contextual Help"
 msgstr ""
 
-#: packages/inspector/src/inspector.ts:51 packages/inspector/src/inspector.ts:52
+#: packages/inspector/src/inspector.ts:52
 msgid "Click on a function to see documentation."
 msgstr "ドキュメントを見るには関数をクリックしてください。"
 
 #: packages/javascript-extension/src/index.ts:41
 msgid "Are you sure that you want to run arbitrary Javascript within your JupyterLab session?"
 msgstr "JupyterLab セッション内で任意の Javascript を実行してもよろしいですか?"
 
-#: packages/javascript-extension/src/index.ts:45 packages/rendermime/src/renderers.ts:66 packages/rendermime/src/renderers.ts:70
+#: packages/javascript-extension/src/index.ts:45 packages/rendermime/src/renderers.ts:66
 msgid "Run"
 msgstr "実行"
 
-#: packages/json-extension/src/component.tsx:63 packages/json-extension/src/component.tsx:78
+#: packages/json-extension/src/component.tsx:78
 msgid "Filter…"
 msgstr "フィルタ…"
 
-#: packages/launcher-extension/src/index.ts:103 packages/launcher-extension/src/index.ts:148 packages/launcher-extension/src/index.ts:76 packages/launcher-extension/src/index.ts:94
+#: packages/launcher-extension/src/index.ts:148 packages/launcher-extension/src/index.ts:94
 msgid "Launcher"
 msgstr "ランチャー"
 
-#: packages/launcher/src/index.tsx:411 packages/launcher/src/widget.tsx:272
+#: packages/launcher-extension/src/index.ts:72 packages/ui-components/src/icon/widgets/tabbarsvg.ts:31
+msgid "New Launcher"
+msgstr "新規ランチャー"
+
+#: packages/launcher/src/widget.tsx:272
 msgctxt "Error"
 msgid "Launcher Error"
 msgstr "ランチャーのエラー"
 
-#: packages/logconsole-extension/src/index.tsx:142 packages/logconsole-extension/src/index.tsx:143 packages/logconsole/src/widget.ts:389
+#: packages/logconsole-extension/src/index.tsx:136 packages/logconsole/src/widget.ts:389
 msgid "Log Console"
 msgstr "ログコンソール"
 
-#: packages/logconsole-extension/src/index.tsx:191 packages/logconsole-extension/src/index.tsx:200
+#: packages/logconsole-extension/src/index.tsx:193
 msgid "Show Log Console"
 msgstr "ログコンソールを表示"
 
-#: packages/logconsole-extension/src/index.tsx:211 packages/logconsole-extension/src/index.tsx:220
+#: packages/logconsole-extension/src/index.tsx:213
 msgid "Add Checkpoint"
 msgstr "チェックポイントを追加"
 
-#: packages/logconsole-extension/src/index.tsx:220 packages/logconsole-extension/src/index.tsx:229
+#: packages/logconsole-extension/src/index.tsx:222
 msgid "Clear Log"
 msgstr "ログを消去"
 
-#: packages/logconsole-extension/src/index.tsx:236 packages/logconsole-extension/src/index.tsx:246
+#: packages/logconsole-extension/src/index.tsx:239
 msgid "Set Log Level to %1"
 msgstr "ログレベルを %1 に設定"
 
-#: packages/logconsole-extension/src/index.tsx:247
+#: packages/logconsole-extension/src/index.tsx:240
 msgid "Set log level to `level`."
 msgstr ""
 
-#: packages/logconsole-extension/src/index.tsx:366 packages/logconsole-extension/src/index.tsx:377
+#: packages/logconsole-extension/src/index.tsx:361
 msgid "Log Level:"
 msgstr "ログレベル:"
 
-#: packages/logconsole-extension/src/index.tsx:374 packages/logconsole-extension/src/index.tsx:385
+#: packages/logconsole-extension/src/index.tsx:369
 msgid "Log level"
 msgstr "ログレベル"
 
-#: packages/logconsole-extension/src/index.tsx:380 packages/logconsole-extension/src/index.tsx:391
+#: packages/logconsole-extension/src/index.tsx:375
 msgid "Critical"
 msgstr "重大"
 
-#: packages/logconsole-extension/src/index.tsx:383 packages/logconsole-extension/src/index.tsx:394
+#: packages/logconsole-extension/src/index.tsx:378
 msgid "Info"
 msgstr "情報"
 
-#: packages/logconsole-extension/src/index.tsx:384 packages/logconsole-extension/src/index.tsx:395
+#: packages/logconsole-extension/src/index.tsx:379
 msgid "Debug"
 msgstr "デバッグ"
 
-#: packages/logconsole-extension/src/status.tsx:29 packages/logconsole-extension/src/status.tsx:30
+#: packages/logconsole-extension/src/status.tsx:29
 msgid "%1 new messages, %2 log entries for %3"
 msgstr "%3 についての %1 件の新しいメッセージ、%2 件のログエントリ"
 
-#: packages/logconsole-extension/src/status.tsx:36 packages/logconsole-extension/src/status.tsx:37
+#: packages/logconsole-extension/src/status.tsx:36
 msgid "%1 log entries for %2"
 msgstr "%2 についての %1 ログエントリ"
 
 #: packages/logconsole/src/widget.ts:390
 msgid "Log: %1"
 msgstr "ログ: %1"
 
@@ -6115,15 +5518,15 @@
 msgid "No log messages."
 msgstr "ログメッセージはありません。"
 
 #: packages/lsp-extension/src/index.ts:257
 msgid "Language servers"
 msgstr ""
 
-#: packages/lsp-extension/src/index.ts:276 packages/mainmenu-extension/src/index.ts:549 packages/mainmenu-extension/src/index.ts:552 packages/running-extension/src/kernels.ts:40 packages/running-extension/src/kernels.ts:67 packages/running/src/index.tsx:222 packages/running/src/index.tsx:357 packages/terminal-extension/src/index.ts:303 packages/terminal-extension/src/index.ts:323
+#: packages/lsp-extension/src/index.ts:276 packages/mainmenu-extension/src/index.ts:549 packages/running-extension/src/kernels.ts:67 packages/running/src/index.tsx:357 packages/terminal-extension/src/index.ts:323
 msgid "Shut Down All"
 msgstr "すべてシャットダウン"
 
 #: packages/lsp-extension/src/index.ts:277
 msgid "Are you sure you want to permanently shut down all running language servers?"
 msgstr ""
 
@@ -6147,566 +5550,318 @@
 msgid "Add server"
 msgstr ""
 
 #: packages/lsp/src/adapters/adapter.ts:455 packages/lsp/src/adapters/adapter.ts:473
 msgid "Message from "
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:185 packages/mainmenu-extension/src/index.ts:193
+#: packages/mainmenu-extension/src/index.ts:193
 msgid "Open Edit Menu"
 msgstr "編集メニューを開く"
 
-#: packages/mainmenu-extension/src/index.ts:189 packages/mainmenu-extension/src/index.ts:197
+#: packages/mainmenu-extension/src/index.ts:197
 msgid "Open File Menu"
 msgstr "ファイルメニューを開く"
 
-#: packages/mainmenu-extension/src/index.ts:193 packages/mainmenu-extension/src/index.ts:201
+#: packages/mainmenu-extension/src/index.ts:201
 msgid "Open Kernel Menu"
 msgstr "カーネルメニューを開く"
 
-#: packages/mainmenu-extension/src/index.ts:197 packages/mainmenu-extension/src/index.ts:205
+#: packages/mainmenu-extension/src/index.ts:205
 msgid "Open Run Menu"
 msgstr "実行メニューを開く"
 
-#: packages/mainmenu-extension/src/index.ts:201 packages/mainmenu-extension/src/index.ts:209
+#: packages/mainmenu-extension/src/index.ts:209
 msgid "Open View Menu"
 msgstr "ビューメニューを開く"
 
-#: packages/mainmenu-extension/src/index.ts:205 packages/mainmenu-extension/src/index.ts:213
+#: packages/mainmenu-extension/src/index.ts:213
 msgid "Open Settings Menu"
 msgstr "設定メニューを開く"
 
-#: packages/mainmenu-extension/src/index.ts:209 packages/mainmenu-extension/src/index.ts:217
+#: packages/mainmenu-extension/src/index.ts:217
 msgid "Open Tabs Menu"
 msgstr "タブメニューを開く"
 
-#: packages/mainmenu-extension/src/index.ts:213 packages/mainmenu-extension/src/index.ts:221
+#: packages/mainmenu-extension/src/index.ts:221
 msgid "Open Help Menu"
 msgstr "ヘルプメニューを開く"
 
-#: packages/mainmenu-extension/src/index.ts:217 packages/mainmenu-extension/src/index.ts:225
+#: packages/mainmenu-extension/src/index.ts:225
 msgid "Open First Menu"
 msgstr "最初のメニューを開く"
 
-#: packages/mainmenu-extension/src/index.ts:237 packages/mainmenu-extension/src/index.ts:245
+#: packages/mainmenu-extension/src/index.ts:245
 msgid "Kernel Operations"
 msgstr "カーネル操作"
 
-#: packages/mainmenu-extension/src/index.ts:282 packages/mainmenu-extension/src/index.ts:301
+#: packages/mainmenu-extension/src/index.ts:301
 msgid "Clear"
 msgstr "消去"
 
-#: packages/mainmenu-extension/src/index.ts:298 packages/mainmenu-extension/src/index.ts:312
+#: packages/mainmenu-extension/src/index.ts:312
 msgid "Clear All"
 msgstr "すべて消去"
 
-#: packages/mainmenu-extension/src/index.ts:341
-msgid "Close and Shutdown"
-msgstr "閉じてシャットダウン"
-
-#: packages/mainmenu-extension/src/index.ts:352 packages/notebook-extension/src/index.ts:1735
+#: packages/mainmenu-extension/src/index.ts:352
 msgid "Close and Shut Down"
 msgstr "閉じてシャットダウン"
 
-#: packages/mainmenu-extension/src/index.ts:368 packages/mainmenu-extension/src/index.ts:371
+#: packages/mainmenu-extension/src/index.ts:368
 msgid "New Console for Activity"
 msgstr "アクティビティの新規コンソール"
 
-#: packages/mainmenu-extension/src/index.ts:376 packages/mainmenu-extension/src/index.ts:383
+#: packages/mainmenu-extension/src/index.ts:376
 msgid "Shut down JupyterLab"
 msgstr "JupyterLabをシャットダウン"
 
-#: packages/mainmenu-extension/src/index.ts:381 packages/mainmenu-extension/src/index.ts:388
+#: packages/mainmenu-extension/src/index.ts:381
 msgid "Shutdown confirmation"
 msgstr "シャットダウンの確認"
 
-#: packages/mainmenu-extension/src/index.ts:382 packages/mainmenu-extension/src/index.ts:389
+#: packages/mainmenu-extension/src/index.ts:382
 msgid "Please confirm you want to shut down JupyterLab."
 msgstr "JupyterLabをシャットダウンするか確認してください。"
 
-#: packages/mainmenu-extension/src/index.ts:414 packages/mainmenu-extension/src/index.ts:421
+#: packages/mainmenu-extension/src/index.ts:414
 msgid "You have shut down the Jupyter server. You can now close this tab."
 msgstr "Jupyter サーバをシャットダウンしました。このタブを閉じることができます。"
 
-#: packages/mainmenu-extension/src/index.ts:418 packages/mainmenu-extension/src/index.ts:425
+#: packages/mainmenu-extension/src/index.ts:418
 msgid "To use JupyterLab again, you will need to relaunch it."
 msgstr "JupyterLabを再び使用するには、再起動する必要があります。"
 
-#: packages/mainmenu-extension/src/index.ts:425 packages/mainmenu-extension/src/index.ts:432
+#: packages/mainmenu-extension/src/index.ts:425
 msgid "Server stopped"
 msgstr "サーバは停止しました"
 
-#: packages/mainmenu-extension/src/index.ts:444 packages/mainmenu-extension/src/index.ts:451
+#: packages/mainmenu-extension/src/index.ts:444
 msgid "Log out of JupyterLab"
 msgstr "JupyterLabからログアウト"
 
-#: packages/mainmenu-extension/src/index.ts:482 packages/mainmenu-extension/src/index.ts:483 packages/notebook-extension/src/index.ts:3081
+#: packages/mainmenu-extension/src/index.ts:482 packages/notebook-extension/src/index.ts:3081
 msgid "Reconnect to Kernel"
 msgstr "カーネルに再接続"
 
 #: packages/mainmenu-extension/src/index.ts:507
 msgid "Restart Kernel and Clear…"
 msgstr "カーネルを再起動してクリア…"
 
 #: packages/mainmenu-extension/src/index.ts:532
 msgid "Shut down kernel"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:539 packages/mainmenu-extension/src/index.ts:542
+#: packages/mainmenu-extension/src/index.ts:539
 msgid "Shut Down All Kernels…"
 msgstr "すべてのカーネルをシャットダウン…"
 
-#: packages/mainmenu-extension/src/index.ts:545 packages/mainmenu-extension/src/index.ts:548
+#: packages/mainmenu-extension/src/index.ts:545
 msgid "Shut Down All?"
 msgstr "すべてシャットダウンしますか?"
 
-#: packages/mainmenu-extension/src/index.ts:546 packages/mainmenu-extension/src/index.ts:549
+#: packages/mainmenu-extension/src/index.ts:546
 msgid "Shut down all kernels?"
 msgstr "すべてのカーネルをシャットダウンしますか?"
 
-#: packages/mainmenu-extension/src/index.ts:622 packages/mainmenu-extension/src/index.ts:623 packages/mainmenu-extension/src/index.ts:645 packages/mainmenu-extension/src/index.ts:654
+#: packages/mainmenu-extension/src/index.ts:622 packages/mainmenu-extension/src/index.ts:623
 msgid "Run Selected"
 msgstr "選択したものを実行"
 
-#: packages/mainmenu-extension/src/index.ts:636 packages/mainmenu-extension/src/index.ts:637 packages/mainmenu-extension/src/index.ts:663 packages/mainmenu-extension/src/index.ts:679
+#: packages/mainmenu-extension/src/index.ts:636 packages/mainmenu-extension/src/index.ts:637
 msgid "Run All"
 msgstr "すべて実行"
 
-#: packages/mainmenu-extension/src/index.ts:648 packages/mainmenu-extension/src/index.ts:649 packages/mainmenu-extension/src/index.ts:699 packages/mainmenu-extension/src/index.ts:715
+#: packages/mainmenu-extension/src/index.ts:648 packages/mainmenu-extension/src/index.ts:649
 msgid "Restart Kernel and Run All"
 msgstr "カーネルを再起動してすべて実行"
 
 #: packages/mainmenu-extension/src/index.ts:677
 msgid "Activate a widget by its `id`."
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:694 packages/mainmenu-extension/src/index.ts:774
+#: packages/mainmenu-extension/src/index.ts:694
 msgid "Activate Previously Used Tab"
 msgstr "前に使用したタブをアクティブにする"
 
-#: packages/mainmenu-extension/src/index.ts:771 packages/mainmenu-extension/src/index.ts:943
+#: packages/mainmenu-extension/src/index.ts:771
 msgid "Menu customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr ""
 
-#: packages/markdownviewer-extension/src/index.ts:117 packages/markdownviewer-extension/src/index.ts:138 packages/markdownviewer-extension/src/index.ts:143
+#: packages/markdownviewer-extension/src/index.ts:117 packages/markdownviewer-extension/src/index.ts:143
 msgid "Markdown Preview"
 msgstr "Markdown プレビュー"
 
-#: packages/markdownviewer-extension/src/index.ts:173 packages/markdownviewer-extension/src/index.ts:178
+#: packages/markdownviewer-extension/src/index.ts:178
 msgid "Show Markdown Editor"
 msgstr "Markdown エディタを表示"
 
 #: packages/metadataform/src/metadataform.ts:54
 msgid "No metadata."
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1012 packages/notebook-extension/src/index.ts:1335 packages/notebook-extension/src/index.ts:2705
+#: packages/notebook-extension/src/index.ts:1113
+msgid "Notebook Tools"
+msgstr "Notebookツール"
+
+#: packages/notebook-extension/src/index.ts:1265
+msgid "Create New View for Cell Output"
+msgstr ""
+
+#: packages/notebook-extension/src/index.ts:1335
 msgid "New Console for Notebook"
 msgstr "Notebook用の新しいコンソール"
 
-#: packages/notebook-extension/src/index.ts:1030 packages/notebook-extension/src/index.ts:1353
+#: packages/notebook-extension/src/index.ts:1353
 msgid "Run Selected Text or Current Line in Console"
 msgstr "選択したテキストまたは現在の行をコンソールで実行"
 
-#: packages/notebook-extension/src/index.ts:1113 packages/notebook-extension/src/index.ts:783
-msgid "Notebook Tools"
-msgstr "Notebookツール"
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
 msgstr "新しいNotebook"
 
-#: packages/notebook-extension/src/index.ts:1484 packages/notebook-extension/src/index.ts:1904
+#: packages/notebook-extension/src/index.ts:1904
 msgid "Create a new notebook"
 msgstr "新しいnotebookを作成する"
 
-#: packages/notebook-extension/src/index.ts:1617 packages/notebook-extension/src/index.ts:2728
-msgid "Run Selected Cells"
-msgstr "選択したセルを実行"
-
-#: packages/notebook-extension/src/index.ts:1630
-msgid "Run Selected Cells and Do not Advance"
-msgstr ""
-
-#: packages/notebook-extension/src/index.ts:1643
-msgid "Run Selected Cells and Insert Below"
-msgstr "選択したセルを実行して下に新規セルを挿入"
-
-#: packages/notebook-extension/src/index.ts:1656 packages/notebook-extension/src/index.ts:2239 packages/notebook-extension/src/index.ts:2730
-msgid "Run All Cells"
-msgstr "すべてのセルを実行"
-
-#: packages/notebook-extension/src/index.ts:1669 packages/notebook-extension/src/index.ts:2258
-msgid "Run All Above Selected Cell"
-msgstr "選択したセルの上にあるすべてを実行"
-
-#: packages/notebook-extension/src/index.ts:1689 packages/notebook-extension/src/index.ts:2283
-msgid "Run Selected Cell and All Below"
-msgstr "選択したセルと下のすべてのセルを実行"
-
-#: packages/notebook-extension/src/index.ts:1710 packages/notebook-extension/src/index.ts:2309
-msgid "Render All Markdown Cells"
-msgstr "すべてのMarkdownセルをレンダリングする"
-
-#: packages/notebook-extension/src/index.ts:1746 packages/notebook-extension/src/index.ts:2356
-msgid "Shut down the notebook?"
-msgstr "Notebookをシャットダウンしますか?"
-
-#: packages/notebook-extension/src/index.ts:1760 packages/notebook-extension/src/index.ts:2372
-msgid "Trust Notebook"
-msgstr "Notebookを信用する"
-
-#: packages/notebook-extension/src/index.ts:1771 packages/notebook-extension/src/index.ts:2684
-msgid "Restart Kernel and Clear All Outputs…"
-msgstr "カーネルを再起動してすべての出力を消去…"
-
-#: packages/notebook-extension/src/index.ts:1786 packages/notebook-extension/src/index.ts:2396
-msgid "Restart Kernel and Run up to Selected Cell…"
-msgstr "カーネルを再起動して選択したセルまで実行…"
-
-#: packages/notebook-extension/src/index.ts:1810 packages/notebook-extension/src/index.ts:2414 packages/notebook-extension/src/index.ts:2733
-msgid "Restart Kernel and Run All Cells…"
-msgstr "カーネルを再起動してすべてのセルを実行…"
-
-#: packages/notebook-extension/src/index.ts:1830 packages/notebook-extension/src/index.ts:2635
-msgid "Clear All Outputs"
-msgstr "すべての出力を消去"
-
-#: packages/notebook-extension/src/index.ts:1841
-msgid "Clear Outputs"
-msgstr "出力を消去"
-
-#: packages/notebook-extension/src/index.ts:1869 packages/notebook-extension/src/index.ts:2470
-msgid "Change to Code Cell Type"
-msgstr "コード形式のセルに変更"
-
-#: packages/notebook-extension/src/index.ts:1880 packages/notebook-extension/src/index.ts:2481
-msgid "Change to Markdown Cell Type"
-msgstr "Markdown形式のセルに変更"
-
-#: packages/notebook-extension/src/index.ts:1891 packages/notebook-extension/src/index.ts:2492
-msgid "Change to Raw Cell Type"
-msgstr "Raw形式のセルに変更"
-
-#: packages/notebook-extension/src/index.ts:1902
-msgid "Cut Cells"
-msgstr "セルを切り取り"
-
-#: packages/notebook-extension/src/index.ts:1903 packages/notebook/src/default-toolbar.tsx:140 packages/notebook/src/default-toolbar.tsx:141
-msgid "Cut the selected cells"
-msgstr "選択したセルを切り取り"
-
-#: packages/notebook-extension/src/index.ts:1915
-msgid "Copy Cells"
-msgstr "セルをコピー"
-
-#: packages/notebook-extension/src/index.ts:1916 packages/notebook/src/default-toolbar.tsx:160 packages/notebook/src/default-toolbar.tsx:161
-msgid "Copy the selected cells"
-msgstr "選択したセルをコピー"
-
-#: packages/notebook-extension/src/index.ts:1928
-msgid "Paste Cells Below"
-msgstr "下にセルを貼り付け"
-
-#: packages/notebook-extension/src/index.ts:1929 packages/notebook/src/default-toolbar.tsx:180 packages/notebook/src/default-toolbar.tsx:181
-msgid "Paste cells from the clipboard"
-msgstr "クリップボードからセルを貼り付け"
-
-#: packages/notebook-extension/src/index.ts:1941
-msgid "Paste Cells Above"
-msgstr "上にセルを貼り付け"
-
-#: packages/notebook-extension/src/index.ts:1952
-msgid "Duplicate Cells Below"
-msgstr "セルを複製"
-
-#: packages/notebook-extension/src/index.ts:1953
-msgid "Copy the selected cells and paste them below the selection"
-msgstr "選択したセルをコピーして、選択範囲の下に貼り付けます"
-
-#: packages/notebook-extension/src/index.ts:1967
-msgid "Paste Cells and Replace"
-msgstr "セルを貼り付けて置換"
-
-#: packages/notebook-extension/src/index.ts:1978
-msgid "Delete Cells"
-msgstr "セルを削除"
-
-#: packages/notebook-extension/src/index.ts:1989 packages/notebook-extension/src/index.ts:2682
-msgid "Split Cell"
-msgstr "セルの分割"
-
-#: packages/notebook-extension/src/index.ts:2000 packages/notebook-extension/src/index.ts:2693
-msgid "Merge Selected Cells"
-msgstr "選択したセルを結合"
-
-#: packages/notebook-extension/src/index.ts:2011 packages/notebook-extension/src/index.ts:2704
-msgid "Merge Cell Above"
-msgstr "上のセルと結合"
-
-#: packages/notebook-extension/src/index.ts:2022 packages/notebook-extension/src/index.ts:2715
-msgid "Merge Cell Below"
-msgstr "下のセルと結合"
-
-#: packages/notebook-extension/src/index.ts:2033 packages/notebook-extension/src/index.ts:2726
-msgid "Insert Cell Above"
-msgstr "上にセルを挿入"
-
-#: packages/notebook-extension/src/index.ts:2045 packages/notebook-extension/src/index.ts:2739
-msgid "Insert Cell Below"
-msgstr "下にセルを挿入"
-
-#: packages/notebook-extension/src/index.ts:2046 packages/notebook-extension/src/index.ts:2740 packages/notebook/src/default-toolbar.tsx:120 packages/notebook/src/default-toolbar.tsx:121
-msgid "Insert a cell below"
-msgstr "下にセルを挿入"
-
-#: packages/notebook-extension/src/index.ts:2058 packages/notebook-extension/src/index.ts:2752
-msgid "Select Cell Above"
-msgstr "上のセルを選択"
-
-#: packages/notebook-extension/src/index.ts:2069 packages/notebook-extension/src/index.ts:2763
-msgid "Select Cell Below"
-msgstr "下のセルを選択"
-
-#: packages/notebook-extension/src/index.ts:2080 packages/notebook-extension/src/index.ts:2821
-msgid "Extend Selection Above"
-msgstr "選択範囲を上に拡張"
-
-#: packages/notebook-extension/src/index.ts:2091 packages/notebook-extension/src/index.ts:2832
-msgid "Extend Selection to Top"
-msgstr "選択範囲を最上部まで拡張"
-
-#: packages/notebook-extension/src/index.ts:2102 packages/notebook-extension/src/index.ts:2843
-msgid "Extend Selection Below"
-msgstr "選択範囲を下に拡張"
-
-#: packages/notebook-extension/src/index.ts:2113 packages/notebook-extension/src/index.ts:2854
-msgid "Extend Selection to Bottom"
-msgstr "選択範囲を最下部まで拡張"
-
-#: packages/notebook-extension/src/index.ts:2124 packages/notebook-extension/src/index.ts:2865
-msgid "Select All Cells"
-msgstr "すべてのセルを選択"
-
-#: packages/notebook-extension/src/index.ts:2135 packages/notebook-extension/src/index.ts:2876
-msgid "Deselect All Cells"
-msgstr "すべてのセルの選択を解除"
-
-#: packages/notebook-extension/src/index.ts:2146
-msgid "Move Cells Up"
-msgstr "セルを上に移動"
-
-#: packages/notebook-extension/src/index.ts:2158
-msgid "Move Cells Down"
-msgstr "セルを下に移動"
-
 #: packages/notebook-extension/src/index.ts:2158
 msgid "Run Selected Cell"
 msgid_plural "Run Selected Cells"
 msgstr[0] ""
 
 #: packages/notebook-extension/src/index.ts:2166
 msgid "Run this cell and advance"
 msgid_plural "Run these %1 cells and advance"
 msgstr[0] ""
 
-#: packages/notebook-extension/src/index.ts:2170
-msgid "Toggle All Line Numbers"
-msgstr "すべての行番号表示を切り替える"
-
-#: packages/notebook-extension/src/index.ts:2181 packages/notebook-extension/src/index.ts:2987
-msgid "Enter Command Mode"
-msgstr "コマンドモードに入る"
-
 #: packages/notebook-extension/src/index.ts:2191
 msgid "Run Selected Cell and Do not Advance"
 msgid_plural "Run Selected Cells and Do not Advance"
 msgstr[0] ""
 
-#: packages/notebook-extension/src/index.ts:2192 packages/notebook-extension/src/index.ts:2998
-msgid "Enter Edit Mode"
-msgstr "エディットモードに入る"
-
-#: packages/notebook-extension/src/index.ts:2203 packages/notebook-extension/src/index.ts:3009
-msgid "Undo Cell Operation"
-msgstr "セル操作を元に戻す"
-
-#: packages/notebook-extension/src/index.ts:2214 packages/notebook-extension/src/index.ts:3020
-msgid "Redo Cell Operation"
-msgstr "セル操作をやり直す"
-
 #: packages/notebook-extension/src/index.ts:2216
 msgid "Run Selected Cell and Insert Below"
 msgid_plural "Run Selected Cells and Insert Below"
 msgstr[0] ""
 
 #: packages/notebook-extension/src/index.ts:2239
-msgid "Reconnect To Kernel"
-msgstr "カーネルに再接続"
+msgid "Run All Cells"
+msgstr "すべてのセルを実行"
 
 #: packages/notebook-extension/src/index.ts:2240
 msgid "Run all cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2256 packages/notebook-extension/src/index.ts:3098
-msgid "Change to Heading 1"
-msgstr "見出し1に変更"
-
-#: packages/notebook-extension/src/index.ts:2267 packages/notebook-extension/src/index.ts:3109
-msgid "Change to Heading 2"
-msgstr "見出し2に変更"
-
-#: packages/notebook-extension/src/index.ts:2278 packages/notebook-extension/src/index.ts:3120
-msgid "Change to Heading 3"
-msgstr "見出し3に変更"
-
-#: packages/notebook-extension/src/index.ts:2289 packages/notebook-extension/src/index.ts:3131
-msgid "Change to Heading 4"
-msgstr "見出し4に変更"
-
-#: packages/notebook-extension/src/index.ts:2300 packages/notebook-extension/src/index.ts:3142
-msgid "Change to Heading 5"
-msgstr "見出し5に変更"
-
-#: packages/notebook-extension/src/index.ts:2311 packages/notebook-extension/src/index.ts:3153
-msgid "Change to Heading 6"
-msgstr "見出し6に変更"
-
-#: packages/notebook-extension/src/index.ts:2322 packages/notebook-extension/src/index.ts:3164
-msgid "Collapse Selected Code"
-msgstr "選択したコードを折りたたむ"
+#: packages/notebook-extension/src/index.ts:2258
+msgid "Run All Above Selected Cell"
+msgstr "選択したセルの上にあるすべてを実行"
 
-#: packages/notebook-extension/src/index.ts:2333 packages/notebook-extension/src/index.ts:3175
-msgid "Expand Selected Code"
-msgstr "選択したコードを展開"
+#: packages/notebook-extension/src/index.ts:2283
+msgid "Run Selected Cell and All Below"
+msgstr "選択したセルと下のすべてのセルを実行"
 
-#: packages/notebook-extension/src/index.ts:2344 packages/notebook-extension/src/index.ts:3186
-msgid "Collapse All Code"
-msgstr "すべてのコードを折りたたむ"
+#: packages/notebook-extension/src/index.ts:2309
+msgid "Render All Markdown Cells"
+msgstr "すべてのMarkdownセルをレンダリングする"
 
 #: packages/notebook-extension/src/index.ts:2345
 msgid "Close and Shut Down Notebook"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2355 packages/notebook-extension/src/index.ts:3197
-msgid "Expand All Code"
-msgstr "すべてのコードを展開"
-
-#: packages/notebook-extension/src/index.ts:2366 packages/notebook-extension/src/index.ts:3208
-msgid "Collapse Selected Outputs"
-msgstr "選択した出力を折りたたむ"
+#: packages/notebook-extension/src/index.ts:2356
+msgid "Shut down the notebook?"
+msgstr "Notebookをシャットダウンしますか?"
 
-#: packages/notebook-extension/src/index.ts:2377 packages/notebook-extension/src/index.ts:3219
-msgid "Expand Selected Outputs"
-msgstr "選択した出力を展開"
+#: packages/notebook-extension/src/index.ts:2372
+msgid "Trust Notebook"
+msgstr "Notebookを信用する"
 
 #: packages/notebook-extension/src/index.ts:2383
 msgid "Restart Kernel and Clear Outputs of All Cells…"
 msgstr ""
 
 #: packages/notebook-extension/src/index.ts:2384
 msgid "Restart the kernel and clear all outputs of all cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2388 packages/notebook-extension/src/index.ts:3230
-msgid "Collapse All Outputs"
-msgstr "すべての出力を折りたたむ"
+#: packages/notebook-extension/src/index.ts:2396
+msgid "Restart Kernel and Run up to Selected Cell…"
+msgstr "カーネルを再起動して選択したセルまで実行…"
 
-#: packages/notebook-extension/src/index.ts:2400 packages/notebook-extension/src/index.ts:3242
-msgid "Render Side-by-Side"
-msgstr ""
+#: packages/notebook-extension/src/index.ts:2414
+msgid "Restart Kernel and Run All Cells…"
+msgstr "カーネルを再起動してすべてのセルを実行…"
 
 #: packages/notebook-extension/src/index.ts:2415
 msgid "Restart the kernel and run all cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2422 packages/notebook-extension/src/index.ts:3264
-msgid "Expand All Outputs"
-msgstr "すべての出力を展開"
-
 #: packages/notebook-extension/src/index.ts:2428
 msgid "Clear Outputs of All Cells"
 msgstr ""
 
 #: packages/notebook-extension/src/index.ts:2429
 msgid "Clear all outputs of all cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2433 packages/notebook-extension/src/index.ts:3275
-msgid "Enable Scrolling for Outputs"
-msgstr "出力のスクロールを有効にする"
-
 #: packages/notebook-extension/src/index.ts:2440
 msgid "Clear Cell Output"
 msgstr ""
 
 #: packages/notebook-extension/src/index.ts:2441
 msgid "Clear outputs for the selected cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2444 packages/notebook-extension/src/index.ts:3286
-msgid "Disable Scrolling for Outputs"
-msgstr "出力のスクロールを無効にする"
+#: packages/notebook-extension/src/index.ts:2470
+msgid "Change to Code Cell Type"
+msgstr "コード形式のセルに変更"
 
-#: packages/notebook-extension/src/index.ts:2455 packages/notebook-extension/src/index.ts:3297
-msgid "Select current running or last run cell"
-msgstr "現在実行中または最後の実行セルを選択"
+#: packages/notebook-extension/src/index.ts:2481
+msgid "Change to Markdown Cell Type"
+msgstr "Markdown形式のセルに変更"
 
-#: packages/notebook-extension/src/index.ts:2466 packages/notebook-extension/src/index.ts:3308
-msgid "Replace Selection in Notebook Cell"
-msgstr "ノートブックセルの選択範囲を置換する"
+#: packages/notebook-extension/src/index.ts:2492
+msgid "Change to Raw Cell Type"
+msgstr "Raw形式のセルに変更"
 
 #: packages/notebook-extension/src/index.ts:2505
 msgid "Cut Cell"
 msgid_plural "Cut Cells"
 msgstr[0] ""
 
 #: packages/notebook-extension/src/index.ts:2513
 msgid "Cut this cell"
 msgid_plural "Cut these %1 cells"
 msgstr[0] ""
 
-#: packages/notebook-extension/src/index.ts:2514 packages/notebook-extension/src/index.ts:3399 packages/notebook-extension/src/index.ts:572 packages/notebook-extension/src/index.ts:657
-msgid "Notebook Operations"
-msgstr "Notebookの操作"
-
 #: packages/notebook-extension/src/index.ts:2532
 msgid "Copy Cell"
 msgid_plural "Copy Cells"
 msgstr[0] ""
 
 #: packages/notebook-extension/src/index.ts:2540
 msgid "Copy this cell"
 msgid_plural "Copy these %1 cells"
 msgstr[0] ""
 
-#: packages/notebook-extension/src/index.ts:2550 packages/notebook-extension/src/index.ts:3435
-msgid "Notebook Cell Operations"
-msgstr "Notebookセルの操作"
-
 #: packages/notebook-extension/src/index.ts:2559
 msgid "Paste Cell Below"
 msgid_plural "Paste Cells Below"
 msgstr[0] ""
 
 #: packages/notebook-extension/src/index.ts:2567 packages/notebook-extension/src/index.ts:2594
 msgid "Paste this cell from the clipboard"
@@ -6724,56 +5879,68 @@
 msgstr[0] ""
 
 #: packages/notebook-extension/src/index.ts:2620
 msgid "Create a duplicate of this cell below"
 msgid_plural "Create duplicates of %1 cells below"
 msgstr[0] ""
 
-#: packages/notebook-extension/src/index.ts:2633
-msgid "Clear Output"
-msgstr "出力を消去"
-
 #: packages/notebook-extension/src/index.ts:2639
 msgid "Paste Cell and Replace"
 msgid_plural "Paste Cells and Replace"
 msgstr[0] ""
 
-#: packages/notebook-extension/src/index.ts:2649
-msgid "Close and Shutdown Notebook"
-msgstr "Notebookを閉じてシャットダウンする"
-
-#: packages/notebook-extension/src/index.ts:2653
-msgid "Shut down the Notebook?"
-msgstr "Notebookをシャットダウンしますか?"
-
 #: packages/notebook-extension/src/index.ts:2657
 msgid "Delete Cell"
 msgid_plural "Delete Cells"
 msgstr[0] ""
 
 #: packages/notebook-extension/src/index.ts:2665
 msgid "Delete this cell"
 msgid_plural "Delete these %1 cells"
 msgstr[0] ""
 
+#: packages/notebook-extension/src/index.ts:2682
+msgid "Split Cell"
+msgstr "セルの分割"
+
+#: packages/notebook-extension/src/index.ts:2693
+msgid "Merge Selected Cells"
+msgstr "選択したセルを結合"
+
+#: packages/notebook-extension/src/index.ts:2704
+msgid "Merge Cell Above"
+msgstr "上のセルと結合"
+
+#: packages/notebook-extension/src/index.ts:2715
+msgid "Merge Cell Below"
+msgstr "下のセルと結合"
+
+#: packages/notebook-extension/src/index.ts:2726
+msgid "Insert Cell Above"
+msgstr "上にセルを挿入"
+
 #: packages/notebook-extension/src/index.ts:2727
 msgid "Insert a cell above"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2729 packages/notebook/src/default-toolbar.tsx:200 packages/notebook/src/default-toolbar.tsx:207
-msgid "Run the selected cells and advance"
-msgstr "選択したセルを実行して次のセルに進めます"
+#: packages/notebook-extension/src/index.ts:2739
+msgid "Insert Cell Below"
+msgstr "下にセルを挿入"
 
-#: packages/notebook-extension/src/index.ts:2731
-msgid "Run the all notebook cells"
-msgstr ""
+#: packages/notebook-extension/src/index.ts:2740 packages/notebook/src/default-toolbar.tsx:121
+msgid "Insert a cell below"
+msgstr "下にセルを挿入"
 
-#: packages/notebook-extension/src/index.ts:2735 packages/notebook/src/default-toolbar.tsx:227 packages/notebook/src/default-toolbar.tsx:238
-msgid "Restart the kernel, then re-run the whole notebook"
-msgstr "カーネルを再起動し、notebook全体を再実行"
+#: packages/notebook-extension/src/index.ts:2752
+msgid "Select Cell Above"
+msgstr "上のセルを選択"
+
+#: packages/notebook-extension/src/index.ts:2763
+msgid "Select Cell Below"
+msgstr "下のセルを選択"
 
 #: packages/notebook-extension/src/index.ts:2773
 msgid "Insert Heading Above Current Heading"
 msgstr ""
 
 #: packages/notebook-extension/src/index.ts:2784
 msgid "Insert Heading Below Current Heading"
@@ -6783,43 +5950,43 @@
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
+msgstr "選択範囲を上に拡張"
 
-#: packages/notebook-extension/src/index.ts:2871 packages/notebook-extension/src/index.ts:3681
-msgid "ReStructured Text"
-msgstr ""
+#: packages/notebook-extension/src/index.ts:2832
+msgid "Extend Selection to Top"
+msgstr "選択範囲を最上部まで拡張"
 
-#: packages/notebook-extension/src/index.ts:2872 packages/notebook-extension/src/index.ts:3682
-msgid "Executable Script"
-msgstr "実行可能なスクリプト"
+#: packages/notebook-extension/src/index.ts:2843
+msgid "Extend Selection Below"
+msgstr "選択範囲を下に拡張"
 
-#: packages/notebook-extension/src/index.ts:2873 packages/notebook-extension/src/index.ts:3683
-msgid "Reveal.js Slides"
-msgstr "Reveal.js スライド"
+#: packages/notebook-extension/src/index.ts:2854
+msgid "Extend Selection to Bottom"
+msgstr "選択範囲を最下部まで拡張"
+
+#: packages/notebook-extension/src/index.ts:2865
+msgid "Select All Cells"
+msgstr "すべてのセルを選択"
+
+#: packages/notebook-extension/src/index.ts:2876
+msgid "Deselect All Cells"
+msgstr "すべてのセルの選択を解除"
 
 #: packages/notebook-extension/src/index.ts:2889
 msgid "Move Cell Up"
 msgid_plural "Move Cells Up"
 msgstr[0] ""
 
-#: packages/notebook-extension/src/index.ts:2891 packages/notebook-extension/src/index.ts:3737
-msgid "For Notebook: %1"
-msgstr "Notebook: %1"
-
-#: packages/notebook-extension/src/index.ts:2892 packages/notebook-extension/src/index.ts:3738
-msgid "For Notebook:"
-msgstr "Notebook:"
-
 #: packages/notebook-extension/src/index.ts:2897
 msgid "Move this cell up"
 msgid_plural "Move these %1 cells up"
 msgstr[0] ""
 
 #: packages/notebook-extension/src/index.ts:2909
 msgid "Notebook cell shifted up successfully"
@@ -6835,14 +6002,106 @@
 msgid_plural "Move these %1 cells down"
 msgstr[0] ""
 
 #: packages/notebook-extension/src/index.ts:2946
 msgid "Notebook cell shifted down successfully"
 msgstr ""
 
+#: packages/notebook-extension/src/index.ts:2987
+msgid "Enter Command Mode"
+msgstr "コマンドモードに入る"
+
+#: packages/notebook-extension/src/index.ts:2998
+msgid "Enter Edit Mode"
+msgstr "エディットモードに入る"
+
+#: packages/notebook-extension/src/index.ts:3009
+msgid "Undo Cell Operation"
+msgstr "セル操作を元に戻す"
+
+#: packages/notebook-extension/src/index.ts:3020
+msgid "Redo Cell Operation"
+msgstr "セル操作をやり直す"
+
+#: packages/notebook-extension/src/index.ts:3098
+msgid "Change to Heading 1"
+msgstr "見出し1に変更"
+
+#: packages/notebook-extension/src/index.ts:3109
+msgid "Change to Heading 2"
+msgstr "見出し2に変更"
+
+#: packages/notebook-extension/src/index.ts:3120
+msgid "Change to Heading 3"
+msgstr "見出し3に変更"
+
+#: packages/notebook-extension/src/index.ts:3131
+msgid "Change to Heading 4"
+msgstr "見出し4に変更"
+
+#: packages/notebook-extension/src/index.ts:3142
+msgid "Change to Heading 5"
+msgstr "見出し5に変更"
+
+#: packages/notebook-extension/src/index.ts:3153
+msgid "Change to Heading 6"
+msgstr "見出し6に変更"
+
+#: packages/notebook-extension/src/index.ts:3164
+msgid "Collapse Selected Code"
+msgstr "選択したコードを折りたたむ"
+
+#: packages/notebook-extension/src/index.ts:3175
+msgid "Expand Selected Code"
+msgstr "選択したコードを展開"
+
+#: packages/notebook-extension/src/index.ts:3186
+msgid "Collapse All Code"
+msgstr "すべてのコードを折りたたむ"
+
+#: packages/notebook-extension/src/index.ts:3197
+msgid "Expand All Code"
+msgstr "すべてのコードを展開"
+
+#: packages/notebook-extension/src/index.ts:3208
+msgid "Collapse Selected Outputs"
+msgstr "選択した出力を折りたたむ"
+
+#: packages/notebook-extension/src/index.ts:3219
+msgid "Expand Selected Outputs"
+msgstr "選択した出力を展開"
+
+#: packages/notebook-extension/src/index.ts:3230
+msgid "Collapse All Outputs"
+msgstr "すべての出力を折りたたむ"
+
+#: packages/notebook-extension/src/index.ts:3242
+msgid "Render Side-by-Side"
+msgstr ""
+
+#: packages/notebook-extension/src/index.ts:3264
+msgid "Expand All Outputs"
+msgstr "すべての出力を展開"
+
+#: packages/notebook-extension/src/index.ts:3275
+msgid "Enable Scrolling for Outputs"
+msgstr "出力のスクロールを有効にする"
+
+#: packages/notebook-extension/src/index.ts:3286
+msgid "Disable Scrolling for Outputs"
+msgstr "出力のスクロールを無効にする"
+
+#: packages/notebook-extension/src/index.ts:3297
+msgid "Select current running or last run cell"
+msgstr "現在実行中または最後の実行セルを選択"
+
+#: packages/notebook-extension/src/index.ts:3308
+msgid "Replace Selection in Notebook Cell"
+msgstr "ノートブックセルの選択範囲を置換する"
+
 #: packages/notebook-extension/src/index.ts:3320
 msgid "Toggle Collapse Notebook Heading"
 msgstr ""
 
 #: packages/notebook-extension/src/index.ts:3330 packages/toc-extension/src/index.ts:141
 msgid "Collapse All Headings"
 msgstr ""
@@ -6851,261 +6110,240 @@
 msgid "Expand All Headings"
 msgstr ""
 
 #: packages/notebook-extension/src/index.ts:3349
 msgid "Select and Run Cell(s) for this Heading"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:504 packages/notebook-extension/src/index.ts:573
-msgid "Save and Export Notebook: %1"
+#: packages/notebook-extension/src/index.ts:3399 packages/notebook-extension/src/index.ts:657
+msgid "Notebook Operations"
+msgstr "Notebookの操作"
+
+#: packages/notebook-extension/src/index.ts:3435
+msgid "Notebook Cell Operations"
+msgstr "Notebookセルの操作"
+
+#: packages/notebook-extension/src/index.ts:3680
+msgid "PDF"
+msgstr ""
+
+#: packages/notebook-extension/src/index.ts:3681
+msgid "ReStructured Text"
 msgstr ""
 
+#: packages/notebook-extension/src/index.ts:3682
+msgid "Executable Script"
+msgstr "実行可能なスクリプト"
+
+#: packages/notebook-extension/src/index.ts:3683
+msgid "Reveal.js Slides"
+msgstr "Reveal.js スライド"
+
+#: packages/notebook-extension/src/index.ts:3737
+msgid "For Notebook: %1"
+msgstr "Notebook: %1"
+
+#: packages/notebook-extension/src/index.ts:3738
+msgid "For Notebook:"
+msgstr "Notebook:"
+
 #: packages/notebook-extension/src/index.ts:569
 msgid "Save and Export Notebook to the given `format`."
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:758
-msgid "Slides"
-msgstr "スライド"
-
-#: packages/notebook-extension/src/index.ts:759
-msgid "Script"
-msgstr "スクリプト"
-
-#: packages/notebook-extension/src/index.ts:761
-msgid "Custom"
-msgstr "カスタム"
-
-#: packages/notebook-extension/src/index.ts:943
-msgid "Create New View for Output"
-msgstr "出力用に新しいビューを作成"
+#: packages/notebook-extension/src/index.ts:573
+msgid "Save and Export Notebook: %1"
+msgstr ""
 
-#: packages/notebook/src/actions.tsx:1881 packages/notebook/src/actions.tsx:2026
+#: packages/notebook/src/actions.tsx:2032
 msgid "A trusted Jupyter notebook may execute hidden malicious code when you open it."
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:1885
-msgid "Selecting trust will re-render this notebook in a trusted state."
-msgstr "\"信頼\"を選択すると、このノートブックは信頼された状態で再レンダリングされます。"
+#: packages/notebook/src/actions.tsx:2036
+msgid "Selecting \"Trust\" will re-render this notebook in a trusted state."
+msgstr ""
 
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
 msgstr "Notebookは既に信頼されています"
 
-#: packages/notebook/src/actions.tsx:1909 packages/notebook/src/actions.tsx:2055
+#: packages/notebook/src/actions.tsx:2061
 msgid "Trust this notebook?"
 msgstr "このnotebookを信頼しますか？"
 
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
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2150 packages/notebook/src/actions.tsx:2273
+#: packages/notebook/src/actions.tsx:2279
 msgid "Kernel Terminating"
 msgstr "カーネル終了中"
 
-#: packages/notebook/src/actions.tsx:2151 packages/notebook/src/actions.tsx:2274
+#: packages/notebook/src/actions.tsx:2280
 msgid "The kernel for %1 appears to be terminating. You can not run any cell for now."
 msgstr "%1 のカーネルが終了しているようです。現在どのセルも実行できません。"
 
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
+msgstr "選択したセルを切り取り"
+
+#: packages/notebook/src/default-toolbar.tsx:161
+msgid "Copy the selected cells"
+msgstr "選択したセルをコピー"
+
+#: packages/notebook/src/default-toolbar.tsx:181
+msgid "Paste cells from the clipboard"
+msgstr "クリップボードからセルを貼り付け"
+
+#: packages/notebook/src/default-toolbar.tsx:207
+msgid "Run the selected cells and advance"
+msgstr "選択したセルを実行して次のセルに進めます"
+
+#: packages/notebook/src/default-toolbar.tsx:238
+msgid "Restart the kernel, then re-run the whole notebook"
+msgstr "カーネルを再起動し、notebook全体を再実行"
+
+#: packages/notebook/src/default-toolbar.tsx:374
 msgid "Cell type"
 msgstr "セルの種類"
 
-#: packages/notebook/src/default-toolbar.tsx:356 packages/notebook/src/default-toolbar.tsx:375
+#: packages/notebook/src/default-toolbar.tsx:375
 msgid "Select the cell type"
 msgstr ""
 
-#: packages/notebook/src/default-toolbar.tsx:359 packages/notebook/src/default-toolbar.tsx:378
+#: packages/notebook/src/default-toolbar.tsx:378
 msgid "Code"
 msgstr "コード"
 
-#: packages/notebook/src/default-toolbar.tsx:361 packages/notebook/src/default-toolbar.tsx:380
+#: packages/notebook/src/default-toolbar.tsx:380
 msgid "Raw"
 msgstr ""
 
-#: packages/notebook/src/default-toolbar.tsx:86 packages/notebook/src/default-toolbar.tsx:87
+#: packages/notebook/src/default-toolbar.tsx:87
 msgid "Save the notebook contents and create checkpoint"
 msgstr "Notebookの内容を保存してチェックポイントを作成"
 
-#: packages/notebook/src/executionindicator.tsx:127 packages/notebook/src/executionindicator.tsx:129 packages/notebook/src/executionindicator.tsx:145 packages/notebook/src/executionindicator.tsx:147
+#: packages/notebook/src/executionindicator.tsx:129 packages/notebook/src/executionindicator.tsx:147
 msgid "Elapsed time: %1 second"
 msgid_plural "Elapsed time: %1 seconds"
 msgstr[0] ""
 
-#: packages/notebook/src/executionindicator.tsx:138 packages/notebook/src/executionindicator.tsx:140
+#: packages/notebook/src/executionindicator.tsx:140
 msgid "Executed %1 cell"
 msgid_plural "Executed %1 cells"
 msgstr[0] ""
 
 #: packages/notebook/src/executionindicator.tsx:71
 msgid "Kernel status"
 msgstr ""
 
-#: packages/notebook/src/executionindicator.tsx:73 packages/notebook/src/executionindicator.tsx:75
+#: packages/notebook/src/executionindicator.tsx:75
 msgid "Kernel status: %1"
 msgstr ""
 
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
 msgstr "Notebookは新しいnotebookフォーマット(v%1) から現在のnotebookフォーマット(v%2) へ変換されました。\n"
 "このnotebookを次回保存する際は、現在のnotebookフォーマット(v%2) が使用されます。\n"
 "以前のnotebookの機能が使えなくなる可能性があります。以前のnotebookの状態を保存したい場合は、notebookを保存せずに閉じてください。"
 
-#: packages/notebook/src/model.ts:371 packages/notebook/src/model.ts:375
+#: packages/notebook/src/model.ts:375
 msgid "Notebook converted"
 msgstr "Notebookは変換されました"
 
-#: packages/notebook/src/modestatus.tsx:24 packages/notebook/src/modestatus.tsx:29
+#: packages/notebook/src/modestatus.tsx:29
 msgid "Mode: %1"
 msgstr "モード: %1"
 
-#: packages/notebook/src/modestatus.tsx:66 packages/notebook/src/modestatus.tsx:71 packages/shortcuts-extension/src/components/TopNav.tsx:181 packages/shortcuts-extension/src/components/TopNav.tsx:273
+#: packages/notebook/src/modestatus.tsx:71 packages/shortcuts-extension/src/components/TopNav.tsx:181
 msgid "Command"
 msgstr "コマンド"
 
-#: packages/notebook/src/modestatus.tsx:67 packages/notebook/src/modestatus.tsx:72 packages/shortcuts-extension/src/components/ShortcutItem.tsx:61 packages/shortcuts-extension/src/components/ShortcutItem.tsx:80
+#: packages/notebook/src/modestatus.tsx:72 packages/shortcuts-extension/src/components/ShortcutItem.tsx:61
 msgid "Edit"
 msgstr "編集"
 
-#: packages/notebook/src/modestatus.tsx:78 packages/notebook/src/modestatus.tsx:83
+#: packages/notebook/src/modestatus.tsx:83
 msgid "Notebook is in %1 mode"
 msgstr "Notebookは %1 モードです"
 
 #: packages/notebook/src/notebookfooter.ts:24
 msgid "Click to add a cell."
 msgstr ""
 
-#: packages/notebook/src/notebooktools.ts:614
-msgid "Notebook Metadata"
-msgstr "Notebookのメタデータ"
-
-#: packages/notebook/src/notebooktools.ts:650
-msgid "Cell Metadata"
-msgstr "セルのメタデータ"
-
-#: packages/notebook/src/notebooktools.ts:78
-msgid "Advanced Tools"
-msgstr "高度なツール"
-
-#: packages/notebook/src/notebooktools.ts:918
-msgid "Slide Type"
-msgstr "スライドの種類"
-
-#: packages/notebook/src/notebooktools.ts:921
-msgid "Slide"
-msgstr "スライド"
-
-#: packages/notebook/src/notebooktools.ts:922
-msgid "Sub-Slide"
-msgstr "サブスライド"
-
-#: packages/notebook/src/notebooktools.ts:923
-msgid "Fragment"
-msgstr "フラグメント"
-
-#: packages/notebook/src/notebooktools.ts:924
-msgid "Skip"
-msgstr "スキップ"
-
-#: packages/notebook/src/notebooktools.ts:925
-msgid "Notes"
-msgstr "ノート"
-
-#: packages/notebook/src/notebooktools.ts:963
-msgid "Raw NBConvert Format"
-msgstr "Raw NBConvert フォーマット"
-
-#: packages/notebook/src/panel.ts:208 packages/notebook/src/panel.ts:214
+#: packages/notebook/src/panel.ts:229
 msgid "Kernel Restarting"
 msgstr "カーネル再起動中"
 
-#: packages/notebook/src/panel.ts:209 packages/notebook/src/panel.ts:215
+#: packages/notebook/src/panel.ts:230
 msgid "The kernel for %1 appears to have died. It will restart automatically."
 msgstr "%1 のカーネルが予期せず終了しました。自動的に再起動します。"
 
-#: packages/notebook/src/searchprovider.ts:223
+#: packages/notebook/src/searchprovider.ts:226
+msgid "Search Cell Outputs"
+msgstr ""
+
+#: packages/notebook/src/searchprovider.ts:227
 msgid "Search in the cell outputs."
 msgstr ""
 
-#: packages/notebook/src/searchprovider.ts:230
+#: packages/notebook/src/searchprovider.ts:234
 msgid "Search in %1 Selected Cell"
 msgid_plural "Search in %1 Selected Cells"
 msgstr[0] ""
 
-#: packages/notebook/src/searchprovider.ts:235
+#: packages/notebook/src/searchprovider.ts:239
 msgid "Search in %1 Selected Line"
 msgid_plural "Search in %1 Selected Lines"
 msgstr[0] ""
 
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
-msgstr "Notebookは信頼されています: %2 のセルの内 %1 のセルが信頼されています。"
-
-#: packages/notebook/src/truststatus.tsx:30
-msgid "Active cell trusted: %1 of %2 cells trusted."
-msgstr "アクティブなセルは信頼されています: %2 のセルの内 %1 のセルが信頼されています。"
-
 #: packages/notebook/src/truststatus.tsx:30
 msgid "Notebook trusted: %1 of %2 code cells trusted."
 msgstr ""
 
 #: packages/notebook/src/truststatus.tsx:36
 msgid "Active cell trusted: %1 of %2 code cells trusted."
 msgstr ""
 
-#: packages/notebook/src/truststatus.tsx:39
-msgid "Notebook not trusted: %1 of %2 cells trusted."
-msgstr "Notebookは信頼されていません: %2 のセルの内 %1 のセルが信頼されています。"
-
 #: packages/notebook/src/truststatus.tsx:42
 msgid "Notebook not trusted: %1 of %2 code cells trusted."
 msgstr ""
 
 #: packages/notebook/src/widget.ts:439
 msgid "The notebook is empty. Click the + button on the toolbar to add a new cell."
 msgstr ""
@@ -7118,35 +6356,35 @@
 msgid "Toggle output scrolling"
 msgstr ""
 
 #: packages/outputarea/src/widget.ts:605
 msgid "Javascript Error: %1"
 msgstr ""
 
-#: packages/property-inspector/src/index.ts:170 packages/property-inspector/src/index.ts:189
+#: packages/property-inspector/src/index.ts:189
 msgid "No properties to inspect."
 msgstr "チェックするプロパティがありません。"
 
-#: packages/rendermime-extension/src/index.ts:58 packages/rendermime-extension/src/index.ts:67
+#: packages/rendermime-extension/src/index.ts:67
 msgid "Handle Local Link"
 msgstr "ローカルリンクの処理"
 
-#: packages/rendermime/src/renderers.ts:62 packages/rendermime/src/renderers.ts:66
+#: packages/rendermime/src/renderers.ts:62
 msgid "This HTML output contains inline scripts. Are you sure that you want to run arbitrary Javascript within your JupyterLab session?"
 msgstr "このHTML出力にはインラインスクリプトが含まれています。JupyterLabセッション内で任意のJavaScriptを実行してもよろしいですか?"
 
-#: packages/rendermime/src/widgets.ts:420 packages/rendermime/src/widgets.ts:428
+#: packages/rendermime/src/widgets.ts:428
 msgid "JavaScript output is disabled in JupyterLab"
 msgstr "JupyterLabではJavaScriptの出力が無効になっています"
 
-#: packages/running-extension/src/index.ts:54 packages/running-extension/src/index.ts:66
+#: packages/running-extension/src/index.ts:66
 msgid "Running Terminals and Kernels"
 msgstr "ターミナルとカーネルの実行"
 
-#: packages/running-extension/src/index.ts:57 packages/running-extension/src/index.ts:69
+#: packages/running-extension/src/index.ts:69
 msgid "Running Sessions section"
 msgstr ""
 
 #: packages/running-extension/src/index.ts:86
 msgid "Sessions and Tabs"
 msgstr ""
 
@@ -7155,116 +6393,86 @@
 msgstr ""
 
 #: packages/running-extension/src/kernels.ts:250
 msgid "%1\n"
 "Path: %2"
 msgstr ""
 
-#: packages/running-extension/src/kernels.ts:30 packages/running-extension/src/kernels.ts:49
+#: packages/running-extension/src/kernels.ts:49
 msgid "Kernels"
 msgstr "カーネル"
 
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
-msgstr "パス: %1\n"
-"カーネル: %2"
-
 #: packages/running-extension/src/kernels.ts:88
 msgid "New Notebook for Kernel"
 msgstr ""
 
-#: packages/running-extension/src/opentabs.ts:70 packages/running-extension/src/opentabs.ts:71
+#: packages/running-extension/src/opentabs.ts:70
 msgid "Open Tabs"
 msgstr "タブを開く"
 
-#: packages/running-extension/src/opentabs.ts:87 packages/running-extension/src/opentabs.ts:88
+#: packages/running-extension/src/opentabs.ts:87
 msgid "Close All"
 msgstr "全て閉じる"
 
-#: packages/running-extension/src/opentabs.ts:88 packages/running-extension/src/opentabs.ts:89
+#: packages/running-extension/src/opentabs.ts:88
 msgid "Are you sure you want to close all open tabs?"
 msgstr ""
 
-#: packages/running/src/index.tsx:288 packages/running/src/index.tsx:443
+#: packages/running/src/index.tsx:443
 msgid "Refresh List"
 msgstr "リストを更新"
 
-#: packages/settingeditor-extension/src/index.ts:141 packages/settingeditor-extension/src/index.ts:145
+#: packages/settingeditor-extension/src/index.ts:145
 msgid "JSON Settings Editor"
 msgstr "JSON設定エディタ"
 
-#: packages/settingeditor-extension/src/index.ts:148 packages/settingeditor-extension/src/index.ts:152 packages/settingeditor-extension/src/index.ts:183 packages/settingeditor-extension/src/index.ts:187 packages/settingeditor-extension/src/index.ts:312 packages/settingeditor-extension/src/index.ts:319 packages/settingeditor/src/jsonsettingeditor.tsx:67 packages/settingeditor/src/pluginlist.tsx:455 packages/settingeditor/src/pluginlist.tsx:467
+#: packages/settingeditor-extension/src/index.ts:152 packages/settingeditor-extension/src/index.ts:187 packages/settingeditor-extension/src/index.ts:319 packages/settingeditor/src/pluginlist.tsx:467
 msgid "Settings"
 msgstr "設定"
 
-#: packages/settingeditor-extension/src/index.ts:177 packages/settingeditor-extension/src/index.ts:302 packages/settingeditor-extension/src/index.ts:309 packages/settingeditor-extension/src/index.ts:315
-msgid "Advanced Settings Editor"
-msgstr "詳細設定エディタ"
-
 #: packages/settingeditor-extension/src/index.ts:181
 msgid "Settings Editor"
 msgstr ""
 
-#: packages/settingeditor-extension/src/index.ts:308
-msgid "Advanced JSON Settings Editor"
-msgstr "JSON詳細設定エディタ"
+#: packages/settingeditor-extension/src/index.ts:309 packages/settingeditor-extension/src/index.ts:315
+msgid "Advanced Settings Editor"
+msgstr "詳細設定エディタ"
 
-#: packages/settingeditor-extension/src/index.ts:322 packages/settingeditor-extension/src/index.ts:329
+#: packages/settingeditor-extension/src/index.ts:329
 msgid "Revert User Settings"
 msgstr "ユーザー設定を元に戻す"
 
-#: packages/settingeditor-extension/src/index.ts:329 packages/settingeditor-extension/src/index.ts:336
+#: packages/settingeditor-extension/src/index.ts:336
 msgid "Save User Settings"
 msgstr "ユーザー設定を保存"
 
 #: packages/settingeditor/src/InstructionsPlaceholder.tsx:21
 msgid "No Plugin Selected"
 msgstr ""
 
-#: packages/settingeditor/src/InstructionsPlaceholder.tsx:23 packages/settingeditor/src/jsonsettingeditor.tsx:71
+#: packages/settingeditor/src/InstructionsPlaceholder.tsx:23
 msgid "Select a plugin from the list to view and edit its preferences."
 msgstr "リストからプラグインを選択して、その設定を表示および編集します。"
 
-#: packages/settingeditor/src/SettingsFormEditor.tsx:158
-msgid "Move Up"
-msgstr "上に移動"
-
-#: packages/settingeditor/src/SettingsFormEditor.tsx:165
-msgid "Move Down"
-msgstr "下に移動"
-
-#: packages/settingeditor/src/SettingsFormEditor.tsx:166 packages/settingeditor/src/SettingsFormEditor.tsx:441
+#: packages/settingeditor/src/SettingsFormEditor.tsx:172
 msgid "Error saving settings."
 msgstr ""
 
-#: packages/settingeditor/src/SettingsFormEditor.tsx:172 packages/settingeditor/src/SettingsFormEditor.tsx:348 packages/ui-components/src/components/form.tsx:183 packages/ui-components/src/components/form.tsx:570
-msgid "Remove"
-msgstr "削除"
-
-#: packages/settingeditor/src/SettingsFormEditor.tsx:183 packages/settingeditor/src/SettingsFormEditor.tsx:225 packages/shortcuts-extension/src/components/ShortcutItem.tsx:416 packages/shortcuts-extension/src/components/ShortcutItem.tsx:432 packages/shortcuts-extension/src/components/ShortcutItem.tsx:66 packages/shortcuts-extension/src/components/ShortcutItem.tsx:71 packages/shortcuts-extension/src/components/ShortcutItem.tsx:85 packages/shortcuts-extension/src/components/ShortcutItem.tsx:90 packages/ui-components/src/components/form.tsx:212
-msgid "Add"
-msgstr "追加"
-
-#: packages/settingeditor/src/SettingsFormEditor.tsx:197 packages/settingeditor/src/SettingsFormEditor.tsx:485
+#: packages/settingeditor/src/SettingsFormEditor.tsx:205
 msgid "Restore to Defaults"
 msgstr ""
 
-#: packages/settingeditor/src/SettingsFormEditor.tsx:356 packages/ui-components/src/components/form.tsx:580
-msgid "Default: %1"
-msgstr "デフォルト:%1"
-
 #: packages/settingeditor/src/inspector.ts:114
 msgid "additional property error"
 msgstr ""
 
 #: packages/settingeditor/src/inspector.ts:115
 msgid "`%1` is not a valid property"
 msgstr ""
@@ -7285,131 +6493,135 @@
 msgid "Any errors will be listed here"
 msgstr "エラーはここにリストされます"
 
 #: packages/settingeditor/src/inspector.ts:90
 msgid "No errors found"
 msgstr "エラーは見つかりませんでした"
 
-#: packages/settingeditor/src/plugineditor.ts:129 packages/settingeditor/src/plugineditor.ts:134
+#: packages/settingeditor/src/plugineditor.ts:129
 msgid "You have unsaved changes."
 msgstr "保存していない変更があります。"
 
-#: packages/settingeditor/src/plugineditor.ts:130 packages/settingeditor/src/plugineditor.ts:135
+#: packages/settingeditor/src/plugineditor.ts:130
 msgid "Do you want to leave without saving?"
 msgstr "保存せずに終了しますか?"
 
-#: packages/settingeditor/src/plugineditor.ts:255 packages/settingeditor/src/plugineditor.ts:257
+#: packages/settingeditor/src/plugineditor.ts:255
 msgid "Your changes were not saved."
 msgstr "変更は保存されませんでした。"
 
-#: packages/settingeditor/src/pluginlist.tsx:442 packages/settingeditor/src/pluginlist.tsx:454 packages/shortcuts-extension/src/components/TopNav.tsx:167
+#: packages/settingeditor/src/pluginlist.tsx:454 packages/shortcuts-extension/src/components/TopNav.tsx:167
 msgid "Search…"
 msgstr "検索…"
 
-#: packages/settingeditor/src/pluginlist.tsx:449 packages/settingeditor/src/pluginlist.tsx:461
+#: packages/settingeditor/src/pluginlist.tsx:461
 msgid "Modified"
 msgstr ""
 
-#: packages/settingeditor/src/pluginlist.tsx:461 packages/settingeditor/src/pluginlist.tsx:473
+#: packages/settingeditor/src/pluginlist.tsx:473
 msgid "No items match your search."
 msgstr ""
 
-#: packages/settingeditor/src/raweditor.ts:368 packages/settingeditor/src/raweditor.ts:377
+#: packages/settingeditor/src/raweditor.ts:368
 msgid "System Defaults"
 msgstr "システムのデフォルト設定"
 
-#: packages/settingeditor/src/raweditor.ts:409 packages/settingeditor/src/raweditor.ts:418
+#: packages/settingeditor/src/raweditor.ts:409
 msgid "User Preferences"
 msgstr "ユーザー設定"
 
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
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:332 packages/shortcuts-extension/src/components/ShortcutItem.tsx:348
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:332
 msgid "or"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:51 packages/shortcuts-extension/src/components/ShortcutItem.tsx:70
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:416 packages/shortcuts-extension/src/components/ShortcutItem.tsx:66 packages/shortcuts-extension/src/components/ShortcutItem.tsx:71 packages/ui-components/src/components/form.tsx:212
+msgid "Add"
+msgstr "追加"
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
 msgstr ""
 
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
 msgstr ""
 
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
 msgstr "カテゴリ"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:183 packages/shortcuts-extension/src/components/TopNav.tsx:275
+#: packages/shortcuts-extension/src/components/TopNav.tsx:183
 msgid "Shortcut"
 msgstr "ショートカット"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:187 packages/shortcuts-extension/src/components/TopNav.tsx:279
+#: packages/shortcuts-extension/src/components/TopNav.tsx:187
 msgid "Selectors"
 msgstr ""
 
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
@@ -7429,52 +6641,44 @@
 "    \"selector\": \"body\",\n"
 "    \"disabled\": true\n"
 "}\n\n"
 "コマンドのリストです。この後にキーボードショートカットが記載されます:\n"
 "%1\n\n"
 "キーボードショートカットのリストです:"
 
-#: packages/statusbar-extension/src/index.ts:52 packages/statusbar-extension/src/index.ts:78
+#: packages/statusbar-extension/src/index.ts:52
 msgid "Show Status Bar"
 msgstr "ステータスバーを表示"
 
-#: packages/statusbar/src/defaults/kernelStatus.tsx:126
-msgid "No Kernel!"
-msgstr "カーネルがありません!"
-
-#: packages/terminal-extension/src/index.ts:103 packages/terminal-extension/src/index.ts:350 packages/terminal-extension/src/index.ts:99 packages/terminal/src/widget.ts:102 packages/terminal/src/widget.ts:74
+#: packages/terminal-extension/src/index.ts:103 packages/terminal-extension/src/index.ts:350 packages/terminal/src/widget.ts:102
 msgid "Terminal"
 msgstr "ターミナル"
 
-#: packages/terminal-extension/src/index.ts:187 packages/terminal-extension/src/index.ts:191
+#: packages/terminal-extension/src/index.ts:191
 msgctxt "menu"
 msgid "Terminal Theme"
 msgstr "ターミナルテーマ"
 
-#: packages/terminal-extension/src/index.ts:192 packages/terminal-extension/src/index.ts:196 packages/terminal-extension/src/index.ts:251 packages/terminal-extension/src/index.ts:534 packages/terminal-extension/src/index.ts:544
+#: packages/terminal-extension/src/index.ts:196 packages/terminal-extension/src/index.ts:251 packages/terminal-extension/src/index.ts:534
 msgid "Inherit"
 msgstr "継承する"
 
-#: packages/terminal-extension/src/index.ts:200 packages/terminal-extension/src/index.ts:204 packages/terminal-extension/src/index.ts:258 packages/terminal-extension/src/index.ts:535 packages/terminal-extension/src/index.ts:545
+#: packages/terminal-extension/src/index.ts:204 packages/terminal-extension/src/index.ts:258 packages/terminal-extension/src/index.ts:535
 msgid "Light"
 msgstr "ライト"
 
-#: packages/terminal-extension/src/index.ts:206 packages/terminal-extension/src/index.ts:210 packages/terminal-extension/src/index.ts:263 packages/terminal-extension/src/index.ts:536 packages/terminal-extension/src/index.ts:546
+#: packages/terminal-extension/src/index.ts:210 packages/terminal-extension/src/index.ts:263 packages/terminal-extension/src/index.ts:536
 msgid "Dark"
 msgstr "ダーク"
 
-#: packages/terminal-extension/src/index.ts:228 packages/terminal-extension/src/index.ts:492
-msgid "Shutdown Terminal"
-msgstr "ターミナルの終了"
-
-#: packages/terminal-extension/src/index.ts:296 packages/terminal-extension/src/index.ts:316
+#: packages/terminal-extension/src/index.ts:316
 msgid "Terminals"
 msgstr "ターミナル"
 
-#: packages/terminal-extension/src/index.ts:304 packages/terminal-extension/src/index.ts:324
+#: packages/terminal-extension/src/index.ts:324
 msgid "Are you sure you want to permanently shut down all running terminals?"
 msgstr ""
 
 #: packages/terminal-extension/src/index.ts:350
 msgid "New Terminal"
 msgstr "新規ターミナル"
 
@@ -7482,110 +6686,82 @@
 msgid "Start a new terminal session"
 msgstr "新しいターミナルセッションを開始"
 
 #: packages/terminal-extension/src/index.ts:389
 msgid "Open a terminal by its `name`."
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:407 packages/terminal-extension/src/index.ts:415
+#: packages/terminal-extension/src/index.ts:407
 msgid "Refresh Terminal"
 msgstr "ターミナルをリフレッシュ"
 
-#: packages/terminal-extension/src/index.ts:408 packages/terminal-extension/src/index.ts:416
+#: packages/terminal-extension/src/index.ts:408
 msgid "Refresh the current terminal session"
 msgstr "現在のターミナルセッションをリフレッシュ"
 
-#: packages/terminal-extension/src/index.ts:506 packages/terminal-extension/src/index.ts:516
+#: packages/terminal-extension/src/index.ts:492
+msgid "Shutdown Terminal"
+msgstr "ターミナルの終了"
+
+#: packages/terminal-extension/src/index.ts:506
 msgid "Increase Terminal Font Size"
 msgstr "ターミナルのフォントサイズを大きく"
 
-#: packages/terminal-extension/src/index.ts:520 packages/terminal-extension/src/index.ts:530
+#: packages/terminal-extension/src/index.ts:520
 msgid "Decrease Terminal Font Size"
 msgstr "ターミナルのフォントサイズを小さくします"
 
 #: packages/terminal-extension/src/index.ts:542
 msgid "Set terminal theme to the provided `theme`."
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:550 packages/terminal-extension/src/index.ts:557
+#: packages/terminal-extension/src/index.ts:550
 msgid "Use Terminal Theme: %1"
 msgstr "ターミナルのテーマを使用します: %1"
 
-#: packages/terminal-extension/src/index.ts:553 packages/terminal-extension/src/index.ts:560
+#: packages/terminal-extension/src/index.ts:553
 msgid "Set the terminal theme"
 msgstr "ターミナルのテーマを設定します"
 
-#: packages/terminal/src/widget.ts:110 packages/terminal/src/widget.ts:345
+#: packages/terminal/src/widget.ts:345
 msgid "Terminal %1"
 msgstr "ターミナル %1"
 
-#: packages/theme-dark-extension/src/index.ts:30 packages/theme-dark-extension/src/index.ts:31
+#: packages/theme-dark-extension/src/index.ts:31
 msgid "JupyterLab Dark"
 msgstr "JupyterLab ダーク"
 
-#: packages/theme-light-extension/src/index.ts:30 packages/theme-light-extension/src/index.ts:31
+#: packages/theme-light-extension/src/index.ts:31
 msgid "JupyterLab Light"
 msgstr "JupyterLab ライト"
 
 #: packages/toc-extension/src/index.ts:113
 msgid "Show output headings"
 msgstr ""
 
-#: packages/toc-extension/src/index.ts:127 packages/toc-extension/src/index.ts:77 packages/toc-extension/src/index.ts:83 packages/toc/src/panel.ts:28 packages/toc/src/panel.ts:79 packages/toc/src/toc.tsx:130
+#: packages/toc-extension/src/index.ts:127 packages/toc-extension/src/index.ts:77 packages/toc/src/panel.ts:28 packages/toc/src/panel.ts:79
 msgid "Table of Contents"
 msgstr "目次"
 
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
-msgstr "自動番号表示の切り替え"
-
-#: packages/toc/src/generators/notebook/tagstool/index.tsx:217
-msgid "No Tags Available"
-msgstr "タグがありません"
-
-#: packages/toc/src/generators/notebook/tagstool/index.tsx:224
-msgid "Clear Filters"
-msgstr "フィルタをクリア"
-
-#: packages/toc/src/generators/notebook/tagstool/index.tsx:255 packages/toc/src/generators/notebook/tagstool/index.tsx:256 packages/toc/src/generators/notebook/tagstool/index.tsx:258 packages/toc/src/generators/notebook/tagstool/index.tsx:266 packages/toc/src/generators/notebook/tagstool/index.tsx:267 packages/toc/src/generators/notebook/tagstool/index.tsx:271
-msgid "Select All Cells With Current Tags"
-msgstr ""
-
-#: packages/toc/src/generators/notebook/toolbar_generator.tsx:182 packages/toc/src/generators/notebook/toolbar_generator.tsx:183
-msgid "Toggle Code Cells"
-msgstr "コードセルの表示切り替え"
-
-#: packages/toc/src/generators/notebook/toolbar_generator.tsx:198 packages/toc/src/generators/notebook/toolbar_generator.tsx:199
-msgid "Toggle Markdown Text Cells"
-msgstr "Markdownテキストセルの表示切り替え"
-
-#: packages/toc/src/generators/notebook/toolbar_generator.tsx:230 packages/toc/src/generators/notebook/toolbar_generator.tsx:231
-msgid "Show Tags Menu"
-msgstr "タグメニューを表示"
-
 #: packages/toc/src/panel.ts:32
 msgid "No Headings"
 msgstr ""
 
 #: packages/toc/src/panel.ts:33
 msgid "The table of contents shows headings in notebooks and supported files."
 msgstr ""
@@ -7594,23 +6770,23 @@
 msgid "Open the tooltip"
 msgstr ""
 
 #: packages/tooltip-extension/src/index.ts:56
 msgid "Dismiss the tooltip"
 msgstr ""
 
-#: packages/translation-extension/src/index.ts:132 packages/translation-extension/src/index.ts:141
+#: packages/translation-extension/src/index.ts:141
 msgid "Change interface language?"
 msgstr "インターフェイスの言語を変更しますか?"
 
-#: packages/translation-extension/src/index.ts:133 packages/translation-extension/src/index.ts:142
+#: packages/translation-extension/src/index.ts:142
 msgid "After changing the interface language to %1, you will need to reload JupyterLab to see the changes."
 msgstr "インターフェイス言語を%1に変更した後、JupyterLabを再読込みして変更を確認する必要があります。"
 
-#: packages/translation-extension/src/index.ts:139 packages/translation-extension/src/index.ts:148
+#: packages/translation-extension/src/index.ts:148
 msgid "Change and reload"
 msgstr "変更して再読込み"
 
 #: packages/translation-extension/src/index.ts:175
 msgid "Display Languages"
 msgstr ""
 
@@ -7618,14 +6794,22 @@
 msgid "Move down"
 msgstr ""
 
 #: packages/ui-components/src/components/form.tsx:146
 msgid "Move up"
 msgstr ""
 
+#: packages/ui-components/src/components/form.tsx:183 packages/ui-components/src/components/form.tsx:570
+msgid "Remove"
+msgstr "削除"
+
+#: packages/ui-components/src/components/form.tsx:580
+msgid "Default: %1"
+msgstr "デフォルト:%1"
+
 #: packages/ui-components/src/components/sidepanel.ts:118
 msgid "side panel actions"
 msgstr ""
 
 #: packages/ui-components/src/components/sidepanel.ts:41
 msgid "side panel content"
 msgstr ""
```

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_git.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_git.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_lsp.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_lsp.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_search_replace.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_search_replace.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_spreadsheet_editor.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_spreadsheet_editor.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_tour.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_tour.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_widgets.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupyterlab_widgets.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupytext.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/jupytext.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/notebook.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/notebook.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: ja\n"
 "X-Crowdin-File: /main/extensions/notebook/locale/notebook.pot\n"
 "X-Crowdin-File-ID: 231\n"
 "Language-Team: Japanese\n"
 "Language: ja_JP\n"
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

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/retrolab.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/retrolab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/spellchecker.po` & `jupyterlab_language_pack_ja_jp-4.0.post0/jupyterlab_language_pack_ja_JP/locale/ja_JP/LC_MESSAGES/spellchecker.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/.gitignore` & `jupyterlab_language_pack_ja_jp-4.0.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/LICENSE.txt` & `jupyterlab_language_pack_ja_jp-4.0.post0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/pyproject.toml` & `jupyterlab_language_pack_ja_jp-4.0.post0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 keywords = ["jupyterlab", "language", "language pack", "localization"]
 dynamic = ["version"]
 
 [project.entry-points."jupyterlab.languagepack"]
 ja_JP = "jupyterlab_language_pack_ja_JP"
 
-[projects.urls]
+[project.urls]
 homepage = "https://github.com/jupyterlab/language-packs"
 
 [tool.hatch.build]
 artifacts = [
     "CONTRIBUTORS.md"
 ]
```

### Comparing `jupyterlab_language_pack_ja_jp-3.6.post3/PKG-INFO` & `jupyterlab_language_pack_ja_jp-4.0.post0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: jupyterlab-language-pack-ja-JP
-Version: 3.6.post3
+Version: 4.0.post0
 Summary: JupyterLab Japanese (Japan) Language Pack
+Project-URL: homepage, https://github.com/jupyterlab/language-packs
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2023 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

