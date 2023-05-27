# Comparing `tmp/cbor_diag-1.0.0.tar.gz` & `tmp/cbor_diag-1.0.1.tar.gz`

## Comparing `cbor_diag-1.0.0.tar` & `cbor_diag-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 cbor_diag-1.0.0/Cargo.toml
--rw-r--r--   0     1001      123     5390 2023-03-18 16:37:34.000000 cbor_diag-1.0.0/.github/workflows/maturin.yml
--rw-r--r--   0     1001      123      755 2023-03-18 16:37:34.000000 cbor_diag-1.0.0/.gitignore
--rw-r--r--   0     1001      123      345 2023-03-18 16:37:34.000000 cbor_diag-1.0.0/.readthedocs.yaml
--rw-r--r--   0     1001      123     1883 2023-03-18 16:37:34.000000 cbor_diag-1.0.0/README.rst
--rw-r--r--   0     1001      123       95 2023-03-18 16:37:34.000000 cbor_diag-1.0.0/doc/conf.py
--rw-r--r--   0     1001      123      160 2023-03-18 16:37:34.000000 cbor_diag-1.0.0/doc/index.rst
--rw-r--r--   0     1001      123      501 2023-03-18 16:37:34.000000 cbor_diag-1.0.0/doctest.txt
--rw-r--r--   0     1001      123      579 2023-03-18 16:37:34.000000 cbor_diag-1.0.0/pyproject.toml
--rw-r--r--   0     1001      123       40 2023-03-18 16:37:34.000000 cbor_diag-1.0.0/pytest.ini
--rw-r--r--   0     1001      123       85 2023-03-18 16:37:34.000000 cbor_diag-1.0.0/python/cbor_diag/__init__.py
--rw-r--r--   0     1001      123     2132 2023-03-18 16:37:34.000000 cbor_diag-1.0.0/src/lib.rs
--rw-r--r--   0     1001      123    12870 2023-03-18 16:39:16.000000 cbor_diag-1.0.0/Cargo.lock
--rw-r--r--   0        0        0     2552 1970-01-01 00:00:00.000000 cbor_diag-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 cbor_diag-1.0.1/Cargo.toml
+-rw-r--r--   0     1001      123     5842 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/.github/workflows/maturin.yml
+-rw-r--r--   0     1001      123      755 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/.gitignore
+-rw-r--r--   0     1001      123      345 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/.readthedocs.yaml
+-rw-r--r--   0     1001      123     2171 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/README.rst
+-rw-r--r--   0     1001      123      130 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/doc/conf.py
+-rw-r--r--   0     1001      123      318 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/doc/index.rst
+-rw-r--r--   0     1001      123      501 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/doctest.txt
+-rw-r--r--   0     1001      123      579 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/pyproject.toml
+-rw-r--r--   0     1001      123       40 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/pytest.ini
+-rw-r--r--   0     1001      123       85 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/python/cbor_diag/__init__.py
+-rw-r--r--   0     1001      123     2132 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/src/lib.rs
+-rw-r--r--   0     1001      123    12905 2023-05-27 20:14:12.000000 cbor_diag-1.0.1/Cargo.lock
+-rw-r--r--   0        0        0     2840 1970-01-01 00:00:00.000000 cbor_diag-1.0.1/PKG-INFO
```

### Comparing `cbor_diag-1.0.0/Cargo.toml` & `cbor_diag-1.0.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "cbor-diag-python-package"
-version = "1.0.0"
+version = "1.0.1"
 edition = "2021"
 license = "MIT OR Apache-2.0"
 description = "Conversion between CBOR and CBOR Diagnostic Notation"
 repository = "https://github.com/chrysn/cbor-diag-py"
 documentation = "https://cbor-diag.readthedocs.io"
 # This is not published through crates.io, but through PyPI.
 publish = false
```

### Comparing `cbor_diag-1.0.0/.github/workflows/maturin.yml` & `cbor_diag-1.0.1/.github/workflows/maturin.yml`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 #    maturin generate-ci --platform all --pytest github
 #
 # and
 #
 # * remove the "Upload to GitHub release" step
 # * remove the emscripten / pytest step -- this fails for reasons that are too
 #   hard to to debug right now
+# * limit target list removing [s390x, ppc64le] -- these are niche enough
+#   architectures that users can be expected to build on their own, and at the
+#   same time have the largest binaries (presumably because their compilers are
+#   not that optimized). Removing them brings the total size below 50MiB, which
+#   is half the default allowed size on PyPI. Thus, if a release needs to be
+#   made urgently, it can be done without needing to ask PyPI for more space.
 #
 on:
   push:
     branches:
       - main
       - master
     tags:
@@ -23,15 +29,15 @@
   contents: read
 
 jobs:
   linux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        target: [x86_64, x86, aarch64, armv7, s390x, ppc64le]
+        target: [x86_64, x86, aarch64, armv7]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
```

### Comparing `cbor_diag-1.0.0/.gitignore` & `cbor_diag-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cbor_diag-1.0.0/README.rst` & `cbor_diag-1.0.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 this module only exposes two very simple functions:
 
 * ``diag2cbor``, which parses diagnostic notation and produces a corresponding CBOR binary string, and
 * ``cbor2diag``, which does the inverse.
 
 It is recommended to use the cbor2_ package to actually process the CBOR data.
 
