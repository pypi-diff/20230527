# Comparing `tmp/mwxlib-0.83.9-py3-none-any.whl.zip` & `tmp/mwxlib-0.84.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 162157 bytes, number of entries: 22
+Zip file size: 162268 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2520 b- defN 23-May-02 16:40 mwx/__init__.py
 -rw-rw-rw-  2.0 fat    43445 b- defN 23-May-02 17:15 mwx/controls.py
--rw-rw-rw-  2.0 fat    73386 b- defN 23-May-24 00:46 mwx/framework.py
--rw-rw-rw-  2.0 fat    69520 b- defN 23-May-24 12:52 mwx/graphman.py
+-rw-rw-rw-  2.0 fat    73540 b- defN 23-May-27 03:59 mwx/framework.py
+-rw-rw-rw-  2.0 fat    69520 b- defN 23-May-25 03:20 mwx/graphman.py
 -rw-rw-rw-  2.0 fat    46248 b- defN 23-Feb-21 08:49 mwx/images.py
 -rw-rw-rw-  2.0 fat    36017 b- defN 23-May-17 04:56 mwx/matplot2.py
 -rw-rw-rw-  2.0 fat    68253 b- defN 23-May-17 11:19 mwx/matplot2g.py
 -rw-rw-rw-  2.0 fat    27606 b- defN 23-Apr-27 09:45 mwx/matplot2lg.py
 -rw-rw-rw-  2.0 fat     6878 b- defN 23-Feb-21 08:50 mwx/mgplt.py
--rw-rw-rw-  2.0 fat   138542 b- defN 23-May-24 00:34 mwx/nutshell.py
--rw-rw-rw-  2.0 fat    37403 b- defN 23-May-24 12:45 mwx/utilus.py
+-rw-rw-rw-  2.0 fat   138667 b- defN 23-May-27 04:10 mwx/nutshell.py
+-rw-rw-rw-  2.0 fat    37403 b- defN 23-May-25 03:20 mwx/utilus.py
 -rw-rw-rw-  2.0 fat    11343 b- defN 23-May-16 07:42 mwx/wxmon.py
 -rw-rw-rw-  2.0 fat    19367 b- defN 23-May-16 07:42 mwx/wxpdb.py
 -rw-rw-rw-  2.0 fat     5254 b- defN 23-May-16 07:42 mwx/wxwil.py
 -rw-rw-rw-  2.0 fat     7424 b- defN 23-May-16 07:42 mwx/wxwit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-23 14:06 mwx/py/__init__.py
 -rw-rw-rw-  2.0 fat    16794 b- defN 23-Apr-27 09:45 mwx/py/filling.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-24 12:57 mwxlib-0.83.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-May-24 12:57 mwxlib-0.83.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-24 12:57 mwxlib-0.83.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-May-24 12:57 mwxlib-0.83.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-May-24 12:57 mwxlib-0.83.9.dist-info/RECORD
-22 files, 614689 bytes uncompressed, 159655 bytes compressed:  74.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-27 16:26 mwxlib-0.84.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-May-27 16:26 mwxlib-0.84.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-27 16:26 mwxlib-0.84.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-May-27 16:26 mwxlib-0.84.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-May-27 16:26 mwxlib-0.84.0.dist-info/RECORD
+22 files, 614968 bytes uncompressed, 159766 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.83.9.dist-info/LICENSE
+Filename: mwxlib-0.84.0.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.83.9.dist-info/METADATA
+Filename: mwxlib-0.84.0.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.83.9.dist-info/WHEEL
+Filename: mwxlib-0.84.0.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.83.9.dist-info/top_level.txt
+Filename: mwxlib-0.84.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.83.9.dist-info/RECORD
+Filename: mwxlib-0.84.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mwx/framework.py

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 """mwxlib framework
 
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 """
-__version__ = "0.83.9"
+__version__ = "0.84.0"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
@@ -118,18 +118,21 @@
     wx.WXK_TAB                  : 'tab',
     wx.WXK_UP                   : 'up',
     wx.WXK_WINDOWS_LEFT         : 'Lwin',
     wx.WXK_WINDOWS_MENU         : 'appskey',
     wx.WXK_WINDOWS_RIGHT        : 'Rwin',
 }
 
-## def speckey_state(key):
-##     for k, v in _speckeys.items():
-##         if v == key:
-##             return wx.GetKeyState(k) # cf. wx.GetMouseState
+def speckey_state(key):
+    """Returns GetKeyState for abbreviation key:str."""
+    try:
+        return wx.GetKeyState(_speckeys_wxkmap[key])
+    except KeyError:
+        pass
+_speckeys_wxkmap = dict((v, k) for k, v in _speckeys.items())
 
 
 def hotkey(evt):
     """Interpret evt.KeyCode as hotkey:str and overwrite evt.key.
     The modifiers are arranged in the same order as matplotlib as
     [LR]win + ctrl + alt(meta) + shift.
     """
