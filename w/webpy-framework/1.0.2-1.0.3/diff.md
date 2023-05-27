# Comparing `tmp/webpy-framework-1.0.2.tar.gz` & `tmp/webpy-framework-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpy-framework-1.0.2.tar", last modified: Fri May 26 17:57:31 2023, max compression
+gzip compressed data, was "webpy-framework-1.0.3.tar", last modified: Sat May 27 01:12:43 2023, max compression
```

## Comparing `webpy-framework-1.0.2.tar` & `webpy-framework-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 17:57:31.297686 webpy-framework-1.0.2/
--rw-rw-rw-   0        0        0     1090 2023-05-26 17:17:20.000000 webpy-framework-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     6100 2023-05-26 17:57:31.296679 webpy-framework-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4221 2023-05-26 17:45:42.000000 webpy-framework-1.0.2/README.md
--rw-rw-rw-   0        0        0      998 2023-05-26 17:57:08.000000 webpy-framework-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 17:57:31.297686 webpy-framework-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 17:57:31.280959 webpy-framework-1.0.2/webpy/
--rw-rw-rw-   0        0        0     1968 2023-03-17 14:31:38.000000 webpy-framework-1.0.2/webpy/__init__.py
--rw-rw-rw-   0        0        0     6647 2023-05-26 17:56:50.000000 webpy-framework-1.0.2/webpy/__main__.py
--rw-rw-rw-   0        0        0     1722 2023-05-26 17:08:09.000000 webpy-framework-1.0.2/webpy/fs_routes.py
--rw-rw-rw-   0        0        0       50 2023-04-23 19:16:48.000000 webpy-framework-1.0.2/webpy/pysite_semantic_tags.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:57:31.295470 webpy-framework-1.0.2/webpy_framework.egg-info/
--rw-rw-rw-   0        0        0     6100 2023-05-26 17:57:31.000000 webpy-framework-1.0.2/webpy_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-05-26 17:57:31.000000 webpy-framework-1.0.2/webpy_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 17:57:31.000000 webpy-framework-1.0.2/webpy_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-26 17:57:31.000000 webpy-framework-1.0.2/webpy_framework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      142 2023-05-26 17:57:31.000000 webpy-framework-1.0.2/webpy_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-26 17:57:31.000000 webpy-framework-1.0.2/webpy_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 01:12:43.566161 webpy-framework-1.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-05-26 17:17:20.000000 webpy-framework-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6406 2023-05-27 01:12:43.564706 webpy-framework-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4527 2023-05-26 18:08:51.000000 webpy-framework-1.0.3/README.md
+-rw-rw-rw-   0        0        0     1019 2023-05-27 01:12:24.000000 webpy-framework-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 01:12:43.566161 webpy-framework-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 01:12:43.536880 webpy-framework-1.0.3/webpy/
+-rw-rw-rw-   0        0        0     1968 2023-03-17 14:31:38.000000 webpy-framework-1.0.3/webpy/__init__.py
+-rw-rw-rw-   0        0        0     7226 2023-05-27 01:11:58.000000 webpy-framework-1.0.3/webpy/__main__.py
+-rw-rw-rw-   0        0        0     1722 2023-05-27 00:55:01.000000 webpy-framework-1.0.3/webpy/fs_routes.py
+-rw-rw-rw-   0        0        0       50 2023-05-26 18:07:53.000000 webpy-framework-1.0.3/webpy/pysite_semantic_tags.py
+drwxrwxrwx   0        0        0        0 2023-05-27 01:12:43.562333 webpy-framework-1.0.3/webpy_framework.egg-info/
+-rw-rw-rw-   0        0        0     6406 2023-05-27 01:12:43.000000 webpy-framework-1.0.3/webpy_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-05-27 01:12:43.000000 webpy-framework-1.0.3/webpy_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 01:12:43.000000 webpy-framework-1.0.3/webpy_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-27 01:12:43.000000 webpy-framework-1.0.3/webpy_framework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      158 2023-05-27 01:12:43.000000 webpy-framework-1.0.3/webpy_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-27 01:12:43.000000 webpy-framework-1.0.3/webpy_framework.egg-info/top_level.txt
```

### Comparing `webpy-framework-1.0.2/LICENSE` & `webpy-framework-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.0.2/PKG-INFO` & `webpy-framework-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 1.0.2
+Version: 1.0.3
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -70,15 +70,15 @@
     js/
       index.js
 
   app.py
   config.json
 ```
 
-The `app.py` file should contain some boilerplate code. You can use the `app` object just like a normal Flask object!. App configurations should be done inside the `webpy_setup` function. Route functions can still be created. The `config.json` file in the same directory as the `app.py` file configures how WebPy will run your app. It takes any arguments that are valid to pass to `app.run()`
+The `app.py` file should contain some boilerplate code. You can use the `app` object just like a normal Flask object! App configurations should be done inside the `webpy_setup` function. Route functions can still be created. The `config.json` file in the same directory as the `app.py` file configures how WebPy will run your app. It takes any arguments that are valid to pass to `app.run()`.
 
 
 Under `root/`, you can use `index.py` and `index.html` files to create filesystem-based webpage routes. If you use an `index.py` file, WebPy will call the `handler` function and pass the app as an argument. If you use `index.html`, WebPy will just return that HTML file to the requester. Each filesystem route has a `config.json` file. In this file, you can pass any keyword arguments that would be valid to pass to `app.route()`.
 
 Let's create a new page at `http://127.0.0.1:5000/hello`. To do this, we can create a new folder called `hello/` under the `root/` folder. Cd into the `root/` directory and type `webpy route hello`. WebPy will automatically create the `hello/` directory for you.
 
 ```
@@ -86,15 +86,15 @@
   hello/
     index.py
     config.json
 
   ...
 ```
 
