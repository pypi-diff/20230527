# Comparing `tmp/desktoptools-0.0.1.tar.gz` & `tmp/desktoptools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktoptools-0.0.1.tar", max compression
+gzip compressed data, was "desktoptools-0.0.7.tar", max compression
```

## Comparing `desktoptools-0.0.1.tar` & `desktoptools-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0       43 2023-04-05 11:23:02.665531 desktoptools-0.0.1/DesktopTools/__init__.py
--rw-r--r--   0        0        0     2959 2023-04-05 11:23:02.665531 desktoptools-0.0.1/DesktopTools/app/msg_systray.py
--rw-r--r--   0        0        0      843 2023-04-05 11:23:02.665531 desktoptools-0.0.1/DesktopTools/args.py
--rw-r--r--   0        0        0     5993 2023-04-05 11:23:02.665531 desktoptools-0.0.1/DesktopTools/feather_hotkey/clip_string.py
--rw-r--r--   0        0        0     2476 2023-04-05 11:23:02.665531 desktoptools-0.0.1/DesktopTools/feather_hotkey/searchbar.ui
--rw-r--r--   0        0        0      469 2023-04-05 11:23:02.665531 desktoptools-0.0.1/DesktopTools/feather_hotkey/thread.py
--rw-r--r--   0        0        0     4175 2023-04-05 11:23:02.665531 desktoptools-0.0.1/DesktopTools/feather_hotkey/ui_searchbar.py
--rw-r--r--   0        0        0     4752 2023-04-05 11:23:02.669532 desktoptools-0.0.1/DesktopTools/feather_hotkey/win_searchbar.py
--rw-r--r--   0        0        0     1052 2023-04-05 11:23:02.669532 desktoptools-0.0.1/DesktopTools/feather_timer/data_alchemy/inputs.py
--rw-r--r--   0        0        0     6612 2023-04-05 11:23:02.669532 desktoptools-0.0.1/DesktopTools/feather_timer/data_alchemy/models.py
--rw-r--r--   0        0        0     1245 2023-04-05 11:23:02.669532 desktoptools-0.0.1/DesktopTools/feather_timer/data_alchemy/worktimes.py
--rw-r--r--   0        0        0     8228 2023-04-05 11:23:02.669532 desktoptools-0.0.1/DesktopTools/feather_timer/halahayawa.py
--rw-r--r--   0        0        0     5447 2023-04-05 11:23:02.669532 desktoptools-0.0.1/DesktopTools/feather_timer/input_counter.py
--rw-r--r--   0        0        0     5525 2023-04-05 11:23:02.669532 desktoptools-0.0.1/DesktopTools/feather_timer/monitor.py
--rw-r--r--   0        0        0     3638 2023-04-05 11:23:02.669532 desktoptools-0.0.1/DesktopTools/harry_potter.ico
--rw-r--r--   0        0        0    25663 2023-04-05 11:23:02.669532 desktoptools-0.0.1/DesktopTools/harry_potter.png
--rw-r--r--   0        0        0     1177 2023-04-05 11:23:02.669532 desktoptools-0.0.1/DesktopTools/logger.py
--rw-r--r--   0        0        0      276 2023-04-05 11:23:02.669532 desktoptools-0.0.1/DesktopTools/main.py
--rw-r--r--   0        0        0     4233 2023-04-05 11:23:02.669532 desktoptools-0.0.1/DesktopTools/tools.py
--rw-r--r--   0        0        0     2131 2023-04-05 11:23:02.669532 desktoptools-0.0.1/DesktopTools/windows_main.py
--rw-r--r--   0        0        0     1063 2023-04-05 11:23:02.669532 desktoptools-0.0.1/LICENSE
--rw-r--r--   0        0        0     2859 2023-04-05 11:23:02.669532 desktoptools-0.0.1/README.md
--rw-r--r--   0        0        0     1088 2023-04-05 11:23:02.669532 desktoptools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3861 1970-01-01 00:00:00.000000 desktoptools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-05-27 14:28:23.162518 desktoptools-0.0.7/DesktopTools/__init__.py
+-rw-r--r--   0        0        0     3343 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/app/msg_systray.py
+-rw-r--r--   0        0        0      850 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/args.py
+-rw-r--r--   0        0        0     6597 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/feather_hotkey/clip_string.py
+-rw-r--r--   0        0        0     2133 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/feather_hotkey/models.py
+-rw-r--r--   0        0        0     2756 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/feather_hotkey/searchbar.ui
+-rw-r--r--   0        0        0     5055 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/feather_hotkey/searchbar_ui.py
+-rw-r--r--   0        0        0      473 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/feather_hotkey/thread.py
+-rw-r--r--   0        0        0     5055 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/feather_hotkey/ui_searchbar.py
+-rw-r--r--   0        0        0     7851 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/feather_hotkey/win_searchbar.py
+-rw-r--r--   0        0        0     1052 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/feather_timer/data_alchemy/inputs.py
+-rw-r--r--   0        0        0     6612 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/feather_timer/data_alchemy/models.py
+-rw-r--r--   0        0        0     1245 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/feather_timer/data_alchemy/worktimes.py
+-rw-r--r--   0        0        0     8649 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/feather_timer/halahayawa.py
+-rw-r--r--   0        0        0     5447 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/feather_timer/input_counter.py
+-rw-r--r--   0        0        0     5525 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/feather_timer/monitor.py
+-rw-r--r--   0        0        0     3638 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/harry_potter.ico
+-rw-r--r--   0        0        0    25663 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/harry_potter.png
+-rw-r--r--   0        0        0     1165 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/logger.py
+-rw-r--r--   0        0        0      276 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/main.py
+-rw-r--r--   0        0        0     4233 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/tools.py
+-rw-r--r--   0        0        0     2223 2023-05-27 14:28:23.166518 desktoptools-0.0.7/DesktopTools/windows_main.py
+-rw-r--r--   0        0        0     1063 2023-05-27 14:28:23.166518 desktoptools-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4564 2023-05-27 14:28:23.166518 desktoptools-0.0.7/README.md
+-rw-r--r--   0        0        0     1090 2023-05-27 14:28:23.166518 desktoptools-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5589 1970-01-01 00:00:00.000000 desktoptools-0.0.7/PKG-INFO
```

### Comparing `desktoptools-0.0.1/DesktopTools/app/msg_systray.py` & `desktoptools-0.0.7/DesktopTools/app/msg_systray.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,30 +37,40 @@
         # 把鼠标点击图标的信号和槽连接
         self.activated.connect(self.iconClicked)
 
         # 把鼠标点击弹出消息的信号和槽连接
         self.messageClicked.connect(self.msgClickEvent)
 
         # 设置图标
