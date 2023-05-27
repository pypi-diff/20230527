# Comparing `tmp/edudraw-1.3.tar.gz` & `tmp/edudraw-1.3.0.1.tar.gz`

## Comparing `edudraw-1.3.tar` & `edudraw-1.3.0.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edudraw-1.3/src/EduDraw/__init__.py
--rw-r--r--   0        0        0    37505 2020-02-02 00:00:00.000000 edudraw-1.3/src/EduDraw/edudraw.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 edudraw-1.3/src/EduDraw/requirements.txt
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 edudraw-1.3/LICENSE.txt
--rw-r--r--   0        0        0    30589 2020-02-02 00:00:00.000000 edudraw-1.3/README.md
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 edudraw-1.3/pyproject.toml
--rw-r--r--   0        0        0    31201 2020-02-02 00:00:00.000000 edudraw-1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edudraw-1.3.0.1/src/EduDraw/__init__.py
+-rw-r--r--   0        0        0    37505 2020-02-02 00:00:00.000000 edudraw-1.3.0.1/src/EduDraw/edudraw.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 edudraw-1.3.0.1/src/EduDraw/requirements.txt
+-rw-r--r--   0        0        0    14630 2020-02-02 00:00:00.000000 edudraw-1.3.0.1/tests/edudraw_tests.py
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 edudraw-1.3.0.1/LICENSE.txt
+-rw-r--r--   0        0        0    30467 2020-02-02 00:00:00.000000 edudraw-1.3.0.1/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 edudraw-1.3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    31083 2020-02-02 00:00:00.000000 edudraw-1.3.0.1/PKG-INFO
```

### Comparing `edudraw-1.3/src/EduDraw/edudraw.py` & `edudraw-1.3.0.1/src/EduDraw/edudraw.py`

 * *Files identical despite different names*

### Comparing `edudraw-1.3/LICENSE.txt` & `edudraw-1.3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edudraw-1.3/README.md` & `edudraw-1.3.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,31 +6,30 @@
 
 The general design of the interface is heavily (if not all) inspired by the [P5.js](https://p5js.org/) library and the Processing library, and is intended to make simple graphical programs easy to do in the .NET environment in the shape of a Windows Forms app and/or in the Python language.
 
 The details of installation and documentation of the respective versions are below. 
 
 ## Installation
 
-In order to use the Python version you can simply download the ```edudraw.py``` and import it in your code like any other library. You'll also need the requirements, which can be installed from the ```requirements.txt``` file.
+You can install the package using PIP by typing the following command: `pip install edudraw`, and import it in your code like any other library.
+You'll need the pygame library as well, in case it doesn't get automatically installed.
 
 ## Setting up
 
 In order to begin using the EduDraw class to make your drawings, you need to do a few steps first:
   
-#### 1. Install the requirements
+#### 1. Install the library and the requirements
 
-You need to install the requirements from the requirements file, you can do this by adding the file on your directory and running the following command:
+The only requirement for this library is `pygame==2.1.2`.
 
-    pip3 install -r requirements.txt
-
-#### 2. Import the implementation file
+#### 2. Import the library
 
 You can do this by adding this to your imports:
 
-    from edudraw import EduDraw
+    from EduDraw import EduDraw
 
 Make sure the file is in the same directory as the file from which you are using it from or that you properly add the path otherwise.
 
 #### 3. Create an instance of the EduDraw class
   
 This can be done by simply creating a new EduDraw instance like this:
     
@@ -47,15 +46,15 @@
  
 Once you run this method on the instance you made for the EduDraw class, the simulation will start and keep running until you give it a halt command or close the window.
 You need to pass the ```setup()``` and ```draw()``` functions you made, and also a ```window_title``` to give the running window a name.
 
 The general structure of your form code may look something like this:
 
 ```
-from eduraw import EduDraw
+from EduDraw import EduDraw
 
 def setup():
     # Setting up goes here...
 
 def draw():
     # Drawing goes here...
 
@@ -66,15 +65,15 @@
 And now you're ready to get onto some drawings :D
 
 ## Getting started (with a simple example)
 
 Now that you have your canvas ready for the show, it's time to actually draw something on the screen. To begin with,let's draw a circle on the screen with a white background. Our code might look something like this:
 
 ```
-from edudraw import EduDraw
+from EduDraw import EduDraw
 
 s = EduDraw(500, 300)
 
 def setup():
     pass
 
 def draw():
@@ -90,15 +89,15 @@
 
 ![img1](https://github.com/MuriloLCN/Simple-Draw-Python/assets/88753590/b6ec2e1f-9b75-4c02-88fc-d66ef73c6909)
 
 
 That's our circle! But this is not very interesting, so let's give it a red filling color, a blue outline and make it move around.
 
 ```
-from edudraw import EduDraw
+from EduDraw import EduDraw
 
 s = EduDraw(500, 300)
 
 
 def setup():
     pass
 
@@ -123,15 +122,15 @@
 
 ![img2](https://github.com/MuriloLCN/Simple-Draw-Python/assets/88753590/b780f016-ef8f-4f66-8d29-120736602985)
 
 
 Now we have a moving red ball :D, but it leaves the screen fairly quickly, so let's make it bounce around.
 
 ```
-from edudraw import EduDraw
+from EduDraw import EduDraw
 
 s = EduDraw(500, 300)
 
 width, height = 0, 0
 velocity = [5, 5]
 ball_position = [50, 50]
```

### Comparing `edudraw-1.3/pyproject.toml` & `edudraw-1.3.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EduDraw"
-version = "1.3"
+version = "1.3.0.1"
 authors = [
   { name="Murilo Luis Calvo Neves", email="muriloluiscalvoneves2004@hotmail.com" },
 ]
 description = "A simple interface for using 2D graphics in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `edudraw-1.3/PKG-INFO` & `edudraw-1.3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EduDraw
-Version: 1.3
+Version: 1.3.0.1
 Summary: A simple interface for using 2D graphics in python
 Project-URL: Homepage, https://github.com/MuriloLCN/Edu-Draw-Python
 Project-URL: Bug Tracker, https://github.com/MuriloLCN/Edu-Draw-Python/issues
 Author-email: Murilo Luis Calvo Neves <muriloluiscalvoneves2004@hotmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
@@ -20,31 +20,30 @@
 
 The general design of the interface is heavily (if not all) inspired by the [P5.js](https://p5js.org/) library and the Processing library, and is intended to make simple graphical programs easy to do in the .NET environment in the shape of a Windows Forms app and/or in the Python language.
 
 The details of installation and documentation of the respective versions are below. 
 
 ## Installation
 
-In order to use the Python version you can simply download the ```edudraw.py``` and import it in your code like any other library. You'll also need the requirements, which can be installed from the ```requirements.txt``` file.
+You can install the package using PIP by typing the following command: `pip install edudraw`, and import it in your code like any other library.
+You'll need the pygame library as well, in case it doesn't get automatically installed.
 
 ## Setting up
 
 In order to begin using the EduDraw class to make your drawings, you need to do a few steps first:
   
-#### 1. Install the requirements
+#### 1. Install the library and the requirements
 
-You need to install the requirements from the requirements file, you can do this by adding the file on your directory and running the following command:
+The only requirement for this library is `pygame==2.1.2`.
 
-    pip3 install -r requirements.txt
-
-#### 2. Import the implementation file
+#### 2. Import the library
 
 You can do this by adding this to your imports:
 
-    from edudraw import EduDraw
+    from EduDraw import EduDraw
 
 Make sure the file is in the same directory as the file from which you are using it from or that you properly add the path otherwise.
 
 #### 3. Create an instance of the EduDraw class
   
 This can be done by simply creating a new EduDraw instance like this:
     
@@ -61,15 +60,15 @@
  
 Once you run this method on the instance you made for the EduDraw class, the simulation will start and keep running until you give it a halt command or close the window.
 You need to pass the ```setup()``` and ```draw()``` functions you made, and also a ```window_title``` to give the running window a name.
 
 The general structure of your form code may look something like this:
 
 ```
-from eduraw import EduDraw
+from EduDraw import EduDraw
 
 def setup():
     # Setting up goes here...
 
 def draw():
     # Drawing goes here...
 
@@ -80,15 +79,15 @@
 And now you're ready to get onto some drawings :D
 
 ## Getting started (with a simple example)
 
 Now that you have your canvas ready for the show, it's time to actually draw something on the screen. To begin with,let's draw a circle on the screen with a white background. Our code might look something like this:
 
 ```
-from edudraw import EduDraw
+from EduDraw import EduDraw
 
 s = EduDraw(500, 300)
 
 def setup():
     pass
 
 def draw():
@@ -104,15 +103,15 @@
 
 ![img1](https://github.com/MuriloLCN/Simple-Draw-Python/assets/88753590/b6ec2e1f-9b75-4c02-88fc-d66ef73c6909)
 
 
 That's our circle! But this is not very interesting, so let's give it a red filling color, a blue outline and make it move around.
 
 ```
-from edudraw import EduDraw
+from EduDraw import EduDraw
 
 s = EduDraw(500, 300)
 
 
 def setup():
     pass
 
@@ -137,15 +136,15 @@
 
 ![img2](https://github.com/MuriloLCN/Simple-Draw-Python/assets/88753590/b780f016-ef8f-4f66-8d29-120736602985)
 
 
 Now we have a moving red ball :D, but it leaves the screen fairly quickly, so let's make it bounce around.
 
 ```
-from edudraw import EduDraw
+from EduDraw import EduDraw
 
 s = EduDraw(500, 300)
 
 width, height = 0, 0
 velocity = [5, 5]
 ball_position = [50, 50]
```

