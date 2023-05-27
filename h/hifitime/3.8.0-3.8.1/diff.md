# Comparing `tmp/hifitime-3.8.0.tar.gz` & `tmp/hifitime-3.8.1.tar.gz`

## Comparing `hifitime-3.8.0.tar` & `hifitime-3.8.1.tar`

### file list

```diff
@@ -1,49 +1,52 @@
--rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 hifitime-3.8.0/Cargo.toml
--rw-r--r--   0     1001      123      145 2022-12-30 16:03:20.000000 hifitime-3.8.0/.github/dependabot.yml
--rw-r--r--   0     1001      123     1103 2022-12-30 16:03:20.000000 hifitime-3.8.0/.github/workflows/benchmarks.yml
--rw-r--r--   0     1001      123     1119 2022-12-30 16:03:20.000000 hifitime-3.8.0/.github/workflows/formal_verification.yml
--rw-r--r--   0     1001      123     1664 2022-12-30 16:03:20.000000 hifitime-3.8.0/.github/workflows/python.yml
--rw-r--r--   0     1001      123     4170 2022-12-30 16:03:20.000000 hifitime-3.8.0/.github/workflows/tests.yml
--rw-r--r--   0     1001      123       41 2022-12-30 16:03:20.000000 hifitime-3.8.0/.gitignore
--rw-r--r--   0     1001      123     2950 2022-12-30 16:03:20.000000 hifitime-3.8.0/.vscode/launch.json
--rw-r--r--   0     1001      123    11357 2022-12-30 16:03:20.000000 hifitime-3.8.0/LICENSE.txt
--rw-r--r--   0     1001      123    24915 2022-12-30 16:03:20.000000 hifitime-3.8.0/README.md
--rw-r--r--   0     1001      123      898 2022-12-30 16:03:20.000000 hifitime-3.8.0/benches/bench_duration.rs
--rw-r--r--   0     1001      123     2606 2022-12-30 16:03:20.000000 hifitime-3.8.0/benches/bench_epoch.rs
--rw-r--r--   0     1001      123     1419 2022-12-30 16:03:20.000000 hifitime-3.8.0/benches/iai_duration.rs
--rw-r--r--   0     1001      123     2045 2022-12-30 16:03:20.000000 hifitime-3.8.0/benches/iai_epoch.rs
--rw-r--r--   0     1001      123     2527 2022-12-30 16:03:20.000000 hifitime-3.8.0/examples/python/basic.py
--rw-r--r--   0     1001      123     2932 2022-12-30 16:03:20.000000 hifitime-3.8.0/examples/python/timescales.py
--rw-r--r--   0     1001      123     6866 2022-12-30 16:03:20.000000 hifitime-3.8.0/naif0012.txt
--rw-r--r--   0     1001      123      430 2022-12-30 16:03:20.000000 hifitime-3.8.0/pyproject.toml
--rwxr-xr-x   0     1001      123      777 2022-12-30 16:03:59.000000 hifitime-3.8.0/run-maturin-action.sh
--rw-r--r--   0     1001      123     5187 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/asn1der.rs
--rw-r--r--   0     1001      123    16117 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/deprecated.rs
--rw-r--r--   0     1001      123    57258 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/duration.rs
--rw-r--r--   0     1001      123    11189 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/efmt/consts.rs
--rw-r--r--   0     1001      123    22238 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/efmt/format.rs
--rw-r--r--   0     1001      123    10754 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/efmt/formatter.rs
--rw-r--r--   0     1001      123      508 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/efmt/mod.rs
--rw-r--r--   0     1001      123   123116 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/epoch.rs
--rw-r--r--   0     1001      123     3319 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/errors.rs
--rw-r--r--   0     1001      123     6166 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/leap_seconds.rs
--rw-r--r--   0     1001      123     3731 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/leap_seconds_file.rs
--rw-r--r--   0     1001      123     5520 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/lib.rs
--rw-r--r--   0     1001      123     3797 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/month.rs
--rw-r--r--   0     1001      123     7585 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/parser.rs
--rw-r--r--   0     1001      123     1058 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/python.rs
--rw-r--r--   0     1001      123     8303 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/timescale.rs
--rw-r--r--   0     1001      123     9906 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/timeseries.rs
--rw-r--r--   0     1001      123     9554 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/timeunits.rs
--rw-r--r--   0     1001      123     4881 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/ut1.rs
--rw-r--r--   0     1001      123     6117 2022-12-30 16:03:20.000000 hifitime-3.8.0/src/weekday.rs
--rw-r--r--   0     1001      123    18373 2022-12-30 16:03:20.000000 hifitime-3.8.0/tests/duration.rs
--rw-r--r--   0     1001      123     2679 2022-12-30 16:03:20.000000 hifitime-3.8.0/tests/efmt.rs
--rw-r--r--   0     1001      123    74191 2022-12-30 16:03:20.000000 hifitime-3.8.0/tests/epoch.rs
--rw-r--r--   0     1001      123       23 2022-12-30 16:03:20.000000 hifitime-3.8.0/tests/lib.rs
--rw-r--r--   0     1001      123     1808 2022-12-30 16:03:20.000000 hifitime-3.8.0/tests/timescale.rs
--rw-r--r--   0     1001      123     3764 2022-12-30 16:03:20.000000 hifitime-3.8.0/tests/timeseries.rs
--rw-r--r--   0     1001      123     1436 2022-12-30 16:03:20.000000 hifitime-3.8.0/tests/ut1.rs
--rw-r--r--   0     1001      123     9406 2022-12-30 16:03:20.000000 hifitime-3.8.0/tests/weekday.rs
--rw-r--r--   0        0        0    42350 2022-12-30 16:04:49.000000 hifitime-3.8.0/Cargo.lock
--rw-r--r--   0        0        0    25701 1970-01-01 00:00:00.000000 hifitime-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 hifitime-3.8.1/Cargo.toml
+-rw-r--r--   0     1001      123      145 2023-05-27 14:18:34.000000 hifitime-3.8.1/.github/dependabot.yml
+-rw-r--r--   0     1001      123     2847 2023-05-27 14:18:34.000000 hifitime-3.8.1/.github/workflows/benchmarks.yml
+-rw-r--r--   0     1001      123      656 2023-05-27 14:18:34.000000 hifitime-3.8.1/.github/workflows/formal_verification.yml
+-rw-r--r--   0     1001      123     4174 2023-05-27 14:18:34.000000 hifitime-3.8.1/.github/workflows/python.yml
+-rw-r--r--   0     1001      123     3819 2023-05-27 14:18:34.000000 hifitime-3.8.1/.github/workflows/tests.yml
+-rw-r--r--   0     1001      123       41 2023-05-27 14:18:34.000000 hifitime-3.8.1/.gitignore
+-rw-r--r--   0     1001      123     2950 2023-05-27 14:18:34.000000 hifitime-3.8.1/.vscode/launch.json
+-rw-r--r--   0     1001      123    11357 2023-05-27 14:18:34.000000 hifitime-3.8.1/LICENSE.txt
+-rw-r--r--   0     1001      123    26478 2023-05-27 14:18:34.000000 hifitime-3.8.1/README.md
+-rw-r--r--   0     1001      123      898 2023-05-27 14:18:34.000000 hifitime-3.8.1/benches/crit_duration.rs
+-rw-r--r--   0     1001      123     2606 2023-05-27 14:18:34.000000 hifitime-3.8.1/benches/crit_epoch.rs
+-rw-r--r--   0     1001      123     1419 2023-05-27 14:18:34.000000 hifitime-3.8.1/benches/iai_duration.rs
+-rw-r--r--   0     1001      123     2045 2023-05-27 14:18:34.000000 hifitime-3.8.1/benches/iai_epoch.rs
+-rw-r--r--   0     1001      123      643 2023-05-27 14:18:34.000000 hifitime-3.8.1/benches/parse_crit_benchmark.py
+-rw-r--r--   0     1001      123     1081 2023-05-27 14:18:34.000000 hifitime-3.8.1/benches/parse_iai_benchmark.py
+-rw-r--r--   0     1001      123     2500 2023-05-27 14:18:34.000000 hifitime-3.8.1/examples/python/basic.py
+-rw-r--r--   0     1001      123     3012 2023-05-27 14:18:34.000000 hifitime-3.8.1/examples/python/timescales.py
+-rw-r--r--   0     1001      123     6866 2023-05-27 14:18:34.000000 hifitime-3.8.1/naif0012.txt
+-rw-r--r--   0     1001      123      430 2023-05-27 14:18:34.000000 hifitime-3.8.1/pyproject.toml
+-rw-r--r--   0     1001      123     5187 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/asn1der.rs
+-rw-r--r--   0     1001      123    16117 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/deprecated.rs
+-rw-r--r--   0     1001      123    58373 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/duration.rs
+-rw-r--r--   0     1001      123    11189 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/efmt/consts.rs
+-rw-r--r--   0     1001      123    22331 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/efmt/format.rs
+-rw-r--r--   0     1001      123    10754 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/efmt/formatter.rs
+-rw-r--r--   0     1001      123      508 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/efmt/mod.rs
+-rw-r--r--   0     1001      123   125125 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/epoch.rs
+-rw-r--r--   0     1001      123     3321 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/errors.rs
+-rw-r--r--   0     1001      123     6465 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/leap_seconds.rs
+-rw-r--r--   0     1001      123     4650 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/leap_seconds_file.rs
+-rw-r--r--   0     1001      123     5520 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/lib.rs
+-rw-r--r--   0     1001      123     3731 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/month.rs
+-rw-r--r--   0     1001      123     7585 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/parser.rs
+-rw-r--r--   0     1001      123     1058 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/python.rs
+-rw-r--r--   0     1001      123     8303 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/timescale.rs
+-rw-r--r--   0     1001      123    11676 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/timeseries.rs
+-rw-r--r--   0     1001      123     9554 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/timeunits.rs
+-rw-r--r--   0     1001      123     5206 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/ut1.rs
+-rw-r--r--   0     1001      123     6117 2023-05-27 14:18:34.000000 hifitime-3.8.1/src/weekday.rs
+-rw-r--r--   0     1001      123       11 2023-05-27 14:18:34.000000 hifitime-3.8.1/tests/.gitignore
+-rw-r--r--   0     1001      123    18373 2023-05-27 14:18:34.000000 hifitime-3.8.1/tests/duration.rs
+-rw-r--r--   0     1001      123     3220 2023-05-27 14:18:34.000000 hifitime-3.8.1/tests/efmt.rs
+-rw-r--r--   0     1001      123    74967 2023-05-27 14:18:34.000000 hifitime-3.8.1/tests/epoch.rs
+-rw-r--r--   0     1001      123        1 2023-05-27 14:18:34.000000 hifitime-3.8.1/tests/lib.rs
+-rw-r--r--   0     1001      123     1084 2023-05-27 14:18:34.000000 hifitime-3.8.1/tests/python/test_epoch.py
+-rw-r--r--   0     1001      123     1808 2023-05-27 14:18:34.000000 hifitime-3.8.1/tests/timescale.rs
+-rw-r--r--   0     1001      123     3764 2023-05-27 14:18:34.000000 hifitime-3.8.1/tests/timeseries.rs
+-rw-r--r--   0     1001      123     1608 2023-05-27 14:18:34.000000 hifitime-3.8.1/tests/ut1.rs
+-rw-r--r--   0     1001      123     9406 2023-05-27 14:18:34.000000 hifitime-3.8.1/tests/weekday.rs
+-rw-r--r--   0     1001      123    45072 2023-05-27 14:20:09.000000 hifitime-3.8.1/Cargo.lock
+-rw-r--r--   0        0        0    27264 1970-01-01 00:00:00.000000 hifitime-3.8.1/PKG-INFO
```

### Comparing `hifitime-3.8.0/Cargo.toml` & `hifitime-3.8.1/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 [package]
 name = "hifitime"
-version = "3.8.0"
+version = "3.8.1"
 authors = ["Christopher Rabotin <christopher.rabotin@gmail.com>"]
 description = "Ultra-precise date and time handling in Rust for scientific applications with leap second support"
 homepage = "https://nyxspace.com/"
 documentation = "https://docs.rs/hifitime/"
 repository = "https://github.com/nyx-space/hifitime"
 keywords = ["date", "time", "science", "leap-second", "no-std"]
-categories = ["date-and-time"]
+categories = ["date-and-time", "no-std"]
 readme = "README.md"
 license = "Apache-2.0"
 exclude = ["*.tar.gz", "data/"]
 edition = "2021"
 
 [lib]
 crate-type = ["cdylib", "rlib"]
 name = "hifitime"
 
 [dependencies]
-serde = {version = "1.0.152", optional = true}
-serde_derive = {version = "1.0.152", optional = true}
+serde = {version = "1.0.155", optional = true}
+serde_derive = {version = "1.0.155", optional = true}
 der = {version = "0.6.1", features = ["derive", "real"], optional = true}
-pyo3 = { version = "0.17.3", features = ["extension-module"], optional = true}
+pyo3 = { version = "0.18.1", features = ["extension-module"], optional = true }
 num-traits = {version = "0.2.15", default-features = false, features = ["libm"]}
 lexical-core = {version = "0.8.5", default-features = false, features = ["parse-integers", "parse-floats"]}
 reqwest = { version = "0.11", features = ["blocking", "json"], optional = true}
-tabled = {version = "0.10.0", optional = true}
+tabled = {version = "0.12.0", optional = true}
 openssl = { version = "0.10", features = ["vendored"], optional = true }
 
 [dev-dependencies]
 serde_json = "1.0.91"
-criterion = "0.4.0"
+criterion = "0.5.1"
 iai = "0.1"
 
 [features]
 default = ["std"]
 std = ["serde", "serde_derive"]
 asn1der = ["der"]
 python = ["std", "asn1der", "pyo3", "ut1"]
 ut1 = ["std", "reqwest", "tabled", "openssl"]
 
 [[bench]]
-name = "bench_epoch"
+name = "crit_epoch"
 harness = false 
 
 [[bench]]
-name = "bench_duration"
+name = "crit_duration"
 harness = false
 
 [[bench]]
 name = "iai_duration"
 harness = false
 
 [[bench]]
```

### Comparing `hifitime-3.8.0/.github/workflows/tests.yml` & `hifitime-3.8.1/.github/workflows/tests.yml`

 * *Files 17% similar despite different names*

```diff
@@ -17,120 +17,105 @@
     name: Check
     runs-on: ubuntu-latest
     steps:
       - name: Checkout sources
         uses: actions/checkout@v3
 
       - name: Install stable toolchain
-        uses: actions-rs/toolchain@v1
+        uses: dtolnay/rust-toolchain@master
         with:
-          profile: minimal
           toolchain: stable
-          override: true
 
       - name: Run cargo check
-        uses: actions-rs/cargo@v1
-        with:
-          command: check
+        run: cargo check
 
   test:
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
         rust:
-          - { version: "1.58", name: MSRV }
+          - { version: "1.64", name: MSRV }
           - { version: stable, name: stable }
 
     runs-on: ${{ matrix.os }}
     name: Test Suite (${{ matrix.os }}, ${{ matrix.rust.name }})
     steps:
       - name: Checkout sources
         uses: actions/checkout@v3
 
       - name: Install ${{ matrix.rust.name }} toolchain
-        uses: actions-rs/toolchain@v1
+        uses: dtolnay/rust-toolchain@master
         with:
-          profile: minimal
           toolchain: ${{ matrix.rust.version }}
-          override: true
 
       - name: Test (default features)
         run: cargo test
 
       - name: Test (ASN1)
         run: cargo test --features asn1der
+      
+      - name: Test (UT1)
+        run: cargo test --features ut1
 
       - name: Test (no default features)
         run: cargo test --no-default-features
-      
+
       - name: Test (serde)
         run: cargo test --features serde
 
   test_no_std:
     strategy:
       matrix:
         target: [aarch64-unknown-none, thumbv6m-none-eabi]
     name: no-std build
     runs-on: ubuntu-latest
     steps:
       - name: Checkout sources
         uses: actions/checkout@v3
 
       - name: Install nightly toolchain
-        uses: actions-rs/toolchain@v1
+        uses: dtolnay/rust-toolchain@master
         with:
-          profile: minimal
           toolchain: nightly
-          override: true
           components: rust-src
 
       - name: Build no default features + no_std target ${{ matrix.target }}
         run: cargo build --no-default-features --target=${{ matrix.target }} -Z build-std=core
 
   lints:
     name: Lints
     runs-on: ubuntu-latest
     steps:
       - name: Checkout sources
         uses: actions/checkout@v3
 
       - name: Install stable toolchain
-        uses: actions-rs/toolchain@v1
+        uses: dtolnay/rust-toolchain@master
         with:
-          profile: minimal
-          toolchain: stable
-          override: true
+          toolchain: 1.64 # Run lints using the MSRV not latest
           components: rustfmt, clippy
 
       - name: Run cargo fmt
-        uses: actions-rs/cargo@v1
-        with:
-          command: fmt
-          args: --all -- --check
+        run: cargo fmt --all -- --check
 
       - name: Run cargo clippy
-        uses: actions-rs/cargo@v1
-        with:
-          command: clippy
-          args: -- -D warnings
+        run: cargo clippy -- -D warnings
 
   coverage:
     name: Coverage
     runs-on: ubuntu-latest
 
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
       - name: Install stable toolchain
-        uses: actions-rs/toolchain@v1
+        uses: dtolnay/rust-toolchain@master
         with:
-          profile: minimal
           toolchain: stable
-          override: true
           components: rustfmt, clippy
 
       - name: Install cargo-llvm-cov
         uses: taiki-e/install-action@cargo-llvm-cov
 
       - name: Generate coverage report
         run: |
@@ -152,19 +137,17 @@
     needs: [check, test, test_no_std, lints, coverage]
     if: github.ref_type == 'tag'
     steps:
       - name: Checkout sources
         uses: actions/checkout@v3
 
       - name: Install stable toolchain
-        uses: actions-rs/toolchain@v1
+        uses: dtolnay/rust-toolchain@master
         with:
-          profile: minimal
           toolchain: stable
-          override: true
           components: rustfmt, clippy
 
       - name: Publish to crates.io
         env:
           TOKEN: ${{ secrets.CRATESIO_API_TOKEN }}
         run: |
           cargo login $TOKEN
```

### Comparing `hifitime-3.8.0/.vscode/launch.json` & `hifitime-3.8.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/LICENSE.txt` & `hifitime-3.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/README.md` & `hifitime-3.8.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,218 +1,285 @@
-# hifitime 3
+# Introduction to Hifitime
 