+Documentation is available `on readthedocs`_.
+
+Installation
+============
+
+This project can be installed `from PyPI`_;
+binary wheels are available there for the common platforms.
+
 Maintenance
 ===========
 
 This package is considered feature-complete at release,
 and maintainened reactively --
 when changes to the ecosystem threaten to make it unusable.
 
@@ -40,12 +48,14 @@
 at the user's choice.
 
 Credit for its functionality goes to Nemo157
 as the maintainer of the underlying `cbor-diag crate`_.
 
 .. _`cbor-diag crate`: https://crates.io/crates/cbor-diag
 .. _cbor2: https://pypi.org/project/cbor2/
+.. _`on readthedocs`: https://cbor-diag.readthedocs.io/
+.. _`from PyPI`: https://pypi.org/project/cbor-diag/
 .. _maturin: https://www.maturin.rs/
 .. _pyo3: https://pyo3.rs/
 .. _`not yet`: https://github.com/PyO3/maturin/issues/1507
 .. _MIT: https://spdx.org/licenses/MIT.html
 .. _Apache-2.0: https://spdx.org/licenses/Apache-2.0.html
```

### Comparing `cbor_diag-1.0.0/pyproject.toml` & `cbor_diag-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cbor_diag-1.0.0/src/lib.rs` & `cbor_diag-1.0.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cbor_diag-1.0.0/Cargo.lock` & `cbor_diag-1.0.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,26 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bs58"
-version = "0.4.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "771fe0050b883fcc3ea2359b1a96bcfbc090b7116eae7c3c512c7a083fdf23d3"
+checksum = "f5353f36341f7451062466f0b755b96ac3a9547e4d7f6b70d603fc721a7d7896"
+dependencies = [
+ "tinyvec",
+]
 
 [[package]]
 name = "cbor-diag"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2644c5bb01d8328b218301180b84ccc6f7fce031d50e30917b07ae762a185b7b"
+checksum = "dc245b6ecd09b23901a4fbad1ad975701fd5061ceaef6afa93a2d70605a64429"
 dependencies = [
  "bs58",
  "chrono",
  "data-encoding",
  "half",
  "nom",
  "num-bigint",
@@ -37,15 +40,15 @@
  "separator",
  "url",
  "uuid",
 ]
 
 [[package]]
 name = "cbor-diag-python-package"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = [
  "cbor-diag",
  "pyo3",
 ]
 
 [[package]]
 name = "cfg-if"
@@ -67,17 +70,17 @@
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
 name = "data-encoding"
-version = "2.3.3"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23d8666cb01533c39dde32bcbab8e227b4ed6679b2c925eba05feabea39508fb"
+checksum = "c2e66c9d817f1720209181c316d28635c050fa304f9c79e47a520882661b7308"
 
 [[package]]
 name = "form_urlencoded"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
@@ -107,17 +110,17 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -137,21 +140,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "minimal-lexical"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
+
+[[package]]
 name = "nom"
-version = "5.1.2"
+version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffb4262d26ed83a1c0a33a38fe2bb15797329c85770da05e6b828ddb782627af"
+checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
- "version_check",
+ "minimal-lexical",
 ]
 
 [[package]]
 name = "num-bigint"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
@@ -225,86 +234,86 @@
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.52"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d0e1ae9e836cc3beddd63db0df682593d7e2d3d891ae8c9083d2113e1744224"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
@@ -341,17 +350,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
@@ -362,23 +371,23 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.11"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "524b68aca1d05e03fdf03fcdce2c6c94b6daf6d16861ddaa7e4f2b6638a9052c"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -400,23 +409,17 @@
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
-
-[[package]]
-name = "version_check"
-version = "0.9.4"
+version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
+checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
```

### Comparing `cbor_diag-1.0.0/PKG-INFO` & `cbor_diag-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbor-diag
-Version: 1.0.0
+Version: 1.0.1
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Rust
@@ -24,14 +24,22 @@
 this module only exposes two very simple functions:
 
 * ``diag2cbor``, which parses diagnostic notation and produces a corresponding CBOR binary string, and
 * ``cbor2diag``, which does the inverse.
 
 It is recommended to use the cbor2_ package to actually process the CBOR data.
 
+Documentation is available `on readthedocs`_.
+
+Installation
+============
+
+This project can be installed `from PyPI`_;
+binary wheels are available there for the common platforms.
+
 Maintenance
 ===========
 
 This package is considered feature-complete at release,
 and maintainened reactively --
 when changes to the ecosystem threaten to make it unusable.
 
@@ -56,13 +64,15 @@
 at the user's choice.
 
 Credit for its functionality goes to Nemo157
 as the maintainer of the underlying `cbor-diag crate`_.
 
 .. _`cbor-diag crate`: https://crates.io/crates/cbor-diag
 .. _cbor2: https://pypi.org/project/cbor2/
+.. _`on readthedocs`: https://cbor-diag.readthedocs.io/
+.. _`from PyPI`: https://pypi.org/project/cbor-diag/
 .. _maturin: https://www.maturin.rs/
 .. _pyo3: https://pyo3.rs/
 .. _`not yet`: https://github.com/PyO3/maturin/issues/1507
 .. _MIT: https://spdx.org/licenses/MIT.html
 .. _Apache-2.0: https://spdx.org/licenses/Apache-2.0.html
```