-        app_path = os.path.dirname(os.path.abspath(__file__))
-        root_path, app_fname = os.path.split(app_path)
-        if app_fname == "app":
-            ico_path = os.path.join(root_path, "harry_potter.ico")
-            self.setIcon(QIcon(ico_path))
+        ico_path = ""
+        if os.path.exists("harry_potter.ico"):
+            ico_path = "harry_potter.ico"
+        else:
+            app_path = os.path.dirname(os.path.abspath(__file__))
+            root_path, app_fname = os.path.split(app_path)
+            if app_fname == "app":
+                ico_path = os.path.join(root_path, "harry_potter.ico")
+        self.setIcon(QIcon(ico_path))
         self.icon = self.MessageIcon(QSystemTrayIcon.MessageIcon.NoIcon)
 
     def iconClicked(self, reason):
         "鼠标点击icon传递的信号会带有一个整形的值, 1是表示单击右键, 2是双击, 3是单击左键, 4是用鼠标中键点击"
         if reason == 2 or reason == 3:
             pw = self.parent()
             if pw.isVisible():
                 pw.hide()
             else:
                 pw.show()
 
+    def show_warning_msg(self, text):
+        self.showMessage("警告", text, self.MessageIcon(QSystemTrayIcon.Warning))
+
+    def show_info_msg(self, text):
+        self.showMessage("提示", text, self.MessageIcon(QSystemTrayIcon.Information))
+
     def msgClickEvent(self):
         """
         Ubuntu没有生效,我的树莓派是生效的
         看来是GNOME在消息点击事件上实现
         和大家不太一致导致的
 
         后经测试发现GNOME在点击其他应用的消息时会触发,点击本应用的就不触发..似乎也合理?
```

### Comparing `desktoptools-0.0.1/DesktopTools/args.py` & `desktoptools-0.0.7/DesktopTools/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 parser.add_argument(
     "--threshold", type=float, default=30, help="rest threshold? n /min"
 )
 parser.add_argument(
     "--work_buffer_len", type=int, default=60, help="work T rest buffer lenth. n /s"
 )
 
-args = parser.parse_args()
+args = parser.parse_args(args=[])
 
 KEYBOARD, MOUSE = "keyboard", "mouse"
 
 KEYBOARD_DeviceNo = 1
 MOUSE_DeviceNo = 0
 TICKER_DeviceNo = -1
```

### Comparing `desktoptools-0.0.1/DesktopTools/feather_hotkey/clip_string.py` & `desktoptools-0.0.7/DesktopTools/feather_hotkey/clip_string.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import datetime
 import os
 import random
 import re
 import shutil
 
-from PySide6.QtCore import Qt
-from PySide6.QtGui import QClipboard, QPixmap
+# from PySide6.QtCore import Qt
+from PySide6.QtGui import QClipboard
 
 from ..logger import logger
+from .models import FuncClass
 
 
 def incremental_copy_files(source_path: str, dest_path: str, number: int):
     """
     增量复制文件: 将指定路径下的所有文件(不包括文件夹)随机复制`Number`份存放到指定位置
     """
     file_list = []  # 存储所有文件的路径
@@ -48,15 +49,19 @@
     - 只允许使用以下内置函数和变量
     - 如果出现异常，说明表达式不合法
     """
     # allowed_globals = {'__builtins__': None, 'abs': abs, 'round': round}
     allowed_globals = {"__builtins__": None}
     allowed_locals = {}
     # 执行表达式
