# Comparing `tmp/webpy-framework-1.0.3.tar.gz` & `tmp/webpy-framework-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpy-framework-1.0.3.tar", last modified: Sat May 27 01:12:43 2023, max compression
+gzip compressed data, was "webpy-framework-1.1.0.tar", last modified: Sat May 27 15:46:25 2023, max compression
```

## Comparing `webpy-framework-1.0.3.tar` & `webpy-framework-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 01:12:43.566161 webpy-framework-1.0.3/
--rw-rw-rw-   0        0        0     1090 2023-05-26 17:17:20.000000 webpy-framework-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     6406 2023-05-27 01:12:43.564706 webpy-framework-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4527 2023-05-26 18:08:51.000000 webpy-framework-1.0.3/README.md
--rw-rw-rw-   0        0        0     1019 2023-05-27 01:12:24.000000 webpy-framework-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 01:12:43.566161 webpy-framework-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 01:12:43.536880 webpy-framework-1.0.3/webpy/
--rw-rw-rw-   0        0        0     1968 2023-03-17 14:31:38.000000 webpy-framework-1.0.3/webpy/__init__.py
--rw-rw-rw-   0        0        0     7226 2023-05-27 01:11:58.000000 webpy-framework-1.0.3/webpy/__main__.py
--rw-rw-rw-   0        0        0     1722 2023-05-27 00:55:01.000000 webpy-framework-1.0.3/webpy/fs_routes.py
--rw-rw-rw-   0        0        0       50 2023-05-26 18:07:53.000000 webpy-framework-1.0.3/webpy/pysite_semantic_tags.py
-drwxrwxrwx   0        0        0        0 2023-05-27 01:12:43.562333 webpy-framework-1.0.3/webpy_framework.egg-info/
--rw-rw-rw-   0        0        0     6406 2023-05-27 01:12:43.000000 webpy-framework-1.0.3/webpy_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-05-27 01:12:43.000000 webpy-framework-1.0.3/webpy_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 01:12:43.000000 webpy-framework-1.0.3/webpy_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-27 01:12:43.000000 webpy-framework-1.0.3/webpy_framework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      158 2023-05-27 01:12:43.000000 webpy-framework-1.0.3/webpy_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-27 01:12:43.000000 webpy-framework-1.0.3/webpy_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 15:46:25.741187 webpy-framework-1.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-05-26 17:17:20.000000 webpy-framework-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     6599 2023-05-27 15:46:25.739021 webpy-framework-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4651 2023-05-27 01:42:52.000000 webpy-framework-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1078 2023-05-27 15:35:35.000000 webpy-framework-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 15:46:25.741187 webpy-framework-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 15:46:25.709660 webpy-framework-1.1.0/webpy/
+-rw-rw-rw-   0        0        0     1968 2023-03-17 14:31:38.000000 webpy-framework-1.1.0/webpy/__init__.py
+-rw-rw-rw-   0        0        0    10520 2023-05-27 15:34:19.000000 webpy-framework-1.1.0/webpy/__main__.py
+-rw-rw-rw-   0        0        0     1809 2023-05-27 15:07:10.000000 webpy-framework-1.1.0/webpy/fs_routes.py
+-rw-rw-rw-   0        0        0     1492 2023-05-27 15:28:10.000000 webpy-framework-1.1.0/webpy/pysite_semantic_tags.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:46:25.736492 webpy-framework-1.1.0/webpy_framework.egg-info/
+-rw-rw-rw-   0        0        0     6599 2023-05-27 15:46:25.000000 webpy-framework-1.1.0/webpy_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-05-27 15:46:25.000000 webpy-framework-1.1.0/webpy_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 15:46:25.000000 webpy-framework-1.1.0/webpy_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-27 15:46:25.000000 webpy-framework-1.1.0/webpy_framework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      158 2023-05-27 15:46:25.000000 webpy-framework-1.1.0/webpy_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-27 15:46:25.000000 webpy-framework-1.1.0/webpy_framework.egg-info/top_level.txt
```

### Comparing `webpy-framework-1.0.3/LICENSE` & `webpy-framework-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.0.3/PKG-INFO` & `webpy-framework-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 1.0.3
+Version: 1.1.0
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,39 +22,41 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/User0332/webpy
+Project-URL: Documentation, https://webpy-framework.readthedocs.io/
 Keywords: framework,flask,web
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WebPy
 
