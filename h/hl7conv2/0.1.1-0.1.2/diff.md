# Comparing `tmp/hl7conv2-0.1.1.tar.gz` & `tmp/hl7conv2-0.1.2.tar.gz`

## Comparing `hl7conv2-0.1.1.tar` & `hl7conv2-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 hl7conv2-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123     2807 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/.gitignore
--rw-r--r--   0     1001      123      767 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/README.md
--rw-r--r--   0     1001      123      141 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/lint.sh
--rw-r--r--   0     1001      123      752 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123      421 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/src/hl7_example.txt
--rw-r--r--   0     1001      123     2461 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/src/hl7_json.rs
--rw-r--r--   0     1001      123        1 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/src/json_hl7.rs
--rw-r--r--   0     1001      123      296 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123      278 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/src/utils.rs
--rw-r--r--   0     1001      123     7652 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 hl7conv2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 hl7conv2-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      123     2807 2023-05-27 19:05:55.000000 hl7conv2-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-05-27 19:05:55.000000 hl7conv2-0.1.2/.gitignore
+-rw-r--r--   0     1001      123      767 2023-05-27 19:05:55.000000 hl7conv2-0.1.2/README.md
+-rw-r--r--   0     1001      123      141 2023-05-27 19:05:55.000000 hl7conv2-0.1.2/lint.sh
+-rw-r--r--   0     1001      123      756 2023-05-27 19:05:55.000000 hl7conv2-0.1.2/pyproject.toml
+-rw-r--r--   0     1001      123      421 2023-05-27 19:05:55.000000 hl7conv2-0.1.2/src/hl7_example.txt
+-rw-r--r--   0     1001      123     2461 2023-05-27 19:05:55.000000 hl7conv2-0.1.2/src/hl7_json.rs
+-rw-r--r--   0     1001      123        1 2023-05-27 19:05:55.000000 hl7conv2-0.1.2/src/json_hl7.rs
+-rw-r--r--   0     1001      123      296 2023-05-27 19:05:55.000000 hl7conv2-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      123      278 2023-05-27 19:05:55.000000 hl7conv2-0.1.2/src/utils.rs
+-rw-r--r--   0     1001      123     7652 2023-05-27 19:05:55.000000 hl7conv2-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 hl7conv2-0.1.2/PKG-INFO
```

### Comparing `hl7conv2-0.1.1/.github/workflows/CI.yml` & `hl7conv2-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `hl7conv2-0.1.1/.gitignore` & `hl7conv2-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hl7conv2-0.1.1/README.md` & `hl7conv2-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hl7conv2-0.1.1/pyproject.toml` & `hl7conv2-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "hl7conv2"
 requires-python = ">=3.7"
-version = "0.1.1"
-repository = "https://github.com/IlyaKalosha/hl7conv"
+version = "0.1.2"
+repository = "https://github.com/IlyaKalosha/hl7conv2"
 keywords = ["hl7", "convert", "JSON"]
 readme = "README.md"
 description = "Converts hl7 and json formats in both ways"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/IlyaKalosha/hl7conv"
-"Change Log" = "https://github.com/IlyaKalosha/hl7conv/releases"
-"Issues" = "https://github.com/IlyaKalosha/hl7conv/issues"
+"Homepage" = "https://github.com/IlyaKalosha/hl7conv2"
+"Change Log" = "https://github.com/IlyaKalosha/hl7conv2/releases"
+"Issues" = "https://github.com/IlyaKalosha/hl7conv2/issues"
 
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
```

### Comparing `hl7conv2-0.1.1/src/hl7_json.rs` & `hl7conv2-0.1.2/src/hl7_json.rs`

 * *Files identical despite different names*

### Comparing `hl7conv2-0.1.1/Cargo.lock` & `hl7conv2-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "hl7conv2"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
```

### Comparing `hl7conv2-0.1.1/PKG-INFO` & `hl7conv2-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: hl7conv2
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Converts hl7 and json formats in both ways
 Keywords: hl7,convert,JSON
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Homepage, https://github.com/IlyaKalosha/hl7conv
-Project-URL: Change Log, https://github.com/IlyaKalosha/hl7conv/releases
-Project-URL: Issues, https://github.com/IlyaKalosha/hl7conv/issues
+Project-URL: Homepage, https://github.com/IlyaKalosha/hl7conv2
+Project-URL: Change Log, https://github.com/IlyaKalosha/hl7conv2/releases
+Project-URL: Issues, https://github.com/IlyaKalosha/hl7conv2/issues
 
 ## About
 This is a python library written in Rust.
 ### Scope
 
 - convert hl7 medical format to json
 - convert json to hl7 medical format (TODO)
```