-Scientifically accurate date and time handling with guaranteed nanosecond precision for 32,768 years _before_ 01 January 1900 and 32,767 years _after_ that reference epoch.
-Formally verified to not crash on operations on epochs and durations using the [`Kani`](https://model-checking.github.io/kani/) model checking.
+Hifitime is a powerful Rust and Python library designed for time management. It provides extensive functionalities with precise operations for time calculation in different time scales, making it suitable for engineering and scientific applications where general relativity and time dilation matter. Hifitime guarantees nanosecond precision for 65,536 years around 01 January 1900 TAI. Hifitime is also formally verified using the [`Kani` model checker](https://model-checking.github.io/kani/), read more about it [this verification here](https://model-checking.github.io/kani-verifier-blog/2023/03/31/how-kani-helped-find-bugs-in-hifitime.html).
 
-[![hifitime on crates.io][cratesio-image]][cratesio]
-[![hifitime on docs.rs][docsrs-image]][docsrs]
-[![minimum rustc: 1.58](https://img.shields.io/badge/minimum%20rustc-1.58-yellowgreen?logo=rust)](https://www.whatrustisit.com)
-[![Build Status](https://github.com/nyx-space/hifitime/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/nyx-space/hifitime/actions)
-[![Build Status](https://github.com/nyx-space/hifitime/actions/workflows/formal_verification.yml/badge.svg?branch=master)](https://github.com/nyx-space/hifitime/actions)
-[![codecov](https://codecov.io/gh/nyx-space/hifitime/branch/master/graph/badge.svg?token=l7zU57rUGs)](https://codecov.io/gh/nyx-space/hifitime)
-
-[cratesio-image]: https://img.shields.io/crates/v/hifitime.svg
-[cratesio]: https://crates.io/crates/hifitime
-[docsrs-image]: https://docs.rs/hifitime/badge.svg
-[docsrs]: https://docs.rs/hifitime/
-
-
-# Features
-
- * [x] Initialize a high precision Epoch from the system time in UTC
- * [x] Leap seconds (as announced by the IETF on a yearly basis)
- * [x] UTC representation with ISO8601 and RFC3339 formatting and blazing fast parsing (45 nanoseconds)
- * [x] Trivial support of time arithmetic: addition (e.g. `2.hours() + 3.seconds()`), subtraction (e.g. `2.hours() - 3.seconds()`), round/floor/ceil operations (e.g. `2.hours().round(3.seconds())`)
- * [x] Supports ranges of Epochs and TimeSeries (linspace of `Epoch`s and `Duration`s)
- * [x] Trivial conversion between many time scales
- * [x] High fidelity Ephemeris Time / Dynamic Barycentric Time (TDB) computations from [ESA's Navipedia](https://gssc.esa.int/navipedia/index.php/Transformations_between_Time_Systems#TDT_-_TDB.2C_TCB)
- * [x] Julian dates and Modified Julian dates
- * [x] Embedded device friendly: `no-std` and `const fn` where possible
-
-This library is validated against NASA/NAIF SPICE for the Ephemeris Time to Universal Coordinated Time computations: there are exactly zero nanoseconds of difference between SPICE and hifitime for the computation of ET and UTC after 01 January 1972. Refer to the [leap second](#leap-second-support) section for details. Other examples are validated with external references, as detailed on a test-by-test basis.
+Most users of Hifitime will only need to rely on the `Epoch` and `Duration` structures, and optionally the `Weekday` enum for week based computations. Scientific applications may make use of the `TimeScale` enum as well.
 
-## Supported time scales
+## Usage
 
-+ Temps Atomique International (TAI)
-+ Universal Coordinated Time (UTC)
-+ Terrestrial Time (TT)
-+ Ephemeris Time (ET) without the small perturbations as per NASA/NAIF SPICE leap seconds kernel
-+ Dynamic Barycentric Time (TDB), a higher fidelity ephemeris time
-+ Global Positioning System (GPST)
-+ Galileo System Time (GST)
-+ BeiDou Time (BDT)
-+ UNIX
-## Non-features
-* Time-agnostic / date-only epochs. Hifitime only supports the combination of date and time, but the `Epoch::{at_midnight, at_noon}` is provided as a helper function.
+First, install `hifitime` either with `cargo add hifitime` in your Rust project or `pip install hifitime` in Python.
 
-# Usage
+If building from source, note that the Python package is only built if the `python` feature is enabled.
 
-Put this in your `Cargo.toml`:
+### Epoch ("datetime" equivalent)
 
-```toml
-[dependencies]
-hifitime = "3.7"
-```
+**Create an epoch in different time scales.**
 
-## Examples:
-### Time creation
 ```rust
-use hifitime::{Epoch, Unit, TimeUnits};
+use hifitime::prelude::*;
 use core::str::FromStr;
+// Create an epoch in UTC
+let epoch = Epoch::from_gregorian_utc(2000, 2, 29, 14, 57, 29, 37);
+// Or from a string
+let epoch_from_str = Epoch::from_str("2000-02-29T14:57:29.000000037 UTC").unwrap();
+assert_eq!(epoch, epoch_from_str);
+// Creating it from TAI will effectively show the number of leap seconds in between UTC an TAI at that epoch
+let epoch_tai = Epoch::from_gregorian_tai(2000, 2, 29, 14, 57, 29, 37);
+// The difference between two epochs is a Duration
+let num_leap_s = epoch - epoch_tai;
+assert_eq!(format!("{num_leap_s}"), "32 s");
+
+// Trivially convert to another time scale
+// Either by grabbing a subdivision of time in that time scale
+assert_eq!(epoch.to_gpst_days(), 7359.623402777777); // Compare to the GPS time scale
+
+// Or by fetching the exact duration
+let mjd_offset = Duration::from_str("51603 days 14 h 58 min 33 s 184 ms 37 ns").unwrap();
+assert_eq!(epoch.to_mjd_tt_duration(), mjd_offset); // Compare to the modified Julian days in the Terrestrial Time time scale.
+```
 
-#[cfg(feature = "std")]
-{
-// Initialization from system time is only available when std feature is enabled
-let now = Epoch::now().unwrap();
-println!("{}", now);
-}
+In Python:
+```python
+>>> from hifitime import *
+>>> epoch = Epoch("2000-02-29T14:57:29.000000037 UTC")
+>>> epoch
+2000-02-29T14:57:29.000000037 UTC
+>>> epoch_tai = Epoch.init_from_gregorian_tai(2000, 2, 29, 14, 57, 29, 37)
+>>> epoch_tai
+2000-02-29T14:57:29.000000037 TAI
+>>> epoch.timedelta(epoch_tai)
+32 s
+>>> epoch.to_gpst_days()
+7359.623402777777
+>>> epoch.to_mjd_tt_duration()
+51603 days 14 h 58 min 33 s 184 ms 37 ns
+>>> 
+```
 
-let mut santa = Epoch::from_gregorian_utc_hms(2017, 12, 25, 01, 02, 14);
-assert_eq!(santa.to_mjd_utc_days(), 58112.043217592590);
-assert_eq!(santa.to_jde_utc_days(), 2458112.5432175924);
+**Hifitime provides several date time formats like RFC2822, ISO8601, or RFC3339.**
 
-assert_eq!(
-    santa + 3600 * Unit::Second,
-    Epoch::from_gregorian_utc_hms(2017, 12, 25, 02, 02, 14),
-    "Could not add one hour to Christmas"
-);
+```rust
+use hifitime::efmt::consts::{ISO8601, RFC2822, RFC3339};
+use hifitime::prelude::*;
 
+let epoch = Epoch::from_gregorian_utc(2000, 2, 29, 14, 57, 29, 37);
+// The default Display shows the UTC time scale
+assert_eq!(format!("{epoch}"), "2000-02-29T14:57:29.000000037 UTC");
+// Format it in RFC 2822
+let fmt = Formatter::new(epoch, RFC2822);
+assert_eq!(format!("{fmt}"), format!("Tue, 29 Feb 2000 14:57:29"));
+
+// Or in ISO8601
+let fmt = Formatter::new(epoch, ISO8601);
 assert_eq!(
-    santa + 60.0.minutes(),
-    Epoch::from_gregorian_utc_hms(2017, 12, 25, 02, 02, 14),
-    "Could not add one hour to Christmas"
+    format!("{fmt}"),
+    format!("2000-02-29T14:57:29.000000037 UTC")
 );
 
+// Which is somewhat similar to RFC3339
+let fmt = Formatter::new(epoch, RFC3339);
 assert_eq!(
-    santa + 1.hours(),
-    Epoch::from_gregorian_utc_hms(2017, 12, 25, 02, 02, 14),
-    "Could not add one hour to Christmas"
+    format!("{fmt}"),
+    format!("2000-02-29T14:57:29.000000037+00:00")
 );
-
-let dt = Epoch::from_gregorian_utc_hms(2017, 1, 14, 0, 31, 55);
-assert_eq!(dt, Epoch::from_str("2017-01-14T00:31:55 UTC").unwrap());
-// And you can print it too, although by default it will print in UTC
-assert_eq!(format!("{}", dt), "2017-01-14T00:31:55 UTC".to_string());
-
 ```
-### Time differences, time unit, and duration handling
 
-Comparing times will lead to a Duration type. Printing that will automatically select the unit.
+**Need some custom format? Hifitime also supports the C89 token, cf. [the documentation](https://docs.rs/hifitime/latest/hifitime/efmt/format/struct.Format.html).**
 
 ```rust
-use hifitime::{Epoch, Unit, Duration, TimeUnits};
+use core::str::FromStr;
+use hifitime::prelude::*;
 
-let at_midnight = Epoch::from_gregorian_utc_at_midnight(2020, 11, 2);
-let at_noon = Epoch::from_gregorian_utc_at_noon(2020, 11, 2);
-assert_eq!(at_noon - at_midnight, 12 * Unit::Hour);
-assert_eq!(at_noon - at_midnight, 1 * Unit::Day / 2);
-assert_eq!(at_midnight - at_noon, -1.days() / 2);
-
-let delta_time = at_noon - at_midnight;
-assert_eq!(format!("{}", delta_time), "12 h".to_string());
-// And we can multiply durations by a scalar...
-let delta2 = 2 * delta_time;
-assert_eq!(format!("{}", delta2), "1 days".to_string());
-// Or divide them by a scalar.
-assert_eq!(format!("{}", delta2 / 2.0), "12 h".to_string());
-
-// And of course, these comparisons account for differences in time scales
-let at_midnight_utc = Epoch::from_gregorian_utc_at_midnight(2020, 11, 2);
-let at_noon_tai = Epoch::from_gregorian_tai_at_noon(2020, 11, 2);
-assert_eq!(format!("{}", at_noon_tai - at_midnight_utc), "11 h 59 min 23 s".to_string());
-```
+let epoch = Epoch::from_gregorian_utc_hms(2015, 2, 7, 11, 22, 33);
 
-Timeunits and frequency units are trivially supported. Hifitime only supports up to nanosecond precision (but guarantees it for 64 millenia), so any duration less than one nanosecond is truncated.
+// Parsing with a custom format
+assert_eq!(
+    Epoch::from_format_str("Sat, 07 Feb 2015 11:22:33", "%a, %d %b %Y %H:%M:%S").unwrap(),
+    epoch
+);
+
+// And printing with a custom format
+let fmt = Format::from_str("%a, %d %b %Y %H:%M:%S").unwrap();
+assert_eq!(
+    format!("{}", Formatter::new(epoch, fmt)),
+    "Sat, 07 Feb 2015 11:22:33"
+);
+```
 
+**You can also grab the current system time in UTC, if the `std` feature is enabled (default), and find the next or previous day of the week.**
 ```rust
-use hifitime::{Epoch, Unit, Freq, Duration, TimeUnits};
+use hifitime::prelude::*;
 
-// One can compare durations
-assert!(10.seconds() > 5.seconds());
-assert!(10.days() + 1.nanoseconds() > 10.days());
-
-// Those durations are more precise than floating point since this is integer math in nanoseconds
-let d: Duration = 1.0.hours() / 3 - 20.minutes();
-assert!(d.abs() < Unit::Nanosecond);
-assert_eq!(3 * 20.minutes(), Unit::Hour);
-
-// And also frequencies but note that frequencies are converted to Durations!
-// So the duration of that frequency is compared, hence the following:
-assert!(10 * Freq::Hertz < 5 * Freq::Hertz);
-assert!(4 * Freq::MegaHertz > 5 * Freq::MegaHertz);
-
-// And asserts on the units themselves
-assert!(Freq::GigaHertz < Freq::MegaHertz);
-assert!(Unit::Second > Unit::Millisecond);
+#[cfg(feature = "std")]
+{
+    let now = Epoch::now().unwrap();
+    println!("{}", now.next(Weekday::Tuesday));
+    println!("{}", now.previous(Weekday::Sunday));
+}
 ```
 
-### Iterating over times ("linspace" of epochs)
-Finally, something which may come in very handy, line spaces between times with a given step.
+**Oftentimes, we'll want to query something at a fixed step between two epochs. Hifitime makes this trivial with `TimeSeries`.**
 
 ```rust
-use hifitime::{Epoch, Unit, TimeSeries};
+use hifitime::prelude::*;
+
 let start = Epoch::from_gregorian_utc_at_midnight(2017, 1, 14);
-let end = Epoch::from_gregorian_utc_at_noon(2017, 1, 14);
-let step = 2 * Unit::Hour;
+let end = start + 12.hours();
+let step = 2.hours();
+
 let time_series = TimeSeries::inclusive(start, end, step);
 let mut cnt = 0;
 for epoch in time_series {
+    #[cfg(feature = "std")]
     println!("{}", epoch);
     cnt += 1
 }
-// Check that there are indeed six two-hour periods in a half a day,
+// Check that there are indeed seven two-hour periods in a half a day,
 // including start and end times.
 assert_eq!(cnt, 7)
 ```
 
+In Python:
+```python
+>>> from hifitime import *
+>>> start = Epoch.init_from_gregorian_utc_at_midnight(2017, 1, 14)
+>>> end = start + Unit.Hour*12
+>>> iterator = TimeSeries(start, end, step=Unit.Hour*2, inclusive=True)
+>>> for epoch in iterator:
+...     print(epoch)
+... 
+2017-01-14T00:00:00 UTC
+2017-01-14T02:00:00 UTC
+2017-01-14T04:00:00 UTC
+2017-01-14T06:00:00 UTC
+2017-01-14T08:00:00 UTC
+2017-01-14T10:00:00 UTC
+2017-01-14T12:00:00 UTC
+>>> 
+
+```
+
+### Duration
+
+```rust
+use hifitime::prelude::*;
+use core::str::FromStr;
+
+// Create a duration using the `TimeUnits` helping trait.
+let d = 5.minutes() + 7.minutes() + 35.nanoseconds();
+assert_eq!(format!("{d}"), "12 min 35 ns");
+
+// Or using the built-in enums
+let d_enum = 12 * Unit::Minute + 35.0 * Unit::Nanosecond;
+
+// But it can also be created from a string
+let d_from_str = Duration::from_str("12 min 35 ns").unwrap();
+assert_eq!(d, d_from_str);
+```
+
+**Hifitime guarantees nanosecond precision, but most human applications don't care too much about that. Durations can be rounded to provide a useful approximation for humans.**
+
+```rust
+use hifitime::prelude::*;
+
+// Create a duration using the `TimeUnits` helping trait.
+let d = 5.minutes() + 7.minutes() + 35.nanoseconds();
+// Round to the nearest minute
+let rounded = d.round(1.minutes());
+assert_eq!(format!("{rounded}"), "12 min");
+
+// And this works on Epochs as well.
+let previous_post = Epoch::from_gregorian_utc_hms(2015, 2, 7, 11, 22, 33);
+let example_now = Epoch::from_gregorian_utc_hms(2015, 8, 17, 22, 55, 01);
+
+// We'll round to the nearest fifteen days
+let this_much_ago = example_now - previous_post;
+assert_eq!(format!("{this_much_ago}"), "191 days 11 h 32 min 29 s");
+let about_this_much_ago_floor = this_much_ago.floor(15.days());
+assert_eq!(format!("{about_this_much_ago_floor}"), "180 days");
+let about_this_much_ago_ceil = this_much_ago.ceil(15.days());
+assert_eq!(format!("{about_this_much_ago_ceil}"), "195 days");
+```
+
+In Python:
+
+```python
+>>> from hifitime import *
+>>> d = Duration("12 min 32 ns")
+>>> d.round(Unit.Minute*1)
+12 min
+>>> d
+12 min 32 ns
+>>> 
+```
+
+[![hifitime on crates.io][cratesio-image]][cratesio]
+[![hifitime on docs.rs][docsrs-image]][docsrs]
+[![minimum rustc: 1.64](https://img.shields.io/badge/minimum%20rustc-1.64-yellowgreen?logo=rust)](https://www.whatrustisit.com)
+[![Build Status](https://github.com/nyx-space/hifitime/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/nyx-space/hifitime/actions)
+[![Build Status](https://github.com/nyx-space/hifitime/actions/workflows/formal_verification.yml/badge.svg?branch=master)](https://github.com/nyx-space/hifitime/actions)
+[![codecov](https://codecov.io/gh/nyx-space/hifitime/branch/master/graph/badge.svg?token=l7zU57rUGs)](https://codecov.io/gh/nyx-space/hifitime)
+
+[cratesio-image]: https://img.shields.io/crates/v/hifitime.svg
+[cratesio]: https://crates.io/crates/hifitime
+[docsrs-image]: https://docs.rs/hifitime/badge.svg
+[docsrs]: https://docs.rs/hifitime/
+
+# Comparison with `time` and `chrono`
+
+First off, both `time` and `chrono` are fantastic libraries in their own right. There's a reason why they have millions and millions of downloads. Secondly, hifitime was started in October 2017, so quite a while before the revival of `time` (~ 2019).
+
+One of the key differences is that both `chrono` and `time` separate the concepts of "time" and "date." Hifitime asserts that this is physically invalid: both a time and a date are an offset from a reference in a given time scale. That's why, Hifitime does not separate the components that make up a date, but instead, only stores a fixed duration with respect to TAI. Moreover, Hifitime is formally verified with a model checker, which is much more thorough than property testing.
+
+More importantly, neither `time` nor `chrono` are suitable for astronomy, astrodynamics, or any physics that must account for time dilation due to relativistic speeds or lack of the Earth as a gravity source (which sets the "tick" of a second).
+
+Hifitime also natively supports the UT1 time scale (the only "true" time) if built with the `ut1` feature.
+
+# Features
+
+ * [x] Initialize a high precision Epoch from the system time in UTC
+ * [x] Leap seconds (as announced by the IETF on a yearly basis)
+ * [x] UTC representation with ISO8601 and RFC3339 formatting and blazing fast parsing (45 nanoseconds)
+ * [x] Trivial support of time arithmetic: addition (e.g. `2.hours() + 3.seconds()`), subtraction (e.g. `2.hours() - 3.seconds()`), round/floor/ceil operations (e.g. `2.hours().round(3.seconds())`)
+ * [x] Supports ranges of Epochs and TimeSeries (linspace of `Epoch`s and `Duration`s)
+ * [x] Trivial conversion between many time scales
+ * [x] High fidelity Ephemeris Time / Dynamic Barycentric Time (TDB) computations from [ESA's Navipedia](https://gssc.esa.int/navipedia/index.php/Transformations_between_Time_Systems#TDT_-_TDB.2C_TCB)
+ * [x] Julian dates and Modified Julian dates
+ * [x] Embedded device friendly: `no-std` and `const fn` where possible
+
+This library is validated against NASA/NAIF SPICE for the Ephemeris Time to Universal Coordinated Time computations: there are exactly zero nanoseconds of difference between SPICE and hifitime for the computation of ET and UTC after 01 January 1972. Refer to the [leap second](#leap-second-support) section for details. Other examples are validated with external references, as detailed on a test-by-test basis.
+
+## Supported time scales
+
++ Temps Atomique International (TAI)
++ Universal Coordinated Time (UTC)
++ Terrestrial Time (TT)
++ Ephemeris Time (ET) without the small perturbations as per NASA/NAIF SPICE leap seconds kernel
++ Dynamic Barycentric Time (TDB), a higher fidelity ephemeris time
++ Global Positioning System (GPST)
++ Galileo System Time (GST)
++ BeiDou Time (BDT)
++ UNIX
+## Non-features
+* Time-agnostic / date-only epochs. Hifitime only supports the combination of date and time, but the `Epoch::{at_midnight, at_noon}` is provided as helper functions.
+
 # Design
-No software is perfect, so please report any issue or bugs on [Github](https://github.com/nyx-space/hifitime/issues/new).
+No software is perfect, so please report any issue or bug on [Github](https://github.com/nyx-space/hifitime/issues/new).
 
 ## Duration
 Under the hood, a Duration is represented as a 16 bit signed integer of centuries (`i16`) and a 64 bit unsigned integer (`u64`) of the nanoseconds past that century. The overflowing and underflowing of nanoseconds is handled by changing the number of centuries such that the nanoseconds number never represents more than one century (just over four centuries can be stored in 64 bits).
 
 Advantages:
 1. Exact precision of a duration: using a floating point value would cause large durations (e.g. Julian Dates) to have less precision than smaller durations. Durations in hifitime have exactly one nanosecond of precision for 65,536 years.
 2. Skipping floating point operations allows this library to be used in embedded devices without a floating point unit.
 3. Duration arithmetics are exact, e.g. one third of an hour is exactly twenty minutes and not "0.33333 hours."
 
 Disadvantages:
 1. Most astrodynamics applications require the computation of a duration in floating point values such as when querying an ephemeris. This design leads to an overhead of about 5.2 nanoseconds according to the benchmarks (`Duration to f64 seconds` benchmark). You may run the benchmarks with `cargo bench`.
 
-### Printing and parsing
-
-When Durations are printed, only the units whose value is non-zero is printed. For example, `5.hours() + 256.0.milliseconds() + 1.0.nanoseconds()` will be printed as "5 h 256 ms 1 ns".
-
-```rust
-use hifitime::{Duration, Unit, TimeUnits};
-use core::str::FromStr;
-
-assert_eq!(
-    format!(
-        "{}",
-        5.hours() + 256.0.milliseconds() + 1.0.nanoseconds()
-    ),
-    "5 h 256 ms 1 ns"
-);
-
-assert_eq!(
-    format!(
-        "{}",
-        5.days() + 1.0.nanoseconds()
-    ),
-    "5 days 1 ns"
-);
-
-
-assert_eq!(
-    Duration::from_str("5 h 256 ms 1 ns").unwrap(),
-    5 * Unit::Hour + 256 * Unit::Millisecond + Unit::Nanosecond
-);
-```
-
 ## Epoch
 The Epoch is simply a wrapper around a Duration. All epochs are stored in TAI duration with respect to 01 January 1900 at noon (the official TAI epoch). The choice of TAI meets the [Standard of Fundamental Astronomy (SOFA)](https://www.iausofa.org/) recommendation of opting for a glitch-free time scale (i.e. without discontinuities like leap seconds or non-uniform seconds like TDB).
 
 ### Printing and parsing
 
 Epochs can be formatted and parsed in the following time scales:
 
@@ -220,58 +287,14 @@
 + TAI: `{epoch:x}`
 + TT: `{epoch:X}`
 + TDB: `{epoch:e}`
 + ET: `{epoch:E}`
 + UNIX: `{epoch:p}`
 + GPS: `{epoch:o}`
 
-```rust
-use hifitime::{Epoch, TimeScale};
-use core::str::FromStr;
-
-let epoch = Epoch::from_gregorian_utc_hms(2022, 9, 6, 23, 24, 29);
-
-assert_eq!(format!("{epoch}"), "2022-09-06T23:24:29 UTC");
-assert_eq!(format!("{epoch:x}"), "2022-09-06T23:25:06 TAI");
-assert_eq!(format!("{epoch:X}"), "2022-09-06T23:25:38.184000000 TT");
-assert_eq!(format!("{epoch:E}"), "2022-09-06T23:25:38.182538909 ET");
-assert_eq!(format!("{epoch:e}"), "2022-09-06T23:25:38.182541259 TDB");
-assert_eq!(format!("{epoch:p}"), "1662506669"); // UNIX seconds
-assert_eq!(format!("{epoch:o}"), "1346541887000000000"); // GPS nanoseconds
-
-// RFC3339 parsing with time scales
-assert_eq!(
-    Epoch::from_gregorian_utc_hms(1994, 11, 5, 13, 15, 30),
-    Epoch::from_str("1994-11-05T08:15:30-05:00").unwrap()
-);
-assert_eq!(
-    Epoch::from_gregorian_utc_hms(1994, 11, 5, 13, 15, 30),
-    Epoch::from_str("1994-11-05T13:15:30Z").unwrap()
-);
-// Same test with different time systems
-// TAI
-assert_eq!(
-    Epoch::from_gregorian_tai_hms(1994, 11, 5, 13, 15, 30),
-    Epoch::from_str("1994-11-05T08:15:30-05:00 TAI").unwrap()
-);
-assert_eq!(
-    Epoch::from_gregorian_tai_hms(1994, 11, 5, 13, 15, 30),
-    Epoch::from_str("1994-11-05T13:15:30Z TAI").unwrap()
-);
-// TDB
-assert_eq!(
-    Epoch::from_gregorian_hms(1994, 11, 5, 13, 15, 30, TimeScale::TDB),
-    Epoch::from_str("1994-11-05T08:15:30-05:00 TDB").unwrap()
-);
-assert_eq!(
-    Epoch::from_gregorian_hms(1994, 11, 5, 13, 15, 30, TimeScale::TDB),
-    Epoch::from_str("1994-11-05T13:15:30Z TDB").unwrap()
-);
-```
-
 ## Leap second support
 
 Leap seconds allow TAI (the absolute time reference) and UTC (the civil time reference) to not drift too much. In short, UTC allows humans to see the sun at zenith at noon, whereas TAI does not worry about that. Leap seconds are introduced to allow for UTC to catch up with the absolute time reference of TAI. Specifically, UTC clocks are "stopped" for one second to make up for the accumulated difference between TAI and UTC. These leap seconds are announced several months in advance by IERS, cf. in the [IETF leap second reference](https://www.ietf.org/timezones/data/leap-seconds.list).
 
 The "placement" of these leap seconds in the formatting of a UTC date is left up to the software: there is no common way to handle this. Some software prevents a second tick, i.e. at 23:59:59 the UTC clock will tick for _two seconds_ (instead of one) before hoping to 00:00:00. Some software, like hifitime, allow UTC dates to be formatted as 23:59:60 on strictly the days when a leap second is inserted. For example, the date `2016-12-31 23:59:60 UTC` is a valid date in hifitime because a leap second was inserted on 01 Jan 2017.
 
 ### Important
@@ -282,14 +305,22 @@
 > Equation \[4\], which ignores small-period fluctuations, is accurate to about 0.000030 seconds.
 
 In order to provide full interoperability with NAIF, hifitime uses the NAIF algorithm for "ephemeris time" and the [ESA algorithm](https://gssc.esa.int/navipedia/index.php/Transformations_between_Time_Systems#TDT_-_TDB.2C_TCB) for "dynamical barycentric time." Hence, if exact NAIF behavior is needed, use all of the functions marked as `et` instead of the `tdb` functions, such as `epoch.to_et_seconds()` instead of `epoch.to_tdb_seconds()`.
 
 
 # Changelog
 
+## 3.8.2
++ Clarify README and add a section comparing Hifitime to `time` and `chrono`, cf. [#221](https://github.com/nyx-space/hifitime/issues/221)
++ Fix incorrect printing of Gregorian dates prior to to 1900, cf. [#204](https://github.com/nyx-space/hifitime/issues/204)
+
+## 3.8.1 (unreleased)
++ Fix documentation for the formatter, cf. [#202](https://github.com/nyx-space/hifitime/pull/202)
++ Update MSRV to 1.59 for rayon v 1.10
+
 ## 3.8.0
 Thanks again to [@gwbres](https://github.com/gwbres) for his work in this release!
 
 + Fix CI of the formal verification and upload artifacts, cf. [#179](https://github.com/nyx-space/hifitime/pull/179)
 + Introduce time of week construction and conversion by [@gwbres](https://github.com/gwbres), cf.[#180](https://github.com/nyx-space/hifitime/pull/180) and [#188](https://github.com/nyx-space/hifitime/pull/188)
 + Fix minor typo in `src/timeunits.rs` by [@gwbres](https://github.com/gwbres), cf. [#189](https://github.com/nyx-space/hifitime/pull/189)
 + Significantly extend formal verification of `Duration` and `Epoch`, and introduce `kani::Arbitrary` to `Duration` and `Epoch` for users to formally verify their use of time, cf. [#192](https://github.com/nyx-space/hifitime/pull/192)
@@ -359,12 +390,7 @@
 + Allow building an `Epoch` from its duration and parts in TAI system
 + Add pure nanosecond (`u64`) constructor and getter for GPST since GPS based clocks will count in nanoseconds
 ### Possibly breaking change
 + `Errors::ParseError` no longer contains a `String` but an enum `ParsingErrors` instead. This is considered possibly breaking because it would only break code in the cases where a datetime parsing or unit parsing was caught and handled (uncommon). Moreover, the output is still `Display`-able.
 ## 3.0.0
 + Backend rewritten from TwoFloat to a struct of the centuries in `i16` and nanoseconds in `u64`. Thanks to [@pwnorbitals](https://github.com/pwnorbitals) for proposing the idea in #[107](https://github.com/nyx-space/hifitime/issues/107) and writing the proof of concept. This leads to at least a 2x speed up in most calculations, cf. [this comment](https://github.com/nyx-space/hifitime/pull/107#issuecomment-1040702004).
 + Fix GPS epoch, and addition of a helper functions in `Epoch` by [@cjordan](https://github.com/cjordan)
-
-## 2.2.3
-+ More deterministic `as_jde_tdb_days()` in `Epoch`. In version 2.2.1, the ephemeris time and TDB _days_ were identical down to machine precision. After a number of validation cases in the rotation equations of the IAU Earth to Earth Mean Equator J2000 frame, the new formulation was shown to lead to less rounding errors when requesting the days. These rounding errors prevented otherwise trivial test cases. However, it adds an error of **40.2 nanoseconds** when initializing an Epoch with the days in ET and requesting the TDB days.
-
-_Note:_ this was originally published as 2.2.2 but I'd forgotten to update one of the tests with the 40.2 ns error.
```

### Comparing `hifitime-3.8.0/benches/bench_duration.rs` & `hifitime-3.8.1/benches/crit_duration.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/benches/bench_epoch.rs` & `hifitime-3.8.1/benches/crit_epoch.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/benches/iai_duration.rs` & `hifitime-3.8.1/benches/iai_duration.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/benches/iai_epoch.rs` & `hifitime-3.8.1/benches/iai_epoch.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/examples/python/basic.py` & `hifitime-3.8.1/examples/python/basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-'''
+"""
  * Hifitime, part of the Nyx Space tools
  * Copyright (C) 2022 Christopher Rabotin <christopher.rabotin@gmail.com> et al. (cf. AUTHORS.md)
  * This Source Code Form is subject to the terms of the Apache
  * v. 2.0. If a copy of the Apache License was not distributed with this
  * file, You can obtain one at https://www.apache.org/licenses/LICENSE-2.0.
  *
  * Documentation: https://nyxspace.com/
-'''
+"""
 
 from hifitime import Duration, Epoch, TimeSeries, TimeScale, Unit
 
 if __name__ == "__main__":
     # All of the functions available in Rust are also available in Python.
     # However, functions that initialize a new Epoch or Duration had to be renamed: `Epoch::from_blah` becomes `Epoch.init_from_blah` in Python.
 
@@ -26,30 +26,35 @@
     print(f"TDB epoch: {e.to_string_gregorian(TimeScale.TDB)}")
 
     # Hifitime mainly allows for nanosecond precision of durations for 64 centuries (centered on J1900).
     print(f"min negative = {Duration.min_negative()}")
     print(f"min positive = {Duration.min_positive()}")
 
     # And more importantly, it does not suffer from rounding issues, even when the duration are very large.
-    print(f"Max duration: {Duration.max()}")    # 1196851200 days
+    print(f"Max duration: {Duration.max()}")  # 1196851200 days
     print(f"Nanosecond precision: {Duration.max() - Unit.Nanosecond * 1.0}")
     assert f"{Unit.Day * 1.2}" == "1 days 4 h 48 min"
     assert f"{Unit.Day * 1.200001598974}" == "1 days 4 h 48 min 138 ms 151 μs 353 ns"
 
     # It also saturates the duration
     print(f"Saturated add: {Duration.max() + Unit.Day * 1.0}")
 
     # You can also get all of the epochs between two different epochs at a specific step size.
     # This is like numpy's `linspace` with high fidelity durations
-    time_series = TimeSeries(Epoch.system_now(),
-                             Epoch.system_now() + Unit.Day * 0.3,
-                             Unit.Hour * 0.5,
-                             inclusive=True)
+    time_series = TimeSeries(
+        Epoch.system_now(),
+        Epoch.system_now() + Unit.Day * 0.3,
+        Unit.Hour * 0.5,
+        inclusive=True,
+    )
     print(time_series)
-    for (num, epoch) in enumerate(time_series):
+    for num, epoch in enumerate(time_series):
         print(f"#{num}:\t{epoch}")
 
     e1 = Epoch.system_now()
     e3 = e1 + Unit.Day * 1.5998
     epoch_delta = e3.timedelta(e1)
-    assert epoch_delta == Unit.Day * 1 + Unit.Hour * 14 + Unit.Minute * 23 + Unit.Second * 42.720
-    print(epoch_delta)
+    assert (
+        epoch_delta
+        == Unit.Day * 1 + Unit.Hour * 14 + Unit.Minute * 23 + Unit.Second * 42.720
+    )
+    print(epoch_delta)
```

### Comparing `hifitime-3.8.0/examples/python/timescales.py` & `hifitime-3.8.1/examples/python/timescales.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,97 @@
-'''
+"""
  * Hifitime, part of the Nyx Space tools
  * Copyright (C) 2022 Christopher Rabotin <christopher.rabotin@gmail.com> et al. (cf. AUTHORS.md)
  * This Source Code Form is subject to the terms of the Apache
  * v. 2.0. If a copy of the Apache License was not distributed with this
  * file, You can obtain one at https://www.apache.org/licenses/LICENSE-2.0.
  *
  * Documentation: https://nyxspace.com/
-'''
+"""
 
 try:
     import plotly.express as px
 except ImportError:
-    print('\nThis script requires `plotly` (pip install plotly)\n')
+    print("\nThis script requires `plotly` (pip install plotly)\n")
 
 try:
     import pandas as pd
 except ImportError:
-    print('\nThis script requires `pandas` (pip install pandas)\n')
+    print("\nThis script requires `pandas` (pip install pandas)\n")
 
 from hifitime import Epoch, TimeSeries, Unit
 
 if __name__ == "__main__":
-    '''
+    """
     The purpose of this script is to plot the differences between time systems.
 
     It will plot the difference between TAI, UTC, and all of the other timescales supported by hifitime.
     Then, as a separate plot, it will remove the UTC line to make the difference between other timescales more evident.
-    '''
+    """
     # Start by building a time series from 1970 until 2023 with a step of 30 days.
-    ts = TimeSeries(Epoch('1970-01-01 00:00:00 UTC'), Epoch('2023-01-01 00:00:00 UTC'),
-                    Unit.Day * 30.0, True)
+    ts = TimeSeries(
+        Epoch("1970-01-01 00:00:00 UTC"),
+        Epoch("2023-01-01 00:00:00 UTC"),
+        Unit.Day * 30.0,
+        True,
+    )
 
     # Define the storage array
     data = []
     # Define the columns
-    columns = ["UTC Epoch", "Δ TT (s)", "Δ ET (s)", "Δ TDB (s)", "Δ UTC (s)", "ET-TDB (s)"]
+    columns = [
+        "UTC Epoch",
+        "Δ TT (s)",
+        "Δ ET (s)",
+        "Δ TDB (s)",
+        "Δ UTC (s)",
+        "ET-TDB (s)",
+    ]
 
     for epoch in ts:
         delta_utc = epoch.to_utc_duration() - epoch.to_tai_duration()
         delta_tt = epoch.to_tt_duration() - epoch.to_tai_duration()
         delta_tdb = epoch.to_tdb_duration_since_j1900() - epoch.to_tai_duration()
         delta_et = epoch.to_et_duration_since_j1900() - epoch.to_tai_duration()
         delta_et_tdb = delta_et - delta_tdb
         # Convert the epoch into a pandas datetime
         pd_epoch = pd.to_datetime(str(epoch))
         # Build the pandas series
-        data.append([
-            pd_epoch,
-            delta_tt.to_seconds(),
-            delta_et.to_seconds(),
-            delta_tdb.to_seconds(),
-            delta_utc.to_seconds(),
-            delta_et_tdb.to_seconds(),
-        ])
+        data.append(
+            [
+                pd_epoch,
+                delta_tt.to_seconds(),
+                delta_et.to_seconds(),
+                delta_tdb.to_seconds(),
+                delta_utc.to_seconds(),
+                delta_et_tdb.to_seconds(),
+            ]
+        )
 
     df = pd.DataFrame(data, columns=columns)
 
-    fig = px.line(df,
-                  x='UTC Epoch',
-                  y=columns[1:-1],
-                  title="Time scale deviation with respect to TAI")
+    fig = px.line(
+        df,
+        x="UTC Epoch",
+        y=columns[1:-1],
+        title="Time scale deviation with respect to TAI",
+    )
     fig.write_html("./target/time-scale-deviation.html")
     fig.show()
 
-    fig = px.line(df,
-                  x='UTC Epoch',
-                  y=columns[1:-2],
-                  title="Time scale deviation with respect to TAI (excl. UTC)")
+    fig = px.line(
+        df,
+        x="UTC Epoch",
+        y=columns[1:-2],
+        title="Time scale deviation with respect to TAI (excl. UTC)",
+    )
     fig.write_html("./target/time-scale-deviation-no-utc.html")
     fig.show()
 
-    fig = px.line(df,
-                  x='UTC Epoch',
-                  y=columns[-1],
-                  title="Time scale deviation of TDB and ET with respect to TAI")
+    fig = px.line(
+        df,
+        x="UTC Epoch",
+        y=columns[-1],
+        title="Time scale deviation of TDB and ET with respect to TAI",
+    )
     fig.write_html("./target/time-scale-deviation-tdb-et.html")
-    fig.show()
+    fig.show()
```

### Comparing `hifitime-3.8.0/naif0012.txt` & `hifitime-3.8.1/naif0012.txt`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/src/asn1der.rs` & `hifitime-3.8.1/src/asn1der.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/src/deprecated.rs` & `hifitime-3.8.1/src/deprecated.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/src/duration.rs` & `hifitime-3.8.1/src/duration.rs`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,18 @@
 #[cfg(feature = "serde")]
 use serde_derive::{Deserialize, Serialize};
 
 use core::str::FromStr;
 
 #[cfg(feature = "python")]
 use pyo3::prelude::*;
-
 #[cfg(feature = "python")]
 use pyo3::pyclass::CompareOp;
+#[cfg(feature = "python")]
+use pyo3::types::PyType;
 
 #[cfg(not(feature = "std"))]
 use num_traits::Float;
 
 #[cfg(kani)]
 use kani::Arbitrary;
 
@@ -108,15 +109,15 @@
 
 impl Default for Duration {
     fn default() -> Self {
         Duration::ZERO
     }
 }
 
-// Defines the methods that should be staticmethods in Python, but must be redefined as per https://github.com/PyO3/pyo3/issues/1003#issuecomment-844433346
+// Defines the methods that should be classmethods in Python, but must be redefined as per https://github.com/PyO3/pyo3/issues/1003#issuecomment-844433346
 impl Duration {
     /// Builds a new duration from the number of centuries and the number of nanoseconds
     #[must_use]
     #[deprecated(note = "Prefer from_parts()", since = "3.6.0")]
     pub fn new(centuries: i16, nanoseconds: u64) -> Self {
         let mut out = Self {
             centuries,
@@ -355,15 +356,15 @@
                     }
                 }
                 None => Err(Errors::Overflow),
             }
         } else {
             // Centuries negative by a decent amount
             Ok(
-                i64::from(self.centuries + 1) * NANOSECONDS_PER_CENTURY as i64
+                i64::from(self.centuries) * NANOSECONDS_PER_CENTURY as i64
                     + self.nanoseconds as i64,
             )
         }
     }
 
     /// Returns the truncated nanoseconds in a signed 64 bit integer, if the duration fits.
     /// WARNING: This function will NOT fail and will return the i64::MIN or i64::MAX depending on
@@ -739,62 +740,63 @@
             CompareOp::Ge => *self >= other,
         }
     }
 
     // Python constructors
 
     #[cfg(feature = "python")]
-    #[staticmethod]
-    fn zero() -> Duration {
+    #[classmethod]
+    fn zero(_cls: &PyType) -> Duration {
         Duration::ZERO
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
-    fn epsilon() -> Duration {
+    #[classmethod]
+    fn epsilon(_cls: &PyType) -> Duration {
         Duration::EPSILON
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
-    fn init_from_max() -> Duration {
+    #[classmethod]
+    fn init_from_max(_cls: &PyType) -> Duration {
         Duration::MAX
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
-    fn init_from_min() -> Duration {
+    #[classmethod]
+    fn init_from_min(_cls: &PyType) -> Duration {
         Duration::MIN
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
-    fn min_positive() -> Duration {
+    #[classmethod]
+    fn min_positive(_cls: &PyType) -> Duration {
         Duration::MIN_POSITIVE
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
-    fn min_negative() -> Duration {
+    #[classmethod]
+    fn min_negative(_cls: &PyType) -> Duration {
         Duration::MIN_NEGATIVE
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Create a normalized duration from its parts
-    fn init_from_parts(centuries: i16, nanoseconds: u64) -> Self {
+    fn init_from_parts(_cls: &PyType, centuries: i16, nanoseconds: u64) -> Self {
         Self::from_parts(centuries, nanoseconds)
     }
 
     /// Creates a new duration from its parts
     #[allow(clippy::too_many_arguments)]
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     #[must_use]
     fn init_from_all_parts(
+        _cls: &PyType,
         sign: i8,
         days: u64,
         hours: u64,
         minutes: u64,
         seconds: u64,
         milliseconds: u64,
         microseconds: u64,
@@ -809,23 +811,23 @@
             milliseconds,
             microseconds,
             nanoseconds,
         )
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
-    fn init_from_total_nanoseconds(nanos: i128) -> Self {
+    #[classmethod]
+    fn init_from_total_nanoseconds(_cls: &PyType, nanos: i128) -> Self {
         Self::from_total_nanoseconds(nanos)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Create a new duration from the truncated nanoseconds (+/- 2927.1 years of duration)
-    fn init_from_truncated_nanoseconds(nanos: i64) -> Self {
+    fn init_from_truncated_nanoseconds(_cls: &PyType, nanos: i64) -> Self {
         Self::from_truncated_nanoseconds(nanos)
     }
 }
 
 impl Mul<i64> for Duration {
     type Output = Duration;
     fn mul(self, q: i64) -> Self::Output {
@@ -1539,53 +1541,71 @@
 
         let recip_ns = dur_from_part.try_truncated_nanoseconds().unwrap();
         assert_eq!(recip_ns, expect_rslt);
     } else if centuries < 0 {
         // We fit on a i64 but we need to account for the number of nanoseconds wrapped to the negative centuries.
 
         let nanos = u_ns.rem_euclid(NANOSECONDS_PER_CENTURY);
-        let expect_rslt = i64::from(centuries + 1) * NANOSECONDS_PER_CENTURY as i64 + nanos as i64;
+        let expect_rslt = i64::from(centuries) * NANOSECONDS_PER_CENTURY as i64 + nanos as i64;
 
         let recip_ns = dur_from_part.try_truncated_nanoseconds().unwrap();
         assert_eq!(recip_ns, expect_rslt);
     } else {
         // Positive duration but enough to fit on an i64.
         let recip_ns = dur_from_part.try_truncated_nanoseconds().unwrap();
 
         assert_eq!(recip_ns, nanoseconds);
     }
 }
 
-// #[cfg(kani)]
-// #[kani::proof]
-#[test]
-fn formal_duration_seconds() {
-    // let seconds: f64 = kani::any();
-    let seconds =
-        f64::from_bits(0b01000000010111111011010000110111101001100000110111100000_00000001);
-
-    // kani::assume(seconds > 1e-9);
-    // kani::assume(seconds < 1e14);
-
-    if seconds.is_finite() {
-        let big_seconds = seconds * 1e9;
-        let floored = big_seconds.floor();
-        // Remove the sub nanoseconds -- but this can lead to rounding errors!
-        let truncated_ns = floored * 1e-9;
-
-        let duration: Duration = Duration::from_seconds(truncated_ns);
-        let truncated_out = duration.to_seconds();
-        let floored_out = truncated_out * 1e9;
-        // So we check that the data times 1e9 matches the rounded data
-        if floored != floored_out {
-            let floored_out_bits = floored_out.to_bits();
-            let floored_bits = floored.to_bits();
-            // Allow for ONE bit error on the LSB
-            if floored_out_bits > floored_bits {
-                assert_eq!(floored_out_bits - floored_bits, 1);
-            } else {
-                assert_eq!(floored_bits - floored_out_bits, 1);
+#[cfg(kani)]
+mod tests {
+    use super::*;
+
+    macro_rules! repeat_test {
+        ($test_name:ident, $bounds:expr) => {
+            #[kani::proof]
+            fn $test_name() {
+                for pair in $bounds.windows(2) {
+                    let seconds: f64 = kani::any();
+
+                    kani::assume(seconds > pair[0]);
+                    kani::assume(seconds < pair[1]);
+
+                    if seconds.is_finite() {
+                        let big_seconds = seconds * 1e9;
+                        let floored = big_seconds.floor();
+                        // Remove the sub nanoseconds -- but this can lead to rounding errors!
+                        let truncated_ns = floored * 1e-9;
+
+                        let duration: Duration = Duration::from_seconds(truncated_ns);
+                        let truncated_out = duration.to_seconds();
+                        let floored_out = truncated_out * 1e9;
+
+                        // So we check that the data times 1e9 matches the rounded data
+                        if floored != floored_out {
+                            let floored_out_bits = floored_out.to_bits();
+                            let floored_bits = floored.to_bits();
+
+                            // Allow for ONE bit error on the LSB
+                            if floored_out_bits > floored_bits {
+                                assert_eq!(floored_out_bits - floored_bits, 1);
+                            } else {
+                                assert_eq!(floored_bits - floored_out_bits, 1);
+                            }
+                        } else {
+                            assert_eq!(floored_out, floored);
+                        }
+                    }
+                }
             }
-        }
-        assert_eq!(floored_out, floored);
+        };
     }
+
+    repeat_test!(test_dur_f64_recip_0, [1e-9, 1e-8, 1e-7, 1e-6, 1e-5]);
+    repeat_test!(test_dur_f64_recip_1, [1e-5, 1e-4, 1e-3]);
+    // repeat_test!(test_dur_f64_recip_2, [1e-2, 1e-1, 1e0]);
+    // repeat_test!(test_dur_f64_recip_3, [1e0, 1e1, 1e2]);
+    // repeat_test!(test_dur_f64_recip_4, [1e2, 1e3, 1e4]);
+    // repeat_test!(test_dur_f64_recip_5, [1e4, 1e5]);
+    // repeat_test!(test_dur_f64_recip_6, [1e5, 1e6]);
 }
```

### Comparing `hifitime-3.8.0/src/efmt/consts.rs` & `hifitime-3.8.1/src/efmt/consts.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/src/efmt/format.rs` & `hifitime-3.8.1/src/efmt/format.rs`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 /// | `%m` | Month number, zero-padded to 2 digits | `03` for March | N/A |
 /// | `%b` | Month name in short form | `Mar` for March | N/A |
 /// | `%B` | Month name in long form | `March` | N/A |
 /// | `%d` | Day number, zero-padded to 2 digits | `07` for the 7th day of the month | N/A |
 /// | `%j` | Day of year, zero-padded to 3 digits | `059` for 29 February 2000 | N/A |
 /// | `%A` | Weekday name in long form | `Monday` | N/A |
 /// | `%a` | Weekday name in short form | `Mon` for Monday | N/A |
-/// | `%H` | Minute number, zero-padded to 2 digits | `39` for the 39th minutes of the hour | N/A |
+/// | `%H` | Hour number, zero-padded to 2 digits | `02` for the 2nd hour of the day | N/A |
+/// | `%M` | Minute number, zero-padded to 2 digits | `39` for the 39th minutes of the hour | N/A |
 /// | `%S` | Seconds, zero-padded to 2 digits | `27` for the 27th second of the minute | N/A |
 /// | `%f` | Sub-seconds, zero-padded to 9 digits | `000000007` for the 7th nanosecond past the second | (2) |
 /// | `%w` | Weekday in decimal form with C89 standard | `01` for Dynamical barycentric time | (3) |
 /// | `%z` | Offset timezone if the formatter is provided with an epoch. | `+15:00` For GMT +15 hours and zero minutes | N/A |
 ///
 /// * (1): Hifitime supports years from -34668 to 34668. If your epoch is larger than +/- 9999 years, the formatting of the years _will_ show all five digits of the year.
 /// * (2): Hifitime supports exactly nanosecond precision, and this is not lost when formatting.
```

### Comparing `hifitime-3.8.0/src/efmt/formatter.rs` & `hifitime-3.8.1/src/efmt/formatter.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/src/epoch.rs` & `hifitime-3.8.1/src/epoch.rs`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 #[cfg(feature = "python")]
 use pyo3::prelude::*;
 
 #[cfg(feature = "python")]
 use pyo3::pyclass::CompareOp;
 
 #[cfg(feature = "python")]
+use pyo3::types::PyType;
+
+#[cfg(feature = "python")]
 use crate::leap_seconds_file::LeapSecondsFile;
 
 #[cfg(feature = "serde")]
 use serde_derive::{Deserialize, Serialize};
 
 use core::str::FromStr;
 #[cfg(feature = "std")]
@@ -234,15 +237,15 @@
 impl Ord for Epoch {
     fn cmp(&self, other: &Self) -> Ordering {
         self.duration_since_j1900_tai
             .cmp(&other.duration_since_j1900_tai)
     }
 }
 
-// Defines the methods that should be staticmethods in Python, but must be redefined as per https://github.com/PyO3/pyo3/issues/1003#issuecomment-844433346
+// Defines the methods that should be classmethods in Python, but must be redefined as per https://github.com/PyO3/pyo3/issues/1003#issuecomment-844433346
 impl Epoch {
     /// Get the accumulated number of leap seconds up to this Epoch from the provided LeapSecondProvider.
     /// Returns None if the epoch is before 1960, year at which UTC was defined.
     ///
     /// # Why does this function return an `Option` when the other returns a value
     /// This is to match the `iauDat` function of SOFA (src/dat.c). That function will return a warning and give up if the start date is before 1960.
     pub fn leap_seconds_with<L: LeapSecondProvider>(
@@ -698,14 +701,15 @@
             // every 400 years we correct our correction. The first one before 1900 is 1600 (years_since_1900 = -300)
             // so we subtract 100 to correct the offset
             duration_wrt_1900 += Unit::Day * i64::from((years_since_1900 - 100) / 400);
         };
 
         // Add the seconds for the months prior to the current month
         duration_wrt_1900 += Unit::Day * i64::from(CUMULATIVE_DAYS_FOR_MONTH[(month - 1) as usize]);
+
         if is_leap_year(year) && month > 2 {
             // NOTE: If on 29th of February, then the day is not finished yet, and therefore
             // the extra seconds are added below as per a normal day.
             duration_wrt_1900 += Unit::Day;
         }
         duration_wrt_1900 += Unit::Day * i64::from(day - 1)
             + Unit::Hour * i64::from(hour)
@@ -1037,14 +1041,21 @@
     }
 
     /// Initializes an Epoch from the provided Format.
     pub fn from_str_with_format(s_in: &str, format: Format) -> Result<Self, Errors> {
         format.parse(s_in)
     }
 
+    /// Initializes an Epoch from the Format as a string.
+    pub fn from_format_str(s_in: &str, format_str: &str) -> Result<Self, Errors> {
+        Format::from_str(format_str)
+            .map_err(Errors::ParseError)?
+            .parse(s_in)
+    }
+
     #[cfg(feature = "ut1")]
     #[must_use]
     /// Initialize an Epoch from the provided UT1 duration since 1900 January 01 at midnight
     ///
     /// # Warning
     /// The time scale of this Epoch will be set to TAI! This is to ensure that no additional computations will change the duration since it's stored in TAI.
     /// However, this also means that calling `to_duration()` on this Epoch will return the TAI duration and not the UT1 duration!
@@ -1116,15 +1127,15 @@
             }
 
             if days_so_far + days_next_month > days_in_year || month == 12 {
                 // We've found the month and can calculate the days
                 day = if sign >= 0 {
                     days_in_year - days_so_far + 1.0
                 } else {
-                    days_in_year - days_so_far - 1.0
+                    days_in_year - days_so_far
                 };
                 break;
             }
 
             // Otherwise, count up the number of days this year so far and keep track of the month.
             days_so_far += days_next_month;
             month += 1;
@@ -1136,31 +1147,37 @@
             year -= 1;
             // NOTE: Leap year is already accounted for in the TAI duration when counting backward.
             day = if days_in_year < 0.0 {
                 days_in_year + usual_days_per_month(11) as f64 + 1.0
             } else {
                 usual_days_per_month(11) as f64
             };
-        } else if sign < 0 {
-            // Must add one day because just below, we'll be ignoring the days when rebuilding the time.
-            day += 1.0;
         }
 
         if sign < 0 {
             let time = Duration::compose(
                 sign,
                 0,
                 hours,
                 minutes,
                 seconds,
                 milliseconds,
                 microseconds,
                 nanos,
             );
 
+            // Last check on the validity of the Gregorian date
+
+            if time == Duration::ZERO || month == 12 && day == 32.0 {
+                // We've underflowed since we're before 1900.
+                year += 1;
+                month = 1;
+                day = 1.0;
+            }
+
             let (_, _, hours, minutes, seconds, milliseconds, microseconds, nanos) =
                 (24 * Unit::Hour + time).decompose();
 
             (
                 year,
                 month,
                 day as u8,
@@ -1258,401 +1275,433 @@
         iers_only: bool,
         provider: LeapSecondsFile,
     ) -> Option<f64> {
         self.leap_seconds_with(iers_only, provider)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Creates a new Epoch from a Duration as the time difference between this epoch and TAI reference epoch.
-    const fn init_from_tai_duration(duration: Duration) -> Self {
+    const fn init_from_tai_duration(_cls: &PyType, duration: Duration) -> Self {
         Self::from_tai_duration(duration)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Creates a new Epoch from its centuries and nanosecond since the TAI reference epoch.
-    fn init_from_tai_parts(centuries: i16, nanoseconds: u64) -> Self {
+    fn init_from_tai_parts(_cls: &PyType, centuries: i16, nanoseconds: u64) -> Self {
         Self::from_tai_parts(centuries, nanoseconds)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the provided TAI seconds since 1900 January 01 at midnight
-    fn init_from_tai_seconds(seconds: f64) -> Self {
+    fn init_from_tai_seconds(_cls: &PyType, seconds: f64) -> Self {
         Self::from_tai_seconds(seconds)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the provided TAI days since 1900 January 01 at midnight
-    fn init_from_tai_days(days: f64) -> Self {
+    fn init_from_tai_days(_cls: &PyType, days: f64) -> Self {
         Self::from_tai_days(days)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the provided UTC seconds since 1900 January 01 at midnight
-    fn init_from_utc_seconds(seconds: f64) -> Self {
+    fn init_from_utc_seconds(_cls: &PyType, seconds: f64) -> Self {
         Self::from_utc_seconds(seconds)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the provided UTC days since 1900 January 01 at midnight
-    fn init_from_utc_days(days: f64) -> Self {
+    fn init_from_utc_days(_cls: &PyType, days: f64) -> Self {
         Self::from_utc_days(days)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from given MJD in TAI time scale
-    fn init_from_mjd_tai(days: f64) -> Self {
+    fn init_from_mjd_tai(_cls: &PyType, days: f64) -> Self {
         Self::from_mjd_tai(days)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from given MJD in UTC time scale
-    fn init_from_mjd_utc(days: f64) -> Self {
+    fn init_from_mjd_utc(_cls: &PyType, days: f64) -> Self {
         Self::from_mjd_utc(days)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from given JDE in TAI time scale
-    fn init_from_jde_tai(days: f64) -> Self {
+    fn init_from_jde_tai(_cls: &PyType, days: f64) -> Self {
         Self::from_jde_tai(days)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from given JDE in UTC time scale
-    fn init_from_jde_utc(days: f64) -> Self {
+    fn init_from_jde_utc(_cls: &PyType, days: f64) -> Self {
         Self::from_jde_utc(days)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the provided TT seconds (approximated to 32.184s delta from TAI)
-    fn init_from_tt_seconds(seconds: f64) -> Self {
+    fn init_from_tt_seconds(_cls: &PyType, seconds: f64) -> Self {
         Self::from_tt_seconds(seconds)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the provided TT seconds (approximated to 32.184s delta from TAI)
-    fn init_from_tt_duration(duration: Duration) -> Self {
+    fn init_from_tt_duration(_cls: &PyType, duration: Duration) -> Self {
         Self::from_tt_duration(duration)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the Ephemeris Time seconds past 2000 JAN 01 (J2000 reference)
-    fn init_from_et_seconds(seconds_since_j2000: f64) -> Epoch {
+    fn init_from_et_seconds(_cls: &PyType, seconds_since_j2000: f64) -> Epoch {
         Self::from_et_seconds(seconds_since_j2000)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the Ephemeris Time duration past 2000 JAN 01 (J2000 reference)
-    fn init_from_et_duration(duration_since_j2000: Duration) -> Self {
+    fn init_from_et_duration(_cls: &PyType, duration_since_j2000: Duration) -> Self {
         Self::from_et_duration(duration_since_j2000)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from Dynamic Barycentric Time (TDB) seconds past 2000 JAN 01 midnight (difference than SPICE)
     /// NOTE: This uses the ESA algorithm, which is a notch more complicated than the SPICE algorithm, but more precise.
     /// In fact, SPICE algorithm is precise +/- 30 microseconds for a century whereas ESA algorithm should be exactly correct.
-    fn init_from_tdb_seconds(seconds_j2000: f64) -> Epoch {
+    fn init_from_tdb_seconds(_cls: &PyType, seconds_j2000: f64) -> Epoch {
         Self::from_tdb_seconds(seconds_j2000)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize from Dynamic Barycentric Time (TDB) (same as SPICE ephemeris time) whose epoch is 2000 JAN 01 noon TAI.
-    fn init_from_tdb_duration(duration_since_j2000: Duration) -> Epoch {
+    fn init_from_tdb_duration(_cls: &PyType, duration_since_j2000: Duration) -> Epoch {
         Self::from_tdb_duration(duration_since_j2000)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize from the JDE days
-    fn init_from_jde_et(days: f64) -> Self {
+    fn init_from_jde_et(_cls: &PyType, days: f64) -> Self {
         Self::from_jde_et(days)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize from Dynamic Barycentric Time (TDB) (same as SPICE ephemeris time) in JD days
-    fn init_from_jde_tdb(days: f64) -> Self {
+    fn init_from_jde_tdb(_cls: &PyType, days: f64) -> Self {
         Self::from_jde_tdb(days)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the number of seconds since the GPS Time Epoch,
     /// defined as UTC midnight of January 5th to 6th 1980 (cf. <https://gssc.esa.int/navipedia/index.php/Time_References_in_GNSS#GPS_Time_.28GPST.29>).
-    fn init_from_gpst_seconds(seconds: f64) -> Self {
+    fn init_from_gpst_seconds(_cls: &PyType, seconds: f64) -> Self {
         Self::from_gpst_seconds(seconds)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the number of days since the GPS Time Epoch,
     /// defined as UTC midnight of January 5th to 6th 1980 (cf. <https://gssc.esa.int/navipedia/index.php/Time_References_in_GNSS#GPS_Time_.28GPST.29>).
-    fn init_from_gpst_days(days: f64) -> Self {
+    fn init_from_gpst_days(_cls: &PyType, days: f64) -> Self {
         Self::from_gpst_days(days)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the number of nanoseconds since the GPS Time Epoch,
     /// defined as UTC midnight of January 5th to 6th 1980 (cf. <https://gssc.esa.int/navipedia/index.php/Time_References_in_GNSS#GPS_Time_.28GPST.29>).
     /// This may be useful for time keeping devices that use GPS as a time source.
-    fn init_from_gpst_nanoseconds(nanoseconds: u64) -> Self {
+    fn init_from_gpst_nanoseconds(_cls: &PyType, nanoseconds: u64) -> Self {
         Self::from_gpst_nanoseconds(nanoseconds)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the number of seconds since the Galileo Time Epoch,
     /// starting on August 21st 1999 Midnight UT,
     /// (cf. <https://gssc.esa.int/navipedia/index.php/Time_References_in_GNSS>).
-    fn init_from_gst_seconds(seconds: f64) -> Self {
+    fn init_from_gst_seconds(_cls: &PyType, seconds: f64) -> Self {
         Self::from_gst_seconds(seconds)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the number of days since the Galileo Time Epoch,
     /// starting on August 21st 1999 Midnight UT,
     /// (cf. <https://gssc.esa.int/navipedia/index.php/Time_References_in_GNSS>).
-    fn init_from_gst_days(days: f64) -> Self {
+    fn init_from_gst_days(_cls: &PyType, days: f64) -> Self {
         Self::from_gst_days(days)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the number of nanoseconds since the Galileo Time Epoch,
     /// starting on August 21st 1999 Midnight UT,
     /// (cf. <https://gssc.esa.int/navipedia/index.php/Time_References_in_GNSS>).
     /// This may be useful for time keeping devices that use GST as a time source.
-    fn init_from_gst_nanoseconds(nanoseconds: u64) -> Self {
+    fn init_from_gst_nanoseconds(_cls: &PyType, nanoseconds: u64) -> Self {
         Self::from_gst_nanoseconds(nanoseconds)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the number of seconds since the BeiDou Time Epoch,
     /// defined as January 1st 2006 (cf. <https://gssc.esa.int/navipedia/index.php/Time_References_in_GNSS>).
-    fn init_from_bdt_seconds(seconds: f64) -> Self {
+    fn init_from_bdt_seconds(_cls: &PyType, seconds: f64) -> Self {
         Self::from_bdt_seconds(seconds)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the number of days since the BeiDou Time Epoch,
     /// defined as January 1st 2006 (cf. <https://gssc.esa.int/navipedia/index.php/Time_References_in_GNSS>).
-    fn init_from_bdt_days(days: f64) -> Self {
+    fn init_from_bdt_days(_cls: &PyType, days: f64) -> Self {
         Self::from_bdt_days(days)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the number of days since the BeiDou Time Epoch,
     /// defined as January 1st 2006 (cf. <https://gssc.esa.int/navipedia/index.php/Time_References_in_GNSS>).
     /// This may be useful for time keeping devices that use BDT as a time source.
-    fn init_from_bdt_nanoseconds(nanoseconds: u64) -> Self {
+    fn init_from_bdt_nanoseconds(_cls: &PyType, nanoseconds: u64) -> Self {
         Self::from_bdt_nanoseconds(nanoseconds)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the provided UNIX second timestamp since UTC midnight 1970 January 01.
-    fn init_from_unix_seconds(seconds: f64) -> Self {
+    fn init_from_unix_seconds(_cls: &PyType, seconds: f64) -> Self {
         Self::from_unix_seconds(seconds)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize an Epoch from the provided UNIX millisecond timestamp since UTC midnight 1970 January 01.
-    fn init_from_unix_milliseconds(milliseconds: f64) -> Self {
+    fn init_from_unix_milliseconds(_cls: &PyType, milliseconds: f64) -> Self {
         Self::from_unix_milliseconds(milliseconds)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     fn init_from_gregorian(
+        _cls: &PyType,
         year: i32,
         month: u8,
         day: u8,
         hour: u8,
         minute: u8,
         second: u8,
         nanos: u32,
         time_scale: TimeScale,
     ) -> Self {
         Self::from_gregorian(year, month, day, hour, minute, second, nanos, time_scale)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
-    fn init_from_gregorian_at_noon(year: i32, month: u8, day: u8, time_scale: TimeScale) -> Self {
+    #[classmethod]
+    fn init_from_gregorian_at_noon(
+        _cls: &PyType,
+        year: i32,
+        month: u8,
+        day: u8,
+        time_scale: TimeScale,
+    ) -> Self {
         Self::from_gregorian_at_noon(year, month, day, time_scale)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     fn init_from_gregorian_at_midnight(
+        _cls: &PyType,
         year: i32,
         month: u8,
         day: u8,
         time_scale: TimeScale,
     ) -> Self {
         Self::from_gregorian_at_midnight(year, month, day, time_scale)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Attempts to build an Epoch from the provided Gregorian date and time in TAI.
     fn maybe_init_from_gregorian_tai(
+        _cls: &PyType,
         year: i32,
         month: u8,
         day: u8,
         hour: u8,
         minute: u8,
         second: u8,
         nanos: u32,
     ) -> Result<Self, Errors> {
         Self::maybe_from_gregorian_tai(year, month, day, hour, minute, second, nanos)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Attempts to build an Epoch from the provided Gregorian date and time in the provided time scale.
     /// NOTE: If the time scale is TDB, this function assumes that the SPICE format is used
     #[allow(clippy::too_many_arguments)]
     fn maybe_init_from_gregorian(
+        _cls: &PyType,
         year: i32,
         month: u8,
         day: u8,
         hour: u8,
         minute: u8,
         second: u8,
         nanos: u32,
         time_scale: TimeScale,
     ) -> Result<Self, Errors> {
         Self::maybe_from_gregorian(year, month, day, hour, minute, second, nanos, time_scale)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Builds an Epoch from the provided Gregorian date and time in TAI. If invalid date is provided, this function will panic.
     /// Use maybe_from_gregorian_tai if unsure.
     fn init_from_gregorian_tai(
+        _cls: &PyType,
         year: i32,
         month: u8,
         day: u8,
         hour: u8,
         minute: u8,
         second: u8,
         nanos: u32,
     ) -> Self {
         Self::from_gregorian_tai(year, month, day, hour, minute, second, nanos)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize from the Gregorian date at midnight in TAI.
-    fn init_from_gregorian_tai_at_midnight(year: i32, month: u8, day: u8) -> Self {
+    fn init_from_gregorian_tai_at_midnight(_cls: &PyType, year: i32, month: u8, day: u8) -> Self {
         Self::from_gregorian_tai_at_midnight(year, month, day)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize from the Gregorian date at noon in TAI
-    fn init_from_gregorian_tai_at_noon(year: i32, month: u8, day: u8) -> Self {
+    fn init_from_gregorian_tai_at_noon(_cls: &PyType, year: i32, month: u8, day: u8) -> Self {
         Self::from_gregorian_tai_at_noon(year, month, day)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize from the Gregorian date and time (without the nanoseconds) in TAI
     fn init_from_gregorian_tai_hms(
+        _cls: &PyType,
         year: i32,
         month: u8,
         day: u8,
         hour: u8,
         minute: u8,
         second: u8,
     ) -> Self {
         Self::from_gregorian_tai_hms(year, month, day, hour, minute, second)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Attempts to build an Epoch from the provided Gregorian date and time in UTC.
     fn maybe_init_from_gregorian_utc(
+        _cls: &PyType,
         year: i32,
         month: u8,
         day: u8,
         hour: u8,
         minute: u8,
         second: u8,
         nanos: u32,
     ) -> Result<Self, Errors> {
         Self::maybe_from_gregorian_utc(year, month, day, hour, minute, second, nanos)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Builds an Epoch from the provided Gregorian date and time in TAI. If invalid date is provided, this function will panic.
     /// Use maybe_from_gregorian_tai if unsure.
     fn init_from_gregorian_utc(
+        _cls: &PyType,
         year: i32,
         month: u8,
         day: u8,
         hour: u8,
         minute: u8,
         second: u8,
         nanos: u32,
     ) -> Self {
         Self::from_gregorian_utc(year, month, day, hour, minute, second, nanos)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize from Gregorian date in UTC at midnight
-    fn init_from_gregorian_utc_at_midnight(year: i32, month: u8, day: u8) -> Self {
+    fn init_from_gregorian_utc_at_midnight(_cls: &PyType, year: i32, month: u8, day: u8) -> Self {
         Self::from_gregorian_utc_at_midnight(year, month, day)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize from Gregorian date in UTC at noon
-    fn init_from_gregorian_utc_at_noon(year: i32, month: u8, day: u8) -> Self {
+    fn init_from_gregorian_utc_at_noon(_cls: &PyType, year: i32, month: u8, day: u8) -> Self {
         Self::from_gregorian_utc_at_noon(year, month, day)
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
+    #[classmethod]
     /// Initialize from the Gregorian date and time (without the nanoseconds) in UTC
     fn init_from_gregorian_utc_hms(
+        _cls: &PyType,
         year: i32,
         month: u8,
         day: u8,
         hour: u8,
         minute: u8,
         second: u8,
     ) -> Self {
         Self::from_gregorian_utc_hms(year, month, day, hour, minute, second)
     }
 
+    #[cfg(feature = "python")]
+    #[classmethod]
+    /// Equivalent to `datetime.strptime, refer to <https://docs.rs/hifitime/latest/hifitime/efmt/format/struct.Format.html> for format options
+    fn strptime(_cls: &PyType, epoch_str: String, format_str: String) -> PyResult<Self> {
+        Self::from_format_str(&epoch_str, &format_str).map_err(|e| PyErr::from(e))
+    }
+
+    #[cfg(feature = "python")]
+    /// Equivalent to `datetime.strftime, refer to <https://docs.rs/hifitime/latest/hifitime/efmt/format/struct.Format.html> for format options
+    fn strftime(&self, format_str: String) -> PyResult<String> {
+        use crate::efmt::Formatter;
+        let fmt = Format::from_str(&format_str)
+            .map_err(Errors::ParseError)
+            .map_err(|e| PyErr::from(e))?;
+        Ok(format!("{}", Formatter::new(*self, fmt)))
+    }
+
     /// Returns this epoch with respect to the time scale this epoch was created in.
     /// This is needed to correctly perform duration conversions in dynamical time scales (e.g. TDB).
     ///
     /// # Examples
     /// 1. If an epoch was initialized as Epoch::from_..._utc(...) then the duration will be the UTC duration from J1900.
     /// 2. If an epoch was initialized as Epoch::from_..._tdb(...) then the duration will be the UTC duration from J2000 because the TDB reference epoch is J2000.
     #[must_use]
@@ -2617,16 +2666,16 @@
         match Self::from_str(&string_repr) {
             Ok(d) => Ok(d),
             Err(e) => Err(PyErr::from(e)),
         }
     }
 
     #[cfg(feature = "python")]
-    #[staticmethod]
-    fn system_now() -> Result<Self, Errors> {
+    #[classmethod]
+    fn system_now(_cls: &PyType) -> Result<Self, Errors> {
         Self::now()
     }
 
     #[cfg(feature = "python")]
     fn __str__(&self) -> String {
         format!("{self}")
     }
@@ -2769,15 +2818,15 @@
             *self
         } else {
             other
         }
     }
 }
 
-// This is in its separate impl far away from the Python feature because pyO3's staticmethod does not work with cfg_attr
+// This is in its separate impl far away from the Python feature because pyO3's classmethod does not work with cfg_attr
 #[cfg(feature = "std")]
 impl Epoch {
     /// Initializes a new Epoch from `now`.
     /// WARNING: This assumes that the system time returns the time in UTC (which is the case on Linux)
     /// Uses [`std::time::SystemTime::now`](https://doc.rust-lang.org/std/time/struct.SystemTime.html#method.now) under the hood
     pub fn now() -> Result<Self, Errors> {
         match SystemTime::now().duration_since(SystemTime::UNIX_EPOCH) {
```

### Comparing `hifitime-3.8.0/src/errors.rs` & `hifitime-3.8.1/src/errors.rs`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     /// date time then a Carry Error is returned as the Result.
     Carry,
     /// ParseError is returned when a provided string could not be parsed and converted to the desired
     /// struct (e.g. Datetime).
     ParseError(ParsingErrors),
     /// Raised when trying to initialize an Epoch or Duration from its hi and lo values, but these overlap
     ConversionOverlapError(f64, f64),
-    /// Raised if an overflow occured
+    /// Raised if an overflow occurred
     Overflow,
     /// Raised if the initialization from system time failed
     SystemTimeError,
 }
 
 #[derive(Copy, Clone, Debug, PartialEq, Eq)]
 pub enum ParsingErrors {
@@ -74,15 +74,15 @@
             Self::Carry => write!(f, "a carry error (e.g. 61 seconds)"),
             Self::ParseError(kind) => write!(f, "ParseError: {:?}", kind),
             Self::ConversionOverlapError(hi, lo) => {
                 write!(f, "hi and lo values overlap: {}, {}", hi, lo)
             }
             Self::Overflow => write!(
                 f,
-                "overflow occured when trying to convert Duration information"
+                "overflow occurred when trying to convert Duration information"
             ),
             Self::SystemTimeError => write!(f, "std::time::SystemTime returned an error"),
         }
     }
 }
 
 impl convert::From<ParseIntError> for Errors {
```

### Comparing `hifitime-3.8.0/src/leap_seconds.rs` & `hifitime-3.8.1/src/leap_seconds.rs`

 * *Files 2% similar despite different names*

```diff
@@ -143,7 +143,21 @@
 
     fn index(&self, index: usize) -> &Self::Output {
         self.data.index(index)
     }
 }
 
 impl LeapSecondProvider for LatestLeapSeconds {}
+
+#[test]
+fn leap_second_fetch() {
+    let leap_seconds = LatestLeapSeconds::default();
+
+    assert_eq!(
+        leap_seconds[0],
+        LeapSecond::new(1_893_369_600.0, 1.417818, false),
+    );
+    assert_eq!(
+        leap_seconds[41],
+        LeapSecond::new(3_692_217_600.0, 37.0, true)
+    );
+}
```

### Comparing `hifitime-3.8.0/src/lib.rs` & `hifitime-3.8.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/src/month.rs` & `hifitime-3.8.1/src/month.rs`

 * *Files 3% similar despite different names*

```diff
@@ -39,18 +39,14 @@
 
 impl Default for MonthName {
     fn default() -> Self {
         Self::January
     }
 }
 
-impl MonthName {
-    const MAX: u8 = 12;
-}
-
 impl FromStr for MonthName {
     type Err = ParsingErrors;
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         match s.trim() {
             "jan" | "Jan" | "JAN" | "January" | "JANUARY" | "january" => Ok(Self::January),
             "feb" | "Feb" | "FEB" | "February" | "FEBRUARY" | "february" => Ok(Self::February),
             "mar" | "Mar" | "MAR" | "March" | "MARCH" | "march" => Ok(Self::March),
@@ -66,15 +62,15 @@
             _ => Err(ParsingErrors::UnknownMonthName),
         }
     }
 }
 
 impl From<u8> for MonthName {
     fn from(u: u8) -> Self {
-        match u.rem_euclid(Self::MAX) {
+        match u {
             1 => Self::January,
             2 => Self::February,
             3 => Self::March,
             4 => Self::April,
             5 => Self::May,
             6 => Self::June,
             7 => Self::July,
```

### Comparing `hifitime-3.8.0/src/parser.rs` & `hifitime-3.8.1/src/parser.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/src/python.rs` & `hifitime-3.8.1/src/python.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/src/timescale.rs` & `hifitime-3.8.1/src/timescale.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/src/timeseries.rs` & `hifitime-3.8.1/src/timeseries.rs`

 * *Files 17% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 */
 
 /// An iterator of a sequence of evenly spaced Epochs.
 #[derive(Clone, Debug, PartialEq, Eq)]
 #[cfg_attr(feature = "python", pyclass)]
 pub struct TimeSeries {
     start: Epoch,
-    end: Epoch,
+    duration: Duration,
     step: Duration,
-    cur: Epoch,
+    cur: i64,
     incl: bool,
 }
 
 impl TimeSeries {
     /// Return an iterator of evenly spaced Epochs, **inclusive** on start and **exclusive** on end.
     /// ```
     /// use hifitime::{Epoch, Unit, TimeSeries};
@@ -50,17 +50,17 @@
     /// assert_eq!(cnt, 6)
     /// ```
     #[inline]
     pub fn exclusive(start: Epoch, end: Epoch, step: Duration) -> TimeSeries {
         // Start one step prior to start because next() just moves forward
         Self {
             start,
-            end,
+            duration: end - start,
             step,
-            cur: start - step,
+            cur: 0,
             incl: false,
         }
     }
 
     /// Return an iterator of evenly spaced Epochs, inclusive on start **and** on end.
     /// ```
     /// use hifitime::{Epoch, Unit, TimeSeries};
@@ -76,135 +76,135 @@
     /// assert_eq!(cnt, 7)
     /// ```
     #[inline]
     pub fn inclusive(start: Epoch, end: Epoch, step: Duration) -> TimeSeries {
         // Start one step prior to start because next() just moves forward
         Self {
             start,
-            end,
+            duration: end - start,
             step,
-            cur: start - step,
+            cur: 0,
             incl: true,
         }
     }
 }
 
 impl fmt::Display for TimeSeries {
     // Prints this duration with automatic selection of the units, i.e. everything that isn't zero is ignored
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         write!(
             f,
             "TimeSeries [{} : {} : {}]",
             self.start,
             if self.incl {
-                self.end
+                self.start + self.duration
             } else {
-                self.end - self.step
+                self.start + self.duration - self.step
             },
             self.step
         )
     }
 }
 
 impl fmt::LowerHex for TimeSeries {
     /// Prints the Epoch in TAI
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         write!(
             f,
             "TimeSeries [{:x} : {:x} : {}]",
             self.start,
             if self.incl {
-                self.end
+                self.start + self.duration
             } else {
-                self.end - self.step
+                self.start + self.duration - self.step
             },
             self.step
         )
     }
 }
 
 impl fmt::UpperHex for TimeSeries {
     /// Prints the Epoch in TT
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         write!(
             f,
             "TimeSeries [{:X} : {:X} : {}]",
             self.start,
             if self.incl {
-                self.end
+                self.start + self.duration
             } else {
-                self.end - self.step
+                self.start + self.duration - self.step
             },
             self.step
         )
     }
 }
 
 impl fmt::LowerExp for TimeSeries {
     /// Prints the Epoch in TDB
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         write!(
             f,
             "TimeSeries [{:e} : {:e} : {}]",
             self.start,
             if self.incl {
-                self.end
+                self.start + self.duration
             } else {
-                self.end - self.step
+                self.start + self.duration - self.step
             },
             self.step
         )
     }
 }
 
 impl fmt::UpperExp for TimeSeries {
     /// Prints the Epoch in ET
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         write!(
             f,
             "TimeSeries [{:E} : {:E} : {}]",
             self.start,
             if self.incl {
-                self.end
+                self.start + self.duration
             } else {
-                self.end - self.step
+                self.start + self.duration - self.step
             },
             self.step
         )
     }
 }
 
 impl fmt::Pointer for TimeSeries {
     /// Prints the Epoch in UNIX
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         write!(
             f,
             "TimeSeries [{:p} : {:p} : {}]",
             self.start,
             if self.incl {
-                self.end
+                self.start + self.duration
             } else {
-                self.end - self.step
+                self.start + self.duration - self.step
             },
             self.step
         )
     }
 }
 
 impl fmt::Octal for TimeSeries {
     /// Prints the Epoch in GPS
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         write!(
             f,
             "TimeSeries [{:o} : {:o} : {}]",
             self.start,
             if self.incl {
-                self.end
+                self.start + self.duration
             } else {
-                self.end - self.step
+                self.start + self.duration - self.step
             },
             self.step
         )
     }
 }
 
 #[cfg(feature = "python")]
@@ -240,46 +240,53 @@
 }
 
 impl Iterator for TimeSeries {
     type Item = Epoch;
 
     #[inline]
     fn next(&mut self) -> Option<Epoch> {
-        let next_item = self.cur + self.step;
-        if (!self.incl && next_item >= self.end) || (self.incl && next_item > self.end) {
+        let next_offset = self.cur * self.step;
+        if (!self.incl && next_offset >= self.duration)
+            || (self.incl && next_offset > self.duration)
+        {
             None
         } else {
-            self.cur = next_item;
-            Some(next_item)
+            self.cur += 1;
+            Some(self.start + next_offset)
         }
     }
 
     fn size_hint(&self) -> (usize, Option<usize>) {
         (self.len(), Some(self.len() + 1))
     }
 }
 
 impl DoubleEndedIterator for TimeSeries {
     #[inline]
     fn next_back(&mut self) -> Option<Epoch> {
-        let next_item = self.cur - self.step;
-        if next_item < self.start {
+        // Offset from the end of the iterator
+        self.cur += 1;
+        let offset = self.cur * self.step;
+        // if offset < -self.duration - self.step {
+        if (!self.incl && offset > self.duration)
+            || (self.incl && offset > self.duration + self.step)
+        {
             None
         } else {
-            Some(next_item)
+            Some(self.start + self.duration - offset)
         }
     }
 }
 
 impl ExactSizeIterator for TimeSeries
 where
     TimeSeries: Iterator,
 {
     fn len(&self) -> usize {
-        let approx = ((self.end - self.start).to_seconds() / self.step.to_seconds()).abs();
+        let approx = (self.duration.to_seconds() / self.step.to_seconds()).abs();
         if self.incl {
             if approx.ceil() >= usize::MAX as f64 {
                 usize::MAX
             } else {
                 approx.ceil() as usize
             }
         } else if approx.floor() >= usize::MAX as f64 {
@@ -349,8 +356,43 @@
         assert_eq!(times.len(), times.size_hint().0);
 
         // For an _inclusive_ time series, we skip the last item, so it's the steps count
         let times = TimeSeries::inclusive(start, end, step);
         assert_eq!(times.len(), steps as usize);
         assert_eq!(times.len(), times.size_hint().0);
     }
+
+    #[test]
+    fn ts_over_leap_second() {
+        let start = Epoch::from_gregorian_utc(2016, 12, 31, 23, 59, 59, 0);
+        let times = TimeSeries::exclusive(start, start + Unit::Second * 5, Unit::Second * 1);
+        let expect_end = start + Unit::Second * 4;
+        let mut cnt = 0;
+        let mut cur_epoch = start;
+
+        for epoch in times {
+            cnt += 1;
+            cur_epoch = epoch;
+        }
+
+        assert_eq!(cnt, 5); // Five because the first item is always inclusive
+        assert_eq!(cur_epoch, expect_end, "incorrect last item in iterator");
+    }
+
+    #[test]
+    fn ts_backward() {
+        let start = Epoch::from_gregorian_utc(2015, 1, 1, 12, 0, 0, 0);
+        let times = TimeSeries::exclusive(start, start + Unit::Second * 5, Unit::Second * 1);
+        let mut cnt = 0;
+        let mut cur_epoch = start;
+
+        for epoch in times.rev() {
+            cnt += 1;
+            cur_epoch = epoch;
+            let expect = start + Unit::Second * (5 - cnt);
+            assert_eq!(expect, epoch, "incorrect item in iterator");
+        }
+
+        assert_eq!(cnt, 5); // Five because the first item is always inclusive
+        assert_eq!(cur_epoch, start, "incorrect last item in iterator");
+    }
 }
```

### Comparing `hifitime-3.8.0/src/timeunits.rs` & `hifitime-3.8.1/src/timeunits.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/src/ut1.rs` & `hifitime-3.8.1/src/ut1.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
  */
 
 #[cfg(feature = "python")]
 use pyo3::prelude::*;
 
 use reqwest::{blocking::get, StatusCode};
 
-use tabled::{Style, Table, Tabled};
+use tabled::settings::Style;
+use tabled::{Table, Tabled};
 
 use std::{fs::File, io::Read};
 
 use core::fmt;
 use core::ops::Index;
 
 use crate::{Duration, Epoch, Errors, ParsingErrors, Unit};
@@ -34,17 +35,25 @@
 /// A structure storing all of the TAI-UT1 data
 pub struct Ut1Provider {
     data: Vec<DeltaTaiUt1>,
     iter_pos: usize,
 }
 
 impl Ut1Provider {
-    /// Build a UT1 provider by downloading the data from <https://eop2-external.jpl.nasa.gov/eop2/latest_eop2.short> (short time scale UT1 data) and parsing it.
+    /// Builds a UT1 provided by downloading the data from <https://eop2-external.jpl.nasa.gov/eop2/latest_eop2.short> (short time scale UT1 data) and parsing it.
     pub fn download_short_from_jpl() -> Result<Self, Errors> {
-        match get("https://eop2-external.jpl.nasa.gov/eop2/latest_eop2.short") {
+        Self::download_from_jpl("latest_eop2.short")
+    }
+
+    /// Build a UT1 provider by downloading the data from <https://eop2-external.jpl.nasa.gov/eop2/latest_eop2.long> (long time scale UT1 data) and parsing it.
+    pub fn download_from_jpl(version: &str) -> Result<Self, Errors> {
+        match get(format!(
+            "https://eop2-external.jpl.nasa.gov/eop2/{}",
+            version
+        )) {
             Ok(resp) => {
                 let eop_data = String::from_utf8(resp.bytes().unwrap().to_vec()).unwrap();
                 Self::from_eop_data(eop_data)
             }
             Err(e) => Err(Errors::ParseError(ParsingErrors::DownloadError(
                 e.status().unwrap_or(StatusCode::SEE_OTHER),
             ))),
@@ -86,19 +95,18 @@
 
             // We have data of interest!
             let data: Vec<&str> = line.split(',').collect();
             if data.len() < 4 {
                 return Err(Errors::ParseError(ParsingErrors::UnknownFormat));
             }
 
-            let mjd_tai_days: f64;
-            match lexical_core::parse(data[0].trim().as_bytes()) {
-                Ok(val) => mjd_tai_days = val,
+            let mjd_tai_days: f64 = match lexical_core::parse(data[0].trim().as_bytes()) {
+                Ok(val) => val,
                 Err(_) => return Err(Errors::ParseError(ParsingErrors::ValueError)),
-            }
+            };
 
             let delta_ut1_ms: f64;
             match lexical_core::parse(data[3].trim().as_bytes()) {
                 Ok(val) => delta_ut1_ms = val,
                 Err(_) => return Err(Errors::ParseError(ParsingErrors::ValueError)),
             }
```

### Comparing `hifitime-3.8.0/src/weekday.rs` & `hifitime-3.8.1/src/weekday.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/tests/duration.rs` & `hifitime-3.8.1/tests/duration.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/tests/efmt.rs` & `hifitime-3.8.1/tests/efmt.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use hifitime::efmt::consts::*;
 use hifitime::prelude::*;
 
 #[test]
 fn epoch_parse_with_format() {
+    use core::str::FromStr;
     let e = Epoch::from_gregorian_utc_hms(2015, 2, 7, 11, 22, 33);
 
     assert_eq!(
         ISO8601_DATE.parse("2015-02-07").unwrap(),
         Epoch::from_gregorian_utc_at_midnight(2015, 2, 7)
     );
 
@@ -24,14 +25,18 @@
 
     assert_eq!(
         ISO8601_ORDINAL
             .parse(&format!("{}", Formatter::new(e, ISO8601_ORDINAL)))
             .unwrap(),
         Epoch::from_gregorian_utc_at_midnight(2015, 2, 7) // Ordinal removes the knowledge below days
     );
+
+    // Confirmation that https://github.com/nyx-space/hifitime/issues/202 is a documentation problem and not a functionality problem.
+    let fmtd = Formatter::new(e, Format::from_str("%H:%M").unwrap());
+    assert_eq!(format!("{fmtd}"), format!("11:22"));
 }
 
 #[test]
 fn epoch_format_rfc2822() {
     let epoch = Epoch::from_gregorian_utc_hms(2015, 2, 7, 11, 22, 33);
 
     assert_eq!(
@@ -81,8 +86,18 @@
     );
 
     // But removing microseconds will cause a rounding the other way.
     assert_eq!(
         format!("{}", Formatter::new(epoch - 2 * Unit::Microsecond, RFC2822)),
         "Sat, 07 Feb 2015 11:22:32"
     );
+
+    assert_eq!(
+        Epoch::from_format_str("Sat, 07 Feb 2015 11:22:33", "%a, %d %b %Y %H:%M:%S").unwrap(),
+        epoch
+    );
+
+    assert_eq!(
+        Epoch::from_str_with_format("Sat, 07 Feb 2015 11:22:33", RFC2822).unwrap(),
+        epoch
+    );
 }
```

### Comparing `hifitime-3.8.0/tests/epoch.rs` & `hifitime-3.8.1/tests/epoch.rs`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #[test]
 fn utc_epochs() {
     assert!(Epoch::from_mjd_tai(J1900_OFFSET).to_tai_seconds() < EPSILON);
     assert!((Epoch::from_mjd_tai(J1900_OFFSET).to_mjd_tai_days() - J1900_OFFSET).abs() < EPSILON);
 
     // Tests are chronological dates.
     // All of the following examples are cross validated against NASA HEASARC,
-    // refered to as "X-Val" for "cross validation."
+    // referred to as "X-Val" for "cross validation."
 
     // X-Val: 03 January 1938 04:12:48 - https://www.timeanddate.com/date/durationresult.html?m1=1&d1=1&y1=1900&m2=1&d2=03&y2=1938&h1=0&i1=0&s1=0&h2=4&i2=12&s2=48
     let this_epoch = Epoch::from_tai_seconds(1_199_333_568.0);
     let epoch_utc = Epoch::maybe_from_gregorian_utc(1938, 1, 3, 4, 12, 48, 0).expect("init epoch");
     assert_eq!(epoch_utc, this_epoch, "Incorrect epoch");
 
     // X-Val: 28 February 1938 00:00:00 - https://www.timeanddate.com/date/durationresult.html?m1=1&d1=1&y1=1900&m2=02&d2=28&y2=1938&h1=0&i1=0&s1=0&h2=0&i2=0&s2=0
@@ -1840,7 +1840,28 @@
     for expected in default {
         if expected.announced_by_iers {
             assert_eq!(expected, provider[pos]);
             pos += 1;
         }
     }
 }
+
+#[test]
+fn regression_test_gh_204() {
+    use core::str::FromStr;
+    use hifitime::Epoch;
+
+    let e1700 = Epoch::from_str("1700-01-01T00:00:00 TAI").unwrap();
+    assert_eq!(format!("{e1700:x}"), "1700-01-01T00:00:00 TAI");
+
+    let e1700 = Epoch::from_str("1700-04-17T02:10:09 TAI").unwrap();
+    assert_eq!(format!("{e1700:x}"), "1700-04-17T02:10:09 TAI");
+
+    let e1799 = Epoch::from_str("1799-01-01T00:00:01 TAI").unwrap();
+    assert_eq!(format!("{e1799:x}"), "1799-01-01T00:00:01 TAI");
+
+    let e1899 = Epoch::from_str("1899-01-01T00:00:00 TAI").unwrap();
+    assert_eq!(format!("{e1899:x}"), "1899-01-01T00:00:00 TAI");
+
+    let e1900_m1 = Epoch::from_str("1899-12-31T23:59:59 TAI").unwrap();
+    assert_eq!(format!("{e1900_m1:x}"), "1899-12-31T23:59:59 TAI");
+}
```

### Comparing `hifitime-3.8.0/tests/timescale.rs` & `hifitime-3.8.1/tests/timescale.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/tests/timeseries.rs` & `hifitime-3.8.1/tests/timeseries.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/tests/ut1.rs` & `hifitime-3.8.1/tests/ut1.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-use core::str::FromStr;
-
-use hifitime::Epoch;
-
 #[cfg(feature = "ut1")]
 #[test]
 fn test_ut1_from_file() {
+    use core::str::FromStr;
     use hifitime::ut1::Ut1Provider;
+    use hifitime::Epoch;
 
     let provider = Ut1Provider::from_eop_file("data/eop-2021-10-12--2023-01-04.short").unwrap();
 
     println!("{}", provider);
 
     // Grabbed from AstroPy:
     // >>> Time("2022-01-03 03:05:06.789101")
@@ -24,26 +22,30 @@
         "2022-01-03T03:05:06.679020600 TAI"
     );
 }
 
 #[cfg(feature = "ut1")]
 #[test]
 fn test_ut1_from_jpl() {
+    use core::str::FromStr;
     use hifitime::ut1::Ut1Provider;
+    use hifitime::Epoch;
 
-    let provider = Ut1Provider::download_short_from_jpl().unwrap();
+    // Download a specific version of the UT1 file
+    let provider = Ut1Provider::download_from_jpl("221222_190002-marge_eop2.short").unwrap();
 
     println!("{}", provider);
 
     // Grabbed from AstroPy:
     // >>> Time("2022-01-03 03:05:06.789101")
     // <Time object: scale='utc' format='iso' value=2022-01-03 03:05:06.789>
     // >>> Time("2022-01-03 03:05:06.789101").ut1
     // <Time object: scale='ut1' format='iso' value=2022-01-03 03:05:06.679>
     // >>>
     //
-    let epoch = Epoch::from_str("2022-01-03 03:05:06.7891").unwrap();
+    let epoch = Epoch::from_str("2022-01-03 03:05:06.7891 UTC").unwrap();
+    let ut1_epoch = epoch.to_ut1(provider);
     assert_eq!(
-        format!("{:x}", epoch.to_ut1(provider)),
-        "2022-01-03T03:05:06.679020600 TAI"
+        format!("{:x}", ut1_epoch),
+        "2022-01-03T03:05:06.679020600 TAI",
     );
 }
```

### Comparing `hifitime-3.8.0/tests/weekday.rs` & `hifitime-3.8.1/tests/weekday.rs`

 * *Files identical despite different names*

### Comparing `hifitime-3.8.0/Cargo.lock` & `hifitime-3.8.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -5,157 +5,157 @@
 [[package]]
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
-name = "atty"
-version = "0.2.14"
+name = "anstyle"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
-dependencies = [
- "hermit-abi 0.1.19",
- "libc",
- "winapi",
-]
+checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "base64"
-version = "0.13.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bumpalo"
-version = "3.11.1"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "572f695136211188308f16ad2ca5c851a712c464060ae6974944458eb83880ba"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "bytecount"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c676a478f63e9fa2dd5368a42f28bba0d6c560b775f38583c8bbaa7fcd67c9c"
 
 [[package]]
 name = "bytes"
-version = "1.3.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfb24e866b15a1af2a1b663f10c6b6b8f397a84aadb828f12e5b289ec23a3a3c"
+checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a20104e2335ce8a659d6dd92a51a767a0c062599c73b343fd152cb401e828c3d"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "ciborium"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0c137568cc60b904a7724001b35ce2630fd00d5d84805fbb608ab89509d788f"
+checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
  "serde",
 ]
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "346de753af073cc87b52b2083a506b38ac176a44cfb05497b622e27be899b369"
+checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
 
 [[package]]
 name = "ciborium-ll"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "213030a2b5a4e0c0892b6652260cf6ccac84827b83a85a534e178e3906c4cf1b"
+checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.23"
+version = "4.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "93aae7a4192245f70fe75dd9157fc7b4a5bf53e88d30bd4396f7d8f9284d5acc"
+dependencies = [
+ "clap_builder",
+]
+
+[[package]]
+name = "clap_builder"
+version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "4f423e341edefb78c9caba2d9c7f7687d0e72e89df3ce3394554754393ac3990"
 dependencies = [
+ "anstyle",
  "bitflags",
  "clap_lex",
- "indexmap",
- "textwrap",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.2.4"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
-dependencies = [
- "os_str_bytes",
-]
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
 name = "core-foundation"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "criterion"
-version = "0.4.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7c76e09c1aae2bc52b3d2f29e13c6572553b30c4aa1b8a49fd70de6412654cb"
+checksum = "f2b12d017a929603d80db1831cd3a24082f8137ce19c69e6447f54f5fc8d692f"
 dependencies = [
  "anes",
- "atty",
  "cast",
  "ciborium",
  "clap",
  "criterion-plot",
+ "is-terminal",
  "itertools",
- "lazy_static",
  "num-traits",
+ "once_cell",
  "oorandom",
  "plotters",
  "rayon",
  "regex",
  "serde",
  "serde_derive",
  "serde_json",
@@ -171,51 +171,51 @@
 dependencies = [
  "cast",
  "itertools",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.6"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2dd04ddaf88237dc3b8d8f9a3c1004b506b54b3313403944054d23c0870c521"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "715e8152b692bba2d374b53d4875445368fdf21a94751410af607a5ac677d1fc"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
 dependencies = [
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.13"
+version = "0.9.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01a9af1f4c2ef74bb8aa1f7e19706bc72d03598c8a570bb5de72243c7a9d9d5a"
+checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.7.1",
+ "memoffset",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.14"
+version = "0.8.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fb766fa798726286dbbb842f174001dab8abc7b627a1dd86e0b7222a95d929f"
+checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "der"
 version = "0.6.1"
@@ -230,37 +230,58 @@
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ef71ddb5b3a1f53dee24817c8f70dfa1cb29e804c18d88c228d4bc9c86ee3b9"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90e5c1c8368803113bf0c9584fc495a58b86dc8a29edbf8fe877d21d9507e797"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.31"
+version = "0.8.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9852635589dc9f9ea1b6fe9f05b50ef208c85c834a562f0c6abb1c475736ec2b"
+checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "errno"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "errno-dragonfly"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "fastrand"
-version = "1.8.0"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a407cfaa3385c4ae6b23e84623d48c2798d06e3e6a1878f7f59f17b3f86499"
+checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
@@ -289,65 +310,65 @@
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52ba265a92256105f45b719605a571ffe2d1f0fea3807304b522c1d778f79eed"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04909a7a7e4633ae6c4a9ab280aeb86da1236243a77b694a49eacd659a4bd3ac"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-io"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00f5fb52a06bdcadeb54e8d3671f8888a39697dcb0b81b23b55174030427f4eb"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-sink"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39c15cf1a4aa79df40f1bb462fb39676d0ad9e366c2a33b590d7c66f4f81fcf9"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ffb393ac5d9a6eaa9d3fdf37ae2776656b706e200c8e16b1bdb227f5198e6ea"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-util"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "197676987abd2f9cadff84926f410af1c183608d36641465df73ae8211dc65d6"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-core",
  "futures-io",
  "futures-task",
  "memchr",
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.15"
+version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f9f29bc9dda355256b2916cf526ab02ce0aeaaaf2bad60d65ef3f12f11dd0f4"
+checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -368,39 +389,36 @@
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "heck"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2540771e65fc8cb83cd6e8a237f70c319bd5c29f78ed1084ba5d50eeac86f7f9"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.1.19"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
+checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
 name = "hifitime"
-version = "3.8.0"
+version = "3.8.1"
 dependencies = [
  "criterion",
  "der",
  "iai",
  "lexical-core",
  "num-traits",
  "openssl",
@@ -410,17 +428,17 @@
  "serde_derive",
  "serde_json",
  "tabled",
 ]
 
 [[package]]
 name = "http"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75f43d41e26995c17e71ee126451dd3941010b0514a81a9d11f3b341debc2399"
+checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
@@ -444,17 +462,17 @@
 name = "httpdate"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
 
 [[package]]
 name = "hyper"
-version = "0.14.23"
+version = "0.14.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "034711faac9d2166cb1baf1a2fb0b60b1f277f8492fd72176c17f3515e1abd3c"
+checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
@@ -497,63 +515,86 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da2d6f23ffea9d7e76c53eee25dfb67bcd8fde7f1198b0855350698c9f07c780"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "io-lifetimes"
+version = "1.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
+dependencies = [
+ "hermit-abi 0.3.1",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "ipnet"
-version = "2.7.0"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11b0d96e660696543b251e58030cf9787df56da39dab19ad60eae7353040917e"
+checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
+
+[[package]]
+name = "is-terminal"
+version = "0.4.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+dependencies = [
+ "hermit-abi 0.3.1",
+ "io-lifetimes",
+ "rustix",
+ "windows-sys 0.48.0",
+]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.5"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.60"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49409df3e3bf0856b916e2ceaca09ee28e6871cf7d9ce97a692cacfdb2a25a47"
+checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -599,23 +640,29 @@
 checksum = "5255b9ff16ff898710eb9eb63cb39248ea8a5bb036bea8085b1a767ff6c4e3fc"
 dependencies = [
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "libm"
-version = "0.2.6"
+version = "0.2.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
+
+[[package]]
+name = "linux-raw-sys"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -636,46 +683,37 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "memoffset"
-version = "0.7.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mime"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a60c7ce501c71e03a9c9c0d35b861413ae925bd979cc7a4e30d060069aaac8d"
+checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "mio"
-version = "0.8.5"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5d732bc30207a6423068df043e3d02e0735b155ad7ce1a6f76fe2baa5b158de"
+checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
 dependencies = [
  "libc",
  "log",
  "wasi",
- "windows-sys 0.42.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "native-tls"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
@@ -710,90 +748,83 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "openssl"
-version = "0.10.45"
+version = "0.10.52"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b102428fd03bc5edf97f62620f7298614c45cedf287c271e7ed450bbaf83f2e1"
+checksum = "01b8574602df80f7b85fdfc5392fa884a4e3b3f4f35402c070ab34c3d3f78d56"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
 
 [[package]]
 name = "openssl-macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b501e44f11665960c7e7fcf062c7d96a14ade4aa98116c004b2e37b5be7d736c"
+checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "111.24.0+1.1.1s"
+version = "111.25.3+1.1.1t"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3498f259dab01178c6228c6b00dcef0ed2a2d5e20d648c017861227773ea4abd"
+checksum = "924757a6a226bf60da5f7dd0311a34d2b52283dd82ddeb103208ddc66362f80c"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.80"
+version = "0.9.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23bbbf7854cd45b83958ebe919f0e8e516793727652e27fda10a8384cfc790b7"
+checksum = "8e17f59264b2809d77ae94f0e1ebabc434773f370d6ca667bd223ea10e06cc7e"
 dependencies = [
- "autocfg",
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
-name = "os_str_bytes"
-version = "6.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
-
-[[package]]
 name = "papergrid"
-version = "0.7.1"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1526bb6aa9f10ec339fb10360f22c57edf81d5678d0278e93bc12a47ffbe4b01"
+checksum = "1fdfe703c51ddc52887ad78fc69cd2ea78d895ffcd6e955c9d03566db8ab5bb1"
 dependencies = [
  "bytecount",
  "fnv",
  "unicode-width",
 ]
 
 [[package]]
@@ -804,23 +835,23 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.5"
+version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff9f3fef3968a3ec5945535ed654cb38ff72d7495a25619e2247fb15a2ed9ba"
+checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
- "windows-sys 0.42.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
@@ -835,17 +866,17 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "plotters"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2538b639e642295546c50fcd545198c9d64ee2a38620a628724a3b266d5fbf97"
 dependencies = [
@@ -876,15 +907,15 @@
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro-error-attr"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -893,105 +924,105 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.49"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57a8eca9f9c4ffde41714334dee777596264c7825420f521abc92b5b5deb63a5"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.6.5",
+ "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db3a213adf02b3bcfd2d3846bb41cb22857d131789e01df434fb7e7bc0759b7"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.10.1"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cac410af5d00ab6884528b4ab69d1e8e146e8d471201800fa1b4524126de6ad3"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
@@ -1001,42 +1032,42 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
-name = "regex"
-version = "1.7.0"
+name = "redox_syscall"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e076559ef8e241f2ae3479e36f97bd5741c0330689e217ad51ce2c76808b868a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "regex-syntax",
+ "bitflags",
 ]
 
 [[package]]
-name = "regex-syntax"
-version = "0.6.28"
+name = "regex"
+version = "1.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
+dependencies = [
+ "regex-syntax",
+]
 
 [[package]]
-name = "remove_dir_all"
-version = "0.5.3"
+name = "regex-syntax"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
-dependencies = [
- "winapi",
-]
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "reqwest"
-version = "0.11.13"
+version = "0.11.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68cc60575865c7831548863cc02356512e3f1dc2f3f82cb837d7fc4cc8f3c97c"
+checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
 dependencies = [
  "base64",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
@@ -1062,92 +1093,105 @@
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
+name = "rustix"
+version = "0.37.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
+dependencies = [
+ "bitflags",
+ "errno",
+ "io-lifetimes",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "ryu"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b4b9743ed687d4b4bcedf9ff5eaa7398495ae14e61cba0a295704edbc7decde"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "schannel"
-version = "0.1.20"
+version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88d6731146462ea25d9244b2ed5fd1d716d25c52e4d54aa4fb0f3c4e9854dbe2"
+checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
 dependencies = [
- "lazy_static",
- "windows-sys 0.36.1",
+ "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "security-framework"
-version = "2.7.0"
+version = "2.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2bc1bb97804af6631813c55739f771071e0f2ed33ee20b68c86ec505d906356c"
+checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
 dependencies = [
  "bitflags",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.6.1"
+version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0160a13a177a45bfb43ce71c01580998474f556ad854dcbca936dd2841a5c556"
+checksum = "f51d0c0d83bec45f16480d0ce0058397a69e48fcdc52d1dc8855fb68acbd31a7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.152"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.91"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "877c235533714907a8c2464236f5c4b2a17262ef1bd71f38f35ea592c8da6883"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1160,105 +1204,109 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "slab"
-version = "0.4.7"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4614a76b2a8be0058caa9dbbaf66d988527d86d003c11a94fbd335d7661edcef"
+checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "socket2"
-version = "0.4.7"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02e2d2db9033d13a1567121ddd7a095ee144db4e1ca1b1bda3419bc0da294ebd"
+checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "syn"
+version = "2.0.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "tabled"
-version = "0.10.0"
+version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56c3ee73732ffceaea7b8f6b719ce3bb17f253fa27461ffeaf568ebd0cdb4b85"
+checksum = "da1a2e56bbf7bfdd08aaa7592157a742205459eff774b73bc01809ae2d99dc2a"
 dependencies = [
  "papergrid",
  "tabled_derive",
  "unicode-width",
 ]
 
 [[package]]
 name = "tabled_derive"
-version = "0.5.0"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "beca1b4eaceb4f2755df858b88d9b9315b7ccfd1ffd0d7a48a52602301f01a57"
+checksum = "99f688a08b54f4f02f0a3c382aefdb7884d3d69609f785bd253dc033243e3fe4"
 dependencies = [
  "heck",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
-version = "3.3.0"
+version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5cdb1ef4eaeeaddc8fbd371e5017057064af0911902ef36b39801f67cc6d79e4"
+checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
  "cfg-if",
  "fastrand",
- "libc",
- "redox_syscall",
- "remove_dir_all",
- "winapi",
+ "redox_syscall 0.3.5",
+ "rustix",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
-name = "textwrap"
-version = "0.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
-
-[[package]]
 name = "tinytemplate"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
 dependencies = [
  "serde",
  "serde_json",
@@ -1271,50 +1319,49 @@
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
  "tinyvec_macros",
 ]
 
 [[package]]
 name = "tinyvec_macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cda74da7e1a664f795bb1f8a87ec406fb89a02522cf6e50620d016add6dbbf5c"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.23.0"
+version = "1.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eab6d665857cc6ca78d6e80303a02cea7a7851e85dfbd77cbdc09bd129f1ef46"
+checksum = "0aa32867d44e6f2ce3385e89dceb990188b8bb0fb25b0cf576647a6f98ac5105"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
- "memchr",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "socket2",
- "windows-sys 0.42.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-native-tls"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7d995660bd2b7f8c1568414c1126076c13fbb725c40112dc0120b78eb9b717b"
+checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
 dependencies = [
  "native-tls",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.4"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bb2e075f03b3d66d8d8785356224ba688d2906a371015e225beeb65ca92c740"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
@@ -1335,38 +1382,38 @@
  "cfg-if",
  "pin-project-lite",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "try-lock"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59547bce71d9c38b83d9c0e92b6066c4253371f15005def0c30d9657f50c7642"
+checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.8"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "099b7128301d285f79ddd55b9a83d5e6b9e97c92e0ea0daebee7263e932de992"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -1406,20 +1453,19 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.3.2"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "808cf2735cd4b6866113f648b791c6adc5714537bc222d9347bb203386ffda56"
+checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
- "winapi",
  "winapi-util",
 ]
 
 [[package]]
 name = "want"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1433,83 +1479,83 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eaf9f5aceeec8be17c128b2e93e031fb8a4d469bb9c4ae2d7dc1888b26887268"
+checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8ffb332579b0557b52d268b91feab8df3615f265d5270fec2a8c95b17c1142"
+checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.33"
+version = "0.4.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23639446165ca5a5de86ae1d8896b737ae80319560fbaa4c2887b7da6e7ebd7d"
+checksum = "2d1985d03709c53167ce907ff394f5316aa22cb4e12761295c5dc57dacb6297e"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "052be0f94026e6cbc75cdefc9bae13fd6052cdcaf532fa6c45e7ae33a1e6c810"
+checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07bc0c051dc5f23e307b13285f9d75df86bfdf816c5721e573dec1f9b8aa193c"
+checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c38c045535d93ec4f0b4defec448e4291638ee608530863b1e2ba115d4fff7f"
+checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
 
 [[package]]
 name = "web-sys"
-version = "0.3.60"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcda906d8be16e728fd5adc5b729afad4e444e106ab28cd1c7256e54fa61510f"
+checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
@@ -1540,111 +1586,158 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.36.1"
+version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea04155a16a59f9eab786fe12a4a450e75cdb175f9e0d80da1e17db09f55b8d2"
+checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
- "windows_aarch64_msvc 0.36.1",
- "windows_i686_gnu 0.36.1",
- "windows_i686_msvc 0.36.1",
- "windows_x86_64_gnu 0.36.1",
- "windows_x86_64_msvc 0.36.1",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+dependencies = [
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+dependencies = [
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc 0.42.0",
- "windows_i686_gnu 0.42.0",
- "windows_i686_msvc 0.42.0",
- "windows_x86_64_gnu 0.42.0",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc 0.42.0",
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.0"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d2aa71f6f0cbe00ae5167d90ef3cfe66527d6f613ca78ac8024c3ccab9a19e"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9bb8c3fd39ade2d67e9874ac4f3db21f0d710bee00fe7cab16949ec184eeaa47"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0f252f5a35cac83d6311b2e795981f5ee6e67eb1f9a7f64eb4500fbc4dcdb4"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "180e6ccf01daf4c426b846dfc66db1fc518f074baa793aa7d9b9aaeffad6a3b6"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbeae19f6716841636c28d695375df17562ca208b2b7d0dc47635a50ae6c5de7"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2e7917148b2812d1eeafaeb22a97e4813dfa60a3f8f78ebe204bcc88f12f024"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c12f65daa39dd2babe6e442988fc329d6243fdce47d7d2d155b8d874862246"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dcd171b8776c41b97521e5da127a2d86ad280114807d0b2ab1e462bc764d9e1"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7b1b21b5362cbc318f686150e5bcea75ecedc74dd157d874d754a2ca44b0ed"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.0"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09d525d2ba30eeb3297665bd434a54297e4170c7f1a44cad4ef58095b4cd2028"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c811ca4a8c853ef420abd8592ba53ddbbac90410fab6903b3e79972a631f7680"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f40009d85759725a34da6d89a94e63d7bdc50a862acf0dbc7c8e488f1edcb6f5"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winreg"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
 dependencies = [
```

### Comparing `hifitime-3.8.0/PKG-INFO` & `hifitime-3.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hifitime
-Version: 3.8.0
+Version: 3.8.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Science/Research
 License-File: LICENSE.txt
 Summary: Ultra-precise date and time handling in Rust for scientific applications with leap second support
 Keywords: date,time,science,leap-second,no-std
@@ -12,225 +12,292 @@
 Author: Christopher Rabotin <christopher.rabotin@gmail.com>
 Author-email: Christopher Rabotin <christopher.rabotin@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/nyx-space/hifitime
 
-# hifitime 3
+# Introduction to Hifitime
 
-Scientifically accurate date and time handling with guaranteed nanosecond precision for 32,768 years _before_ 01 January 1900 and 32,767 years _after_ that reference epoch.
-Formally verified to not crash on operations on epochs and durations using the [`Kani`](https://model-checking.github.io/kani/) model checking.
+Hifitime is a powerful Rust and Python library designed for time management. It provides extensive functionalities with precise operations for time calculation in different time scales, making it suitable for engineering and scientific applications where general relativity and time dilation matter. Hifitime guarantees nanosecond precision for 65,536 years around 01 January 1900 TAI. Hifitime is also formally verified using the [`Kani` model checker](https://model-checking.github.io/kani/), read more about it [this verification here](https://model-checking.github.io/kani-verifier-blog/2023/03/31/how-kani-helped-find-bugs-in-hifitime.html).
 
-[![hifitime on crates.io][cratesio-image]][cratesio]
-[![hifitime on docs.rs][docsrs-image]][docsrs]
-[![minimum rustc: 1.58](https://img.shields.io/badge/minimum%20rustc-1.58-yellowgreen?logo=rust)](https://www.whatrustisit.com)
-[![Build Status](https://github.com/nyx-space/hifitime/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/nyx-space/hifitime/actions)
-[![Build Status](https://github.com/nyx-space/hifitime/actions/workflows/formal_verification.yml/badge.svg?branch=master)](https://github.com/nyx-space/hifitime/actions)
-[![codecov](https://codecov.io/gh/nyx-space/hifitime/branch/master/graph/badge.svg?token=l7zU57rUGs)](https://codecov.io/gh/nyx-space/hifitime)
-
-[cratesio-image]: https://img.shields.io/crates/v/hifitime.svg
-[cratesio]: https://crates.io/crates/hifitime
-[docsrs-image]: https://docs.rs/hifitime/badge.svg
-[docsrs]: https://docs.rs/hifitime/
-
-
-# Features
-
- * [x] Initialize a high precision Epoch from the system time in UTC
- * [x] Leap seconds (as announced by the IETF on a yearly basis)
- * [x] UTC representation with ISO8601 and RFC3339 formatting and blazing fast parsing (45 nanoseconds)
- * [x] Trivial support of time arithmetic: addition (e.g. `2.hours() + 3.seconds()`), subtraction (e.g. `2.hours() - 3.seconds()`), round/floor/ceil operations (e.g. `2.hours().round(3.seconds())`)
- * [x] Supports ranges of Epochs and TimeSeries (linspace of `Epoch`s and `Duration`s)
- * [x] Trivial conversion between many time scales
- * [x] High fidelity Ephemeris Time / Dynamic Barycentric Time (TDB) computations from [ESA's Navipedia](https://gssc.esa.int/navipedia/index.php/Transformations_between_Time_Systems#TDT_-_TDB.2C_TCB)
- * [x] Julian dates and Modified Julian dates
- * [x] Embedded device friendly: `no-std` and `const fn` where possible
-
-This library is validated against NASA/NAIF SPICE for the Ephemeris Time to Universal Coordinated Time computations: there are exactly zero nanoseconds of difference between SPICE and hifitime for the computation of ET and UTC after 01 January 1972. Refer to the [leap second](#leap-second-support) section for details. Other examples are validated with external references, as detailed on a test-by-test basis.
+Most users of Hifitime will only need to rely on the `Epoch` and `Duration` structures, and optionally the `Weekday` enum for week based computations. Scientific applications may make use of the `TimeScale` enum as well.
 
-## Supported time scales
+## Usage
 
-+ Temps Atomique International (TAI)
-+ Universal Coordinated Time (UTC)
-+ Terrestrial Time (TT)
-+ Ephemeris Time (ET) without the small perturbations as per NASA/NAIF SPICE leap seconds kernel
-+ Dynamic Barycentric Time (TDB), a higher fidelity ephemeris time
-+ Global Positioning System (GPST)
-+ Galileo System Time (GST)
-+ BeiDou Time (BDT)
-+ UNIX
-## Non-features
-* Time-agnostic / date-only epochs. Hifitime only supports the combination of date and time, but the `Epoch::{at_midnight, at_noon}` is provided as a helper function.
+First, install `hifitime` either with `cargo add hifitime` in your Rust project or `pip install hifitime` in Python.
 
-# Usage
+If building from source, note that the Python package is only built if the `python` feature is enabled.
 
-Put this in your `Cargo.toml`:
+### Epoch ("datetime" equivalent)
 
-```toml
-[dependencies]
-hifitime = "3.7"
-```
+**Create an epoch in different time scales.**
 
-## Examples:
-### Time creation
 ```rust
-use hifitime::{Epoch, Unit, TimeUnits};
+use hifitime::prelude::*;
 use core::str::FromStr;
+// Create an epoch in UTC
+let epoch = Epoch::from_gregorian_utc(2000, 2, 29, 14, 57, 29, 37);
+// Or from a string
+let epoch_from_str = Epoch::from_str("2000-02-29T14:57:29.000000037 UTC").unwrap();
+assert_eq!(epoch, epoch_from_str);
+// Creating it from TAI will effectively show the number of leap seconds in between UTC an TAI at that epoch
+let epoch_tai = Epoch::from_gregorian_tai(2000, 2, 29, 14, 57, 29, 37);
+// The difference between two epochs is a Duration
+let num_leap_s = epoch - epoch_tai;
+assert_eq!(format!("{num_leap_s}"), "32 s");
+
+// Trivially convert to another time scale
+// Either by grabbing a subdivision of time in that time scale
+assert_eq!(epoch.to_gpst_days(), 7359.623402777777); // Compare to the GPS time scale
+
+// Or by fetching the exact duration
+let mjd_offset = Duration::from_str("51603 days 14 h 58 min 33 s 184 ms 37 ns").unwrap();
+assert_eq!(epoch.to_mjd_tt_duration(), mjd_offset); // Compare to the modified Julian days in the Terrestrial Time time scale.
+```
 
-#[cfg(feature = "std")]
-{
-// Initialization from system time is only available when std feature is enabled
-let now = Epoch::now().unwrap();
-println!("{}", now);
-}
+In Python:
+```python
+>>> from hifitime import *
+>>> epoch = Epoch("2000-02-29T14:57:29.000000037 UTC")
+>>> epoch
+2000-02-29T14:57:29.000000037 UTC
+>>> epoch_tai = Epoch.init_from_gregorian_tai(2000, 2, 29, 14, 57, 29, 37)
+>>> epoch_tai
+2000-02-29T14:57:29.000000037 TAI
+>>> epoch.timedelta(epoch_tai)
+32 s
+>>> epoch.to_gpst_days()
+7359.623402777777
+>>> epoch.to_mjd_tt_duration()
+51603 days 14 h 58 min 33 s 184 ms 37 ns
+>>> 
+```
 
-let mut santa = Epoch::from_gregorian_utc_hms(2017, 12, 25, 01, 02, 14);
-assert_eq!(santa.to_mjd_utc_days(), 58112.043217592590);
-assert_eq!(santa.to_jde_utc_days(), 2458112.5432175924);
+**Hifitime provides several date time formats like RFC2822, ISO8601, or RFC3339.**
 
-assert_eq!(
-    santa + 3600 * Unit::Second,
-    Epoch::from_gregorian_utc_hms(2017, 12, 25, 02, 02, 14),
-    "Could not add one hour to Christmas"
-);
+```rust
+use hifitime::efmt::consts::{ISO8601, RFC2822, RFC3339};
+use hifitime::prelude::*;
 
+let epoch = Epoch::from_gregorian_utc(2000, 2, 29, 14, 57, 29, 37);
+// The default Display shows the UTC time scale
+assert_eq!(format!("{epoch}"), "2000-02-29T14:57:29.000000037 UTC");
+// Format it in RFC 2822
+let fmt = Formatter::new(epoch, RFC2822);
+assert_eq!(format!("{fmt}"), format!("Tue, 29 Feb 2000 14:57:29"));
+
+// Or in ISO8601
+let fmt = Formatter::new(epoch, ISO8601);
 assert_eq!(
-    santa + 60.0.minutes(),
-    Epoch::from_gregorian_utc_hms(2017, 12, 25, 02, 02, 14),
-    "Could not add one hour to Christmas"
+    format!("{fmt}"),
+    format!("2000-02-29T14:57:29.000000037 UTC")
 );
 
+// Which is somewhat similar to RFC3339
+let fmt = Formatter::new(epoch, RFC3339);
 assert_eq!(
-    santa + 1.hours(),
-    Epoch::from_gregorian_utc_hms(2017, 12, 25, 02, 02, 14),
-    "Could not add one hour to Christmas"
+    format!("{fmt}"),
+    format!("2000-02-29T14:57:29.000000037+00:00")
 );
-
-let dt = Epoch::from_gregorian_utc_hms(2017, 1, 14, 0, 31, 55);
-assert_eq!(dt, Epoch::from_str("2017-01-14T00:31:55 UTC").unwrap());
-// And you can print it too, although by default it will print in UTC
-assert_eq!(format!("{}", dt), "2017-01-14T00:31:55 UTC".to_string());
-
 ```
-### Time differences, time unit, and duration handling
 
-Comparing times will lead to a Duration type. Printing that will automatically select the unit.
+**Need some custom format? Hifitime also supports the C89 token, cf. [the documentation](https://docs.rs/hifitime/latest/hifitime/efmt/format/struct.Format.html).**
 
 ```rust
-use hifitime::{Epoch, Unit, Duration, TimeUnits};
+use core::str::FromStr;
+use hifitime::prelude::*;
 
-let at_midnight = Epoch::from_gregorian_utc_at_midnight(2020, 11, 2);
-let at_noon = Epoch::from_gregorian_utc_at_noon(2020, 11, 2);
-assert_eq!(at_noon - at_midnight, 12 * Unit::Hour);
-assert_eq!(at_noon - at_midnight, 1 * Unit::Day / 2);
-assert_eq!(at_midnight - at_noon, -1.days() / 2);
-
-let delta_time = at_noon - at_midnight;
-assert_eq!(format!("{}", delta_time), "12 h".to_string());
-// And we can multiply durations by a scalar...
-let delta2 = 2 * delta_time;
-assert_eq!(format!("{}", delta2), "1 days".to_string());
-// Or divide them by a scalar.
-assert_eq!(format!("{}", delta2 / 2.0), "12 h".to_string());
-
-// And of course, these comparisons account for differences in time scales
-let at_midnight_utc = Epoch::from_gregorian_utc_at_midnight(2020, 11, 2);
-let at_noon_tai = Epoch::from_gregorian_tai_at_noon(2020, 11, 2);
-assert_eq!(format!("{}", at_noon_tai - at_midnight_utc), "11 h 59 min 23 s".to_string());
-```
+let epoch = Epoch::from_gregorian_utc_hms(2015, 2, 7, 11, 22, 33);
 
-Timeunits and frequency units are trivially supported. Hifitime only supports up to nanosecond precision (but guarantees it for 64 millenia), so any duration less than one nanosecond is truncated.
+// Parsing with a custom format
+assert_eq!(
+    Epoch::from_format_str("Sat, 07 Feb 2015 11:22:33", "%a, %d %b %Y %H:%M:%S").unwrap(),
+    epoch
+);
+
+// And printing with a custom format
+let fmt = Format::from_str("%a, %d %b %Y %H:%M:%S").unwrap();
+assert_eq!(
+    format!("{}", Formatter::new(epoch, fmt)),
+    "Sat, 07 Feb 2015 11:22:33"
+);
+```
 
+**You can also grab the current system time in UTC, if the `std` feature is enabled (default), and find the next or previous day of the week.**
 ```rust
-use hifitime::{Epoch, Unit, Freq, Duration, TimeUnits};
+use hifitime::prelude::*;
 
-// One can compare durations
-assert!(10.seconds() > 5.seconds());
-assert!(10.days() + 1.nanoseconds() > 10.days());
-
-// Those durations are more precise than floating point since this is integer math in nanoseconds
-let d: Duration = 1.0.hours() / 3 - 20.minutes();
-assert!(d.abs() < Unit::Nanosecond);
-assert_eq!(3 * 20.minutes(), Unit::Hour);
-
-// And also frequencies but note that frequencies are converted to Durations!
-// So the duration of that frequency is compared, hence the following:
-assert!(10 * Freq::Hertz < 5 * Freq::Hertz);
-assert!(4 * Freq::MegaHertz > 5 * Freq::MegaHertz);
-
-// And asserts on the units themselves
-assert!(Freq::GigaHertz < Freq::MegaHertz);
-assert!(Unit::Second > Unit::Millisecond);
+#[cfg(feature = "std")]
+{
+    let now = Epoch::now().unwrap();
+    println!("{}", now.next(Weekday::Tuesday));
+    println!("{}", now.previous(Weekday::Sunday));
+}
 ```
 
-### Iterating over times ("linspace" of epochs)
-Finally, something which may come in very handy, line spaces between times with a given step.
+**Oftentimes, we'll want to query something at a fixed step between two epochs. Hifitime makes this trivial with `TimeSeries`.**
 
 ```rust
-use hifitime::{Epoch, Unit, TimeSeries};
+use hifitime::prelude::*;
+
 let start = Epoch::from_gregorian_utc_at_midnight(2017, 1, 14);
-let end = Epoch::from_gregorian_utc_at_noon(2017, 1, 14);
-let step = 2 * Unit::Hour;
+let end = start + 12.hours();
+let step = 2.hours();
+
 let time_series = TimeSeries::inclusive(start, end, step);
 let mut cnt = 0;
 for epoch in time_series {
+    #[cfg(feature = "std")]
     println!("{}", epoch);
     cnt += 1
 }
-// Check that there are indeed six two-hour periods in a half a day,
+// Check that there are indeed seven two-hour periods in a half a day,
 // including start and end times.
 assert_eq!(cnt, 7)
 ```
 
+In Python:
+```python
+>>> from hifitime import *
+>>> start = Epoch.init_from_gregorian_utc_at_midnight(2017, 1, 14)
+>>> end = start + Unit.Hour*12
+>>> iterator = TimeSeries(start, end, step=Unit.Hour*2, inclusive=True)
+>>> for epoch in iterator:
+...     print(epoch)
+... 
+2017-01-14T00:00:00 UTC
+2017-01-14T02:00:00 UTC
+2017-01-14T04:00:00 UTC
+2017-01-14T06:00:00 UTC
+2017-01-14T08:00:00 UTC
+2017-01-14T10:00:00 UTC
+2017-01-14T12:00:00 UTC
+>>> 
+
+```
+
+### Duration
+
+```rust
+use hifitime::prelude::*;
+use core::str::FromStr;
+
+// Create a duration using the `TimeUnits` helping trait.
+let d = 5.minutes() + 7.minutes() + 35.nanoseconds();
+assert_eq!(format!("{d}"), "12 min 35 ns");
+
+// Or using the built-in enums
+let d_enum = 12 * Unit::Minute + 35.0 * Unit::Nanosecond;
+
+// But it can also be created from a string
+let d_from_str = Duration::from_str("12 min 35 ns").unwrap();
+assert_eq!(d, d_from_str);
+```
+
+**Hifitime guarantees nanosecond precision, but most human applications don't care too much about that. Durations can be rounded to provide a useful approximation for humans.**
+
+```rust
+use hifitime::prelude::*;
+
+// Create a duration using the `TimeUnits` helping trait.
+let d = 5.minutes() + 7.minutes() + 35.nanoseconds();
+// Round to the nearest minute
+let rounded = d.round(1.minutes());
+assert_eq!(format!("{rounded}"), "12 min");
+
+// And this works on Epochs as well.
+let previous_post = Epoch::from_gregorian_utc_hms(2015, 2, 7, 11, 22, 33);
+let example_now = Epoch::from_gregorian_utc_hms(2015, 8, 17, 22, 55, 01);
+
+// We'll round to the nearest fifteen days
+let this_much_ago = example_now - previous_post;
+assert_eq!(format!("{this_much_ago}"), "191 days 11 h 32 min 29 s");
+let about_this_much_ago_floor = this_much_ago.floor(15.days());
+assert_eq!(format!("{about_this_much_ago_floor}"), "180 days");
+let about_this_much_ago_ceil = this_much_ago.ceil(15.days());
+assert_eq!(format!("{about_this_much_ago_ceil}"), "195 days");
+```
+
+In Python:
+
+```python
+>>> from hifitime import *
+>>> d = Duration("12 min 32 ns")
+>>> d.round(Unit.Minute*1)
+12 min
+>>> d
+12 min 32 ns
+>>> 
+```
+
+[![hifitime on crates.io][cratesio-image]][cratesio]
+[![hifitime on docs.rs][docsrs-image]][docsrs]
+[![minimum rustc: 1.64](https://img.shields.io/badge/minimum%20rustc-1.64-yellowgreen?logo=rust)](https://www.whatrustisit.com)
+[![Build Status](https://github.com/nyx-space/hifitime/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/nyx-space/hifitime/actions)
+[![Build Status](https://github.com/nyx-space/hifitime/actions/workflows/formal_verification.yml/badge.svg?branch=master)](https://github.com/nyx-space/hifitime/actions)
+[![codecov](https://codecov.io/gh/nyx-space/hifitime/branch/master/graph/badge.svg?token=l7zU57rUGs)](https://codecov.io/gh/nyx-space/hifitime)
+
+[cratesio-image]: https://img.shields.io/crates/v/hifitime.svg
+[cratesio]: https://crates.io/crates/hifitime
+[docsrs-image]: https://docs.rs/hifitime/badge.svg
+[docsrs]: https://docs.rs/hifitime/
+
+# Comparison with `time` and `chrono`
+
+First off, both `time` and `chrono` are fantastic libraries in their own right. There's a reason why they have millions and millions of downloads. Secondly, hifitime was started in October 2017, so quite a while before the revival of `time` (~ 2019).
+
+One of the key differences is that both `chrono` and `time` separate the concepts of "time" and "date." Hifitime asserts that this is physically invalid: both a time and a date are an offset from a reference in a given time scale. That's why, Hifitime does not separate the components that make up a date, but instead, only stores a fixed duration with respect to TAI. Moreover, Hifitime is formally verified with a model checker, which is much more thorough than property testing.
+
+More importantly, neither `time` nor `chrono` are suitable for astronomy, astrodynamics, or any physics that must account for time dilation due to relativistic speeds or lack of the Earth as a gravity source (which sets the "tick" of a second).
+
+Hifitime also natively supports the UT1 time scale (the only "true" time) if built with the `ut1` feature.
+
+# Features
+
+ * [x] Initialize a high precision Epoch from the system time in UTC
+ * [x] Leap seconds (as announced by the IETF on a yearly basis)
+ * [x] UTC representation with ISO8601 and RFC3339 formatting and blazing fast parsing (45 nanoseconds)
+ * [x] Trivial support of time arithmetic: addition (e.g. `2.hours() + 3.seconds()`), subtraction (e.g. `2.hours() - 3.seconds()`), round/floor/ceil operations (e.g. `2.hours().round(3.seconds())`)
+ * [x] Supports ranges of Epochs and TimeSeries (linspace of `Epoch`s and `Duration`s)
+ * [x] Trivial conversion between many time scales
+ * [x] High fidelity Ephemeris Time / Dynamic Barycentric Time (TDB) computations from [ESA's Navipedia](https://gssc.esa.int/navipedia/index.php/Transformations_between_Time_Systems#TDT_-_TDB.2C_TCB)
+ * [x] Julian dates and Modified Julian dates
+ * [x] Embedded device friendly: `no-std` and `const fn` where possible
+
+This library is validated against NASA/NAIF SPICE for the Ephemeris Time to Universal Coordinated Time computations: there are exactly zero nanoseconds of difference between SPICE and hifitime for the computation of ET and UTC after 01 January 1972. Refer to the [leap second](#leap-second-support) section for details. Other examples are validated with external references, as detailed on a test-by-test basis.
+
+## Supported time scales
+
++ Temps Atomique International (TAI)
++ Universal Coordinated Time (UTC)
++ Terrestrial Time (TT)
++ Ephemeris Time (ET) without the small perturbations as per NASA/NAIF SPICE leap seconds kernel
++ Dynamic Barycentric Time (TDB), a higher fidelity ephemeris time
++ Global Positioning System (GPST)
++ Galileo System Time (GST)
++ BeiDou Time (BDT)
++ UNIX
+## Non-features
+* Time-agnostic / date-only epochs. Hifitime only supports the combination of date and time, but the `Epoch::{at_midnight, at_noon}` is provided as helper functions.
+
 # Design
-No software is perfect, so please report any issue or bugs on [Github](https://github.com/nyx-space/hifitime/issues/new).
+No software is perfect, so please report any issue or bug on [Github](https://github.com/nyx-space/hifitime/issues/new).
 
 ## Duration
 Under the hood, a Duration is represented as a 16 bit signed integer of centuries (`i16`) and a 64 bit unsigned integer (`u64`) of the nanoseconds past that century. The overflowing and underflowing of nanoseconds is handled by changing the number of centuries such that the nanoseconds number never represents more than one century (just over four centuries can be stored in 64 bits).
 
 Advantages:
 1. Exact precision of a duration: using a floating point value would cause large durations (e.g. Julian Dates) to have less precision than smaller durations. Durations in hifitime have exactly one nanosecond of precision for 65,536 years.
 2. Skipping floating point operations allows this library to be used in embedded devices without a floating point unit.
 3. Duration arithmetics are exact, e.g. one third of an hour is exactly twenty minutes and not "0.33333 hours."
 
 Disadvantages:
 1. Most astrodynamics applications require the computation of a duration in floating point values such as when querying an ephemeris. This design leads to an overhead of about 5.2 nanoseconds according to the benchmarks (`Duration to f64 seconds` benchmark). You may run the benchmarks with `cargo bench`.
 
-### Printing and parsing
-
-When Durations are printed, only the units whose value is non-zero is printed. For example, `5.hours() + 256.0.milliseconds() + 1.0.nanoseconds()` will be printed as "5 h 256 ms 1 ns".
-
-```rust
-use hifitime::{Duration, Unit, TimeUnits};
-use core::str::FromStr;
-
-assert_eq!(
-    format!(
-        "{}",
-        5.hours() + 256.0.milliseconds() + 1.0.nanoseconds()
-    ),
-    "5 h 256 ms 1 ns"
-);
-
-assert_eq!(
-    format!(
-        "{}",
-        5.days() + 1.0.nanoseconds()
-    ),
-    "5 days 1 ns"
-);
-
-
-assert_eq!(
-    Duration::from_str("5 h 256 ms 1 ns").unwrap(),
-    5 * Unit::Hour + 256 * Unit::Millisecond + Unit::Nanosecond
-);
-```
-
 ## Epoch
 The Epoch is simply a wrapper around a Duration. All epochs are stored in TAI duration with respect to 01 January 1900 at noon (the official TAI epoch). The choice of TAI meets the [Standard of Fundamental Astronomy (SOFA)](https://www.iausofa.org/) recommendation of opting for a glitch-free time scale (i.e. without discontinuities like leap seconds or non-uniform seconds like TDB).
 
 ### Printing and parsing
 
 Epochs can be formatted and parsed in the following time scales:
 
@@ -238,58 +305,14 @@
 + TAI: `{epoch:x}`
 + TT: `{epoch:X}`
 + TDB: `{epoch:e}`
 + ET: `{epoch:E}`
 + UNIX: `{epoch:p}`
 + GPS: `{epoch:o}`
 
-```rust
-use hifitime::{Epoch, TimeScale};
-use core::str::FromStr;
-
-let epoch = Epoch::from_gregorian_utc_hms(2022, 9, 6, 23, 24, 29);
-
-assert_eq!(format!("{epoch}"), "2022-09-06T23:24:29 UTC");
-assert_eq!(format!("{epoch:x}"), "2022-09-06T23:25:06 TAI");
-assert_eq!(format!("{epoch:X}"), "2022-09-06T23:25:38.184000000 TT");
-assert_eq!(format!("{epoch:E}"), "2022-09-06T23:25:38.182538909 ET");
-assert_eq!(format!("{epoch:e}"), "2022-09-06T23:25:38.182541259 TDB");
-assert_eq!(format!("{epoch:p}"), "1662506669"); // UNIX seconds
-assert_eq!(format!("{epoch:o}"), "1346541887000000000"); // GPS nanoseconds
-
-// RFC3339 parsing with time scales
-assert_eq!(
-    Epoch::from_gregorian_utc_hms(1994, 11, 5, 13, 15, 30),
-    Epoch::from_str("1994-11-05T08:15:30-05:00").unwrap()
-);
-assert_eq!(
-    Epoch::from_gregorian_utc_hms(1994, 11, 5, 13, 15, 30),
-    Epoch::from_str("1994-11-05T13:15:30Z").unwrap()
-);
-// Same test with different time systems
-// TAI
-assert_eq!(
-    Epoch::from_gregorian_tai_hms(1994, 11, 5, 13, 15, 30),
-    Epoch::from_str("1994-11-05T08:15:30-05:00 TAI").unwrap()
-);
-assert_eq!(
-    Epoch::from_gregorian_tai_hms(1994, 11, 5, 13, 15, 30),
-    Epoch::from_str("1994-11-05T13:15:30Z TAI").unwrap()
-);
-// TDB
-assert_eq!(
-    Epoch::from_gregorian_hms(1994, 11, 5, 13, 15, 30, TimeScale::TDB),
-    Epoch::from_str("1994-11-05T08:15:30-05:00 TDB").unwrap()
-);
-assert_eq!(
-    Epoch::from_gregorian_hms(1994, 11, 5, 13, 15, 30, TimeScale::TDB),
-    Epoch::from_str("1994-11-05T13:15:30Z TDB").unwrap()
-);
-```
-
 ## Leap second support
 
 Leap seconds allow TAI (the absolute time reference) and UTC (the civil time reference) to not drift too much. In short, UTC allows humans to see the sun at zenith at noon, whereas TAI does not worry about that. Leap seconds are introduced to allow for UTC to catch up with the absolute time reference of TAI. Specifically, UTC clocks are "stopped" for one second to make up for the accumulated difference between TAI and UTC. These leap seconds are announced several months in advance by IERS, cf. in the [IETF leap second reference](https://www.ietf.org/timezones/data/leap-seconds.list).
 
 The "placement" of these leap seconds in the formatting of a UTC date is left up to the software: there is no common way to handle this. Some software prevents a second tick, i.e. at 23:59:59 the UTC clock will tick for _two seconds_ (instead of one) before hoping to 00:00:00. Some software, like hifitime, allow UTC dates to be formatted as 23:59:60 on strictly the days when a leap second is inserted. For example, the date `2016-12-31 23:59:60 UTC` is a valid date in hifitime because a leap second was inserted on 01 Jan 2017.
 
 ### Important
@@ -300,14 +323,22 @@
 > Equation \[4\], which ignores small-period fluctuations, is accurate to about 0.000030 seconds.
 
 In order to provide full interoperability with NAIF, hifitime uses the NAIF algorithm for "ephemeris time" and the [ESA algorithm](https://gssc.esa.int/navipedia/index.php/Transformations_between_Time_Systems#TDT_-_TDB.2C_TCB) for "dynamical barycentric time." Hence, if exact NAIF behavior is needed, use all of the functions marked as `et` instead of the `tdb` functions, such as `epoch.to_et_seconds()` instead of `epoch.to_tdb_seconds()`.
 
 
 # Changelog
 
+## 3.8.2
++ Clarify README and add a section comparing Hifitime to `time` and `chrono`, cf. [#221](https://github.com/nyx-space/hifitime/issues/221)
++ Fix incorrect printing of Gregorian dates prior to to 1900, cf. [#204](https://github.com/nyx-space/hifitime/issues/204)
+
+## 3.8.1 (unreleased)
++ Fix documentation for the formatter, cf. [#202](https://github.com/nyx-space/hifitime/pull/202)
++ Update MSRV to 1.59 for rayon v 1.10
+
 ## 3.8.0
 Thanks again to [@gwbres](https://github.com/gwbres) for his work in this release!
 
 + Fix CI of the formal verification and upload artifacts, cf. [#179](https://github.com/nyx-space/hifitime/pull/179)
 + Introduce time of week construction and conversion by [@gwbres](https://github.com/gwbres), cf.[#180](https://github.com/nyx-space/hifitime/pull/180) and [#188](https://github.com/nyx-space/hifitime/pull/188)
 + Fix minor typo in `src/timeunits.rs` by [@gwbres](https://github.com/gwbres), cf. [#189](https://github.com/nyx-space/hifitime/pull/189)
 + Significantly extend formal verification of `Duration` and `Epoch`, and introduce `kani::Arbitrary` to `Duration` and `Epoch` for users to formally verify their use of time, cf. [#192](https://github.com/nyx-space/hifitime/pull/192)
@@ -378,12 +409,7 @@
 + Add pure nanosecond (`u64`) constructor and getter for GPST since GPS based clocks will count in nanoseconds
 ### Possibly breaking change
 + `Errors::ParseError` no longer contains a `String` but an enum `ParsingErrors` instead. This is considered possibly breaking because it would only break code in the cases where a datetime parsing or unit parsing was caught and handled (uncommon). Moreover, the output is still `Display`-able.
 ## 3.0.0
 + Backend rewritten from TwoFloat to a struct of the centuries in `i16` and nanoseconds in `u64`. Thanks to [@pwnorbitals](https://github.com/pwnorbitals) for proposing the idea in #[107](https://github.com/nyx-space/hifitime/issues/107) and writing the proof of concept. This leads to at least a 2x speed up in most calculations, cf. [this comment](https://github.com/nyx-space/hifitime/pull/107#issuecomment-1040702004).
 + Fix GPS epoch, and addition of a helper functions in `Epoch` by [@cjordan](https://github.com/cjordan)
 
-## 2.2.3
-+ More deterministic `as_jde_tdb_days()` in `Epoch`. In version 2.2.1, the ephemeris time and TDB _days_ were identical down to machine precision. After a number of validation cases in the rotation equations of the IAU Earth to Earth Mean Equator J2000 frame, the new formulation was shown to lead to less rounding errors when requesting the days. These rounding errors prevented otherwise trivial test cases. However, it adds an error of **40.2 nanoseconds** when initializing an Epoch with the days in ET and requesting the TDB days.
-
-_Note:_ this was originally published as 2.2.2 but I'd forgotten to update one of the tests with the 40.2 ns error.
-
```