-Since we only want this route to be a simple HTML page, we can delete `index.py` and replace it with `index.html`
+Since we only want this route to be a simple HTML page, we can delete `index.py` and replace it with an `index.html` file.
 
 `index.html`
 ```html
 <!DOCTYPE html>
 <html>
 	<head>
 		<link rel="stylesheet" href="/static/css/index.css"/>
@@ -103,10 +103,17 @@
 		<h1 id="heading">Hello, World!</h1>
 	</body>
 </html>
 ```
 
 Now, we can run our app using `webpy run`. Notice that when visiting `http://127.0.0.1:5000/hello`, the CSS that we linked from the `static/` folder is included.
 
-If you want to make your app a little more compact, you can use `webpy build`. This will compile all of your Python and HTML into a single minifed file, `build.py`, which can be run like a normal Python script. However, the the `html/` and `static/` directories are not packaged into the build file, so these must still be present to run `build.py`. When using `webpy run`, changes in the files under `root/` and changes in files under `static/` are guaranteed to be reflected in the app without having to restart it, but if the app is being run from a `build.py`, changes in HTML, Python, and config files under `root/` will not be reflected.
+If you want to make your app a little more compact, you can use `webpy build`. This will compile all of your Python and HTML into a single minifed file, `build.py`, which can be run like a normal Python script. However, the the `html/` and `static/` directories are not packaged into the build file, so these must still be present to run `build.py`. When using `webpy run` to run the app, changes in the files under `root/` and changes in files under `static/` are guaranteed to be reflected in the app without having to restart it, but if the app is being run from a `build.py` file, changes in HTML, Python, and config files under `root/` will not be reflected.
 