@@ -1439,33 +1442,31 @@
         self.debugger.send_input('\n') # terminates the reader
         shell = self.debugger.interactive_shell # reset interp locals
         del shell.locals
         del shell.globals
         self.indicator.Value = 1
         self.message("Quit")
     
-    def load(self, obj, show=True, focus=False):
+    def load(self, filename, lineno=0, show=True, focus=False):
         """Load file @where the object is defined.
         
         Args:
-            obj     : target object.
-            focus   : Set the focus if the window is displayed.
+            filename : target filename or object.
+            focus    : Set the focus if the window is displayed.
         """
-        if not isinstance(obj, str):
-            obj = where(obj)
-        if obj is None:
-            return False
-        
-        m = re.match("(.*?):([0-9]+)", obj)
-        if m:
-            filename, ln = m.groups()
-            lineno = int(ln)
-        else:
-            filename = obj
-            lineno = 0
+        if not isinstance(filename, str):
+            filename = where(filename)
+            if filename is None:
+                return False
+        ## Support <'filename:lineno'>
+        if not lineno:
+            m = re.match("(.*?):([0-9]+)", filename)
+            if m:
+                filename, ln = m.groups()
+                lineno = int(ln)
         book = next((x for x in self.get_all_pages(type(self.Log))
                              if x.find_buffer(filename)), self.Log)
         self.popup_window(book, show, focus)
         return book.load_file(filename, lineno)
     
     def info(self, obj):
         self.rootshell.info(obj)
```

## mwx/nutshell.py

```diff
@@ -516,16 +516,17 @@
         """Retrieve a range of text.
         
         The range must be given as 0 <= start:end <= TextLength,
         otherwise it will be modified to be in [0:TextLength].
         """
         if start > end:
             start, end = end, start
