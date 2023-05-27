# Comparing `tmp/hl7conv2-0.1.0.tar.gz` & `tmp/hl7conv2-0.1.1.tar.gz`

## Comparing `hl7conv2-0.1.0.tar` & `hl7conv2-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 hl7conv2-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     2807 2023-05-26 23:20:28.000000 hl7conv2-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-05-26 23:20:28.000000 hl7conv2-0.1.0/.gitignore
--rw-r--r--   0     1001      123      767 2023-05-26 23:20:28.000000 hl7conv2-0.1.0/README.md
--rw-r--r--   0     1001      123      368 2023-05-26 23:20:28.000000 hl7conv2-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123      421 2023-05-26 23:20:28.000000 hl7conv2-0.1.0/src/hl7_example.txt
--rw-r--r--   0     1001      123     2461 2023-05-26 23:20:28.000000 hl7conv2-0.1.0/src/hl7_json.rs
--rw-r--r--   0     1001      123        1 2023-05-26 23:20:28.000000 hl7conv2-0.1.0/src/json_hl7.rs
--rw-r--r--   0     1001      123      296 2023-05-26 23:20:28.000000 hl7conv2-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123      278 2023-05-26 23:20:28.000000 hl7conv2-0.1.0/src/utils.rs
--rw-r--r--   0     1001      123     7652 2023-05-26 23:20:28.000000 hl7conv2-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 hl7conv2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 hl7conv2-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123     2807 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/.gitignore
+-rw-r--r--   0     1001      123      767 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/README.md
+-rw-r--r--   0     1001      123      141 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/lint.sh
+-rw-r--r--   0     1001      123      752 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123      421 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/src/hl7_example.txt
+-rw-r--r--   0     1001      123     2461 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/src/hl7_json.rs
+-rw-r--r--   0     1001      123        1 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/src/json_hl7.rs
+-rw-r--r--   0     1001      123      296 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123      278 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/src/utils.rs
+-rw-r--r--   0     1001      123     7652 2023-05-27 18:50:19.000000 hl7conv2-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 hl7conv2-0.1.1/PKG-INFO
```

### Comparing `hl7conv2-0.1.0/.github/workflows/CI.yml` & `hl7conv2-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `hl7conv2-0.1.0/.gitignore` & `hl7conv2-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hl7conv2-0.1.0/README.md` & `hl7conv2-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hl7conv2-0.1.0/src/hl7_json.rs` & `hl7conv2-0.1.1/src/hl7_json.rs`

 * *Files identical despite different names*

### Comparing `hl7conv2-0.1.0/Cargo.lock` & `hl7conv2-0.1.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "hl7conv2"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
@@ -85,17 +85,17 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -154,17 +154,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
```

### Comparing `hl7conv2-0.1.0/PKG-INFO` & `hl7conv2-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: hl7conv2
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Summary: Converts hl7 and json formats in both ways
+Keywords: hl7,convert,JSON
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Homepage, https://github.com/IlyaKalosha/hl7conv
+Project-URL: Change Log, https://github.com/IlyaKalosha/hl7conv/releases
+Project-URL: Issues, https://github.com/IlyaKalosha/hl7conv/issues
 
 ## About
 This is a python library written in Rust.
 ### Scope
 
 - convert hl7 medical format to json
 - convert json to hl7 medical format (TODO)
```