-[PyX](https://github.com/User0332/pyx) can also be integrated into WebPy apps by changing Python files to `.pyx` files. These files can be compiled to Python files using `webpy buildpyx`, which is automatically run by the `webpy build`, `webpy compile`, and `webpy run` commands. WebPy comes with PySite/PyX as a dependency.
+[PyX](https://github.com/User0332/pyx) can also be integrated into WebPy apps by changing Python files to `.pyx` files. These files can be compiled to Python files using `webpy buildpyx`, which is automatically run by the `webpy build`, `webpy compile`, and `webpy run` commands. WebPy comes with PySite/PyX as a dependency. Note that one must still import PySite HTML tags in every file that PyX is used, as shown below:
+```py
+from webpy.pysite_semantic_tags import * # recommended
+
+### OR
+
+from pysite.tags import * # also works, but doesn't filter out unnecessary classes such as Element
+```
```

### Comparing `webpy-framework-1.0.2/README.md` & `webpy-framework-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -100,32 +100,32 @@
 00000630: 0d0a 0d0a 5468 6520 6061 7070 2e70 7960  ....The `app.py`
 00000640: 2066 696c 6520 7368 6f75 6c64 2063 6f6e   file should con
 00000650: 7461 696e 2073 6f6d 6520 626f 696c 6572  tain some boiler
 00000660: 706c 6174 6520 636f 6465 2e20 596f 7520  plate code. You 
 00000670: 6361 6e20 7573 6520 7468 6520 6061 7070  can use the `app
 00000680: 6020 6f62 6a65 6374 206a 7573 7420 6c69  ` object just li
 00000690: 6b65 2061 206e 6f72 6d61 6c20 466c 6173  ke a normal Flas
-000006a0: 6b20 6f62 6a65 6374 212e 2041 7070 2063  k object!. App c
-000006b0: 6f6e 6669 6775 7261 7469 6f6e 7320 7368  onfigurations sh
-000006c0: 6f75 6c64 2062 6520 646f 6e65 2069 6e73  ould be done ins
-000006d0: 6964 6520 7468 6520 6077 6562 7079 5f73  ide the `webpy_s
-000006e0: 6574 7570 6020 6675 6e63 7469 6f6e 2e20  etup` function. 
-000006f0: 526f 7574 6520 6675 6e63 7469 6f6e 7320  Route functions 
-00000700: 6361 6e20 7374 696c 6c20 6265 2063 7265  can still be cre
-00000710: 6174 6564 2e20 5468 6520 6063 6f6e 6669  ated. The `confi
-00000720: 672e 6a73 6f6e 6020 6669 6c65 2069 6e20  g.json` file in 
-00000730: 7468 6520 7361 6d65 2064 6972 6563 746f  the same directo
-00000740: 7279 2061 7320 7468 6520 6061 7070 2e70  ry as the `app.p
-00000750: 7960 2066 696c 6520 636f 6e66 6967 7572  y` file configur
-00000760: 6573 2068 6f77 2057 6562 5079 2077 696c  es how WebPy wil
-00000770: 6c20 7275 6e20 796f 7572 2061 7070 2e20  l run your app. 
-00000780: 4974 2074 616b 6573 2061 6e79 2061 7267  It takes any arg
-00000790: 756d 656e 7473 2074 6861 7420 6172 6520  uments that are 
-000007a0: 7661 6c69 6420 746f 2070 6173 7320 746f  valid to pass to
-000007b0: 2060 6170 702e 7275 6e28 2960 0d0a 0d0a   `app.run()`....
+000006a0: 6b20 6f62 6a65 6374 2120 4170 7020 636f  k object! App co
+000006b0: 6e66 6967 7572 6174 696f 6e73 2073 686f  nfigurations sho
+000006c0: 756c 6420 6265 2064 6f6e 6520 696e 7369  uld be done insi
+000006d0: 6465 2074 6865 2060 7765 6270 795f 7365  de the `webpy_se
+000006e0: 7475 7060 2066 756e 6374 696f 6e2e 2052  tup` function. R
+000006f0: 6f75 7465 2066 756e 6374 696f 6e73 2063  oute functions c
+00000700: 616e 2073 7469 6c6c 2062 6520 6372 6561  an still be crea
+00000710: 7465 642e 2054 6865 2060 636f 6e66 6967  ted. The `config
+00000720: 2e6a 736f 6e60 2066 696c 6520 696e 2074  .json` file in t
+00000730: 6865 2073 616d 6520 6469 7265 6374 6f72  he same director
+00000740: 7920 6173 2074 6865 2060 6170 702e 7079  y as the `app.py
+00000750: 6020 6669 6c65 2063 6f6e 6669 6775 7265  ` file configure
+00000760: 7320 686f 7720 5765 6250 7920 7769 6c6c  s how WebPy will
+00000770: 2072 756e 2079 6f75 7220 6170 702e 2049   run your app. I
+00000780: 7420 7461 6b65 7320 616e 7920 6172 6775  t takes any argu
+00000790: 6d65 6e74 7320 7468 6174 2061 7265 2076  ments that are v
+000007a0: 616c 6964 2074 6f20 7061 7373 2074 6f20  alid to pass to 
+000007b0: 6061 7070 2e72 756e 2829 602e 0d0a 0d0a  `app.run()`.....
 000007c0: 0d0a 556e 6465 7220 6072 6f6f 742f 602c  ..Under `root/`,
 000007d0: 2079 6f75 2063 616e 2075 7365 2060 696e   you can use `in
 000007e0: 6465 782e 7079 6020 616e 6420 6069 6e64  dex.py` and `ind
 000007f0: 6578 2e68 746d 6c60 2066 696c 6573 2074  ex.html` files t
 00000800: 6f20 6372 6561 7465 2066 696c 6573 7973  o create filesys
 00000810: 7465 6d2d 6261 7365 6420 7765 6270 6167  tem-based webpag
 00000820: 6520 726f 7574 6573 2e20 4966 2079 6f75  e routes. If you
@@ -173,92 +173,111 @@
 00000ac0: 0d0a 0d0a 2020 2e2e 2e0d 0a60 6060 0d0a  ....  .....```..
 00000ad0: 0d0a 5369 6e63 6520 7765 206f 6e6c 7920  ..Since we only 
 00000ae0: 7761 6e74 2074 6869 7320 726f 7574 6520  want this route 
 00000af0: 746f 2062 6520 6120 7369 6d70 6c65 2048  to be a simple H
 00000b00: 544d 4c20 7061 6765 2c20 7765 2063 616e  TML page, we can
 00000b10: 2064 656c 6574 6520 6069 6e64 6578 2e70   delete `index.p
 00000b20: 7960 2061 6e64 2072 6570 6c61 6365 2069  y` and replace i
-00000b30: 7420 7769 7468 2060 696e 6465 782e 6874  t with `index.ht
-00000b40: 6d6c 600d 0a0d 0a60 696e 6465 782e 6874  ml`....`index.ht
-00000b50: 6d6c 600d 0a60 6060 6874 6d6c 0d0a 3c21  ml`..```html..<!
-00000b60: 444f 4354 5950 4520 6874 6d6c 3e0d 0a3c  DOCTYPE html>..<
-00000b70: 6874 6d6c 3e0d 0a09 3c68 6561 643e 0d0a  html>...<head>..
-00000b80: 0909 3c6c 696e 6b20 7265 6c3d 2273 7479  ..<link rel="sty
-00000b90: 6c65 7368 6565 7422 2068 7265 663d 222f  lesheet" href="/
-00000ba0: 7374 6174 6963 2f63 7373 2f69 6e64 6578  static/css/index
-00000bb0: 2e63 7373 222f 3e0d 0a09 3c2f 6865 6164  .css"/>...</head
-00000bc0: 3e0d 0a09 3c62 6f64 793e 0d0a 0909 3c68  >...<body>....<h
-00000bd0: 3120 6964 3d22 6865 6164 696e 6722 3e48  1 id="heading">H
-00000be0: 656c 6c6f 2c20 576f 726c 6421 3c2f 6831  ello, World!</h1
-00000bf0: 3e0d 0a09 3c2f 626f 6479 3e0d 0a3c 2f68  >...</body>..</h
-00000c00: 746d 6c3e 0d0a 6060 600d 0a0d 0a4e 6f77  tml>..```....Now
-00000c10: 2c20 7765 2063 616e 2072 756e 206f 7572  , we can run our
-00000c20: 2061 7070 2075 7369 6e67 2060 7765 6270   app using `webp
-00000c30: 7920 7275 6e60 2e20 4e6f 7469 6365 2074  y run`. Notice t
-00000c40: 6861 7420 7768 656e 2076 6973 6974 696e  hat when visitin
-00000c50: 6720 6068 7474 703a 2f2f 3132 372e 302e  g `http://127.0.
-00000c60: 302e 313a 3530 3030 2f68 656c 6c6f 602c  0.1:5000/hello`,
-00000c70: 2074 6865 2043 5353 2074 6861 7420 7765   the CSS that we
-00000c80: 206c 696e 6b65 6420 6672 6f6d 2074 6865   linked from the
-00000c90: 2060 7374 6174 6963 2f60 2066 6f6c 6465   `static/` folde
-00000ca0: 7220 6973 2069 6e63 6c75 6465 642e 0d0a  r is included...
-00000cb0: 0d0a 4966 2079 6f75 2077 616e 7420 746f  ..If you want to
-00000cc0: 206d 616b 6520 796f 7572 2061 7070 2061   make your app a
-00000cd0: 206c 6974 746c 6520 6d6f 7265 2063 6f6d   little more com
-00000ce0: 7061 6374 2c20 796f 7520 6361 6e20 7573  pact, you can us
-00000cf0: 6520 6077 6562 7079 2062 7569 6c64 602e  e `webpy build`.
-00000d00: 2054 6869 7320 7769 6c6c 2063 6f6d 7069   This will compi
-00000d10: 6c65 2061 6c6c 206f 6620 796f 7572 2050  le all of your P
-00000d20: 7974 686f 6e20 616e 6420 4854 4d4c 2069  ython and HTML i
-00000d30: 6e74 6f20 6120 7369 6e67 6c65 206d 696e  nto a single min
-00000d40: 6966 6564 2066 696c 652c 2060 6275 696c  ifed file, `buil
-00000d50: 642e 7079 602c 2077 6869 6368 2063 616e  d.py`, which can
-00000d60: 2062 6520 7275 6e20 6c69 6b65 2061 206e   be run like a n
-00000d70: 6f72 6d61 6c20 5079 7468 6f6e 2073 6372  ormal Python scr
-00000d80: 6970 742e 2048 6f77 6576 6572 2c20 7468  ipt. However, th
-00000d90: 6520 7468 6520 6068 746d 6c2f 6020 616e  e the `html/` an
-00000da0: 6420 6073 7461 7469 632f 6020 6469 7265  d `static/` dire
-00000db0: 6374 6f72 6965 7320 6172 6520 6e6f 7420  ctories are not 
-00000dc0: 7061 636b 6167 6564 2069 6e74 6f20 7468  packaged into th
-00000dd0: 6520 6275 696c 6420 6669 6c65 2c20 736f  e build file, so
-00000de0: 2074 6865 7365 206d 7573 7420 7374 696c   these must stil
-00000df0: 6c20 6265 2070 7265 7365 6e74 2074 6f20  l be present to 
-00000e00: 7275 6e20 6062 7569 6c64 2e70 7960 2e20  run `build.py`. 
-00000e10: 5768 656e 2075 7369 6e67 2060 7765 6270  When using `webp
-00000e20: 7920 7275 6e60 2c20 6368 616e 6765 7320  y run`, changes 
-00000e30: 696e 2074 6865 2066 696c 6573 2075 6e64  in the files und
-00000e40: 6572 2060 726f 6f74 2f60 2061 6e64 2063  er `root/` and c
-00000e50: 6861 6e67 6573 2069 6e20 6669 6c65 7320  hanges in files 
-00000e60: 756e 6465 7220 6073 7461 7469 632f 6020  under `static/` 
-00000e70: 6172 6520 6775 6172 616e 7465 6564 2074  are guaranteed t
-00000e80: 6f20 6265 2072 6566 6c65 6374 6564 2069  o be reflected i
-00000e90: 6e20 7468 6520 6170 7020 7769 7468 6f75  n the app withou
-00000ea0: 7420 6861 7669 6e67 2074 6f20 7265 7374  t having to rest
-00000eb0: 6172 7420 6974 2c20 6275 7420 6966 2074  art it, but if t
-00000ec0: 6865 2061 7070 2069 7320 6265 696e 6720  he app is being 
-00000ed0: 7275 6e20 6672 6f6d 2061 2060 6275 696c  run from a `buil
-00000ee0: 642e 7079 602c 2063 6861 6e67 6573 2069  d.py`, changes i
-00000ef0: 6e20 4854 4d4c 2c20 5079 7468 6f6e 2c20  n HTML, Python, 
-00000f00: 616e 6420 636f 6e66 6967 2066 696c 6573  and config files
-00000f10: 2075 6e64 6572 2060 726f 6f74 2f60 2077   under `root/` w
-00000f20: 696c 6c20 6e6f 7420 6265 2072 6566 6c65  ill not be refle
-00000f30: 6374 6564 2e0d 0a0d 0a5b 5079 585d 2868  cted.....[PyX](h
-00000f40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000f50: 6d2f 5573 6572 3033 3332 2f70 7978 2920  m/User0332/pyx) 
-00000f60: 6361 6e20 616c 736f 2062 6520 696e 7465  can also be inte
-00000f70: 6772 6174 6564 2069 6e74 6f20 5765 6250  grated into WebP
-00000f80: 7920 6170 7073 2062 7920 6368 616e 6769  y apps by changi
-00000f90: 6e67 2050 7974 686f 6e20 6669 6c65 7320  ng Python files 
-00000fa0: 746f 2060 2e70 7978 6020 6669 6c65 732e  to `.pyx` files.
-00000fb0: 2054 6865 7365 2066 696c 6573 2063 616e   These files can
-00000fc0: 2062 6520 636f 6d70 696c 6564 2074 6f20   be compiled to 
-00000fd0: 5079 7468 6f6e 2066 696c 6573 2075 7369  Python files usi
-00000fe0: 6e67 2060 7765 6270 7920 6275 696c 6470  ng `webpy buildp
-00000ff0: 7978 602c 2077 6869 6368 2069 7320 6175  yx`, which is au
-00001000: 746f 6d61 7469 6361 6c6c 7920 7275 6e20  tomatically run 
-00001010: 6279 2074 6865 2060 7765 6270 7920 6275  by the `webpy bu
-00001020: 696c 6460 2c20 6077 6562 7079 2063 6f6d  ild`, `webpy com
-00001030: 7069 6c65 602c 2061 6e64 2060 7765 6270  pile`, and `webp
-00001040: 7920 7275 6e60 2063 6f6d 6d61 6e64 732e  y run` commands.
-00001050: 2057 6562 5079 2063 6f6d 6573 2077 6974   WebPy comes wit
-00001060: 6820 5079 5369 7465 2f50 7958 2061 7320  h PySite/PyX as 
-00001070: 6120 6465 7065 6e64 656e 6379 2e         a dependency.
+00000b30: 7420 7769 7468 2061 6e20 6069 6e64 6578  t with an `index
+00000b40: 2e68 746d 6c60 2066 696c 652e 0d0a 0d0a  .html` file.....
+00000b50: 6069 6e64 6578 2e68 746d 6c60 0d0a 6060  `index.html`..``
+00000b60: 6068 746d 6c0d 0a3c 2144 4f43 5459 5045  `html..<!DOCTYPE
+00000b70: 2068 746d 6c3e 0d0a 3c68 746d 6c3e 0d0a   html>..<html>..
+00000b80: 093c 6865 6164 3e0d 0a09 093c 6c69 6e6b  .<head>....<link
+00000b90: 2072 656c 3d22 7374 796c 6573 6865 6574   rel="stylesheet
+00000ba0: 2220 6872 6566 3d22 2f73 7461 7469 632f  " href="/static/
+00000bb0: 6373 732f 696e 6465 782e 6373 7322 2f3e  css/index.css"/>
+00000bc0: 0d0a 093c 2f68 6561 643e 0d0a 093c 626f  ...</head>...<bo
+00000bd0: 6479 3e0d 0a09 093c 6831 2069 643d 2268  dy>....<h1 id="h
+00000be0: 6561 6469 6e67 223e 4865 6c6c 6f2c 2057  eading">Hello, W
+00000bf0: 6f72 6c64 213c 2f68 313e 0d0a 093c 2f62  orld!</h1>...</b
+00000c00: 6f64 793e 0d0a 3c2f 6874 6d6c 3e0d 0a60  ody>..</html>..`
+00000c10: 6060 0d0a 0d0a 4e6f 772c 2077 6520 6361  ``....Now, we ca
+00000c20: 6e20 7275 6e20 6f75 7220 6170 7020 7573  n run our app us
+00000c30: 696e 6720 6077 6562 7079 2072 756e 602e  ing `webpy run`.
+00000c40: 204e 6f74 6963 6520 7468 6174 2077 6865   Notice that whe
+00000c50: 6e20 7669 7369 7469 6e67 2060 6874 7470  n visiting `http
+00000c60: 3a2f 2f31 3237 2e30 2e30 2e31 3a35 3030  ://127.0.0.1:500
+00000c70: 302f 6865 6c6c 6f60 2c20 7468 6520 4353  0/hello`, the CS
+00000c80: 5320 7468 6174 2077 6520 6c69 6e6b 6564  S that we linked
+00000c90: 2066 726f 6d20 7468 6520 6073 7461 7469   from the `stati
+00000ca0: 632f 6020 666f 6c64 6572 2069 7320 696e  c/` folder is in
+00000cb0: 636c 7564 6564 2e0d 0a0d 0a49 6620 796f  cluded.....If yo
+00000cc0: 7520 7761 6e74 2074 6f20 6d61 6b65 2079  u want to make y
+00000cd0: 6f75 7220 6170 7020 6120 6c69 7474 6c65  our app a little
+00000ce0: 206d 6f72 6520 636f 6d70 6163 742c 2079   more compact, y
+00000cf0: 6f75 2063 616e 2075 7365 2060 7765 6270  ou can use `webp
+00000d00: 7920 6275 696c 6460 2e20 5468 6973 2077  y build`. This w
+00000d10: 696c 6c20 636f 6d70 696c 6520 616c 6c20  ill compile all 
+00000d20: 6f66 2079 6f75 7220 5079 7468 6f6e 2061  of your Python a
+00000d30: 6e64 2048 544d 4c20 696e 746f 2061 2073  nd HTML into a s
+00000d40: 696e 676c 6520 6d69 6e69 6665 6420 6669  ingle minifed fi
+00000d50: 6c65 2c20 6062 7569 6c64 2e70 7960 2c20  le, `build.py`, 
+00000d60: 7768 6963 6820 6361 6e20 6265 2072 756e  which can be run
+00000d70: 206c 696b 6520 6120 6e6f 726d 616c 2050   like a normal P
+00000d80: 7974 686f 6e20 7363 7269 7074 2e20 486f  ython script. Ho
+00000d90: 7765 7665 722c 2074 6865 2074 6865 2060  wever, the the `
+00000da0: 6874 6d6c 2f60 2061 6e64 2060 7374 6174  html/` and `stat
+00000db0: 6963 2f60 2064 6972 6563 746f 7269 6573  ic/` directories
+00000dc0: 2061 7265 206e 6f74 2070 6163 6b61 6765   are not package
+00000dd0: 6420 696e 746f 2074 6865 2062 7569 6c64  d into the build
+00000de0: 2066 696c 652c 2073 6f20 7468 6573 6520   file, so these 
+00000df0: 6d75 7374 2073 7469 6c6c 2062 6520 7072  must still be pr
+00000e00: 6573 656e 7420 746f 2072 756e 2060 6275  esent to run `bu
+00000e10: 696c 642e 7079 602e 2057 6865 6e20 7573  ild.py`. When us
+00000e20: 696e 6720 6077 6562 7079 2072 756e 6020  ing `webpy run` 
+00000e30: 746f 2072 756e 2074 6865 2061 7070 2c20  to run the app, 
+00000e40: 6368 616e 6765 7320 696e 2074 6865 2066  changes in the f
+00000e50: 696c 6573 2075 6e64 6572 2060 726f 6f74  iles under `root
+00000e60: 2f60 2061 6e64 2063 6861 6e67 6573 2069  /` and changes i
+00000e70: 6e20 6669 6c65 7320 756e 6465 7220 6073  n files under `s
+00000e80: 7461 7469 632f 6020 6172 6520 6775 6172  tatic/` are guar
+00000e90: 616e 7465 6564 2074 6f20 6265 2072 6566  anteed to be ref
+00000ea0: 6c65 6374 6564 2069 6e20 7468 6520 6170  lected in the ap
+00000eb0: 7020 7769 7468 6f75 7420 6861 7669 6e67  p without having
+00000ec0: 2074 6f20 7265 7374 6172 7420 6974 2c20   to restart it, 
+00000ed0: 6275 7420 6966 2074 6865 2061 7070 2069  but if the app i
+00000ee0: 7320 6265 696e 6720 7275 6e20 6672 6f6d  s being run from
+00000ef0: 2061 2060 6275 696c 642e 7079 6020 6669   a `build.py` fi
+00000f00: 6c65 2c20 6368 616e 6765 7320 696e 2048  le, changes in H
+00000f10: 544d 4c2c 2050 7974 686f 6e2c 2061 6e64  TML, Python, and
+00000f20: 2063 6f6e 6669 6720 6669 6c65 7320 756e   config files un
+00000f30: 6465 7220 6072 6f6f 742f 6020 7769 6c6c  der `root/` will
+00000f40: 206e 6f74 2062 6520 7265 666c 6563 7465   not be reflecte
+00000f50: 642e 0d0a 0d0a 5b50 7958 5d28 6874 7470  d.....[PyX](http
+00000f60: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f55  s://github.com/U
+00000f70: 7365 7230 3333 322f 7079 7829 2063 616e  ser0332/pyx) can
+00000f80: 2061 6c73 6f20 6265 2069 6e74 6567 7261   also be integra
+00000f90: 7465 6420 696e 746f 2057 6562 5079 2061  ted into WebPy a
+00000fa0: 7070 7320 6279 2063 6861 6e67 696e 6720  pps by changing 
+00000fb0: 5079 7468 6f6e 2066 696c 6573 2074 6f20  Python files to 
+00000fc0: 602e 7079 7860 2066 696c 6573 2e20 5468  `.pyx` files. Th
+00000fd0: 6573 6520 6669 6c65 7320 6361 6e20 6265  ese files can be
+00000fe0: 2063 6f6d 7069 6c65 6420 746f 2050 7974   compiled to Pyt
+00000ff0: 686f 6e20 6669 6c65 7320 7573 696e 6720  hon files using 
+00001000: 6077 6562 7079 2062 7569 6c64 7079 7860  `webpy buildpyx`
+00001010: 2c20 7768 6963 6820 6973 2061 7574 6f6d  , which is autom
+00001020: 6174 6963 616c 6c79 2072 756e 2062 7920  atically run by 
+00001030: 7468 6520 6077 6562 7079 2062 7569 6c64  the `webpy build
+00001040: 602c 2060 7765 6270 7920 636f 6d70 696c  `, `webpy compil
+00001050: 6560 2c20 616e 6420 6077 6562 7079 2072  e`, and `webpy r
+00001060: 756e 6020 636f 6d6d 616e 6473 2e20 5765  un` commands. We
+00001070: 6250 7920 636f 6d65 7320 7769 7468 2050  bPy comes with P
+00001080: 7953 6974 652f 5079 5820 6173 2061 2064  ySite/PyX as a d
+00001090: 6570 656e 6465 6e63 792e 204e 6f74 6520  ependency. Note 
+000010a0: 7468 6174 206f 6e65 206d 7573 7420 7374  that one must st
+000010b0: 696c 6c20 696d 706f 7274 2050 7953 6974  ill import PySit
+000010c0: 6520 4854 4d4c 2074 6167 7320 696e 2065  e HTML tags in e
+000010d0: 7665 7279 2066 696c 6520 7468 6174 2050  very file that P
+000010e0: 7958 2069 7320 7573 6564 2c20 6173 2073  yX is used, as s
+000010f0: 686f 776e 2062 656c 6f77 3a0d 0a60 6060  hown below:..```
+00001100: 7079 0d0a 6672 6f6d 2077 6562 7079 2e70  py..from webpy.p
+00001110: 7973 6974 655f 7365 6d61 6e74 6963 5f74  ysite_semantic_t
+00001120: 6167 7320 696d 706f 7274 202a 2023 2072  ags import * # r
+00001130: 6563 6f6d 6d65 6e64 6564 0d0a 0d0a 2323  ecommended....##
+00001140: 2320 4f52 0d0a 0d0a 6672 6f6d 2070 7973  # OR....from pys
+00001150: 6974 652e 7461 6773 2069 6d70 6f72 7420  ite.tags import 
+00001160: 2a20 2320 616c 736f 2077 6f72 6b73 2c20  * # also works, 
+00001170: 6275 7420 646f 6573 6e27 7420 6669 6c74  but doesn't filt
+00001180: 6572 206f 7574 2075 6e6e 6563 6573 7361  er out unnecessa
+00001190: 7279 2063 6c61 7373 6573 2073 7563 6820  ry classes such 
+000011a0: 6173 2045 6c65 6d65 6e74 0d0a 6060 60    as Element..```
```

### Comparing `webpy-framework-1.0.2/pyproject.toml` & `webpy-framework-1.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webpy-framework"
-version = "1.0.2"
+version = "1.0.3"
 description = "Easy-to-use Python web framework built on top of Flask"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
@@ -21,16 +21,16 @@
 	"flask >= 2.2.2",
 	"dill >= 0.3.5.1",
 	"python-minifier >= 2.8.0",
 	"dill >= 0.3.6",
 	"flask-session >= 0.5.0",
 	"flask-sqlalchemy >= 3.0.0",
 	"py-domapi >= 1.0.0",
-	"pyx-pysite >= 1.0.1"
-
+	"pyx-pysite >= 1.0.1",
+	"markdown >= 3.4.0"
 ]
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://github.com/User0332/webpy"
 
 [project.scripts]
```

### Comparing `webpy-framework-1.0.2/webpy/__init__.py` & `webpy-framework-1.0.3/webpy/__init__.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.0.2/webpy/__main__.py` & `webpy-framework-1.0.3/webpy/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,42 @@
 from json import load, dumps
 from shutil import rmtree
 from sys import argv
 from importlib import import_module
 from typing import Union
 from subprocess import call as subproc_call
 from types import FunctionType
+from markdown import markdown
+
+def buildmd():
+	for path, directories, files in os.walk(os.getcwd()):
+		for file in files:
+			file: str
+			if file.endswith(".md"):
+				actual =  os.path.join(path, file)
+				html = '\n\t\t'.join(
+					markdown(open(actual, 'r').read())
+					.splitlines()
+				)
+				
+
+				with open(actual.removesuffix(".md")+".html", 'w') as f:
+					f.write(
+						f"""<!DOCTYPE html>
+<html>
+	<head></head>
+	<body>
+		{html}
+	</body>
+</html>
+""")
 
 def build():
 	buildpyx()
+	buildmd()
 
 	conf = {}
 
 	if os.path.exists("config.json"):
 		with open("config.json", 'r') as f:
 			conf: dict = load(f)
 
@@ -115,14 +140,15 @@
 
 		code+=(f"app.run({','.join(f'{key}={value!r}' for key, value in conf.items())})")
 
 		f.write(minify(code, rename_globals=True))
 
 def run():
 	buildpyx()
+	buildmd()
 
 	conf = {}
 
 	if os.path.exists("config.json"):
 		with open("config.json", 'r') as f:
 			conf: dict = load(f)
 
@@ -295,12 +321,16 @@
 		webpy_compile()
 		exit(0)
 
 	if argv[1] == "buildpyx":
 		buildpyx()
 		exit(0)
 
+	if argv[1] == "buildmd":
+		buildmd()
+		exit(0)
+
 	print(f"Invalid command {repr(argv[1]) if argv[1] else '<none>'}")
-	print("Possible commands:\n- webpy new {projectname}\n- webpy route {routename}\n- webpy run\n- webpy build\n- webpy compile\n- webpy buildpyx")
+	print("Possible commands:\n- webpy new {projectname}\n- webpy route {routename}\n- webpy run\n- webpy build\n- webpy compile\n- webpy buildpyx\n- webpy buildmd")
 
 if __name__ == "__main__":
 	main()
```

### Comparing `webpy-framework-1.0.2/webpy/fs_routes.py` & `webpy-framework-1.0.3/webpy/fs_routes.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.0.2/webpy_framework.egg-info/PKG-INFO` & `webpy-framework-1.0.3/webpy_framework.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 1.0.2
+Version: 1.0.3
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -70,15 +70,15 @@
     js/
       index.js
 
   app.py
   config.json
 ```
 
-The `app.py` file should contain some boilerplate code. You can use the `app` object just like a normal Flask object!. App configurations should be done inside the `webpy_setup` function. Route functions can still be created. The `config.json` file in the same directory as the `app.py` file configures how WebPy will run your app. It takes any arguments that are valid to pass to `app.run()`
+The `app.py` file should contain some boilerplate code. You can use the `app` object just like a normal Flask object! App configurations should be done inside the `webpy_setup` function. Route functions can still be created. The `config.json` file in the same directory as the `app.py` file configures how WebPy will run your app. It takes any arguments that are valid to pass to `app.run()`.
 
 
 Under `root/`, you can use `index.py` and `index.html` files to create filesystem-based webpage routes. If you use an `index.py` file, WebPy will call the `handler` function and pass the app as an argument. If you use `index.html`, WebPy will just return that HTML file to the requester. Each filesystem route has a `config.json` file. In this file, you can pass any keyword arguments that would be valid to pass to `app.route()`.
 
 Let's create a new page at `http://127.0.0.1:5000/hello`. To do this, we can create a new folder called `hello/` under the `root/` folder. Cd into the `root/` directory and type `webpy route hello`. WebPy will automatically create the `hello/` directory for you.
 
 ```
@@ -86,15 +86,15 @@
   hello/
     index.py
     config.json
 
   ...
 ```
 
-Since we only want this route to be a simple HTML page, we can delete `index.py` and replace it with `index.html`
+Since we only want this route to be a simple HTML page, we can delete `index.py` and replace it with an `index.html` file.
 
 `index.html`
 ```html
 <!DOCTYPE html>
 <html>
 	<head>
 		<link rel="stylesheet" href="/static/css/index.css"/>
@@ -103,10 +103,17 @@
 		<h1 id="heading">Hello, World!</h1>
 	</body>
 </html>
 ```
 
 Now, we can run our app using `webpy run`. Notice that when visiting `http://127.0.0.1:5000/hello`, the CSS that we linked from the `static/` folder is included.
 
-If you want to make your app a little more compact, you can use `webpy build`. This will compile all of your Python and HTML into a single minifed file, `build.py`, which can be run like a normal Python script. However, the the `html/` and `static/` directories are not packaged into the build file, so these must still be present to run `build.py`. When using `webpy run`, changes in the files under `root/` and changes in files under `static/` are guaranteed to be reflected in the app without having to restart it, but if the app is being run from a `build.py`, changes in HTML, Python, and config files under `root/` will not be reflected.
+If you want to make your app a little more compact, you can use `webpy build`. This will compile all of your Python and HTML into a single minifed file, `build.py`, which can be run like a normal Python script. However, the the `html/` and `static/` directories are not packaged into the build file, so these must still be present to run `build.py`. When using `webpy run` to run the app, changes in the files under `root/` and changes in files under `static/` are guaranteed to be reflected in the app without having to restart it, but if the app is being run from a `build.py` file, changes in HTML, Python, and config files under `root/` will not be reflected.
 
-[PyX](https://github.com/User0332/pyx) can also be integrated into WebPy apps by changing Python files to `.pyx` files. These files can be compiled to Python files using `webpy buildpyx`, which is automatically run by the `webpy build`, `webpy compile`, and `webpy run` commands. WebPy comes with PySite/PyX as a dependency.
+[PyX](https://github.com/User0332/pyx) can also be integrated into WebPy apps by changing Python files to `.pyx` files. These files can be compiled to Python files using `webpy buildpyx`, which is automatically run by the `webpy build`, `webpy compile`, and `webpy run` commands. WebPy comes with PySite/PyX as a dependency. Note that one must still import PySite HTML tags in every file that PyX is used, as shown below:
+```py
+from webpy.pysite_semantic_tags import * # recommended
+
+### OR
+
+from pysite.tags import * # also works, but doesn't filter out unnecessary classes such as Element
+```
```