-    result = eval(expr, allowed_globals, allowed_locals)
+    result = None
+    try:
+        result = eval(expr, allowed_globals, allowed_locals)
+    except Exception:
+        pass
     return result
 
 
 def data2json(str_data: str) -> str:
     """
     - data 字符串转json字符串(包含格式化)
     - 不做异常处理, 同一在使用处捕获
@@ -80,24 +85,29 @@
     pattern = r"[+-]?(?:(?:\d+\.\d*)|(?:\.\d+)|(?:\d+))(?:[eE][+-]?\d+)?"
     numbers = [float(x) for x in re.findall(pattern, string)]
     return numbers
 
 
 def unixtime_to_datetime_str(unixtime_str):
     list_float = extract_float(unixtime_str)
-    dt = datetime.datetime.fromtimestamp(0)
+    logger.debug(f"unixtime_str: {unixtime_str} - list_float: {list_float}")
+    unixtime = 0
     if list_float:
-        dt = datetime.datetime.fromtimestamp(list_float[0])
+        unixtime = list_float[0]
     else:
         unixtime_str = extract_numbers(unixtime_str)
         if not unixtime_str or not unixtime_str.isdigit():
             return ""
         unixtime = int(unixtime_str)
+    dt_str = ""
+    try:
         dt = datetime.datetime.fromtimestamp(unixtime)
-    dt_str = dt.strftime("%Y-%m-%d %H:%M:%S")
+        dt_str = dt.strftime("%Y-%m-%d %H:%M:%S")
+    except Exception:
+        pass
     return dt_str
 
 
 def modify_import_path(file_path: str) -> str:
     # 将 '\' 转换为 '/'
     file_path = file_path.replace("\\", "/")
     # 查找最后一个 '/' 的索引
@@ -114,68 +124,79 @@
 
 
 class ClipFuncs:
     SplitSign: str = ": "
 
     def __init__(self, clipboard: QClipboard) -> None:
         self.clipboard = clipboard
-        self.dict_registered: dict = {
-            f"clip-连续空格替换为指定符号{self.SplitSign}": self.replace_spaces,
-            "clip-data转为JSON字符串": self.data2json,
-            "clip-unixtime转datetime": self.unixtime_to_datetime_str,
-            "clip-路径转python导入import语句": self.modify_import_path,
-        }
+        self.list_registered_funcclass: list[FuncClass] = [
+            FuncClass(desc="连续空格替换为指定符号", func=self.replace_spaces),
+            FuncClass(desc="data转为JSON字符串", func=self.data2json),
+            FuncClass(desc="unixtime转datetime", func=self.unixtime_to_datetime_str),
+            FuncClass(desc="路径转python导入import语句", func=self.modify_import_path),
+        ]
+
+    def list_all_result(self, text: str) -> list[FuncClass]:
+        """
+        列出所有功能函数的计算结果
+        """
+        list_rst: list[FuncClass] = []
+        for i in self.list_registered_funcclass:
+            if not i.get_result(text):
+                continue
+            list_rst.append(i)
+        return list_rst
 
-    def get_clipboard_text(self):
-        originalText = self.clipboard.text()
-        if originalText:
-            return originalText
-        return ""
+    def set_clipboard(self, content):
+        self.clipboard.setText(content)
 
-    def unixtime_to_datetime_str(self):
-        content = unixtime_to_datetime_str(self.get_clipboard_text() or 0)
+    def unixtime_to_datetime_str(self, text):
+        content = unixtime_to_datetime_str(text or 0)
         if not content:
             return False, "非unix时间"
-        self.clipboard.setText(content)
-        return True, ""
+        # self.set_clipboard(content)
+        return True, content
 
-    def data2json(self):
+    def data2json(self, text):
         """
         将data转为json字符串
         """
-        originalText = self.clipboard.text()
+        originalText = text
+        content = ""
         if originalText:
             try:
                 content = data2json(originalText)
-                self.clipboard.setText(content)
+                # self.set_clipboard(content)
             except Exception as err:
                 logger.error(f"data2json: {err}")
                 return False, str(err)
-        return True, ""
+        return text != content, content
 
-    def replace_spaces(self, target_symbol: str):
+    def replace_spaces(self, text, target_symbol: str = "|"):
         """
         将连续空格替换为|
         多为复制表格数据转Markdown使用
         """
-        originalText = self.clipboard.text()
+        originalText = text
         if originalText:
             content = replace_spaces(originalText, target_symbol)
             logger.debug(f"{originalText} chg2(by: {target_symbol}) {content}")
-            self.clipboard.setText(content)
-        return True, ""
+            # self.set_clipboard(content)
+        return text != content, content
 
-    def modify_import_path(self):
+    def modify_import_path(self, text):
         """
         将文件路径切换成python导入语句
         """
-        file_path: str = self.get_clipboard_text()
+        if ("\\" not in text) and ("/" not in text):
+            return False, ""
+        file_path: str = text
         import_path = modify_import_path(file_path=file_path)
-        self.clipboard.setText(import_path)
-        return True, ""
+        # self.set_clipboard(import_path)
+        return True, import_path
 
 
 if __name__ == "__main__":
     # rst = replace_spaces(
     #     "Hello   world  nihao haha  liuliuliu  niubi \n 1 2 3 4  5", "|"
     # )
     # print(rst)
```

### Comparing `desktoptools-0.0.1/DesktopTools/feather_hotkey/searchbar.ui` & `desktoptools-0.0.7/DesktopTools/feather_hotkey/searchbar.ui`

 * *Files 16% similar despite different names*

#### Comparing `desktoptools-0.0.1/DesktopTools/feather_hotkey/searchbar.ui` & `desktoptools-0.0.7/DesktopTools/feather_hotkey/searchbar.ui`

```diff
@@ -57,29 +57,42 @@
                     <string>确定</string>
                   </property>
                 </widget>
               </item>
             </layout>
           </item>
           <item>
-            <widget class="QListView" name="listView">
-              <property name="enabled">
-                <bool>true</bool>
+            <widget class="QListWidget" name="listWidget">
+              <property name="layoutDirection">
+                <enum>Qt::LeftToRight</enum>
               </property>
               <property name="styleSheet">
                 <string notr="true">background-color: #FFFFFF;
-border-radius: 10px;
+border-radius: 16px;
 border: 2px solid #CCCCCC;
 padding: 20px;
-font-size: 18px;
-font-family: Arial, sans-serif;</string>
+font-size: 20px;
+font-family: Arial, sans-serif;
+line-height: 2.5;
+margin-bottom: 10px;	
+margin: 1px;</string>
               </property>
-              <property name="locale">
-                <locale language="Chinese" country="China"/>
+              <property name="currentRow">
+                <number>0</number>
               </property>
+              <item>
+                <property name="text">
+                  <string>你好</string>
+                </property>
+              </item>
+              <item>
+                <property name="text">
+                  <string>hello</string>
+                </property>
+              </item>
             </widget>
           </item>
         </layout>
       </item>
     </layout>
   </widget>
   <resources/>
```

### Comparing `desktoptools-0.0.1/DesktopTools/feather_hotkey/ui_searchbar.py` & `desktoptools-0.0.7/DesktopTools/feather_hotkey/searchbar_ui.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,140 +1,159 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'searchbar.ui'
-##
-## Created by: Qt User Interface Compiler version 6.4.2
-##
-## WARNING! All changes made in this file will be lost when recompiling UI file!
-################################################################################
-
-from PySide6.QtCore import (
-    QCoreApplication,
-    QDate,
-    QDateTime,
-    QLocale,
-    QMetaObject,
-    QObject,
-    QPoint,
-    QRect,
-    QSize,
-    Qt,
-    QTime,
-    QUrl,
-)
-from PySide6.QtGui import (
-    QBrush,
-    QColor,
-    QConicalGradient,
-    QCursor,
-    QFont,
-    QFontDatabase,
-    QGradient,
-    QIcon,
-    QImage,
-    QKeySequence,
-    QLinearGradient,
-    QPainter,
-    QPalette,
-    QPixmap,
-    QRadialGradient,
-    QTransform,
-)
-from PySide6.QtWidgets import (
-    QApplication,
-    QHBoxLayout,
-    QLineEdit,
-    QListView,
-    QPushButton,
-    QSizePolicy,
-    QVBoxLayout,
-    QWidget,
-)
-
-
-class Ui_SearchBar(object):
-    def setupUi(self, SearchBar):
-        if not SearchBar.objectName():
-            SearchBar.setObjectName("SearchBar")
-        SearchBar.setEnabled(True)
-        SearchBar.resize(701, 280)
-        SearchBar.setStyleSheet(
-            "            background-color: #F9F9F9;\n"
-            "            color: #333333;\n"
-            "            font-size: 16px;\n"
-            "            font-family: Arial, sans-serif;"
-        )
-        self.horizontalLayout_2 = QHBoxLayout(SearchBar)
-        self.horizontalLayout_2.setObjectName("horizontalLayout_2")
-        self.verticalLayout = QVBoxLayout()
-        self.verticalLayout.setObjectName("verticalLayout")
-        self.horizontalLayout_3 = QHBoxLayout()
-        self.horizontalLayout_3.setObjectName("horizontalLayout_3")
-        self.lineEdit = QLineEdit(SearchBar)
-        self.lineEdit.setObjectName("lineEdit")
-        self.lineEdit.setStyleSheet(
-            "            background-color: #FFFFFF;\n"
-            "            border-radius: 40px;\n"
-            "            border: 2px solid #CCCCCC;\n"
-            "            padding: 20px;\n"
-            "            font-size: 18px;\n"
-            "            font-family: Arial, sans-serif;"
-        )
-
-        self.horizontalLayout_3.addWidget(self.lineEdit)
-
-        self.pushButton = QPushButton(SearchBar)
-        self.pushButton.setObjectName("pushButton")
-        self.pushButton.setStyleSheet(
-            "            background-color: #008CBA;\n"
-            "            border-radius: 40px;\n"
-            "            border: none;\n"
-            "            padding: 20px 40px;\n"
-            "            font-size: 18px;\n"
-            "            font-family: Arial, sans-serif;\n"
-            "            color: #FFFFFF;"
-        )
-
-        self.horizontalLayout_3.addWidget(self.pushButton)
-
-        self.verticalLayout.addLayout(self.horizontalLayout_3)
-
-        self.listView = QListView(SearchBar)
-        self.listView.setObjectName("listView")
-        self.listView.setEnabled(True)
-        self.listView.setStyleSheet(
-            "background-color: #FFFFFF;\n"
-            "border-radius: 10px;\n"
-            "border: 2px solid #CCCCCC;\n"
-            "padding: 20px;\n"
-            "font-size: 18px;\n"
-            "font-family: Arial, sans-serif;"
-        )
-        self.listView.setLocale(QLocale(QLocale.Chinese, QLocale.China))
-
-        self.verticalLayout.addWidget(self.listView)
-
-        self.horizontalLayout_2.addLayout(self.verticalLayout)
-
-        self.retranslateUi(SearchBar)
-
-        QMetaObject.connectSlotsByName(SearchBar)
-
-    # setupUi
-
-    def retranslateUi(self, SearchBar):
-        SearchBar.setWindowTitle(
-            QCoreApplication.translate(
-                "SearchBar", "\u5c0f\u547d\u4ee4\u5de5\u5177", None
-            )
-        )
-        self.lineEdit.setPlaceholderText(
-            QCoreApplication.translate(
-                "SearchBar", "\u5f00\u59cb\u8f93\u5165\u547d\u4ee4...", None
-            )
-        )
-        self.pushButton.setText(
-            QCoreApplication.translate("SearchBar", "\u786e\u5b9a", None)
-        )
-
-    # retranslateUi
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'searchbar.ui'
+##
+## Created by: Qt User Interface Compiler version 6.4.2
+##
+## WARNING! All changes made in this file will be lost when recompiling UI file!
+################################################################################
+
+from PySide6.QtCore import (
+    QCoreApplication,
+    QDate,
+    QDateTime,
+    QLocale,
+    QMetaObject,
+    QObject,
+    QPoint,
+    QRect,
+    QSize,
+    Qt,
+    QTime,
+    QUrl,
+)
+from PySide6.QtGui import (
+    QBrush,
+    QColor,
+    QConicalGradient,
+    QCursor,
+    QFont,
+    QFontDatabase,
+    QGradient,
+    QIcon,
+    QImage,
+    QKeySequence,
+    QLinearGradient,
+    QPainter,
+    QPalette,
+    QPixmap,
+    QRadialGradient,
+    QTransform,
+)
+from PySide6.QtWidgets import (
+    QApplication,
+    QHBoxLayout,
+    QLineEdit,
+    QListWidget,
+    QListWidgetItem,
+    QPushButton,
+    QSizePolicy,
+    QVBoxLayout,
+    QWidget,
+)
+
+
+class Ui_SearchBar(object):
+    def setupUi(self, SearchBar):
+        if not SearchBar.objectName():
+            SearchBar.setObjectName("SearchBar")
+        SearchBar.setEnabled(True)
+        SearchBar.resize(701, 280)
+        SearchBar.setStyleSheet(
+            "            background-color: #F9F9F9;\n"
+            "            color: #333333;\n"
+            "            font-size: 16px;\n"
+            "            font-family: Arial, sans-serif;"
+        )
+        self.horizontalLayout_2 = QHBoxLayout(SearchBar)
+        self.horizontalLayout_2.setObjectName("horizontalLayout_2")
+        self.verticalLayout = QVBoxLayout()
+        self.verticalLayout.setObjectName("verticalLayout")
+        self.horizontalLayout_3 = QHBoxLayout()
+        self.horizontalLayout_3.setObjectName("horizontalLayout_3")
+        self.lineEdit = QLineEdit(SearchBar)
+        self.lineEdit.setObjectName("lineEdit")
+        self.lineEdit.setStyleSheet(
+            "            background-color: #FFFFFF;\n"
+            "            border-radius: 40px;\n"
+            "            border: 2px solid #CCCCCC;\n"
+            "            padding: 20px;\n"
+            "            font-size: 18px;\n"
+            "            font-family: Arial, sans-serif;"
+        )
+
+        self.horizontalLayout_3.addWidget(self.lineEdit)
+
+        self.pushButton = QPushButton(SearchBar)
+        self.pushButton.setObjectName("pushButton")
+        self.pushButton.setStyleSheet(
+            "            background-color: #008CBA;\n"
+            "            border-radius: 40px;\n"
+            "            border: none;\n"
+            "            padding: 20px 40px;\n"
+            "            font-size: 18px;\n"
+            "            font-family: Arial, sans-serif;\n"
+            "            color: #FFFFFF;"
+        )
+
+        self.horizontalLayout_3.addWidget(self.pushButton)
+
+        self.verticalLayout.addLayout(self.horizontalLayout_3)
+
+        self.listWidget = QListWidget(SearchBar)
+        QListWidgetItem(self.listWidget)
+        QListWidgetItem(self.listWidget)
+        self.listWidget.setObjectName("listWidget")
+        self.listWidget.setLayoutDirection(Qt.LeftToRight)
+        self.listWidget.setStyleSheet(
+            "background-color: #FFFFFF;\n"
+            "border-radius: 16px;\n"
+            "border: 2px solid #CCCCCC;\n"
+            "padding: 20px;\n"
+            "font-size: 20px;\n"
+            "font-family: Arial, sans-serif;\n"
+            "line-height: 2.5;\n"
+            "margin-bottom: 10px;	\n"
+            "margin: 1px; "
+        )
+
+        self.verticalLayout.addWidget(self.listWidget)
+
+        self.horizontalLayout_2.addLayout(self.verticalLayout)
+
+        self.retranslateUi(SearchBar)
+
+        self.listWidget.setCurrentRow(0)
+
+        QMetaObject.connectSlotsByName(SearchBar)
+
+    # setupUi
+
+    def retranslateUi(self, SearchBar):
+        SearchBar.setWindowTitle(
+            QCoreApplication.translate(
+                "SearchBar", "\u5c0f\u547d\u4ee4\u5de5\u5177", None
+            )
+        )
+        self.lineEdit.setPlaceholderText(
+            QCoreApplication.translate(
+                "SearchBar", "\u5f00\u59cb\u8f93\u5165\u547d\u4ee4...", None
+            )
+        )
+        self.pushButton.setText(
+            QCoreApplication.translate("SearchBar", "\u786e\u5b9a", None)
+        )
+
+        __sortingEnabled = self.listWidget.isSortingEnabled()
+        self.listWidget.setSortingEnabled(False)
+        ___qlistwidgetitem = self.listWidget.item(0)
+        ___qlistwidgetitem.setText(
+            QCoreApplication.translate("SearchBar", "\u4f60\u597d", None)
+        )
+        ___qlistwidgetitem1 = self.listWidget.item(1)
+        ___qlistwidgetitem1.setText(
+            QCoreApplication.translate("SearchBar", "hello", None)
+        )
+        self.listWidget.setSortingEnabled(__sortingEnabled)
+
+    # retranslateUi
```

### Comparing `desktoptools-0.0.1/DesktopTools/feather_timer/data_alchemy/inputs.py` & `desktoptools-0.0.7/DesktopTools/feather_timer/data_alchemy/inputs.py`

 * *Files identical despite different names*

### Comparing `desktoptools-0.0.1/DesktopTools/feather_timer/data_alchemy/models.py` & `desktoptools-0.0.7/DesktopTools/feather_timer/data_alchemy/models.py`

 * *Files identical despite different names*

### Comparing `desktoptools-0.0.1/DesktopTools/feather_timer/data_alchemy/worktimes.py` & `desktoptools-0.0.7/DesktopTools/feather_timer/data_alchemy/worktimes.py`

 * *Files identical despite different names*

### Comparing `desktoptools-0.0.1/DesktopTools/feather_timer/halahayawa.py` & `desktoptools-0.0.7/DesktopTools/feather_timer/halahayawa.py`

 * *Files 5% similar despite different names*

```diff
@@ -142,20 +142,24 @@
     def initUI(self):
         # self.tooltip()
         # self.setGeometry(300, 300, 300, 220)
         self.center()
         self.setWindowTitle("Pendulum")
 
         # 设置图标
-        app_path = os.path.dirname(os.path.abspath(__file__))
-        root_path, feather_fname = os.path.split(app_path)
-        if feather_fname.startswith("feather"):
-            ico_path = os.path.join(root_path, "harry_potter.ico")
-            self.setWindowIcon(QIcon(ico_path))
-            # self.setWindowIcon(QIcon("harry_potter.ico"))
+        ico_path = ""
+        if os.path.exists("harry_potter.ico"):
+            ico_path = "harry_potter.ico"
+        else:
+            app_path = os.path.dirname(os.path.abspath(__file__))
+            root_path, feather_fname = os.path.split(app_path)
+            if feather_fname.startswith("feather"):
+                ico_path = os.path.join(root_path, "harry_potter.ico")
+        self.setWindowIcon(QIcon(ico_path))
+        # self.setWindowIcon(QIcon("harry_potter.ico"))
 
         self.vbox, self.hbox, self.hbox2, self.hbox3 = self.initBoxLayout()
         self.initMainWidgets()
 
         self.hbox.addWidget(self.dictLabels["timeNow"])
         self.hbox.addWidget(self.dictLabels["vtimeNow"])
         self.hbox2.addWidget(self.dictLabels["workAll"])
@@ -164,15 +168,15 @@
         self.hbox3.addWidget(self.dictButtons["abc"])
 
         self.vbox.addLayout(self.hbox)
         self.vbox.addLayout(self.hbox2)
         self.vbox.addLayout(self.hbox3)
         self.setLayout(self.vbox)
 
-        self.show()
+        # self.show()
 
     def initBoxLayout(self):
         vbox = QVBoxLayout()
         hbox = QHBoxLayout()
         hbox2 = QHBoxLayout()
         hbox3 = QHBoxLayout()
         return vbox, hbox, hbox2, hbox3
@@ -234,13 +238,22 @@
         size = self.geometry()
         screen = self.screen
         self.move(
             (screen.width() - size.width()) / 2, (screen.height() - size.height()) / 2
         )
         # 此方法不警告了,不过多屏居中会..居中在所有屏幕总和的中间
 
+    def closeEvent(self, event):
+        """
+        点击x关闭窗口时
+        如果不ignore掉该信号的话会导致主进程退出
+        """
+        self.hide()
+        event.ignore()
+
 
 if __name__ == "__main__":
+    """这段应该不能正常运行了, 有空儿再琢磨下怎么单模块测试"""
     app = QApplication(sys.argv)
     screen = app.primaryScreen().geometry()
     ex = WinHowLongHadYouWork(screen, app=app)
     sys.exit(app.exec())
```

### Comparing `desktoptools-0.0.1/DesktopTools/feather_timer/input_counter.py` & `desktoptools-0.0.7/DesktopTools/feather_timer/input_counter.py`

 * *Files identical despite different names*

### Comparing `desktoptools-0.0.1/DesktopTools/feather_timer/monitor.py` & `desktoptools-0.0.7/DesktopTools/feather_timer/monitor.py`

 * *Files identical despite different names*

### Comparing `desktoptools-0.0.1/DesktopTools/harry_potter.ico` & `desktoptools-0.0.7/DesktopTools/harry_potter.ico`

 * *Files identical despite different names*

### Comparing `desktoptools-0.0.1/DesktopTools/harry_potter.png` & `desktoptools-0.0.7/DesktopTools/harry_potter.png`

 * *Files identical despite different names*

### Comparing `desktoptools-0.0.1/DesktopTools/logger.py` & `desktoptools-0.0.7/DesktopTools/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import sys
-
 from loguru import logger
 
 from .args import args
 
 if not args.debug:
     logger.remove(handler_id=None)
```

### Comparing `desktoptools-0.0.1/DesktopTools/tools.py` & `desktoptools-0.0.7/DesktopTools/tools.py`

 * *Files identical despite different names*

### Comparing `desktoptools-0.0.1/DesktopTools/windows_main.py` & `desktoptools-0.0.7/DesktopTools/windows_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,22 @@
     """
 
     def __init__(self, screen=False, app=None):
         super().__init__(None)
 
         self.screen = screen
         self.tray = TrayIcon(self)