-A web framework built on top of Flask that allows you to add filesystem routes (in the `root/` folder of your project directory). Install it with `pip install webpy-framework`.
+A web framework built on top of Flask that allows you to add filesystem routes (in the `root/` folder of your project directory). Install it with `pip install webpy-framework`. Docs are located [here](https://webpy-framework.readthedocs.io/).
 
 ## Commands
 
 ### Creating your project
 - `webpy new {proj-name}` - Create a new project
 - `webpy route {route-name}` - Create a new filesystem route (this must be under `root/`)
 
 ### Deploying your project
 - `webpy run` - Run this in the project dir to start your app using Flask
 - `webpy build` - Package the program into a `build.py` file
 - `webpy compile` - Package the program into a `build.pyc` file
 - `webpy buildpyx` - Compile the `.pyx` files into `.py` files -- automatically runs through the `build`, `compile`, and `run` commands
+- `webpy buildmd` - Transpile all Markdown files to HTML
 
 WebPy allows developers to use just a minimal amount of Python (the bare minimum needed) for their web apps while also allowing for the full functionality of Flask. Take a look at [webpy-app](https://github.com/User0332/webpy-app/) for example, where the majority of the codebase is HTML and JS while still allowing Flask to be fully utilized. WebPy web servers can also be compiled to standalone exectuables by compiling the output of `webpy build` with a tool such as Nuitka.
 
 ### Your First WebPy Application
 
 Start with `webpy new myfirstproject`. Then cd into the `myfirstproject` directory and open up your editor. It should look something like this:
 ```
```

### Comparing `webpy-framework-1.0.3/README.md` & `webpy-framework-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # WebPy
 
-A web framework built on top of Flask that allows you to add filesystem routes (in the `root/` folder of your project directory). Install it with `pip install webpy-framework`.
+A web framework built on top of Flask that allows you to add filesystem routes (in the `root/` folder of your project directory). Install it with `pip install webpy-framework`. Docs are located [here](https://webpy-framework.readthedocs.io/).
 
 ## Commands
 
 ### Creating your project
 - `webpy new {proj-name}` - Create a new project
 - `webpy route {route-name}` - Create a new filesystem route (this must be under `root/`)
 
 ### Deploying your project
 - `webpy run` - Run this in the project dir to start your app using Flask
 - `webpy build` - Package the program into a `build.py` file
 - `webpy compile` - Package the program into a `build.pyc` file
 - `webpy buildpyx` - Compile the `.pyx` files into `.py` files -- automatically runs through the `build`, `compile`, and `run` commands
+- `webpy buildmd` - Transpile all Markdown files to HTML
 
 WebPy allows developers to use just a minimal amount of Python (the bare minimum needed) for their web apps while also allowing for the full functionality of Flask. Take a look at [webpy-app](https://github.com/User0332/webpy-app/) for example, where the majority of the codebase is HTML and JS while still allowing Flask to be fully utilized. WebPy web servers can also be compiled to standalone exectuables by compiling the output of `webpy build` with a tool such as Nuitka.
 
 ### Your First WebPy Application
 
 Start with `webpy new myfirstproject`. Then cd into the `myfirstproject` directory and open up your editor. It should look something like this:
 ```
```

### Comparing `webpy-framework-1.0.3/pyproject.toml` & `webpy-framework-1.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webpy-framework"
-version = "1.0.3"
+version = "1.1.0"
 description = "Easy-to-use Python web framework built on top of Flask"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
@@ -28,10 +28,11 @@
 	"pyx-pysite >= 1.0.1",
 	"markdown >= 3.4.0"
 ]
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://github.com/User0332/webpy"
+Documentation = "https://webpy-framework.readthedocs.io/"
 
 [project.scripts]
 webpy = "webpy.__main__:main"
```

### Comparing `webpy-framework-1.0.3/webpy/__init__.py` & `webpy-framework-1.1.0/webpy/__init__.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.0.3/webpy/__main__.py` & `webpy-framework-1.1.0/webpy/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,42 +8,99 @@
 from json import load, dumps
 from shutil import rmtree
 from sys import argv
 from importlib import import_module
 from typing import Union
 from subprocess import call as subproc_call
 from types import FunctionType
-from markdown import markdown
+from marko import convert as md_to_html
+from argparse import ArgumentParser
+from threading import Thread
+
+WATCH_FILES: dict[str, int] = {}
+
+def watch_md():
+	while 1:
+		for path, directories, files in os.walk(os.getcwd()):
+			for file in files:
+				file: str
+				if file.endswith(".md"):
+					actual =  os.path.join(path, file)
+
+					mtime = os.stat(actual).st_mtime
+
+					if WATCH_FILES[actual] != mtime:
+						WATCH_FILES[actual] = mtime
+
+						html = '\n\t\t'.join(
+							md_to_html(open(actual, 'r').read())
+							.splitlines()
+						)
+
+						print(f"webpy: detected change in {actual!r}, recompiling")
+
+						with open(actual.removesuffix(".md")+".html", 'w') as f:
+							f.write(
+								f"""<!DOCTYPE html>
+<html>
+	<head></head>
+	<body>
+		{html}
+	</body>
+</html>
+""")
+						
+def watch_pyx():
+	while 1:
+		shell = ["powershell"] if os.name == "nt" else ["bash", "-c"]
+		for path, directories, files in os.walk(os.getcwd()):
+			for file in files:
+				file: str
+				if file.endswith(".pyx"):
+					actual =  os.path.join(path, file)
+
+					mtime = os.stat(actual).st_mtime
+
+					if WATCH_FILES[actual] != mtime:
+						WATCH_FILES[actual] = mtime
+
+						print(f"webpy: detected change in {actual!r}, reloading")
+
+						subproc_call(
+							[*shell, "pyxc", repr(actual)]
+						)
 
 def buildmd():
 	for path, directories, files in os.walk(os.getcwd()):
 		for file in files:
 			file: str
 			if file.endswith(".md"):
 				actual =  os.path.join(path, file)
 				html = '\n\t\t'.join(
-					markdown(open(actual, 'r').read())
+					md_to_html(open(actual, 'r').read())
 					.splitlines()
 				)
+
+				WATCH_FILES[actual] = os.stat(actual).st_mtime
 				
 
 				with open(actual.removesuffix(".md")+".html", 'w') as f:
 					f.write(
 						f"""<!DOCTYPE html>
 <html>
 	<head></head>
 	<body>
 		{html}
 	</body>
 </html>
 """)
 
-def build():
-	buildpyx()
-	buildmd()
+def build(force_debug: bool, compile_md: bool, compile_pyx: bool):
+	if compile_pyx: buildpyx()
+	if compile_md: buildmd()
 
 	conf = {}
 
 	if os.path.exists("config.json"):
 		with open("config.json", 'r') as f:
 			conf: dict = load(f)
 
@@ -55,14 +112,16 @@
 	
 	try:
 		app: Flask = appmod.app
 		setup: FunctionType = appmod.webpy_setup
 	except AttributeError:
 		print("app object and webpy_setup function are missing from app.py!")
 
+	if force_debug: app.debug = True
+	else: app.debug = False
 
 	prerules = list(app.url_map.iter_rules())
 
 	# TODO: use TypedDict for this
 	routes: dict[str, dict[str, Union[dict[str, str], bytes, str]]] = {}
 
 	if not parse_fs_routes(app, "root", routes):
@@ -138,17 +197,24 @@
 				f"app, {route+'_handler'!r}))\n"
 			)
 
 		code+=(f"app.run({','.join(f'{key}={value!r}' for key, value in conf.items())})")
 
 		f.write(minify(code, rename_globals=True))
 
-def run():
-	buildpyx()
-	buildmd()
+def run(
+		force_debug: bool,
+		compile_md: bool,
+		compile_pyx: bool,
+		reload_md: bool,
+		reload_pyx: bool
+	):
+	
+	if compile_pyx: buildpyx()
+	if compile_md: buildmd()
 
 	conf = {}
 
 	if os.path.exists("config.json"):
 		with open("config.json", 'r') as f:
 			conf: dict = load(f)
 
@@ -160,31 +226,36 @@
 	
 	try:
 		app: Flask = appmod.app
 		setup: FunctionType = appmod.webpy_setup
 	except AttributeError:
 		print("app object and webpy_setup function are missing from app.py!")
 
+	if force_debug: app.debug = True
 
 	routes = {}
 
 	setup(app)
 
-	if not parse_fs_routes(app, "root", routes):
+	if not parse_fs_routes(app, "root", WATCH_FILES, routes):
 		exit(1)
 
+	if reload_md and compile_md:
+		t = Thread(target=watch_md)
+		t.daemon = True
+		t.start()
+
+	if reload_pyx and app.debug and compile_pyx:
+		t = Thread(target=watch_pyx)
+		t.daemon = True
+		t.start()
+		
 	app.run(**conf)
 
-def new():
-	if len(argv) < 3:
-		print("Missing project name!")
-		exit(1)
-
-	name = argv[2]
-
+def new(name: str):
 	if os.path.exists(name): rmtree(name)
 
 	defaultconf = {
 		"host": "127.0.0.1",
 		"port": 5000
 	}
 
@@ -242,48 +313,44 @@
 		dumps(defaultrouteconf, indent='\t')
 	)
 
 	open(f"{name}/root/index.py", 'w').write(
 		defaultroutecode
 	)
 
-def route():
-	if len(argv) < 3:
-		print("Missing route name!")
-		exit(1)
-
-	name = argv[2]
-
+def route(name: str):
 	if os.path.exists(name): rmtree(name)
 
 	os.mkdir(f"{name}")
 	open(f"{name}/config.json", 'w').write(
 		dumps(defaultrouteconf, indent='\t')
 	)
 
 	open(f"{name}/index.py", 'w').write(
 		defaultroutecode
 	)
 
-def webpy_compile():
-	build()
+def webpy_compile(force_debug: bool, compile_md: bool, compile_pyx: bool):
+	build(force_debug, compile_md, compile_pyx)
 	compile("build.py", "build.pyc", optimize=2)
 
 	try: os.remove("build.py")
 	except FileNotFoundError: pass
 
 def buildpyx():
 	shell = ["powershell"] if os.name == "nt" else ["bash", "-c"]
 
 	for path, directories, files in os.walk(os.getcwd()):
 		for file in files:
 			file: str
 			if file.endswith(".pyx"):
 				actual =  os.path.join(path, file)
 
+				WATCH_FILES[actual] = os.stat(actual).st_mtime
+
 				subproc_call(
 					[*shell, "pyxc", repr(actual)]
 				)
 
 if len(argv) < 2: argv.append('')
 
 defaultroutecode = """import webpy
@@ -297,40 +364,89 @@
 """
 
 defaultrouteconf = {
 	"methods": ["GET"]
 }
 
 def main():
-	if argv[1] == "run":
-		run()
+	parser = ArgumentParser("webpy", description="CLI for the webpy framework")
+	parser.add_argument(
+		"command", 
+		choices=(
+		"run",
+		"build",
+		"new",
+		"route",
+		"compile",
+		"buildpyx",
+		"buildmd"
+		),
+		help="Possible commands --- webpy new {projectname} (create a new project) --- webpy route {routename} (create a new route directory) --- webpy run (start the application) --- webpy build (compile root/ and app.py into build.py) --- webpy compile (like build but create build.pyc) --- webpy buildpyx (compile all .pyx to .py) --- webpy buildmd (compile all .md to .html)"
+	)
+
+	parser.add_argument("name", help="name to be used for 'new' or 'route' commands", default=None, nargs='?')
+
+	parser.add_argument("--no-compile-md", action="store_true")
+	parser.add_argument("--no-compile-pyx", action="store_true")
+	parser.add_argument("--no-reload-md", action="store_true")
+	parser.add_argument("--no-reload-pyx", action="store_true")
+	parser.add_argument("--force-debug", action="store_true")
+
+
+	args = parser.parse_args()
+	cmd = args.command
+	name = args.name
+
+	compile_md = not args.no_compile_md
+	compile_pyx = not args.no_compile_pyx
+	reload_md = not args.no_reload_md
+	reload_pyx = not args.no_reload_pyx
+	force_debug = args.force_debug
+
+	if cmd == "run":
+		run(
+			force_debug,
+			compile_md,
+			compile_pyx,
+			reload_md,
+			reload_pyx
+		)
 		exit(0)
 
-	if argv[1] == "build":
-		build()
+	if cmd == "build":
+		build(
+			force_debug,
+			compile_md,
+			compile_pyx,
+		)
 		exit(0)
 
-	if argv[1] == "new":
-		new()
+	if cmd == "new":
+		if not name:
+			print("webpy: error: expected name to be used with 'new'")
+			exit(1)
+
+		new(name)
 		exit(0)
 
-	if argv[1] == "route":
-		route()
+	if cmd == "route":
+		if not name:
+			print("webpy: error: expected name to be used with 'route'")
+			exit(1)
+			
+		route(name)
 		exit(0)
 
-	if argv[1] == "compile":
-		webpy_compile()
+	if cmd == "compile":
+		webpy_compile(force_debug, compile_md, compile_pyx)
 		exit(0)
 
-	if argv[1] == "buildpyx":
+	if cmd == "buildpyx":
 		buildpyx()
 		exit(0)
 
-	if argv[1] == "buildmd":
+	if cmd == "buildmd":
 		buildmd()
 		exit(0)
 
-	print(f"Invalid command {repr(argv[1]) if argv[1] else '<none>'}")
-	print("Possible commands:\n- webpy new {projectname}\n- webpy route {routename}\n- webpy run\n- webpy build\n- webpy compile\n- webpy buildpyx\n- webpy buildmd")
-
 if __name__ == "__main__":
 	main()
```

### Comparing `webpy-framework-1.0.3/webpy/fs_routes.py` & `webpy-framework-1.1.0/webpy/fs_routes.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,28 +18,29 @@
 		code,
 		mod.__dict__
 	)
 
 	return mod
 	
 
