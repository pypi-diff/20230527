# Comparing `tmp/jdNBTExplorer-1.2.tar.gz` & `tmp/jdNBTExplorer-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdNBTExplorer-1.2.tar", last modified: Sun Jan  9 10:19:58 2022, max compression
+gzip compressed data, was "jdNBTExplorer-2.0.tar", last modified: Sat May 27 08:53:19 2023, max compression
```

## Comparing `jdNBTExplorer-1.2.tar` & `jdNBTExplorer-2.0.tar`

### file list

```diff
@@ -1,30 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-09 10:19:58.678443 jdNBTExplorer-1.2/
--rw-rw-rw-   0 root         (0) root         (0)    35071 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1435 2022-01-09 10:19:58.678443 jdNBTExplorer-1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-09 10:19:58.675443 jdNBTExplorer-1.2/jdNBTExplorer/
--rw-rw-rw-   0 root         (0) root         (0)     1589 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/AboutWindow.py
--rw-rw-rw-   0 root         (0) root         (0)     5442 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/EditWindow.py
--rw-rw-rw-   0 root         (0) root         (0)     1343 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/Enviroment.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/Functions.py
--rw-rw-rw-   0 root         (0) root         (0)    17770 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/Logo.png
--rw-rw-rw-   0 root         (0) root         (0)     9790 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/MainWindow.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/Settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2935 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/SettingsWindow.py
--rw-rw-rw-   0 root         (0) root         (0)    14820 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/TreeWidget.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/jdNBTExplorer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-09 10:19:58.677443 jdNBTExplorer-1.2/jdNBTExplorer/translation/
--rw-rw-rw-   0 root         (0) root         (0)     3209 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/translation/de_DE.lang
--rw-rw-rw-   0 root         (0) root         (0)     2891 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/jdNBTExplorer/translation/en_GB.lang
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-09 10:19:58.677443 jdNBTExplorer-1.2/jdNBTExplorer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1435 2022-01-09 10:19:58.000000 jdNBTExplorer-1.2/jdNBTExplorer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      668 2022-01-09 10:19:58.000000 jdNBTExplorer-1.2/jdNBTExplorer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-09 10:19:58.000000 jdNBTExplorer-1.2/jdNBTExplorer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2022-01-09 10:19:58.000000 jdNBTExplorer-1.2/jdNBTExplorer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-01-09 10:19:58.000000 jdNBTExplorer-1.2/jdNBTExplorer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-01-09 10:19:58.000000 jdNBTExplorer-1.2/jdNBTExplorer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-09 10:19:58.678443 jdNBTExplorer-1.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1848 2022-01-09 10:19:50.000000 jdNBTExplorer-1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35071 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      173 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5178 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3642 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/jdNBTExplorer/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/AboutWindow.py
+-rw-r--r--   0 root         (0) root         (0)     4782 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/EditWindow.py
+-rw-r--r--   0 root         (0) root         (0)      751 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/Environment.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/Functions.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/Languages.py
+-rw-r--r--   0 root         (0) root         (0)    17770 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/Logo.png
+-rw-r--r--   0 root         (0) root         (0)     7815 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/MainWindow.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/Settings.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/SettingsWindow.py
+-rw-r--r--   0 root         (0) root         (0)    14346 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/TreeWidget.py
+-rw-r--r--   0 root         (0) root         (0)     2379 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/jdNBTExplorer/translations/
+-rw-r--r--   0 root         (0) root         (0)    14190 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/translations/jdNBTExplorer_de.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/jdNBTExplorer/ui/
+-rw-r--r--   0 root         (0) root         (0)     2020 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/ui/AboutWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/ui/EditWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     5515 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/ui/MainWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/ui/SettingsWindow.ui
+-rw-r--r--   0 root         (0) root         (0)        3 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5178 2023-05-27 08:53:19.000000 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      815 2023-05-27 08:53:19.000000 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 08:53:19.000000 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-27 08:53:19.000000 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-27 08:53:19.000000 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-27 08:53:19.000000 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/setup.cfg
```

### Comparing `jdNBTExplorer-1.2/LICENSE` & `jdNBTExplorer-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-1.2/jdNBTExplorer/EditWindow.py` & `jdNBTExplorer-2.0/jdNBTExplorer/EditWindow.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,81 +1,68 @@
-from PyQt6.QtWidgets import QWidget, QLabel, QPushButton, QLineEdit, QComboBox, QHBoxLayout, QVBoxLayout, QGridLayout
-from .Functions import showMessageBox
+from .ui_compiled.EditWindow import Ui_EditWindow
+from PyQt6.QtWidgets import QDialog, QMessageBox
+from PyQt6.QtCore import QCoreApplication
+from typing import TYPE_CHECKING
 from .TreeWidget import TagItem
 
