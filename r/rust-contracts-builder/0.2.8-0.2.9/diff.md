# Comparing `tmp/rust-contracts-builder-0.2.8.tar.gz` & `tmp/rust-contracts-builder-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rust-contracts-builder-0.2.8.tar", last modified: Fri May 26 01:44:15 2023, max compression
+gzip compressed data, was "rust-contracts-builder-0.2.9.tar", last modified: Sat May 27 03:17:30 2023, max compression
```

## Comparing `rust-contracts-builder-0.2.8.tar` & `rust-contracts-builder-0.2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/pysrc/
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:44:15.705428 rust-contracts-builder-0.2.8/pysrc/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/pysrc/templates/abigen/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/abigen/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/abigen/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/pysrc/templates/init/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/_Cargo.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       20 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/build.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/wasm_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-26 01:44:15.000000 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-26 01:44:15.000000 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:44:15.000000 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-26 01:44:15.000000 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 01:44:15.000000 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 01:44:15.000000 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:17:30.207278 rust-contracts-builder-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-27 03:17:30.207278 rust-contracts-builder-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:17:30.199277 rust-contracts-builder-0.2.9/pysrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/pysrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/pysrc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:17:30.195277 rust-contracts-builder-0.2.9/pysrc/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:17:30.199277 rust-contracts-builder-0.2.9/pysrc/templates/abigen/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/pysrc/templates/abigen/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/pysrc/templates/abigen/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:17:30.203277 rust-contracts-builder-0.2.9/pysrc/templates/init/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/pysrc/templates/init/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/pysrc/templates/init/_Cargo.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       20 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/pysrc/templates/init/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/pysrc/templates/init/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/pysrc/templates/init/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/pysrc/templates/init/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/pysrc/templates/init/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/pysrc/wasm_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:17:30.203277 rust-contracts-builder-0.2.9/rust_contracts_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-27 03:17:30.000000 rust-contracts-builder-0.2.9/rust_contracts_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-27 03:17:30.000000 rust-contracts-builder-0.2.9/rust_contracts_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 03:17:30.000000 rust-contracts-builder-0.2.9/rust_contracts_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-27 03:17:30.000000 rust-contracts-builder-0.2.9/rust_contracts_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-27 03:17:30.000000 rust-contracts-builder-0.2.9/rust_contracts_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 03:17:30.000000 rust-contracts-builder-0.2.9/rust_contracts_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-27 03:17:30.207278 rust-contracts-builder-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-27 03:17:18.000000 rust-contracts-builder-0.2.9/setup.py
```

### Comparing `rust-contracts-builder-0.2.8/LICENSE` & `rust-contracts-builder-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rust-contracts-builder-0.2.8/pysrc/__init__.py` & `rust-contracts-builder-0.2.9/pysrc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import platform
 import tempfile
 import toml
 import shutil
 import argparse
 from .wasm_checker import check_import_section
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 src_dir = os.path.dirname(__file__).replace('\\', '/')
 
 
 #https://stackabuse.com/how-to-print-colored-text-in-python/
 #https://stackoverflow.com/questions/287871/how-do-i-print-colored-text-to-the-terminal
 HEADER = '\033[95m'
@@ -36,15 +36,18 @@
     print(f'{FAIL}:{msg}{ENDC}')
 
 def print_warning(msg):
     print(f'{WARNING}:{msg}{ENDC}')
 
 def build_contract(package_name, build_mode, target_dir, stack_size):
     os.environ['RUSTFLAGS'] = f'-C link-arg=-zstack-size={stack_size} -Clinker-plugin-lto'
-    cmd = fr'cargo +nightly build --target=wasm32-wasi --target-dir={target_dir} -Zbuild-std --no-default-features {build_mode} -Zbuild-std-features=panic_immediate_abort'
+    os.environ['RUSTC_BOOTSTRAP'] = '1'
+    print(f"RUSTC_BOOTSTRAP=\"{os.environ['RUSTC_BOOTSTRAP']}\"")
+    print(f"RUSTFLAGS=\"{os.environ['RUSTFLAGS']}\"")
+    cmd = fr'cargo build --target=wasm32-wasi --target-dir={target_dir} -Zbuild-std --no-default-features {build_mode} -Zbuild-std-features=panic_immediate_abort'
     print(cmd)
     cmd = shlex.split(cmd)
     ret_code = subprocess.call(cmd, stdout=sys.stdout, stderr=sys.stderr)
     if not ret_code == 0:
         sys.exit(ret_code)
 
     try:
```

### Comparing `rust-contracts-builder-0.2.8/pysrc/templates/init/lib.rs` & `rust-contracts-builder-0.2.9/pysrc/templates/init/lib.rs`

 * *Files identical despite different names*

### Comparing `rust-contracts-builder-0.2.8/pysrc/templates/init/test.py` & `rust-contracts-builder-0.2.9/pysrc/templates/init/test.py`

 * *Files identical despite different names*

### Comparing `rust-contracts-builder-0.2.8/pysrc/wasm_checker.py` & `rust-contracts-builder-0.2.9/pysrc/wasm_checker.py`

 * *Files identical despite different names*

### Comparing `rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/SOURCES.txt` & `rust-contracts-builder-0.2.9/rust_contracts_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rust-contracts-builder-0.2.8/setup.py` & `rust-contracts-builder-0.2.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for f in files:
         release_files.append(os.path.join(root.replace('pysrc/', ''), f))    
 
 # print(release_files)
 
 setup(
     name="rust-contracts-builder",
-    version="0.2.8",
+    version="0.2.9",
     description="Rust Contracts Builder",
     author='The UUOSIO Team',
     license="Apache 2.0",
     url="https://github.com/uuosio/rust-contracts-builder",
     packages=['rust_contracts_builder'],
     package_dir={'rust_contracts_builder': 'pysrc'},
     package_data={
```