-def parse_fs_routes(app: Flask, rootdir: str, routedict: dict, parent: str='/') -> bool:
+def parse_fs_routes(app: Flask, rootdir: str, routedict: dict, watchfiles: dict[str, int], parent: str='/') -> bool:
 	conf = f"{rootdir}/config.json"
 	index = f"{rootdir}/index.py"
 	index_html = f"{rootdir}/index.html"
 	
 	if os.path.exists(conf):
 		with open(conf, 'r') as f:
 			try: config: dict = json.load(f)
 			except json.decoder.JSONDecodeError:
 				print(f"{conf} is invaliZd!")
 				return False
 	else: config = {}
 
 	if os.path.exists(index):
+		watchfiles[index] = os.stat(index).st_mtime
 		try:
 			index = modularize(index)
 		except Exception as e:
 			print(f"{index} threw an error!\n{e}")
 			return False
 
 		if not hasattr(index, "handler"):
@@ -73,12 +74,12 @@
 
 		app.route(parent, **config)(handler)
 
 
 	for subdir in os.listdir(rootdir):
 		sub_qual = f"{rootdir}/{subdir}"
 		if os.path.isdir(sub_qual):
-			if not parse_fs_routes(app, sub_qual, routedict, f"{parent}{subdir}/"):
+			if not parse_fs_routes(app, sub_qual, routedict, watchfiles, f"{parent}{subdir}/"):
 				return False
 
 	return True