+
+if TYPE_CHECKING:
+    from .Environment import Environment
+
+
 class TypeIndexNames():
     INT = 0
     INT_ARRAY = 1
     LONG = 2
     LONG_ARRAY = 3
     DOUBLE = 4
     FLOAT = 5
     BYTE = 6
     BYTE_ARRAY = 7
     STRING = 8
     SHORT = 9
     NONE = 10
 
-class EditWindow(QWidget):
-    def __init__(self, env):
+
+class EditWindow(QDialog, Ui_EditWindow):
+    def __init__(self, env: "Environment"):
         super().__init__()
         self.env = env
-        self.nameEdit = QLineEdit()
-        self.valueEdit = QLineEdit()
-        self.typeComboBox = QComboBox()
+
+        self.setupUi(self)
+
         self.typelist = ["int","int_array","long","long_array","double","float","byte","byte_array","string","short","none"]
-        okButton = QPushButton(env.translate("button.ok"))
-        cancelButton = QPushButton(env.translate("button.cancel"))
 
         self.typeComboBox.addItem("Int")
         self.typeComboBox.addItem("IntArray")
         self.typeComboBox.addItem("Long")
         self.typeComboBox.addItem("LongArray")
         self.typeComboBox.addItem("Double")
         self.typeComboBox.addItem("Float")
         self.typeComboBox.addItem("Byte")
         self.typeComboBox.addItem("ByteArray")
         self.typeComboBox.addItem("String")
         self.typeComboBox.addItem("Short")
         self.typeComboBox.addItem("None")
 
-        okButton.clicked.connect(self.okButtonClicked)
-        cancelButton.clicked.connect(self.close)
+        self.buttonBox.accepted.connect(self.okButtonClicked)
+        self.buttonBox.rejected.connect(self.close)
 
-        gridLayout = QGridLayout()
-        gridLayout.addWidget(QLabel(env.translate("editWindow.label.name")),0,0)
-        gridLayout.addWidget(self.nameEdit,0,1)
-        gridLayout.addWidget(QLabel(env.translate("editWindow.label.value")),1,0)
-        gridLayout.addWidget(self.valueEdit,1,1)
-        gridLayout.addWidget(QLabel(env.translate("editWindow.label.type")),2,0)
-        gridLayout.addWidget(self.typeComboBox,2,1)
-
-        buttonLayout = QHBoxLayout()
-        buttonLayout.addStretch(1)
-        buttonLayout.addWidget(okButton)
-        buttonLayout.addWidget(cancelButton)
-
-        mainLayout = QVBoxLayout()
-        mainLayout.addLayout(gridLayout)
-        mainLayout.addLayout(buttonLayout)
-
-        self.setLayout(mainLayout)
-
-    def openWindow(self, isNew, item, taglist: bool=False,name: str=None):
+    def openWindow(self, isNew, item, taglist: bool = False, name: str | None = None):
         if isNew:
             self.nameEdit.setText(name or "")
             self.valueEdit.setText("")
             self.typeComboBox.setCurrentIndex(0)
-            self.setWindowTitle(self.env.translate("editWindow.title.new"))
+            self.setWindowTitle(QCoreApplication.translate("EditWindow", "New"))
         else:
             self.nameEdit.setText(item.text(0))
             self.valueEdit.setText(item.text(1))
             tagType = item.tagType()
             self.typeComboBox.setCurrentIndex(self.typelist.index(tagType))
-            self.setWindowTitle(self.env.translate("editWindow.title.edit"))
+            self.setWindowTitle(QCoreApplication.translate("EditWindow", "Edit"))
         if taglist:
             self.nameEdit.setEnabled(False)
             self.typeComboBox.setEnabled(False)
             if isNew:
                 if item.childCount() == 0:
                     self.typeComboBox.setEnabled(True)
                 else:
@@ -86,47 +73,49 @@
                 else:
                     self.typeComboBox.setCurrentIndex(self.typelist.index(item.parent().child(0).tagType()))
         else:
             self.nameEdit.setEnabled(True)
             self.typeComboBox.setEnabled(True)
         self.item = item
         self.isNew = isNew
-        self.show()
-        self.setFocus()
+        self.exec()
 
     def okButtonClicked(self):
