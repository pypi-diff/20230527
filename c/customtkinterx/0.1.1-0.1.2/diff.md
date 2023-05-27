# Comparing `tmp/customtkinterx-0.1.1.tar.gz` & `tmp/customtkinterx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkinterx-0.1.1.tar", max compression
+gzip compressed data, was "customtkinterx-0.1.2.tar", max compression
```

## Comparing `customtkinterx-0.1.1.tar` & `customtkinterx-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      251 2023-05-27 08:34:56.407692 customtkinterx-0.1.1/customtkinterx/__init__.py
--rw-r--r--   0        0        0     3775 2023-05-27 09:25:30.265070 customtkinterx-0.1.1/customtkinterx/CTkCustom.py
--rw-r--r--   0        0        0     5306 2023-05-27 08:36:14.109297 customtkinterx-0.1.1/customtkinterx/CTkFluentTheme.py
--rw-r--r--   0        0        0     4686 2023-05-27 08:31:22.732978 customtkinterx-0.1.1/customtkinterx/Fluent.json
--rw-r--r--   0        0        0      343 2023-05-27 09:47:17.417981 customtkinterx-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1048 2023-05-27 09:39:01.342825 customtkinterx-0.1.1/README.md
--rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 customtkinterx-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      251 2023-05-27 08:34:56.407692 customtkinterx-0.1.2/customtkinterx/__init__.py
+-rw-r--r--   0        0        0     3776 2023-05-27 10:59:38.605996 customtkinterx-0.1.2/customtkinterx/CTkCustom.py
+-rw-r--r--   0        0        0     5306 2023-05-27 08:36:14.109297 customtkinterx-0.1.2/customtkinterx/CTkFluentTheme.py
+-rw-r--r--   0        0        0     1204 2023-05-27 11:45:12.773768 customtkinterx-0.1.2/customtkinterx/CTkListBox.py
+-rw-r--r--   0        0        0     4686 2023-05-27 08:31:22.732978 customtkinterx-0.1.2/customtkinterx/Fluent.json
+-rw-r--r--   0        0        0      343 2023-05-27 11:00:26.467432 customtkinterx-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1048 2023-05-27 09:39:01.342825 customtkinterx-0.1.2/README.md
+-rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 customtkinterx-0.1.2/PKG-INFO
```

### Comparing `customtkinterx-0.1.1/customtkinterx/CTkCustom.py` & `customtkinterx-0.1.2/customtkinterx/CTkCustom.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,27 +25,27 @@
             res = windll.user32.SetWindowLongW(hwnd, GWL_EXSTYLE, style)
         except:
             self.wm_attributes("-topmost", True)
 
         self.minsize(150, 180)
 
         self.__frame_border = CTkFrame(self, border_width=1)
-        self.__frame_border.pack(fill="both", expand=True, padx=2, pady=2)
+        self.__frame_border.pack(fill="both", expand=True, padx=0, pady=0)
 
         self.__frame_title = CTkFrame(self.__frame_border, border_width=0, corner_radius=2)
         self.__frame_title.pack(fill="x", side="top", padx=2, pady=2)
         self.bind_move(self.__frame_title)
 
         self.__label_title = CTkLabel(self.__frame_title, text=self.wm_title())
         self.__label_title.pack(side="left", anchor="w", padx=10, pady=5)
         self.bind_move(self.__label_title)
 
         self.maximized = False
 
-        self.__button_close = CTkButton(self.__frame_title, text="✕", width=30, height=30, command=lambda: self.quit())
+        self.__button_close = CTkButton(self.__frame_title, text="✕", width=30, height=30, command=lambda: self.destroy())
         self.__button_close.pack(side="right", anchor="e", padx=5, pady=5)
 
         self.__button_minimize = CTkButton(self.__frame_title, text="–", width=30, height=30, command=lambda: self.minimize())
         self.__button_minimize.pack(side="right", anchor="e", padx=5, pady=5)
 
         self.x, self.y = 0, 0
 
@@ -88,16 +88,16 @@
 
     def _click(self, event):
         self.x, self.y = event.x, event.y
 
     def _move(self, event):
         new_x = (event.x - self.x) + self.winfo_x()
         new_y = (event.y - self.y) + self.winfo_y()
-        if new_y <= -2:
-            new_y = -2
+        if new_y <= 0:
+            new_y = 0
         s = f"+{new_x}+{new_y}"
         self.geometry(s)
 
 
 if __name__ == '__main__':
     root = CTkCustom()
     root.title("helloworld")
```

### Comparing `customtkinterx-0.1.1/customtkinterx/CTkFluentTheme.py` & `customtkinterx-0.1.2/customtkinterx/CTkFluentTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.1.1/customtkinterx/Fluent.json` & `customtkinterx-0.1.2/customtkinterx/Fluent.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.1.1/README.md` & `customtkinterx-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.1.1/PKG-INFO` & `customtkinterx-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customtkinterx
-Version: 0.1.1
+Version: 0.1.2
 Summary: extra widgets for customtkinter
 Author: XiangQinxi
 Author-email: XiangQinxi@outlook.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