-        return self.GetTextRange(max(start, 0),
-                                 min(end, self.TextLength))
+        p = max(start, 0)
+        q = min(end, self.TextLength)
+        return self.GetTextRange(p, q)
     
     anchor = property(
         lambda self: self.GetAnchor(),
         lambda self,v: self.SetAnchor(v))
     
     cpos = property(
         lambda self: self.GetCurrentPos(),
@@ -1047,16 +1048,15 @@
             self.goto_char(p)
             self.goto_char(self.bol)
             self.mark = self.cpos
             self.EnsureVisible(self.cline)
             yield err
     
     def grep(self, pattern, flags=re.M):
-        text = self.GetTextRange(0, self.TextLength)
-        yield from re.finditer(pattern, text, flags)
+        yield from re.finditer(pattern, self.Text, flags)
     
     def search_text(self, text):
         """Yields raw-positions where `text` is found."""
         word = text.encode()
         raw = self.TextRaw
         pos = -1
         while 1:
@@ -1333,15 +1333,14 @@
         p = self.cpos
         self.skip_chars_backward(' \t')
         self.Replace(max(self.cpos, self.bol), p, '')
     
     @editable
     def kill_line(self):
         p = self.eol
-        text, lp = self.CurLine
         if p == self.cpos:
             if self.get_char(p) == '\r': p += 1
             if self.get_char(p) == '\n': p += 1
         self.Replace(self.cpos, p, '')
     
     @editable
     def backward_kill_line(self):
@@ -1564,22 +1563,24 @@
         if evt.Updated & (stc.STC_UPDATE_SELECTION | stc.STC_UPDATE_CONTENT):
             self.trace_position()
             if evt.Updated & stc.STC_UPDATE_CONTENT:
                 self.handler('buffer_modified', self)
         evt.Skip()
     
     def OnIndicatorClick(self, evt):
-        if self.SelectedText:
+        if self.SelectedText or not wx.GetKeyState(wx.WXK_CONTROL):
+            ## Processing text selection, dragging, or dragging+
             evt.Skip()
             return
         pos = evt.Position
         if self.IndicatorValueAt(2, pos):
             p = self.IndicatorStart(2, pos)
             q = self.IndicatorEnd(2, pos)
             text = self.GetTextRange(p, q).strip()
+            self.message("URL {!r}".format(text))
             ## Note: Do postcall a confirmation dialog.
             wx.CallAfter(self.parent.load_url, text)
     
     def on_modified(self, buf):
         """Called when the buffer is modified."""
         self.SetIndicatorCurrent(2)
         self.IndicatorClearRange(0, self.TextLength)
@@ -1962,20 +1963,20 @@
     ## --------------------------------
     wildcards = [
         "PY files (*.py)|*.py",
         "ALL files (*.*)|*.*",
     ]
     
     def load_url(self, url, lineno=0):
+        surl = re.sub(r"(https?://.+?)/(.+)/(.+)", r"\1 ... \3", url)
         import requests
         if wx.MessageBox( # Confirm URL load.
                 "You are loading URL contents.\n\n"
-               f"{url!r}\n"
                 "Continue loading?",
-                "Load URL",
+                "Load {!r}".format(surl),
                 style=wx.YES_NO|wx.ICON_INFORMATION) != wx.YES:
             self.post_message("The load has been canceled.")
             return None
         try:
             res = requests.get(url)
         except Exception as e:
             self.post_message("Failed to load URL: {}".format(e))
```

## Comparing `mwxlib-0.83.9.dist-info/LICENSE` & `mwxlib-0.84.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.83.9.dist-info/METADATA` & `mwxlib-0.84.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.83.9
+Version: 0.84.0
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mwxlib-0.83.9.dist-info/RECORD` & `mwxlib-0.84.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 mwx/__init__.py,sha256=bSRdncjfSCKycMFQVnagOi9R2vUCC5snGkjea7jqPgU,2520
 mwx/controls.py,sha256=7hnSimA3bKDgTct29l6Hqpq7BCKqCeOjZJ6JQ1xjh7I,43445
-mwx/framework.py,sha256=LBSHrpP5cfNHsEVjXLc-MtrDFutRkFoHoHfkvYf4YYQ,73386
+mwx/framework.py,sha256=0-TskOOmOfvwyJSbY54eTSvp9mnyVsO5PesbiVxy4ys,73540
 mwx/graphman.py,sha256=v11sec3cS5Od__pmWecCi_ivJe65wvr-DzYYnL2Lwb0,69520
 mwx/images.py,sha256=9e8X7OpJ6Z3fF3ez17P_qk2D1NMO10-lN8TCtulAqT0,46248
 mwx/matplot2.py,sha256=W_FpY0S33crCAh7N9YTXo-jgYzj8uL9gqXkekfQo7Pk,36017
 mwx/matplot2g.py,sha256=cBuLMnQt3XSKQL9io0XJb_v8Lv0pO9hm0IMjVIERtu4,68253
 mwx/matplot2lg.py,sha256=h_aFij_7ksG2DXuYCaGmjtlcl122vZnwbMTv21Mprcg,27606
 mwx/mgplt.py,sha256=49_wpFZUEKErQmtobqrlNKDjWlAsdLft-izlqSyGPD0,6878
-mwx/nutshell.py,sha256=UFGa7QTDrFRpQlaY2sDXzJudnfP3bAb1KzTquZnb9sI,138542
+mwx/nutshell.py,sha256=Ca8cCd5oG1N4-KfjKSs4vpX1-vq7Xz2acMjrwIH0A9w,138667
 mwx/utilus.py,sha256=KaYBW7X9AY172bYumKewHenz5uIq4Pzk1GRPzlsexec,37403
 mwx/wxmon.py,sha256=hEXto7dD5JunPf-iv2hhcwTIILLkNPlcl6wRt20_Wqc,11343
 mwx/wxpdb.py,sha256=M_xxXzIYhAwO1IHXVkjIC4Y2JCCCGLdgPL5R4bRtp04,19367
 mwx/wxwil.py,sha256=DPXXx4OdEzvHr-_jxz9J29Ozufmb6Vr7rXVkG_LKQd0,5254
 mwx/wxwit.py,sha256=UG361QTUheO_hlSIRgkprrGUYh0IzHB8ZqOoJeeMzUs,7424
 mwx/py/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mwx/py/filling.py,sha256=f6KMBcBv7gwrl6qmJYLTL-O0Z47bWNAdTCZtUZIo8vM,16794
-mwxlib-0.83.9.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
-mwxlib-0.83.9.dist-info/METADATA,sha256=2RNsOmrIZpl6KTPyepLd7IbS4efpizB5m4ndmsrti94,1893
-mwxlib-0.83.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mwxlib-0.83.9.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
-mwxlib-0.83.9.dist-info/RECORD,,
+mwxlib-0.84.0.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
+mwxlib-0.84.0.dist-info/METADATA,sha256=pZ-EhFlfc44CSwg1OfBcifxpZ-K-Y-vP7SUIHmkdydQ,1893
+mwxlib-0.84.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mwxlib-0.84.0.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
+mwxlib-0.84.0.dist-info/RECORD,,
```