-        if self.nameEdit.text() =="":
-            showMessageBox(self.env.translate("editWindow.messageBox.noName.title"),self.env.translate("editWindow.messageBox.noName.text"))
+        if self.nameEdit.text().strip() == "":
+            QMessageBox.critical(self, QCoreApplication.translate("EditWindow", "Name can't be empty"), QCoreApplication.translate("EditWindow", "You need to set a Name"))
             return
+
         typeIndex = self.typeComboBox.currentIndex()
         if typeIndex == TypeIndexNames.INT or typeIndex == TypeIndexNames.LONG or typeIndex == TypeIndexNames.BYTE or typeIndex == TypeIndexNames.SHORT:
             try:
                 int(self.valueEdit.text())
-            except:
-                showMessageBox(self.env.translate("editWindow.messageBox.wrongValue.title"),self.env.translate("editWindow.messageBox.wrongValue.text"))
+            except Exception:
+                QMessageBox.critical(self, QCoreApplication.translate("EditWindow", "Invalid Value"), QCoreApplication.translate("EditWindow", "This value is not allowed for this type"))
                 return
         elif typeIndex == TypeIndexNames.DOUBLE or typeIndex == TypeIndexNames.FLOAT:
             try:
                 float(self.valueEdit.text())
-            except:
-                showMessageBox(self.env.translate("editWindow.messageBox.wrongValue.title"),self.env.translate("editWindow.messageBox.wrongValue.text"))
+            except Exception:
+                QMessageBox.critical(self, QCoreApplication.translate("EditWindow", "Invalid Value"), QCoreApplication.translate("EditWindow", "This value is not allowed for this type"))
                 return
         elif typeIndex == TypeIndexNames.INT_ARRAY:
             checkstr = self.valueEdit.text()[1:-1]
             for i in checkstr.split(","):
                 if i == "":
                     continue
                 try:
                     int(i)
-                except:
-                    showMessageBox(self.env.translate("editWindow.messageBox.wrongValue.title"),self.env.translate("editWindow.messageBox.wrongValue.text"))
+                except Exception:
+                    QMessageBox.critical(self, QCoreApplication.translate("EditWindow", "Invalid Value"), QCoreApplication.translate("EditWindow", "This value is not allowed for this type"))
                     return
+
         if self.isNew:
             item = TagItem(self.item)
         else:
             item = self.item
+
         item.setText(0,self.nameEdit.text())
         item.setText(1,self.valueEdit.text())
         item.setTagType(self.typelist[self.typeComboBox.currentIndex()])
         item.updateTypeText()
         self.env.modified = True
         self.close()
```

### Comparing `jdNBTExplorer-1.2/jdNBTExplorer/Enviroment.py` & `jdNBTExplorer-2.0/jdNBTExplorer/Environment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,20 @@
-from jdTranslationHelper import jdTranslationHelper
 from .Functions import getDataPath, readJsonFile
-from .Settings import Settings
 from PyQt6.QtCore import QLocale
+from .Settings import Settings
 from PyQt6.QtGui import QIcon
 import os
 
-class Enviroment():
+class Environment():
     def __init__(self):
-        self.version = "1.2"
         self.modified = False
         self.dataDir = getDataPath()
         self.programDir = os.path.dirname(os.path.realpath(__file__))
         self.programIcon = QIcon(os.path.join(self.programDir, "Logo.png"))
 
-        default_settings = {
-            "language": "default",
-            "maxRecentFiles": 10,
-            "showWelcomeMessage": True,
-            "checkSave": True
-        }
-        self.settings = Settings(default_settings=default_settings)
-        self.settings.load_from_file(os.path.join(self.dataDir,"settings.json"))
-
-        if self.settings.get("language") == "default":
-            self.translations = jdTranslationHelper(QLocale.system().name())
-        else:
-            self.translations = jdTranslationHelper(self.settings.get("language"))
-
-        self.translations.loadDirectory(os.path.join(self.programDir,"translation"))
+        with open(os.path.join(self.programDir, "version.txt"), "r", encoding="utf-8") as f:
+            self.version = f.read()
 
-        self.recentFiles = readJsonFile(os.path.join(self.dataDir,"recentfiles.json"),[])
+        self.settings = Settings()
+        self.settings.load_from_file(os.path.join(self.dataDir,"settings.json"))
 