-        self.win_searchbar = WinSearchBar(app)
+
         self.win_timer = WinHowLongHadYouWork(screen, self.tray)
+        dict_win_feather = {"工作时长": self.win_timer}
+        self.win_searchbar = WinSearchBar(app, self.tray, dict_win_feather)
 
         self.initSearchBar()
 
-        self.win_timer.show()
+        # self.win_timer.show()
         self.tray.show()
 
     def initSearchBar(self):
         """
         使用线程初始化SearchBar, 在线程中绑定热键
         """
         thread_hotkey = SignalHotKey()
```

### Comparing `desktoptools-0.0.1/LICENSE` & `desktoptools-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `desktoptools-0.0.1/pyproject.toml` & `desktoptools-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "DesktopTools"
-version = "0.0.1"
-description = "Python Http File Server: Added file upload function to `http.server`"
+version = "0.0.7"
+description = "A desktop tool that includes some useful scripts."
 authors = ["ianvzs <ianvzs@outlook.com>", "saint <ysudqfs@163.com>"]
 readme = "README.md"
 repository = "https://github.com/IanVzs/Halahayawa"
 license = "MIT"
 packages = [
     { include = "DesktopTools" },
     { include = "DesktopTools/app" },
@@ -20,14 +20,15 @@
 python = ">=3.7,<3.12"
 PySide6 = { version = "^6.0.0", optional = true }
 pynput = "^1.7.6"
 loguru = "^0.6.0"
 SQLAlchemy = "^2.0.0"
 yapf = "^0.32.0"
 wheel = "^0.40.0"
+pydantic = "^1.10.7"
 
 
 [tool.poetry.extras]
 ui = ["PySide6"]
 
 
 [tool.poetry.dev-dependencies]
```