```

### Comparing `webpy-framework-1.0.3/webpy_framework.egg-info/PKG-INFO` & `webpy-framework-1.1.0/webpy_framework.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 1.0.3
+Version: 1.1.0
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,39 +22,41 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/User0332/webpy
+Project-URL: Documentation, https://webpy-framework.readthedocs.io/
 Keywords: framework,flask,web
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WebPy
 
-A web framework built on top of Flask that allows you to add filesystem routes (in the `root/` folder of your project directory). Install it with `pip install webpy-framework`.
+A web framework built on top of Flask that allows you to add filesystem routes (in the `root/` folder of your project directory). Install it with `pip install webpy-framework`. Docs are located [here](https://webpy-framework.readthedocs.io/).
 
 ## Commands
 
 ### Creating your project
 - `webpy new {proj-name}` - Create a new project
 - `webpy route {route-name}` - Create a new filesystem route (this must be under `root/`)
 
 ### Deploying your project
 - `webpy run` - Run this in the project dir to start your app using Flask
 - `webpy build` - Package the program into a `build.py` file
 - `webpy compile` - Package the program into a `build.pyc` file
 - `webpy buildpyx` - Compile the `.pyx` files into `.py` files -- automatically runs through the `build`, `compile`, and `run` commands
+- `webpy buildmd` - Transpile all Markdown files to HTML
 
 WebPy allows developers to use just a minimal amount of Python (the bare minimum needed) for their web apps while also allowing for the full functionality of Flask. Take a look at [webpy-app](https://github.com/User0332/webpy-app/) for example, where the majority of the codebase is HTML and JS while still allowing Flask to be fully utilized. WebPy web servers can also be compiled to standalone exectuables by compiling the output of `webpy build` with a tool such as Nuitka.
 
 ### Your First WebPy Application
 
 Start with `webpy new myfirstproject`. Then cd into the `myfirstproject` directory and open up your editor. It should look something like this:
 ```
```