-    def translate(self, string):
-        #Just a litle shortcut
-        return self.translations.translate(string)
+        self.recentFiles = readJsonFile(os.path.join(self.dataDir,"recentfiles.json"), [])
```

### Comparing `jdNBTExplorer-1.2/jdNBTExplorer/Functions.py` & `jdNBTExplorer-2.0/jdNBTExplorer/Functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,38 @@
-from PyQt6.QtWidgets import QMessageBox
 from pathlib import Path
 from typing import Any
 import platform
 import json
 import sys
 import os
 
 
-def showMessageBox(title, text):
-    messageBox = QMessageBox()
-    messageBox.setWindowTitle(title)
-    messageBox.setText(text)
-    messageBox.setStandardButtons(QMessageBox.StandardButton.Ok)
-    messageBox.exec()
-
-
-def stringToList(string,content_type):
+def stringToList(string: str, content_type):
     string = string[1:-1]
     array = []
     for i in string.split(","):
         if i == "":
             continue
         else:
             array.append(content_type(i))
     return array
 
 
 def getDataPath() -> str:
     if platform.system() == "Windows":
-        return os.path.join(os.getenv("appdata"), "jdNBTExplorer")
+        return os.path.join(os.getenv("APPDATA"), "JakobDev", "jdNBTExplorer")
     elif platform.system() == "Darwin":
-        return os.path.join(str(Path.home()),"Library", "Application Support", "jdNBTExplorer")
+        return os.path.join(str(Path.home()),"Library", "Application Support", "JakobDev", "jdNBTExplorer")
     elif platform.system() == "Haiku":
-        return os.path.join(str(Path.home()),"config", "settings", "jdNBTExplorer")
+        return os.path.join(str(Path.home()),"config", "settings", "JakobDev", "jdNBTExplorer")
     else:
         if os.getenv("XDG_DATA_HOME"):
-            return os.path.join(os.getenv("XDG_DATA_HOME"), "jdNBTExplorer")
+            return os.path.join(os.getenv("XDG_DATA_HOME"), "JakobDev", "jdNBTExplorer")
         else:
-            return os.path.join(str(Path.home()), ".local", "share", "jdNBTExplorer")
+            return os.path.join(str(Path.home()), ".local", "share", "JakobDev", "jdNBTExplorer")
 
 
 def readJsonFile(path: str,default: Any) -> Any:
     """
     Tries to parse the given JSON file and prints a error if the file couldn't be parsed
     Returns default if the file is not found or couldn't be parsed
     """
@@ -49,12 +40,12 @@
         try:
             with open(path,"r",encoding="utf-8") as f:
                 data = json.load(f)
                 return data
         except json.decoder.JSONDecodeError as e:
             print(f"Can't parse {os.path.basename(path)}: {e.msg}: line {e.lineno} column {e.colno} (char {e.pos})",file=sys.stderr)
             return default
-        except:
+        except Exception:
             print("Can't read " + os.path.basename(path),file=sys.stderr)
             return default
     else:
         return default
```

### Comparing `jdNBTExplorer-1.2/jdNBTExplorer/Logo.png` & `jdNBTExplorer-2.0/jdNBTExplorer/Logo.png`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-1.2/jdNBTExplorer/Settings.py` & `jdNBTExplorer-2.0/jdNBTExplorer/Settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from .Functions import readJsonFile
 from typing import Any
 import json
 import os
 
 
 class Settings():
-    def __init__(self,default_settings={}):
-        self.default_settings = default_settings
+    def __init__(self):
+        self.default_settings = {
+            "language": "default",
+            "maxRecentFiles": 10,
+            "showWelcomeMessage": True,
+            "checkSave": True
+        }
+
         self.custom_settings = {}
 
     def get(self,key: str) -> Any:
         if key in self.custom_settings:
             return self.custom_settings[key]
         else:
             return self.default_settings[key]
```

### Comparing `jdNBTExplorer-1.2/jdNBTExplorer/TreeWidget.py` & `jdNBTExplorer-2.0/jdNBTExplorer/TreeWidget.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from PyQt6.QtWidgets import QTreeWidget, QTreeWidgetItem, QInputDialog, QHeaderView
-from .Functions import showMessageBox, stringToList
+from PyQt6.QtWidgets import QTreeWidget, QTreeWidgetItem, QInputDialog, QHeaderView, QMessageBox
+from PyQt6.QtCore import QCoreApplication
+from .Functions import stringToList
 from PyQt6.QtGui import QCursor
 import copy
 import nbt
 import os
 
+
 class TagItem(QTreeWidgetItem):
     def __init__(self, parent):
         super().__init__(parent)
         self.tag_type = None
         self.file_path = None
         self.file_type = None
         self.pos_x = None
@@ -65,33 +67,30 @@
     def setChunkCords(self, x, z):
         self.pos_x = x
         self.pos_z = z
 
     def getChunkCords(self):
         return self.pos_x, self.pos_z
 
+
 class TreeWidget(QTreeWidget):
     def __init__(self, env):
         super().__init__()
         self.setAcceptDrops(True)
         self.env = env
         self.NoneTag = None
-        self.setHeaderLabels((env.translate("treeWidget.header.name"), env.translate("treeWidget.header.value"),env.translate("treeWidget.header.type")))
+        self.setHeaderLabels((QCoreApplication.translate("TreeWidget", "Name"), QCoreApplication.translate("TreeWidget", "Value"), QCoreApplication.translate("TreeWidget", "Type")))
         self.header().setSectionResizeMode(0, QHeaderView.ResizeMode.Stretch)
         self.header().setSectionResizeMode(1, QHeaderView.ResizeMode.Stretch)
         self.header().setSectionResizeMode(2, QHeaderView.ResizeMode.Stretch)
         self.itemDoubleClicked.connect(self.editTag)
         self.currentItemChanged.connect(self.updateMenu)
-         # self.setDragDropMode(QtGui.QAbstractItemView.DragDrop)
-        #self.setAcceptDrops(True)
-        #self.setDragEnabled(True)
-        #self.setAllowDrag(True)
 
     def updateMenu(self, item):
-        if item == None:
+        if item is None:
             return
         if item.tagType() == "compound" or item.tagType() == "root":
             self.env.mainWindow.editTagAction.setEnabled(False)
         else:
             self.env.mainWindow.editTagAction.setEnabled(True)
         if item.tagType() != "root":
             if item.parent().tagType() != "list":
@@ -104,38 +103,38 @@
             self.env.mainWindow.removeTagAction.setEnabled(False)
         else:
             self.env.mainWindow.removeTagAction.setEnabled(True)
         self.env.mainWindow.newTagAction.setEnabled(True)
         self.env.mainWindow.newCompoundAction.setEnabled(True)
         self.env.mainWindow.newListAction.setEnabled(True)
 
-    def newFile(self, path):
+    def newFile(self, path: str) -> None:
         rootItem = TagItem(0)
         rootItem.setText(0,os.path.basename(path))
         rootItem.setPath(path)
         rootItem.setTagType("root")
         rootItem.setFileType("nbt")
         self.addTopLevelItem(rootItem)
 
-    def openNBTFile(self, path):
+    def openNBTFile(self, path: str) -> None:
         try:
             nbtfile = nbt.nbt.NBTFile(path,"rb")
-        except:
-            print("FFF")
-            showMessageBox(self.env.translate("treeWidget.messageBox.cantRead.title"),self.env.translate("treeWidget.messageBox.cantRead.text") % path)
+        except Exception:
+            QMessageBox.critical(self, QCoreApplication.translate("TreeWidget", "Can't read file"), QCoreApplication.translate("TreeWidget", "Can't read {{path}}. Maybe it's not a NBT File.").replace("{{path}}", path))
             return
+
         rootItem = TagItem(0)
         rootItem.setText(0,os.path.basename(path))
         rootItem.setPath(path)
         rootItem.setTagType("root")
         rootItem.setFileType("nbt")
         self.parseCombound(rootItem,nbtfile)
         self.addTopLevelItem(rootItem)
 
-    def openRegionFile(self,path):
+    def openRegionFile(self, path: str) -> None:
         region = nbt.region.RegionFile(path,"rb")
         rootItem = TagItem(0)
         rootItem.setText(0,os.path.basename(path))
         rootItem.setPath(path)
         rootItem.setTagType("root")
         rootItem.setFileType("region")
         for i in region.get_chunks():
@@ -171,19 +170,17 @@
             item.setTagType("string")
         elif isinstance(value,nbt.nbt.TAG_Short):
             item.setTagType("short")
         elif isinstance(value,nbt.nbt.TAG_Compound):
             item.setTagType("compound")
         elif isinstance(value,nbt.nbt.TAG_List):
             item.setTagType("list")
-        elif value.value == None:
+        elif value.value is None:
             item.setTagType("none")
             self.NoneTag = value
-        else:
-            print(type(value))
         item.updateTypeText()
         if hasattr(value,"items"):
             self.parseCombound(item,value)
         elif isinstance(value,nbt.nbt.TAG_List):
             self.parseList(item,value)
         elif  isinstance(value,nbt.nbt.TAG_Byte_Array):
             s = "["
@@ -206,24 +203,15 @@
         for i in range(self.topLevelItemCount()):
             item = self.topLevelItem(i)
             if item.getFileType() == "nbt":
                 f = nbt.nbt.NBTFile()
                 self.getSaveList(item,f.tags)
                 f.write_file(item.getPath())
             elif item.getFileType() == "region":
-                showMessageBox("Not supported","Saving a region file is currently not supported")
-                #region = nbt.region.RegionFile(item.getPath(),"rb")
-                #for i in range(item.childCount()):
-                    #x, z = item.child(i).getChunkCords()
-                   # self.getItems(item.child(i),region.get_nbt(x,z).tags)
-                    #self.getSaveList(item.child(i),region.get_nbt(x,z).tags)
-                    #f = nbt.nbt.NBTFile()
-                    #region.write_chunk(x,z,f)
-                #region.close()
-                #region.close()
+                QMessageBox.critical(self, QCoreApplication.translate("TreeWidget", "Not supported"), QCoreApplication.translate("TreeWidget", "Saving a region file is currently not supported"))
             self.env.modified = False
 
     def getTag(self, child):
         tagType = child.tagType()
         if tagType == "int":
             data = nbt.nbt.TAG_Int(int(child.text(1)),name=child.text(0))
         elif tagType == "int_array":
@@ -266,21 +254,19 @@
             data = nbt.nbt.TAG_String("Error",name=child.text(0))
         data.name = child.text(0)
         return data
 
     def getSaveList(self,item,tags):
         for i in range(item.childCount()):
             child = item.child(i)
-            tagType = child.tagType()
             tags.append(self.getTag(child))
 
     def getSaveCompound(self,item,tags):
         for i in range(item.childCount()):
             child = item.child(i)
-            tagType = child.tagType()
             tag = self.getTag(child)
             tags[tag.name] = tag
 
     def newTag(self):
         item = self.currentItem()
         if item:
             if item.tagType() == "compound" or item.tagType() == "root":
@@ -300,45 +286,45 @@
                     self.env.editWindow.openWindow(False,item,taglist=True)
                 else:
                     self.env.editWindow.openWindow(False,item)
 
     def newCompound(self):
         item = self.currentItem()
         if item:
-            name, ok = QInputDialog.getText(self,self.env.translate("treeWidget.messageBox.newCompound.title"),self.env.translate("treeWidget.messageBox.newCompound.text"))
+            name, ok = QInputDialog.getText(self, QCoreApplication.translate("TreeWidget", "New Compound"), QCoreApplication.translate("TreeWidget", "Please enter a name for the new compound"))
             if not ok or name == '':
                 return
             if item.tagType() == "compound" or item.tagType() == "list" or item.tagType() == "root":
                 newComp = TagItem(item)
             else:
                 newComp = TagItem(item.parent())
             newComp.setText(0,name)
             newComp.setTagType("compound")
             newComp.updateTypeText()
             self.env.modified = True
 
     def newList(self):
         item = self.currentItem()
         if item:
-            name, ok = QInputDialog.getText(self,self.env.translate("treeWidget.messageBox.newCompound.title"),self.env.translate("treeWidget.messageBox.newCompound.text"))
+            name, ok = QInputDialog.getText(self, QCoreApplication.translate("TreeWidget", "New List"), QCoreApplication.translate("TreeWidget", "Please enter a name for the new List"))
             if not ok or name == '':
                 return
             if item.tagType() == "compound" or item.tagType() == "list" or item.tagType() == "root":
                 newComp = TagItem(item)
             else:
                 newComp = TagItem(item.parent())
             newComp.setText(0,name)
             newComp.setTagType("list")
             newComp.updateTypeText()
             self.env.modified = True
 
     def renameItem(self):
         item = self.currentItem()
         if item:
-            name, ok = QInputDialog.getText(self,self.env.translate("treeWidget.messageBox.rename.title"),self.env.translate("treeWidget.messageBox.rename.text"),text=item.text(0))
+            name, ok = QInputDialog.getText(self, QCoreApplication.translate("TreeWidget", "Rename"), QCoreApplication.translate("TreeWidget", "Please enter a new Name"), text=item.text(0))
             if ok and name != '':
                 item.setText(0,name)
                 self.env.modified = True
 
     def removeTag(self):
         item = self.currentItem()
         if item:
```

