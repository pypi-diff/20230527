# Comparing `tmp/fast-matrix-market-1.5.1.tar.gz` & `tmp/fast-matrix-market-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-matrix-market-1.5.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "fast-matrix-market-1.6.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `fast-matrix-market-1.5.1.tar` & `fast-matrix-market-1.6.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/CMakeLists.txt
--rw-r--r--   0        0        0     1275 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/LICENSE.txt
--rw-r--r--   0        0        0     5292 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/README.md
--rw-r--r--   0        0        0     6336 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/benchmark/bench_fmm.py
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/benchmark/requirements.txt
--rwxr-xr-x   0        0        0      742 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/benchmark/run.sh
--rw-r--r--   0        0        0     4592 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/CMakeLists.txt
--rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/Blaze.cmake
--rw-r--r--   0        0        0      269 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/Dragonbox.cmake
--rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/Eigen.cmake
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/GoogleBenchmark.cmake
--rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/GoogleTest.cmake
--rw-r--r--   0        0        0     1529 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/GraphBLAS.cmake
--rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/fast_float.cmake
--rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/from_chars_tests.cmake
--rw-r--r--   0        0        0      986 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/to_chars_tests.cmake
--rw-r--r--   0        0        0     1026 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/README.md
--rw-r--r--   0        0        0     3811 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt
--rw-r--r--   0        0        0    12262 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM
--rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/cmake/dragonboxConfig.cmake
--rw-r--r--   0        0        0   144785 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h
--rw-r--r--   0        0        0     4769 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h
--rw-r--r--   0        0        0    25425 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp
--rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/CMakeLists.txt
--rw-r--r--   0        0        0    10767 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE
--rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/LICENSE-MIT
--rw-r--r--   0        0        0   118134 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h
--rw-r--r--   0        0        0     1695 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/CMakeLists.txt
--rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/LICENSE-Apache2
--rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/LICENSE-Boost
--rw-r--r--   0        0        0     3648 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/common.h
--rw-r--r--   0        0        0    26321 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c
--rw-r--r--   0        0        0   329074 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h
--rw-r--r--   0        0        0    17721 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s.c
--rw-r--r--   0        0        0    34501 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h
--rw-r--r--   0        0        0    13015 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h
--rw-r--r--   0        0        0     7434 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h
--rw-r--r--   0        0        0     1745 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/digit_table.h
--rw-r--r--   0        0        0    11279 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/f2s.c
--rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h
--rw-r--r--   0        0        0     4294 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h
--rw-r--r--   0        0        0    11093 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/generic_128.c
--rw-r--r--   0        0        0    34192 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/generic_128.h
--rw-r--r--   0        0        0     1360 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/ryu.h
--rw-r--r--   0        0        0     2721 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/ryu_generic_128.h
--rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/ryu_parse.h
--rw-r--r--   0        0        0     8362 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/s2d.c
--rw-r--r--   0        0        0     8591 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/s2f.c
--rw-r--r--   0        0        0    15697 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/3rdparty/BS_thread_pool_light.hpp
--rw-r--r--   0        0        0     3967 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp
--rw-r--r--   0        0        0    15486 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp
--rw-r--r--   0        0        0     3152 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp
--rw-r--r--   0        0        0     7152 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp
--rw-r--r--   0        0        0    57554 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp
--rw-r--r--   0        0        0     4512 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/array.hpp
--rw-r--r--   0        0        0     4077 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp
--rw-r--r--   0        0        0     4111 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp
--rw-r--r--   0        0        0     3147 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/chunking.hpp
--rw-r--r--   0        0        0     5210 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp
--rw-r--r--   0        0        0    21141 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/field_conv.hpp
--rw-r--r--   0        0        0    14705 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/formatters.hpp
--rw-r--r--   0        0        0    10063 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/header.hpp
--rw-r--r--   0        0        0     9271 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp
--rw-r--r--   0        0        0    18534 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/read_body.hpp
--rw-r--r--   0        0        0     5487 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp
--rw-r--r--   0        0        0     4977 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/types.hpp
--rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/write_body.hpp
--rw-r--r--   0        0        0     2497 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp
--rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/pyproject.toml
--rw-r--r--   0        0        0    16022 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/src/fast_matrix_market/__init__.py
--rw-r--r--   0        0        0    23643 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/src/fast_matrix_market/core.cpp
--rw-r--r--   0        0        0    19432 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/src/fast_matrix_market/pystreambuf.h
--rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/eye3.mtx
--rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/long_double/longcomplex_array.mtx
--rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/long_double/longcomplex_coordinate.mtx
--rw-r--r--   0        0        0      113 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/long_double/longdouble_array.mtx
--rw-r--r--   0        0        0      124 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/long_double/longdouble_coordinate.mtx
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_array_complex_general.mtx
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_array_integer_general.mtx
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_array_real_general.mtx
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_complex_general.mtx
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_complex_hermitian.mtx
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_integer_general.mtx
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_pattern_general.mtx
--rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_pattern_symmetric.mtx
--rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_real_general.mtx
--rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_real_general.mtx.bz2
--rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_real_general.mtx.gz
--rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_real_skew-symmetric.mtx
--rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_real_symmetric.mtx
--rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/misc/windows_newlines.mtx
--rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/scipy_crashes/dim_over_32_bit.mtx
--rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/scipy_crashes/vector_array_real_general.mtx
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/scipy_crashes/vector_coordinate_real_general.mtx
--rw-r--r--   0        0        0     1769 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/test_array.py
--rw-r--r--   0        0        0      428 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/test_basic.py
--rw-r--r--   0        0        0     3194 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/test_coo.py
--rw-r--r--   0        0        0     3477 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/test_header.py
--rw-r--r--   0        0        0    13095 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/test_scipy.py
--rw-r--r--   0        0        0      927 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/testsuite_scipy/test_scipy_suite.py
--rw-r--r--   0        0        0     6405 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/CMakeLists.txt
+-rw-r--r--   0        0        0     1275 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     5292 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/README.md
+-rw-r--r--   0        0        0     6377 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/benchmark/bench_fmm.py
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/benchmark/requirements.txt
+-rwxr-xr-x   0        0        0      742 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/benchmark/run.sh
+-rw-r--r--   0        0        0     4592 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/CMakeLists.txt
+-rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/Blaze.cmake
+-rw-r--r--   0        0        0      269 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/Dragonbox.cmake
+-rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/Eigen.cmake
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/GoogleBenchmark.cmake
+-rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/GoogleTest.cmake
+-rw-r--r--   0        0        0     1529 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/GraphBLAS.cmake
+-rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/fast_float.cmake
+-rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/from_chars_tests.cmake
+-rw-r--r--   0        0        0      986 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/to_chars_tests.cmake
+-rw-r--r--   0        0        0     1026 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/README.md
+-rw-r--r--   0        0        0     3811 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt
+-rw-r--r--   0        0        0    12262 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM
+-rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/cmake/dragonboxConfig.cmake
+-rw-r--r--   0        0        0   144785 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h
+-rw-r--r--   0        0        0     4769 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h
+-rw-r--r--   0        0        0    25425 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp
+-rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/CMakeLists.txt
+-rw-r--r--   0        0        0    10767 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE
+-rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/LICENSE-MIT
+-rw-r--r--   0        0        0   115829 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h
+-rw-r--r--   0        0        0     1695 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/CMakeLists.txt
+-rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/LICENSE-Apache2
+-rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/LICENSE-Boost
+-rw-r--r--   0        0        0     3648 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/common.h
+-rw-r--r--   0        0        0    26321 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c
+-rw-r--r--   0        0        0   329074 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h
+-rw-r--r--   0        0        0    17721 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s.c
+-rw-r--r--   0        0        0    34501 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h
+-rw-r--r--   0        0        0    13015 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h
+-rw-r--r--   0        0        0     7434 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h
+-rw-r--r--   0        0        0     1745 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/digit_table.h
+-rw-r--r--   0        0        0    11279 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/f2s.c
+-rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h
+-rw-r--r--   0        0        0     4294 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h
+-rw-r--r--   0        0        0    11093 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/generic_128.c
+-rw-r--r--   0        0        0    34192 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/generic_128.h
+-rw-r--r--   0        0        0     1360 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/ryu.h
+-rw-r--r--   0        0        0     2721 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/ryu_generic_128.h
+-rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/ryu_parse.h
+-rw-r--r--   0        0        0     8362 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/s2d.c
+-rw-r--r--   0        0        0     8591 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/s2f.c
+-rw-r--r--   0        0        0     4008 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp
+-rw-r--r--   0        0        0    15527 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp
+-rw-r--r--   0        0        0     3193 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp
+-rw-r--r--   0        0        0     7193 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp
+-rw-r--r--   0        0        0    57595 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp
+-rw-r--r--   0        0        0     4553 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/array.hpp
+-rw-r--r--   0        0        0     4118 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp
+-rw-r--r--   0        0        0     4207 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp
+-rw-r--r--   0        0        0     3188 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/chunking.hpp
+-rw-r--r--   0        0        0     5251 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp
+-rw-r--r--   0        0        0    21182 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/field_conv.hpp
+-rw-r--r--   0        0        0    14746 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/formatters.hpp
+-rw-r--r--   0        0        0    10104 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/header.hpp
+-rw-r--r--   0        0        0     9312 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp
+-rw-r--r--   0        0        0    18575 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/read_body.hpp
+-rw-r--r--   0        0        0     5539 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp
+-rw-r--r--   0        0        0    15554 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/thirdparty/task_thread_pool.hpp
+-rw-r--r--   0        0        0     5018 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/types.hpp
+-rw-r--r--   0        0        0     2442 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/write_body.hpp
+-rw-r--r--   0        0        0     2549 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp
+-rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    15990 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/src/fast_matrix_market/__init__.py
+-rw-r--r--   0        0        0    23684 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/src/fast_matrix_market/core.cpp
+-rw-r--r--   0        0        0    19485 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/src/fast_matrix_market/pystreambuf.h
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/eye3.mtx
+-rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/long_double/longcomplex_array.mtx
+-rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/long_double/longcomplex_coordinate.mtx
+-rw-r--r--   0        0        0      113 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/long_double/longdouble_array.mtx
+-rw-r--r--   0        0        0      124 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/long_double/longdouble_coordinate.mtx
+-rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_array_complex_general.mtx
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_array_integer_general.mtx
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_array_real_general.mtx
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_complex_general.mtx
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_complex_hermitian.mtx
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_integer_general.mtx
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_pattern_general.mtx
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_pattern_symmetric.mtx
+-rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_real_general.mtx
+-rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_real_general.mtx.bz2
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_real_general.mtx.gz
+-rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_real_skew-symmetric.mtx
+-rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_real_symmetric.mtx
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/misc/windows_newlines.mtx
+-rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/scipy_crashes/dim_over_32_bit.mtx
+-rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/scipy_crashes/vector_array_real_general.mtx
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/scipy_crashes/vector_coordinate_real_general.mtx
+-rw-r--r--   0        0        0     1810 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/test_array.py
+-rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/test_basic.py
+-rw-r--r--   0        0        0     3235 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/test_coo.py
+-rw-r--r--   0        0        0     3518 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/test_header.py
+-rw-r--r--   0        0        0    13136 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/test_scipy.py
+-rw-r--r--   0        0        0      968 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/testsuite_scipy/test_scipy_suite.py
+-rw-r--r--   0        0        0     6405 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/PKG-INFO
```

### Comparing `fast-matrix-market-1.5.1/CMakeLists.txt` & `fast-matrix-market-1.6.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/LICENSE.txt` & `fast-matrix-market-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/README.md` & `fast-matrix-market-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/benchmark/bench_fmm.py` & `fast-matrix-market-1.6.0/benchmark/bench_fmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Copyright (C) 2022-2023 Adam Lugowski. All rights reserved.
 # Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+# SPDX-License-Identifier: BSD-2-Clause
+
 import math
 from io import BytesIO
 from pathlib import Path
 import tempfile
 
 import numpy as np
 import scipy.io
```

### Comparing `fast-matrix-market-1.5.1/benchmark/run.sh` & `fast-matrix-market-1.6.0/benchmark/run.sh`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/CMakeLists.txt` & `fast-matrix-market-1.6.0/fast_matrix_market/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/cmake/GraphBLAS.cmake` & `fast-matrix-market-1.6.0/fast_matrix_market/cmake/GraphBLAS.cmake`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/cmake/from_chars_tests.cmake` & `fast-matrix-market-1.6.0/fast_matrix_market/cmake/from_chars_tests.cmake`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/cmake/to_chars_tests.cmake` & `fast-matrix-market-1.6.0/fast_matrix_market/cmake/to_chars_tests.cmake`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/README.md` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/README.md`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/CMakeLists.txt` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/LICENSE-MIT` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 // fast_float by Daniel Lemire
 // fast_float by João Paulo Magalhaes
 //
+//
 // with contributions from Eugene Golushkov
 // with contributions from Maksim Kita
 // with contributions from Marcin Wojdyr
 // with contributions from Neal Richardson
 // with contributions from Tim Paine
 // with contributions from Fabio Pellacini
 // with contributions from Lénárd Szolnoki
+// with contributions from Jan Pharago//
 //
 // Licensed under the Apache License, Version 2.0, or the
-// MIT License at your option. This file may not be copied,
+// MIT License or the Boost License. This file may not be copied,
 // modified, or distributed except according to those terms.
 //
 // MIT License Notice
 //
 //    MIT License
 //    
 //    Copyright (c) 2021 The fast_float authors
@@ -53,14 +55,40 @@
 //    http://www.apache.org/licenses/LICENSE-2.0
 //    
 //    Unless required by applicable law or agreed to in writing, software
 //    distributed under the License is distributed on an "AS IS" BASIS,
 //    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //    See the License for the specific language governing permissions and
 //
+// BOOST License Notice
+//
+//    Boost Software License - Version 1.0 - August 17th, 2003
+//
+//    Permission is hereby granted, free of charge, to any person or organization
+//    obtaining a copy of the software and accompanying documentation covered by
+//    this license (the "Software") to use, reproduce, display, distribute,
+//    execute, and transmit the Software, and to prepare derivative works of the
+//    Software, and to permit third-parties to whom the Software is furnished to
+//    do so, all subject to the following:
+//
+//    The copyright notices in the Software and this entire statement, including
+//    the above license grant, this restriction and the following disclaimer,
+//    must be included in all copies of the Software, in whole or in part, and
+//    all derivative works of the Software, unless such copies or derivative
+//    works are solely in the form of machine-executable object code generated by
+//    a source language processor.
+//
+//    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+//    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+//    FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
+//    SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
+//    FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
+//    ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+//    DEALINGS IN THE SOFTWARE.
+//
 
 #ifndef FASTFLOAT_CONSTEXPR_FEATURE_DETECT_H
 #define FASTFLOAT_CONSTEXPR_FEATURE_DETECT_H
 
 #ifdef __has_include
 #if __has_include(<version>)
 #include <version>
@@ -70,21 +98,21 @@
 // Testing for https://wg21.link/N3652, adopted in C++14
 #if __cpp_constexpr >= 201304
 #define FASTFLOAT_CONSTEXPR14 constexpr
 #else
 #define FASTFLOAT_CONSTEXPR14
 #endif
 
-#if __cpp_lib_bit_cast >= 201806L
+#if defined(__cpp_lib_bit_cast) && __cpp_lib_bit_cast >= 201806L
 #define FASTFLOAT_HAS_BIT_CAST 1
 #else
 #define FASTFLOAT_HAS_BIT_CAST 0
 #endif
 
-#if __cpp_lib_is_constant_evaluated >= 201811L
+#if defined(__cpp_lib_is_constant_evaluated) && __cpp_lib_is_constant_evaluated >= 201811L
 #define FASTFLOAT_HAS_IS_CONSTANT_EVALUATED 1
 #else
 #define FASTFLOAT_HAS_IS_CONSTANT_EVALUATED 0
 #endif
 
 // Testing for relevant C++20 constexpr library features
 #if FASTFLOAT_HAS_IS_CONSTANT_EVALUATED \
@@ -95,88 +123,55 @@
 #else
 #define FASTFLOAT_CONSTEXPR20
 #define FASTFLOAT_IS_CONSTEXPR 0
 #endif
 
 #endif // FASTFLOAT_CONSTEXPR_FEATURE_DETECT_H
 
-#ifndef FASTFLOAT_FAST_FLOAT_H
-#define FASTFLOAT_FAST_FLOAT_H
+#ifndef FASTFLOAT_FLOAT_COMMON_H
+#define FASTFLOAT_FLOAT_COMMON_H
 
+#include <cfloat>
+#include <cstdint>
+#include <cassert>
+#include <cstring>
+#include <type_traits>
 #include <system_error>
 
 
 namespace fast_float {
+
 enum chars_format {
-    scientific = 1<<0,
-    fixed = 1<<2,
-    hex = 1<<3,
-    general = fixed | scientific
+  scientific = 1 << 0,
+  fixed = 1 << 2,
+  hex = 1 << 3,
+  general = fixed | scientific
 };
 
-
-struct from_chars_result {
-  const char *ptr;
+template <typename UC>
+struct from_chars_result_t {
+  UC const* ptr;
   std::errc ec;
 };
+using from_chars_result = from_chars_result_t<char>;
 
-struct parse_options {
-  constexpr explicit parse_options(chars_format fmt = chars_format::general,
-                         char dot = '.')
+template <typename UC>
+struct parse_options_t {
+  constexpr explicit parse_options_t(chars_format fmt = chars_format::general,
+    UC dot = UC('.'))
     : format(fmt), decimal_point(dot) {}
 
   /** Which number formats are accepted */
   chars_format format;
   /** The character used as decimal point */
-  char decimal_point;
+  UC decimal_point;
 };
+using parse_options = parse_options_t<char>;
 
-/**
- * This function parses the character sequence [first,last) for a number. It parses floating-point numbers expecting
- * a locale-indepent format equivalent to what is used by std::strtod in the default ("C") locale.
- * The resulting floating-point value is the closest floating-point values (using either float or double),
- * using the "round to even" convention for values that would otherwise fall right in-between two values.
- * That is, we provide exact parsing according to the IEEE standard.
- *
- * Given a successful parse, the pointer (`ptr`) in the returned value is set to point right after the
- * parsed number, and the `value` referenced is set to the parsed value. In case of error, the returned
- * `ec` contains a representative error, otherwise the default (`std::errc()`) value is stored.
- *
- * The implementation does not throw and does not allocate memory (e.g., with `new` or `malloc`).
- *
- * Like the C++17 standard, the `fast_float::from_chars` functions take an optional last argument of
- * the type `fast_float::chars_format`. It is a bitset value: we check whether
- * `fmt & fast_float::chars_format::fixed` and `fmt & fast_float::chars_format::scientific` are set
- * to determine whether we allow the fixed point and scientific notation respectively.
- * The default is  `fast_float::chars_format::general` which allows both `fixed` and `scientific`.
- */
-template<typename T>
-FASTFLOAT_CONSTEXPR20
-from_chars_result from_chars(const char *first, const char *last,
-                             T &value, chars_format fmt = chars_format::general)  noexcept;
-
-/**
- * Like from_chars, but accepts an `options` argument to govern number parsing.
- */
-template<typename T>
-FASTFLOAT_CONSTEXPR20
-from_chars_result from_chars_advanced(const char *first, const char *last,
-                                      T &value, parse_options options)  noexcept;
-
-} // namespace fast_float
-#endif // FASTFLOAT_FAST_FLOAT_H
-
-#ifndef FASTFLOAT_FLOAT_COMMON_H
-#define FASTFLOAT_FLOAT_COMMON_H
-
-#include <cfloat>
-#include <cstdint>
-#include <cassert>
-#include <cstring>
-#include <type_traits>
+}
 
 #if FASTFLOAT_HAS_BIT_CAST
 #include <bit>
 #endif
 
 #if (defined(__x86_64) || defined(__x86_64__) || defined(_M_X64)   \
        || defined(__amd64) || defined(__aarch64__) || defined(_M_ARM64) \
@@ -269,19 +264,20 @@
   return std::is_constant_evaluated();
 #else
   return false;
 #endif
 }
 
 // Compares two ASCII strings in a case insensitive manner.
+template <typename UC>
 inline FASTFLOAT_CONSTEXPR14 bool
-fastfloat_strncasecmp(const char *input1, const char *input2, size_t length) {
+fastfloat_strncasecmp(UC const * input1, UC const * input2, size_t length) {
   char running_diff{0};
-  for (size_t i = 0; i < length; i++) {
-    running_diff |= (input1[i] ^ input2[i]);
+  for (size_t i = 0; i < length; ++i) {
+    running_diff |= (char(input1[i]) ^ char(input2[i]));
   }
   return (running_diff == 0) || (running_diff == 32);
 }
 
 #ifndef FLT_EVAL_METHOD
 #error "FLT_EVAL_METHOD should be defined, please include cfloat."
 #endif
@@ -414,24 +410,51 @@
     return mantissa != o.mantissa || power2 != o.power2;
   }
 };
 
 // Bias so we can get the real exponent with an invalid adjusted_mantissa.
 constexpr static int32_t invalid_am_bias = -0x8000;
 
-constexpr static double powers_of_ten_double[] = {
-    1e0,  1e1,  1e2,  1e3,  1e4,  1e5,  1e6,  1e7,  1e8,  1e9,  1e10, 1e11,
-    1e12, 1e13, 1e14, 1e15, 1e16, 1e17, 1e18, 1e19, 1e20, 1e21, 1e22};
-constexpr static float powers_of_ten_float[] = {1e0f, 1e1f, 1e2f, 1e3f, 1e4f, 1e5f,
-                                                1e6f, 1e7f, 1e8f, 1e9f, 1e10f};
-// used for max_mantissa_double and max_mantissa_float
+// used for binary_format_lookup_tables<T>::max_mantissa
 constexpr uint64_t constant_55555 = 5 * 5 * 5 * 5 * 5;
-// Largest integer value v so that (5**index * v) <= 1<<53.
-// 0x10000000000000 == 1 << 53
-constexpr static uint64_t max_mantissa_double[] = {
+
+template <typename T, typename U = void>
+struct binary_format_lookup_tables;
+
+template <typename T> struct binary_format : binary_format_lookup_tables<T> {
+  using equiv_uint = typename std::conditional<sizeof(T) == 4, uint32_t, uint64_t>::type;
+
+  static inline constexpr int mantissa_explicit_bits();
+  static inline constexpr int minimum_exponent();
+  static inline constexpr int infinite_power();
+  static inline constexpr int sign_index();
+  static inline constexpr int min_exponent_fast_path(); // used when fegetround() == FE_TONEAREST
+  static inline constexpr int max_exponent_fast_path();
+  static inline constexpr int max_exponent_round_to_even();
+  static inline constexpr int min_exponent_round_to_even();
+  static inline constexpr uint64_t max_mantissa_fast_path(int64_t power);
+  static inline constexpr uint64_t max_mantissa_fast_path(); // used when fegetround() == FE_TONEAREST
+  static inline constexpr int largest_power_of_ten();
+  static inline constexpr int smallest_power_of_ten();
+  static inline constexpr T exact_power_of_ten(int64_t power);
+  static inline constexpr size_t max_digits();
+  static inline constexpr equiv_uint exponent_mask();
+  static inline constexpr equiv_uint mantissa_mask();
+  static inline constexpr equiv_uint hidden_bit_mask();
+};
+
+template <typename U>
+struct binary_format_lookup_tables<double, U> {
+  static constexpr double powers_of_ten[] = {
+      1e0,  1e1,  1e2,  1e3,  1e4,  1e5,  1e6,  1e7,  1e8,  1e9,  1e10, 1e11,
+      1e12, 1e13, 1e14, 1e15, 1e16, 1e17, 1e18, 1e19, 1e20, 1e21, 1e22};
+
+  // Largest integer value v so that (5**index * v) <= 1<<53.
+  // 0x10000000000000 == 1 << 53
+  static constexpr uint64_t max_mantissa[] = {
       0x10000000000000,
       0x10000000000000 / 5,
       0x10000000000000 / (5 * 5),
       0x10000000000000 / (5 * 5 * 5),
       0x10000000000000 / (5 * 5 * 5 * 5),
       0x10000000000000 / (constant_55555),
       0x10000000000000 / (constant_55555 * 5),
@@ -448,51 +471,49 @@
       0x10000000000000 / (constant_55555 * constant_55555 * constant_55555 * 5 * 5 * 5),
       0x10000000000000 / (constant_55555 * constant_55555 * constant_55555 * 5 * 5 * 5 * 5),
       0x10000000000000 / (constant_55555 * constant_55555 * constant_55555 * constant_55555),
       0x10000000000000 / (constant_55555 * constant_55555 * constant_55555 * constant_55555 * 5),
       0x10000000000000 / (constant_55555 * constant_55555 * constant_55555 * constant_55555 * 5 * 5),
       0x10000000000000 / (constant_55555 * constant_55555 * constant_55555 * constant_55555 * 5 * 5 * 5),
       0x10000000000000 / (constant_55555 * constant_55555 * constant_55555 * constant_55555 * 5 * 5 * 5 * 5)};
+};
+
+template <typename U>
+constexpr double binary_format_lookup_tables<double, U>::powers_of_ten[];
+
+template <typename U>
+constexpr uint64_t binary_format_lookup_tables<double, U>::max_mantissa[];
+
+template <typename U>
+struct binary_format_lookup_tables<float, U> {
+  static constexpr float powers_of_ten[] = {1e0f, 1e1f, 1e2f, 1e3f, 1e4f, 1e5f,
+                                     1e6f, 1e7f, 1e8f, 1e9f, 1e10f};
+
   // Largest integer value v so that (5**index * v) <= 1<<24.
   // 0x1000000 == 1<<24
-  constexpr static uint64_t max_mantissa_float[] = {
-      0x1000000,
-      0x1000000 / 5,
-      0x1000000 / (5 * 5),
-      0x1000000 / (5 * 5 * 5),
-      0x1000000 / (5 * 5 * 5 * 5),
-      0x1000000 / (constant_55555),
-      0x1000000 / (constant_55555 * 5),
-      0x1000000 / (constant_55555 * 5 * 5),
-      0x1000000 / (constant_55555 * 5 * 5 * 5),
-      0x1000000 / (constant_55555 * 5 * 5 * 5 * 5),
-      0x1000000 / (constant_55555 * constant_55555),
-      0x1000000 / (constant_55555 * constant_55555 * 5)};
+  static constexpr uint64_t max_mantissa[] = {
+        0x1000000,
+        0x1000000 / 5,
+        0x1000000 / (5 * 5),
+        0x1000000 / (5 * 5 * 5),
+        0x1000000 / (5 * 5 * 5 * 5),
+        0x1000000 / (constant_55555),
+        0x1000000 / (constant_55555 * 5),
+        0x1000000 / (constant_55555 * 5 * 5),
+        0x1000000 / (constant_55555 * 5 * 5 * 5),
+        0x1000000 / (constant_55555 * 5 * 5 * 5 * 5),
+        0x1000000 / (constant_55555 * constant_55555),
+        0x1000000 / (constant_55555 * constant_55555 * 5)};
+};
 
-template <typename T> struct binary_format {
-  using equiv_uint = typename std::conditional<sizeof(T) == 4, uint32_t, uint64_t>::type;
+template <typename U>
+constexpr float binary_format_lookup_tables<float, U>::powers_of_ten[];
 
-  static inline constexpr int mantissa_explicit_bits();
-  static inline constexpr int minimum_exponent();
-  static inline constexpr int infinite_power();
-  static inline constexpr int sign_index();
-  static inline constexpr int min_exponent_fast_path(); // used when fegetround() == FE_TONEAREST
-  static inline constexpr int max_exponent_fast_path();
-  static inline constexpr int max_exponent_round_to_even();
-  static inline constexpr int min_exponent_round_to_even();
-  static inline constexpr uint64_t max_mantissa_fast_path(int64_t power);
-  static inline constexpr uint64_t max_mantissa_fast_path(); // used when fegetround() == FE_TONEAREST
-  static inline constexpr int largest_power_of_ten();
-  static inline constexpr int smallest_power_of_ten();
-  static inline constexpr T exact_power_of_ten(int64_t power);
-  static inline constexpr size_t max_digits();
-  static inline constexpr equiv_uint exponent_mask();
-  static inline constexpr equiv_uint mantissa_mask();
-  static inline constexpr equiv_uint hidden_bit_mask();
-};
+template <typename U>
+constexpr uint64_t binary_format_lookup_tables<float, U>::max_mantissa[];
 
 template <> inline constexpr int binary_format<double>::min_exponent_fast_path() {
 #if (FLT_EVAL_METHOD != 1) && (FLT_EVAL_METHOD != 0)
   return 0;
 #else
   return -22;
 #endif
@@ -548,41 +569,45 @@
 
 template <> inline constexpr int binary_format<double>::max_exponent_fast_path() {
   return 22;
 }
 template <> inline constexpr int binary_format<float>::max_exponent_fast_path() {
   return 10;
 }
+
 template <> inline constexpr uint64_t binary_format<double>::max_mantissa_fast_path() {
   return uint64_t(2) << mantissa_explicit_bits();
 }
 template <> inline constexpr uint64_t binary_format<double>::max_mantissa_fast_path(int64_t power) {
   // caller is responsible to ensure that
   // power >= 0 && power <= 22
   //
-  return max_mantissa_double[power];
+  // Work around clang bug https://godbolt.org/z/zedh7rrhc
+  return (void)max_mantissa[0], max_mantissa[power];
 }
 template <> inline constexpr uint64_t binary_format<float>::max_mantissa_fast_path() {
   return uint64_t(2) << mantissa_explicit_bits();
 }
 template <> inline constexpr uint64_t binary_format<float>::max_mantissa_fast_path(int64_t power) {
   // caller is responsible to ensure that
   // power >= 0 && power <= 10
   //
-  return max_mantissa_float[power];
+  // Work around clang bug https://godbolt.org/z/zedh7rrhc
+  return (void)max_mantissa[0], max_mantissa[power];
 }
 
 template <>
 inline constexpr double binary_format<double>::exact_power_of_ten(int64_t power) {
-  return powers_of_ten_double[power];
+  // Work around clang bug https://godbolt.org/z/zedh7rrhc
+  return (void)powers_of_ten[0], powers_of_ten[power];
 }
 template <>
 inline constexpr float binary_format<float>::exact_power_of_ten(int64_t power) {
-
-  return powers_of_ten_float[power];
+  // Work around clang bug https://godbolt.org/z/zedh7rrhc
+  return (void)powers_of_ten[0], powers_of_ten[power];
 }
 
 
 template <>
 inline constexpr int binary_format<double>::largest_power_of_ten() {
   return 308;
 }
@@ -644,15 +669,15 @@
 #if FASTFLOAT_HAS_BIT_CAST
   value = std::bit_cast<T>(word);
 #else
   ::memcpy(&value, &word, sizeof(T));
 #endif
 }
 
-#if FASTFLOAT_SKIP_WHITE_SPACE // disabled by default
+#ifdef FASTFLOAT_SKIP_WHITE_SPACE // disabled by default
 template <typename = void>
 struct space_lut {
   static constexpr bool value[] = {
     0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
@@ -666,33 +691,137 @@
 };
 
 template <typename T>
 constexpr bool space_lut<T>::value[];
 
 inline constexpr bool is_space(uint8_t c) { return space_lut<>::value[c]; }
 #endif
+
+template<typename UC>
+static constexpr uint64_t int_cmp_zeros()
+{
+    static_assert((sizeof(UC) == 1) || (sizeof(UC) == 2) || (sizeof(UC) == 4), "Unsupported character size");
+    return (sizeof(UC) == 1) ? 0x3030303030303030 : (sizeof(UC) == 2) ? (uint64_t(UC('0')) << 48 | uint64_t(UC('0')) << 32 | uint64_t(UC('0')) << 16 | UC('0')) : (uint64_t(UC('0')) << 32 | UC('0'));
+}
+template<typename UC>
+static constexpr int int_cmp_len()
+{
+    return sizeof(uint64_t) / sizeof(UC);
+}
+template<typename UC>
+static constexpr UC const * str_const_nan()
+{
+    return nullptr;
+}
+template<>
+constexpr char const * str_const_nan<char>()
+{
+    return "nan";
+}
+template<>
+constexpr wchar_t const * str_const_nan<wchar_t>()
+{
+    return L"nan";
+}
+template<>
+constexpr char16_t const * str_const_nan<char16_t>()
+{
+    return u"nan";
+}
+template<>
+constexpr char32_t const * str_const_nan<char32_t>()
+{
+    return U"nan";
+}
+template<typename UC>
+static constexpr UC const * str_const_inf()
+{
+    return nullptr;
+}
+template<>
+constexpr char const * str_const_inf<char>()
+{
+    return "infinity";
+}
+template<>
+constexpr wchar_t const * str_const_inf<wchar_t>()
+{
+    return L"infinity";
+}
+template<>
+constexpr char16_t const * str_const_inf<char16_t>()
+{
+    return u"infinity";
+}
+template<>
+constexpr char32_t const * str_const_inf<char32_t>()
+{
+    return U"infinity";
+}
 } // namespace fast_float
 
 #endif
 
+
+#ifndef FASTFLOAT_FAST_FLOAT_H
+#define FASTFLOAT_FAST_FLOAT_H
+
+
+namespace fast_float {
+/**
+ * This function parses the character sequence [first,last) for a number. It parses floating-point numbers expecting
+ * a locale-indepent format equivalent to what is used by std::strtod in the default ("C") locale.
+ * The resulting floating-point value is the closest floating-point values (using either float or double),
+ * using the "round to even" convention for values that would otherwise fall right in-between two values.
+ * That is, we provide exact parsing according to the IEEE standard.
+ *
+ * Given a successful parse, the pointer (`ptr`) in the returned value is set to point right after the
+ * parsed number, and the `value` referenced is set to the parsed value. In case of error, the returned
+ * `ec` contains a representative error, otherwise the default (`std::errc()`) value is stored.
+ *
+ * The implementation does not throw and does not allocate memory (e.g., with `new` or `malloc`).
+ *
+ * Like the C++17 standard, the `fast_float::from_chars` functions take an optional last argument of
+ * the type `fast_float::chars_format`. It is a bitset value: we check whether
+ * `fmt & fast_float::chars_format::fixed` and `fmt & fast_float::chars_format::scientific` are set
+ * to determine whether we allow the fixed point and scientific notation respectively.
+ * The default is  `fast_float::chars_format::general` which allows both `fixed` and `scientific`.
+ */
+template<typename T, typename UC = char>
+FASTFLOAT_CONSTEXPR20
+from_chars_result_t<UC> from_chars(UC const * first, UC const * last,
+                             T &value, chars_format fmt = chars_format::general)  noexcept;
+
+/**
+ * Like from_chars, but accepts an `options` argument to govern number parsing.
+ */
+template<typename T, typename UC = char>
+FASTFLOAT_CONSTEXPR20
+from_chars_result_t<UC> from_chars_advanced(UC const * first, UC const * last,
+                                      T &value, parse_options_t<UC> options)  noexcept;
+
+} // namespace fast_float
+#endif // FASTFLOAT_FAST_FLOAT_H
+
 #ifndef FASTFLOAT_ASCII_NUMBER_H
 #define FASTFLOAT_ASCII_NUMBER_H
 
 #include <cctype>
 #include <cstdint>
 #include <cstring>
 #include <iterator>
 
 
 namespace fast_float {
 
 // Next function can be micro-optimized, but compilers are entirely
 // able to optimize it well.
-fastfloat_really_inline constexpr bool is_integer(char c) noexcept {
-  return c >= '0' && c <= '9';
+template <typename UC>
+fastfloat_really_inline constexpr bool is_integer(UC c) noexcept {
+  return !(c > UC('9') || c < UC('0'));
 }
 
 fastfloat_really_inline constexpr uint64_t byteswap(uint64_t val) {
   return (val & 0xFF00000000000000) >> 56
     | (val & 0x00FF000000000000) >> 40
     | (val & 0x0000FF0000000000) >> 24
     | (val & 0x000000FF00000000) >> 8
@@ -746,126 +875,149 @@
   const uint64_t mul2 = 0x0000271000000001; // 1 + (10000ULL << 32)
   val -= 0x3030303030303030;
   val = (val * 10) + (val >> 8); // val = (val * 2561) >> 8;
   val = (((val & mask) * mul1) + (((val >> 16) & mask) * mul2)) >> 32;
   return uint32_t(val);
 }
 
+fastfloat_really_inline constexpr
+uint32_t parse_eight_digits_unrolled(const char16_t *)  noexcept  {
+  return 0;
+}
+
+fastfloat_really_inline constexpr
+uint32_t parse_eight_digits_unrolled(const char32_t *)  noexcept  {
+  return 0;
+}
+
 fastfloat_really_inline FASTFLOAT_CONSTEXPR20
 uint32_t parse_eight_digits_unrolled(const char *chars)  noexcept  {
   return parse_eight_digits_unrolled(read_u64(chars));
 }
 
 // credit @aqrit
 fastfloat_really_inline constexpr bool is_made_of_eight_digits_fast(uint64_t val)  noexcept  {
   return !((((val + 0x4646464646464646) | (val - 0x3030303030303030)) &
      0x8080808080808080));
 }
 
+fastfloat_really_inline constexpr
+bool is_made_of_eight_digits_fast(const char16_t *)  noexcept  {
+  return false;
+}
+
+fastfloat_really_inline constexpr
+bool is_made_of_eight_digits_fast(const char32_t *)  noexcept  {
+  return false;
+}
+
 fastfloat_really_inline FASTFLOAT_CONSTEXPR20
 bool is_made_of_eight_digits_fast(const char *chars)  noexcept  {
   return is_made_of_eight_digits_fast(read_u64(chars));
 }
 
-typedef span<const char> byte_span;
-
-struct parsed_number_string {
+template <typename UC>
+struct parsed_number_string_t {
   int64_t exponent{0};
   uint64_t mantissa{0};
-  const char *lastmatch{nullptr};
+  UC const * lastmatch{nullptr};
   bool negative{false};
   bool valid{false};
   bool too_many_digits{false};
   // contains the range of the significant digits
-  byte_span integer{};  // non-nullable
-  byte_span fraction{}; // nullable
+  span<const UC> integer{};  // non-nullable
+  span<const UC> fraction{}; // nullable
 };
-
+using byte_span = span<char>;
+using parsed_number_string = parsed_number_string_t<char>;
 // Assuming that you use no more than 19 digits, this will
 // parse an ASCII string.
+template <typename UC>
 fastfloat_really_inline FASTFLOAT_CONSTEXPR20
-parsed_number_string parse_number_string(const char *p, const char *pend, parse_options options) noexcept {
-  const chars_format fmt = options.format;
-  const char decimal_point = options.decimal_point;
+parsed_number_string_t<UC> parse_number_string(UC const *p, UC const * pend, parse_options_t<UC> options) noexcept {
+  chars_format const fmt = options.format;
+  UC const decimal_point = options.decimal_point;
 
-  parsed_number_string answer;
+  parsed_number_string_t<UC> answer;
   answer.valid = false;
   answer.too_many_digits = false;
-  answer.negative = (*p == '-');
-#if FASTFLOAT_ALLOWS_LEADING_PLUS // disabled by default
-  if ((*p == '-') || (*p == '+')) {
+  answer.negative = (*p == UC('-'));
+#ifdef FASTFLOAT_ALLOWS_LEADING_PLUS // disabled by default
+  if ((*p == UC('-')) || (*p == UC('+'))) {
 #else
-  if (*p == '-') { // C++17 20.19.3.(7.1) explicitly forbids '+' sign here
+  if (*p == UC('-')) { // C++17 20.19.3.(7.1) explicitly forbids '+' sign here
 #endif
     ++p;
     if (p == pend) {
       return answer;
     }
     if (!is_integer(*p) && (*p != decimal_point)) { // a sign must be followed by an integer or the dot
       return answer;
     }
   }
-  const char *const start_digits = p;
+  UC const * const start_digits = p;
 
   uint64_t i = 0; // an unsigned int avoids signed overflows (which are bad)
 
   while ((p != pend) && is_integer(*p)) {
     // a multiplication by 10 is cheaper than an arbitrary integer
     // multiplication
     i = 10 * i +
-        uint64_t(*p - '0'); // might overflow, we will handle the overflow later
+        uint64_t(*p - UC('0')); // might overflow, we will handle the overflow later
     ++p;
   }
-  const char *const end_of_integer_part = p;
+  UC const * const end_of_integer_part = p;
   int64_t digit_count = int64_t(end_of_integer_part - start_digits);
-  answer.integer = byte_span(start_digits, size_t(digit_count));
+  answer.integer = span<const UC>(start_digits, size_t(digit_count));
   int64_t exponent = 0;
   if ((p != pend) && (*p == decimal_point)) {
     ++p;
-    const char* before = p;
+    UC const * before = p;
     // can occur at most twice without overflowing, but let it occur more, since
     // for integers with many digits, digit parsing is the primary bottleneck.
-    while ((std::distance(p, pend) >= 8) && is_made_of_eight_digits_fast(p)) {
-      i = i * 100000000 + parse_eight_digits_unrolled(p); // in rare cases, this will overflow, but that's ok
-      p += 8;
+    if (std::is_same<UC,char>::value) {
+      while ((std::distance(p, pend) >= 8) && is_made_of_eight_digits_fast(p)) {
+        i = i * 100000000 + parse_eight_digits_unrolled(p); // in rare cases, this will overflow, but that's ok
+        p += 8;
+      }
     }
     while ((p != pend) && is_integer(*p)) {
-      uint8_t digit = uint8_t(*p - '0');
+      uint8_t digit = uint8_t(*p - UC('0'));
       ++p;
       i = i * 10 + digit; // in rare cases, this will overflow, but that's ok
     }
     exponent = before - p;
-    answer.fraction = byte_span(before, size_t(p - before));
+    answer.fraction = span<const UC>(before, size_t(p - before));
     digit_count -= exponent;
   }
   // we must have encountered at least one integer!
   if (digit_count == 0) {
     return answer;
   }
   int64_t exp_number = 0;            // explicit exponential part
-  if ((fmt & chars_format::scientific) && (p != pend) && (('e' == *p) || ('E' == *p))) {
-    const char * location_of_e = p;
+  if ((fmt & chars_format::scientific) && (p != pend) && ((UC('e') == *p) || (UC('E') == *p))) {
+    UC const * location_of_e = p;
     ++p;
     bool neg_exp = false;
-    if ((p != pend) && ('-' == *p)) {
+    if ((p != pend) && (UC('-') == *p)) {
       neg_exp = true;
       ++p;
-    } else if ((p != pend) && ('+' == *p)) { // '+' on exponent is allowed by C++17 20.19.3.(7.1)
+    } else if ((p != pend) && (UC('+') == *p)) { // '+' on exponent is allowed by C++17 20.19.3.(7.1)
       ++p;
     }
     if ((p == pend) || !is_integer(*p)) {
       if(!(fmt & chars_format::fixed)) {
         // We are in error.
         return answer;
       }
       // Otherwise, we will be ignoring the 'e'.
       p = location_of_e;
     } else {
       while ((p != pend) && is_integer(*p)) {
-        uint8_t digit = uint8_t(*p - '0');
+        uint8_t digit = uint8_t(*p - UC('0'));
         if (exp_number < 0x10000000) {
           exp_number = 10 * exp_number + digit;
         }
         ++p;
       }
       if(neg_exp) { exp_number = - exp_number; }
       exponent += exp_number;
@@ -883,39 +1035,39 @@
   //
   // We can deal with up to 19 digits.
   if (digit_count > 19) { // this is uncommon
     // It is possible that the integer had an overflow.
     // We have to handle the case where we have 0.0000somenumber.
     // We need to be mindful of the case where we only have zeroes...
     // E.g., 0.000000000...000.
-    const char *start = start_digits;
-    while ((start != pend) && (*start == '0' || *start == decimal_point)) {
-      if(*start == '0') { digit_count --; }
+    UC const * start = start_digits;
+    while ((start != pend) && (*start == UC('0') || *start == decimal_point)) {
+      if(*start == UC('0')) { digit_count --; }
       start++;
     }
     if (digit_count > 19) {
       answer.too_many_digits = true;
       // Let us start again, this time, avoiding overflows.
       // We don't need to check if is_integer, since we use the
       // pre-tokenized spans from above.
       i = 0;
       p = answer.integer.ptr;
-      const char* int_end = p + answer.integer.len();
+      UC const * int_end = p + answer.integer.len();
       const uint64_t minimal_nineteen_digit_integer{1000000000000000000};
       while((i < minimal_nineteen_digit_integer) && (p != int_end)) {
-        i = i * 10 + uint64_t(*p - '0');
+        i = i * 10 + uint64_t(*p - UC('0'));
         ++p;
       }
       if (i >= minimal_nineteen_digit_integer) { // We have a big integers
         exponent = end_of_integer_part - p + exp_number;
       } else { // We have a value with a fractional component.
           p = answer.fraction.ptr;
-          const char* frac_end = p + answer.fraction.len();
+          UC const * frac_end = p + answer.fraction.len();
           while((i < minimal_nineteen_digit_integer) && (p != frac_end)) {
-            i = i * 10 + uint64_t(*p - '0');
+            i = i * 10 + uint64_t(*p - UC('0'));
             ++p;
           }
           exponent = answer.fraction.ptr - p + exp_number;
       }
       // We have now corrected both exponent and i, to a truncated value
     }
   }
@@ -1673,17 +1825,17 @@
  * For q in (0,350), we have that
  *  f = (((152170 + 65536) * q ) >> 16);
  * is equal to
  *   floor(p) + q
  * where
  *   p = log(5**q)/log(2) = q * log(5)/log(2)
  *
- * For negative values of q in (-400,0), we have that 
+ * For negative values of q in (-400,0), we have that
  *  f = (((152170 + 65536) * q ) >> 16);
- * is equal to 
+ * is equal to
  *   -ceil(p) + q
  * where
  *   p = log(5**-q)/log(2) = -q * log(5)/log(2)
  */
   constexpr fastfloat_really_inline int32_t power(int32_t q)  noexcept  {
     return (((152170 + 65536) * q) >> 16) + 63;
   }
@@ -2430,268 +2582,14 @@
   }
 };
 
 } // namespace fast_float
 
 #endif
 
-#ifndef FASTFLOAT_ASCII_NUMBER_H
-#define FASTFLOAT_ASCII_NUMBER_H
-
-#include <cctype>
-#include <cstdint>
-#include <cstring>
-#include <iterator>
-
-
-namespace fast_float {
-
-// Next function can be micro-optimized, but compilers are entirely
-// able to optimize it well.
-fastfloat_really_inline constexpr bool is_integer(char c) noexcept {
-  return c >= '0' && c <= '9';
-}
-
-fastfloat_really_inline constexpr uint64_t byteswap(uint64_t val) {
-  return (val & 0xFF00000000000000) >> 56
-    | (val & 0x00FF000000000000) >> 40
-    | (val & 0x0000FF0000000000) >> 24
-    | (val & 0x000000FF00000000) >> 8
-    | (val & 0x00000000FF000000) << 8
-    | (val & 0x0000000000FF0000) << 24
-    | (val & 0x000000000000FF00) << 40
-    | (val & 0x00000000000000FF) << 56;
-}
-
-fastfloat_really_inline FASTFLOAT_CONSTEXPR20
-uint64_t read_u64(const char *chars) {
-  if (cpp20_and_in_constexpr()) {
-    uint64_t val = 0;
-    for(int i = 0; i < 8; ++i) {
-      val |= uint64_t(*chars) << (i*8);
-      ++chars;
-    }
-    return val;
-  }
-  uint64_t val;
-  ::memcpy(&val, chars, sizeof(uint64_t));
-#if FASTFLOAT_IS_BIG_ENDIAN == 1
-  // Need to read as-if the number was in little-endian order.
-  val = byteswap(val);
-#endif
-  return val;
-}
-
-fastfloat_really_inline FASTFLOAT_CONSTEXPR20
-void write_u64(uint8_t *chars, uint64_t val) {
-  if (cpp20_and_in_constexpr()) {
-    for(int i = 0; i < 8; ++i) {
-      *chars = uint8_t(val);
-      val >>= 8;
-      ++chars;
-    }
-    return;
-  }
-#if FASTFLOAT_IS_BIG_ENDIAN == 1
-  // Need to read as-if the number was in little-endian order.
-  val = byteswap(val);
-#endif
-  ::memcpy(chars, &val, sizeof(uint64_t));
-}
-
-// credit  @aqrit
-fastfloat_really_inline FASTFLOAT_CONSTEXPR14
-uint32_t parse_eight_digits_unrolled(uint64_t val) {
-  const uint64_t mask = 0x000000FF000000FF;
-  const uint64_t mul1 = 0x000F424000000064; // 100 + (1000000ULL << 32)
-  const uint64_t mul2 = 0x0000271000000001; // 1 + (10000ULL << 32)
-  val -= 0x3030303030303030;
-  val = (val * 10) + (val >> 8); // val = (val * 2561) >> 8;
-  val = (((val & mask) * mul1) + (((val >> 16) & mask) * mul2)) >> 32;
-  return uint32_t(val);
-}
-
-fastfloat_really_inline FASTFLOAT_CONSTEXPR20
-uint32_t parse_eight_digits_unrolled(const char *chars)  noexcept  {
-  return parse_eight_digits_unrolled(read_u64(chars));
-}
-
-// credit @aqrit
-fastfloat_really_inline constexpr bool is_made_of_eight_digits_fast(uint64_t val)  noexcept  {
-  return !((((val + 0x4646464646464646) | (val - 0x3030303030303030)) &
-     0x8080808080808080));
-}
-
-fastfloat_really_inline FASTFLOAT_CONSTEXPR20
-bool is_made_of_eight_digits_fast(const char *chars)  noexcept  {
-  return is_made_of_eight_digits_fast(read_u64(chars));
-}
-
-typedef span<const char> byte_span;
-
-struct parsed_number_string {
-  int64_t exponent{0};
-  uint64_t mantissa{0};
-  const char *lastmatch{nullptr};
-  bool negative{false};
-  bool valid{false};
-  bool too_many_digits{false};
-  // contains the range of the significant digits
-  byte_span integer{};  // non-nullable
-  byte_span fraction{}; // nullable
-};
-
-// Assuming that you use no more than 19 digits, this will
-// parse an ASCII string.
-fastfloat_really_inline FASTFLOAT_CONSTEXPR20
-parsed_number_string parse_number_string(const char *p, const char *pend, parse_options options) noexcept {
-  const chars_format fmt = options.format;
-  const char decimal_point = options.decimal_point;
-
-  parsed_number_string answer;
-  answer.valid = false;
-  answer.too_many_digits = false;
-  answer.negative = (*p == '-');
-#if FASTFLOAT_ALLOWS_LEADING_PLUS // disabled by default
-  if ((*p == '-') || (*p == '+')) {
-#else
-  if (*p == '-') { // C++17 20.19.3.(7.1) explicitly forbids '+' sign here
-#endif
-    ++p;
-    if (p == pend) {
-      return answer;
-    }
-    if (!is_integer(*p) && (*p != decimal_point)) { // a sign must be followed by an integer or the dot
-      return answer;
-    }
-  }
-  const char *const start_digits = p;
-
-  uint64_t i = 0; // an unsigned int avoids signed overflows (which are bad)
-
-  while ((p != pend) && is_integer(*p)) {
-    // a multiplication by 10 is cheaper than an arbitrary integer
-    // multiplication
-    i = 10 * i +
-        uint64_t(*p - '0'); // might overflow, we will handle the overflow later
-    ++p;
-  }
-  const char *const end_of_integer_part = p;
-  int64_t digit_count = int64_t(end_of_integer_part - start_digits);
-  answer.integer = byte_span(start_digits, size_t(digit_count));
-  int64_t exponent = 0;
-  if ((p != pend) && (*p == decimal_point)) {
-    ++p;
-    const char* before = p;
-    // can occur at most twice without overflowing, but let it occur more, since
-    // for integers with many digits, digit parsing is the primary bottleneck.
-    while ((std::distance(p, pend) >= 8) && is_made_of_eight_digits_fast(p)) {
-      i = i * 100000000 + parse_eight_digits_unrolled(p); // in rare cases, this will overflow, but that's ok
-      p += 8;
-    }
-    while ((p != pend) && is_integer(*p)) {
-      uint8_t digit = uint8_t(*p - '0');
-      ++p;
-      i = i * 10 + digit; // in rare cases, this will overflow, but that's ok
-    }
-    exponent = before - p;
-    answer.fraction = byte_span(before, size_t(p - before));
-    digit_count -= exponent;
-  }
-  // we must have encountered at least one integer!
-  if (digit_count == 0) {
-    return answer;
-  }
-  int64_t exp_number = 0;            // explicit exponential part
-  if ((fmt & chars_format::scientific) && (p != pend) && (('e' == *p) || ('E' == *p))) {
-    const char * location_of_e = p;
-    ++p;
-    bool neg_exp = false;
-    if ((p != pend) && ('-' == *p)) {
-      neg_exp = true;
-      ++p;
-    } else if ((p != pend) && ('+' == *p)) { // '+' on exponent is allowed by C++17 20.19.3.(7.1)
-      ++p;
-    }
-    if ((p == pend) || !is_integer(*p)) {
-      if(!(fmt & chars_format::fixed)) {
-        // We are in error.
-        return answer;
-      }
-      // Otherwise, we will be ignoring the 'e'.
-      p = location_of_e;
-    } else {
-      while ((p != pend) && is_integer(*p)) {
-        uint8_t digit = uint8_t(*p - '0');
-        if (exp_number < 0x10000000) {
-          exp_number = 10 * exp_number + digit;
-        }
-        ++p;
-      }
-      if(neg_exp) { exp_number = - exp_number; }
-      exponent += exp_number;
-    }
-  } else {
-    // If it scientific and not fixed, we have to bail out.
-    if((fmt & chars_format::scientific) && !(fmt & chars_format::fixed)) { return answer; }
-  }
-  answer.lastmatch = p;
-  answer.valid = true;
-
-  // If we frequently had to deal with long strings of digits,
-  // we could extend our code by using a 128-bit integer instead
-  // of a 64-bit integer. However, this is uncommon.
-  //
-  // We can deal with up to 19 digits.
-  if (digit_count > 19) { // this is uncommon
-    // It is possible that the integer had an overflow.
-    // We have to handle the case where we have 0.0000somenumber.
-    // We need to be mindful of the case where we only have zeroes...
-    // E.g., 0.000000000...000.
-    const char *start = start_digits;
-    while ((start != pend) && (*start == '0' || *start == decimal_point)) {
-      if(*start == '0') { digit_count --; }
-      start++;
-    }
-    if (digit_count > 19) {
-      answer.too_many_digits = true;
-      // Let us start again, this time, avoiding overflows.
-      // We don't need to check if is_integer, since we use the
-      // pre-tokenized spans from above.
-      i = 0;
-      p = answer.integer.ptr;
-      const char* int_end = p + answer.integer.len();
-      const uint64_t minimal_nineteen_digit_integer{1000000000000000000};
-      while((i < minimal_nineteen_digit_integer) && (p != int_end)) {
-        i = i * 10 + uint64_t(*p - '0');
-        ++p;
-      }
-      if (i >= minimal_nineteen_digit_integer) { // We have a big integers
-        exponent = end_of_integer_part - p + exp_number;
-      } else { // We have a value with a fractional component.
-          p = answer.fraction.ptr;
-          const char* frac_end = p + answer.fraction.len();
-          while((i < minimal_nineteen_digit_integer) && (p != frac_end)) {
-            i = i * 10 + uint64_t(*p - '0');
-            ++p;
-          }
-          exponent = answer.fraction.ptr - p + exp_number;
-      }
-      // We have now corrected both exponent and i, to a truncated value
-    }
-  }
-  answer.exponent = exponent;
-  answer.mantissa = i;
-  return answer;
-}
-
-} // namespace fast_float
-
-#endif
-
 #ifndef FASTFLOAT_DIGIT_COMPARISON_H
 #define FASTFLOAT_DIGIT_COMPARISON_H
 
 #include <algorithm>
 #include <cstdint>
 #include <cstring>
 #include <iterator>
@@ -2706,16 +2604,17 @@
     100000000000000UL, 1000000000000000UL, 10000000000000000UL, 100000000000000000UL,
     1000000000000000000UL, 10000000000000000000UL};
 
 // calculate the exponent, in scientific notation, of the number.
 // this algorithm is not even close to optimized, but it has no practical
 // effect on performance: in order to have a faster algorithm, we'd need
 // to slow down performance for faster algorithms, and this is still fast.
+template <typename UC>
 fastfloat_really_inline FASTFLOAT_CONSTEXPR14
-int32_t scientific_exponent(parsed_number_string& num) noexcept {
+int32_t scientific_exponent(parsed_number_string_t<UC> & num) noexcept {
   uint64_t mantissa = num.mantissa;
   int32_t exponent = int32_t(num.exponent);
   while (mantissa >= 10000) {
     mantissa /= 10000;
     exponent += 4;
   }
   while (mantissa >= 100) {
@@ -2836,71 +2735,83 @@
   if (shift == 64) {
     am.mantissa = 0;
   } else {
     am.mantissa >>= shift;
   }
   am.power2 += shift;
 }
-
+template <typename UC>
 fastfloat_really_inline FASTFLOAT_CONSTEXPR20
-void skip_zeros(const char*& first, const char* last) noexcept {
+void skip_zeros(UC const * & first, UC const * last) noexcept {
   uint64_t val;
-  while (!cpp20_and_in_constexpr() && std::distance(first, last) >= 8) {
+  while (!cpp20_and_in_constexpr() && std::distance(first, last) >= int_cmp_len<UC>()) {
     ::memcpy(&val, first, sizeof(uint64_t));
-    if (val != 0x3030303030303030) {
+    if (val != int_cmp_zeros<UC>()) {
       break;
     }
-    first += 8;
+    first += int_cmp_len<UC>();
   }
   while (first != last) {
-    if (*first != '0') {
+    if (*first != UC('0')) {
       break;
     }
     first++;
   }
 }
 
 // determine if any non-zero digits were truncated.
 // all characters must be valid digits.
+template <typename UC>
 fastfloat_really_inline FASTFLOAT_CONSTEXPR20
-bool is_truncated(const char* first, const char* last) noexcept {
+bool is_truncated(UC const * first, UC const * last) noexcept {
   // do 8-bit optimizations, can just compare to 8 literal 0s.
   uint64_t val;
-  while (!cpp20_and_in_constexpr() && std::distance(first, last) >= 8) {
+  while (!cpp20_and_in_constexpr() && std::distance(first, last) >= int_cmp_len<UC>()) {
     ::memcpy(&val, first, sizeof(uint64_t));
-    if (val != 0x3030303030303030) {
+    if (val != int_cmp_zeros<UC>()) {
       return true;
     }
-    first += 8;
+    first += int_cmp_len<UC>();
   }
   while (first != last) {
-    if (*first != '0') {
+    if (*first != UC('0')) {
       return true;
     }
-    first++;
+    ++first;
   }
   return false;
 }
-
+template <typename UC>
 fastfloat_really_inline FASTFLOAT_CONSTEXPR20
-bool is_truncated(byte_span s) noexcept {
+bool is_truncated(span<const UC> s) noexcept {
   return is_truncated(s.ptr, s.ptr + s.len());
 }
 
 fastfloat_really_inline FASTFLOAT_CONSTEXPR20
+void parse_eight_digits(const char16_t*& , limb& , size_t& , size_t& ) noexcept {
+  // currently unused
+}
+
+fastfloat_really_inline FASTFLOAT_CONSTEXPR20
+void parse_eight_digits(const char32_t*& , limb& , size_t& , size_t& ) noexcept {
+  // currently unused
+}
+
+fastfloat_really_inline FASTFLOAT_CONSTEXPR20
 void parse_eight_digits(const char*& p, limb& value, size_t& counter, size_t& count) noexcept {
   value = value * 100000000 + parse_eight_digits_unrolled(p);
   p += 8;
   counter += 8;
   count += 8;
 }
 
+template <typename UC>
 fastfloat_really_inline FASTFLOAT_CONSTEXPR14
-void parse_one_digit(const char*& p, limb& value, size_t& counter, size_t& count) noexcept {
-  value = value * 10 + limb(*p - '0');
+void parse_one_digit(UC const *& p, limb& value, size_t& counter, size_t& count) noexcept {
+  value = value * 10 + limb(*p - UC('0'));
   p++;
   counter++;
   count++;
 }
 
 fastfloat_really_inline FASTFLOAT_CONSTEXPR20
 void add_native(bigint& big, limb power, limb value) noexcept {
@@ -2913,36 +2824,39 @@
   // need to round-up the digits, but need to avoid rounding
   // ....9999 to ...10000, which could cause a false halfway point.
   add_native(big, 10, 1);
   count++;
 }
 
 // parse the significant digits into a big integer
+template <typename UC>
 inline FASTFLOAT_CONSTEXPR20
-void parse_mantissa(bigint& result, parsed_number_string& num, size_t max_digits, size_t& digits) noexcept {
+void parse_mantissa(bigint& result, parsed_number_string_t<UC>& num, size_t max_digits, size_t& digits) noexcept {
   // try to minimize the number of big integer and scalar multiplication.
   // therefore, try to parse 8 digits at a time, and multiply by the largest
   // scalar value (9 or 19 digits) for each step.
   size_t counter = 0;
   digits = 0;
   limb value = 0;
 #ifdef FASTFLOAT_64BIT_LIMB
   size_t step = 19;
 #else
   size_t step = 9;
 #endif
 
   // process all integer digits.
-  const char* p = num.integer.ptr;
-  const char* pend = p + num.integer.len();
+  UC const * p = num.integer.ptr;
+  UC const * pend = p + num.integer.len();
   skip_zeros(p, pend);
   // process all digits, in increments of step per loop
   while (p != pend) {
-    while ((std::distance(p, pend) >= 8) && (step - counter >= 8) && (max_digits - digits >= 8)) {
-      parse_eight_digits(p, value, counter, digits);
+    if (std::is_same<UC,char>::value) {
+      while ((std::distance(p, pend) >= 8) && (step - counter >= 8) && (max_digits - digits >= 8)) {
+        parse_eight_digits(p, value, counter, digits);
+      }
     }
     while (counter < step && p != pend && digits < max_digits) {
       parse_one_digit(p, value, counter, digits);
     }
     if (digits == max_digits) {
       // add the temporary value, then check if we've truncated any digits
       add_native(result, limb(powers_of_ten_uint64[counter]), value);
@@ -2966,16 +2880,18 @@
     p = num.fraction.ptr;
     pend = p + num.fraction.len();
     if (digits == 0) {
       skip_zeros(p, pend);
     }
     // process all digits, in increments of step per loop
     while (p != pend) {
-      while ((std::distance(p, pend) >= 8) && (step - counter >= 8) && (max_digits - digits >= 8)) {
-        parse_eight_digits(p, value, counter, digits);
+      if (std::is_same<UC,char>::value) {
+        while ((std::distance(p, pend) >= 8) && (step - counter >= 8) && (max_digits - digits >= 8)) {
+          parse_eight_digits(p, value, counter, digits);
+        }
       }
       while (counter < step && p != pend && digits < max_digits) {
         parse_one_digit(p, value, counter, digits);
       }
       if (digits == max_digits) {
         // add the temporary value, then check if we've truncated any digits
         add_native(result, limb(powers_of_ten_uint64[counter]), value);
@@ -3078,17 +2994,17 @@
 // 1234), we create a big-integer representation, get the high 64-bits,
 // determine if any lower bits are truncated, and use that to direct
 // rounding. in case of a negative exponent relative to the significant
 // digits (such as 1.2345), we create a theoretical representation of
 // `b` as a big-integer type, scaled to the same binary exponent as
 // the actual digits. we then compare the big integer representations
 // of both, and use that to direct rounding.
-template <typename T>
+template <typename T, typename UC>
 inline FASTFLOAT_CONSTEXPR20
-adjusted_mantissa digit_comp(parsed_number_string& num, adjusted_mantissa am) noexcept {
+adjusted_mantissa digit_comp(parsed_number_string_t<UC>& num, adjusted_mantissa am) noexcept {
   // remove the invalid exponent bias
   am.power2 -= invalid_am_bias;
 
   int32_t sci_exp = scientific_exponent(num);
   size_t max_digits = binary_format<T>::max_digits();
   size_t digits = 0;
   bigint bigmant;
@@ -3120,49 +3036,49 @@
 
 namespace detail {
 /**
  * Special case +inf, -inf, nan, infinity, -infinity.
  * The case comparisons could be made much faster given that we know that the
  * strings a null-free and fixed.
  **/
-template <typename T>
-from_chars_result FASTFLOAT_CONSTEXPR14
-parse_infnan(const char *first, const char *last, T &value)  noexcept  {
-  from_chars_result answer{};
+template <typename T, typename UC>
+from_chars_result_t<UC> FASTFLOAT_CONSTEXPR14
+parse_infnan(UC const * first, UC const * last, T &value)  noexcept  {
+  from_chars_result_t<UC> answer{};
   answer.ptr = first;
   answer.ec = std::errc(); // be optimistic
   bool minusSign = false;
-  if (*first == '-') { // assume first < last, so dereference without checks; C++17 20.19.3.(7.1) explicitly forbids '+' here
+  if (*first == UC('-')) { // assume first < last, so dereference without checks; C++17 20.19.3.(7.1) explicitly forbids '+' here
       minusSign = true;
       ++first;
   }
-#if FASTFLOAT_ALLOWS_LEADING_PLUS // disabled by default
-  if (*first == '+') {
+#ifdef FASTFLOAT_ALLOWS_LEADING_PLUS // disabled by default
+  if (*first == UC('+')) {
       ++first;
   }
 #endif
   if (last - first >= 3) {
-    if (fastfloat_strncasecmp(first, "nan", 3)) {
+    if (fastfloat_strncasecmp(first, str_const_nan<UC>(), 3)) {
       answer.ptr = (first += 3);
       value = minusSign ? -std::numeric_limits<T>::quiet_NaN() : std::numeric_limits<T>::quiet_NaN();
       // Check for possible nan(n-char-seq-opt), C++17 20.19.3.7, C11 7.20.1.3.3. At least MSVC produces nan(ind) and nan(snan).
-      if(first != last && *first == '(') {
-        for(const char* ptr = first + 1; ptr != last; ++ptr) {
-          if (*ptr == ')') {
+      if(first != last && *first == UC('(')) {
+        for(UC const * ptr = first + 1; ptr != last; ++ptr) {
+          if (*ptr == UC(')')) {
             answer.ptr = ptr + 1; // valid nan(n-char-seq-opt)
             break;
           }
-          else if(!(('a' <= *ptr && *ptr <= 'z') || ('A' <= *ptr && *ptr <= 'Z') || ('0' <= *ptr && *ptr <= '9') || *ptr == '_'))
+          else if(!((UC('a') <= *ptr && *ptr <= UC('z')) || (UC('A') <= *ptr && *ptr <= UC('Z')) || (UC('0') <= *ptr && *ptr <= UC('9')) || *ptr == UC('_')))
             break; // forbidden char, not nan(n-char-seq-opt)
         }
       }
       return answer;
     }
-    if (fastfloat_strncasecmp(first, "inf", 3)) {
-      if ((last - first >= 8) && fastfloat_strncasecmp(first + 3, "inity", 5)) {
+    if (fastfloat_strncasecmp(first, str_const_inf<UC>(), 3)) {
+      if ((last - first >= 8) && fastfloat_strncasecmp(first + 3, str_const_inf<UC>() + 3, 5)) {
         answer.ptr = first + 8;
       } else {
         answer.ptr = first + 3;
       }
       value = minusSign ? -std::numeric_limits<T>::infinity() : std::numeric_limits<T>::infinity();
       return answer;
     }
@@ -3210,64 +3126,67 @@
   //
   // FE_DOWNWARD or  FE_TOWARDZERO:
   //  fmin + 1.0f == 1
   //  1.0f - fmin < 1
   //
   // Note: This may fail to be accurate if fast-math has been
   // enabled, as rounding conventions may not apply.
-  #if FASTFLOAT_VISUAL_STUDIO
+  #ifdef FASTFLOAT_VISUAL_STUDIO
   #   pragma warning(push)
   //  todo: is there a VS warning?
   //  see https://stackoverflow.com/questions/46079446/is-there-a-warning-for-floating-point-equality-checking-in-visual-studio-2013
   #elif defined(__clang__)
   #   pragma clang diagnostic push
   #   pragma clang diagnostic ignored "-Wfloat-equal"
   #elif defined(__GNUC__)
   #   pragma GCC diagnostic push
   #   pragma GCC diagnostic ignored "-Wfloat-equal"
   #endif
   return (fmini + 1.0f == 1.0f - fmini);
-  #if FASTFLOAT_VISUAL_STUDIO
+  #ifdef FASTFLOAT_VISUAL_STUDIO
   #   pragma warning(pop)
   #elif defined(__clang__)
   #   pragma clang diagnostic pop
   #elif defined(__GNUC__)
   #   pragma GCC diagnostic pop
   #endif
 }
 
 } // namespace detail
 
-template<typename T>
+template<typename T, typename UC>
 FASTFLOAT_CONSTEXPR20
-from_chars_result from_chars(const char *first, const char *last,
+from_chars_result_t<UC> from_chars(UC const * first, UC const * last,
                              T &value, chars_format fmt /*= chars_format::general*/)  noexcept  {
-  return from_chars_advanced(first, last, value, parse_options{fmt});
+  return from_chars_advanced(first, last, value, parse_options_t<UC>{fmt});
 }
 
-template<typename T>
+template<typename T, typename UC>
 FASTFLOAT_CONSTEXPR20
-from_chars_result from_chars_advanced(const char *first, const char *last,
-                                      T &value, parse_options options)  noexcept  {
+from_chars_result_t<UC> from_chars_advanced(UC const * first, UC const * last,
+                                      T &value, parse_options_t<UC> options)  noexcept  {
 
   static_assert (std::is_same<T, double>::value || std::is_same<T, float>::value, "only float and double are supported");
+  static_assert (std::is_same<UC, char>::value ||
+                 std::is_same<UC, wchar_t>::value ||
+                 std::is_same<UC, char16_t>::value ||
+                 std::is_same<UC, char32_t>::value , "only char, wchar_t, char16_t and char32_t are supported");
 
-
-  from_chars_result answer;
-#if FASTFLOAT_SKIP_WHITE_SPACE  // disabled by default
+  from_chars_result_t<UC> answer;
+#ifdef FASTFLOAT_SKIP_WHITE_SPACE  // disabled by default
   while ((first != last) && fast_float::is_space(uint8_t(*first))) {
     first++;
   }
 #endif
   if (first == last) {
     answer.ec = std::errc::invalid_argument;
     answer.ptr = first;
     return answer;
   }
-  parsed_number_string pns = parse_number_string(first, last, options);
+  parsed_number_string_t<UC> pns = parse_number_string<UC>(first, last, options);
   if (!pns.valid) {
     return detail::parse_infnan(first, last, value);
   }
   answer.ec = std::errc(); // be optimistic
   answer.ptr = pns.lastmatch;
   // The implementation of the Clinger's fast path is convoluted because
   // we want round-to-nearest in all cases, irrespective of the rounding mode
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/CMakeLists.txt` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/LICENSE-Apache2` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/LICENSE-Apache2`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/LICENSE-Boost` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/LICENSE-Boost`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/common.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/common.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s.c` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/digit_table.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/digit_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/f2s.c` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/f2s.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/generic_128.c` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/generic_128.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/generic_128.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/generic_128.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/ryu.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/ryu.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/ryu_generic_128.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/ryu_generic_128.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/ryu_parse.h` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/ryu_parse.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/s2d.c` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/s2d.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/s2f.c` & `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/s2f.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022-2023 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include "../fast_matrix_market.hpp"
 
 #include <armadillo>
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022-2023 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include "../fast_matrix_market.hpp"
 
 #include <blaze/Blaze.h>
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include "../fast_matrix_market.hpp"
 
 namespace fast_matrix_market {
     /**
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include "../fast_matrix_market.hpp"
 
 #if defined(__clang__)
 // Disable some pedantic warnings from Eigen headers.
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022-2023 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include "../fast_matrix_market.hpp"
 
 extern "C" {
 #include <GraphBLAS.h>
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/array.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/array.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include "../fast_matrix_market.hpp"
 
 namespace fast_matrix_market {
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include "../fast_matrix_market.hpp"
 
 namespace fast_matrix_market {
 #if __cplusplus >= 202002L
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include "../fast_matrix_market.hpp"
 
 namespace fast_matrix_market {
 #if __cplusplus >= 202002L
@@ -81,15 +82,17 @@
                                      const write_options& options = {}) {
         using IT = typename std::iterator_traits<decltype(rows.begin())>::value_type;
         using VT = typename std::iterator_traits<decltype(values.begin())>::value_type;
 
         header.nnz = values.size();
 
         header.object = matrix;
-        header.field = get_field_type((const VT*)nullptr);
+        if (header.field != pattern) {
+            header.field = get_field_type((const VT *) nullptr);
+        }
         header.format = coordinate;
 
         write_header(os, header);
 
         line_formatter<IT, VT> lf(header, options);
         auto formatter = triplet_formatter(lf,
                                            rows.cbegin(), rows.cend(),
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/chunking.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/chunking.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include <istream>
 #include <string>
 
 namespace fast_matrix_market {
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #ifndef FAST_MATRIX_MARKET_H
 #define FAST_MATRIX_MARKET_H
 
 #pragma once
 
 #include <algorithm>
@@ -18,16 +19,16 @@
 #include "types.hpp"
 
 namespace fast_matrix_market {
 
     // Version macros.
     // Keep in sync with python/pyproject.toml
 #define FAST_MATRIX_MARKET_VERSION_MAJOR 1
-#define FAST_MATRIX_MARKET_VERSION_MINOR 5
-#define FAST_MATRIX_MARKET_VERSION_PATCH 1
+#define FAST_MATRIX_MARKET_VERSION_MINOR 6
+#define FAST_MATRIX_MARKET_VERSION_PATCH 0
 
     constexpr std::string_view kSpace = " ";
     constexpr std::string_view kNewline = "\n";
 
     template<class T> struct is_complex : std::false_type {};
     template<class T> struct is_complex<std::complex<T>> : std::true_type {};
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/field_conv.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/field_conv.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include <charconv>
 #include <cmath>
 #include <complex>
 #include <limits>
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/formatters.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/formatters.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include <algorithm>
 #include <utility>
 
 #include "fast_matrix_market.hpp"
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/header.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/header.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include <fast_matrix_market/fast_matrix_market.hpp>
 
 #include "chunking.hpp"
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include <algorithm>
 #include <charconv>
 #include <complex>
 #include <functional>
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/read_body.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/read_body.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include <functional>
 #include "fast_matrix_market.hpp"
 
 #include "chunking.hpp"
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include <future>
 #include <queue>
 
 #include "fast_matrix_market.hpp"
-#include "3rdparty/BS_thread_pool_light.hpp"
+#include "thirdparty//task_thread_pool.hpp"
 
 namespace fast_matrix_market {
 
     struct line_count_result {
         std::string chunk;
         line_counts counts;
     };
@@ -49,22 +50,22 @@
          * The line count step is significantly faster than the parse step. As a form of backpressure we don't read
          * additional chunks if there are too many inflight chunks.
          */
         line_counts lc{header.header_line_count, 0};
 
         std::queue<std::future<line_count_result>> line_count_futures;
         std::queue<std::future<void>> parse_futures;
-        BS::thread_pool_light pool(options.num_threads);
+        task_thread_pool::task_thread_pool pool(options.num_threads);
 
         int generalizing_symmetry_factor = (header.symmetry != general && options.generalize_symmetry) ? 2 : 1;
 
         // Number of concurrent chunks available to work on.
         // Too few may starve workers (such as due to uneven chunk splits)
         // Too many increases costs, such as storing chunk results in memory before they're written.
-        const unsigned inflight_count = 5 * pool.get_thread_count();
+        const unsigned inflight_count = 5 * pool.get_num_threads();
 
         // Start reading chunks and counting lines.
         for (unsigned seed_i = 0; seed_i < inflight_count && instream.good(); ++seed_i) {
             line_count_result lcr;
             lcr.chunk = get_next_chunk(instream, options);
 
             line_count_futures.push(pool.submit(count_chunk_lines, lcr));
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/types.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/types.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include <map>
 #include <string>
 
 namespace fast_matrix_market {
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/write_body.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/write_body.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include "fast_matrix_market.hpp"
 
 #include "write_body_threads.hpp"
```

### Comparing `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp` & `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 // Copyright (C) 2022 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include <queue>
 
 #include "fast_matrix_market.hpp"
-#include "3rdparty/BS_thread_pool_light.hpp"
+#include "thirdparty//task_thread_pool.hpp"
 
 namespace fast_matrix_market {
     /**
      * Write Matrix Market body.
      *
      * Chunk based so that it can be made parallel. Each chunk is written by a FORMATTER class.
      * @tparam FORMATTER implementation class that writes chunks.
@@ -29,20 +30,20 @@
          *
          * The biggest obstacle is the final requirement to write all chunks sequentially.
          *
          * We take a simple approach. The main thread handles the serial chunk generation and I/O,
          * and a thread pool performs the parallel work.
          */
         std::queue<std::future<std::string>> futures;
-        BS::thread_pool_light pool(options.num_threads);
+        task_thread_pool::task_thread_pool pool(options.num_threads);
 
         // Number of concurrent chunks available to work on.
         // Too few may starve workers (such as due to uneven chunk splits)
         // Too many increases costs, such as storing chunk results in memory before they're written.
-        const int inflight_count = 5 * (int)pool.get_thread_count();
+        const int inflight_count = 5 * (int)pool.get_num_threads();
 
         // Start computing tasks.
         for (int batch_i = 0; batch_i < inflight_count && formatter.has_next(); ++batch_i) {
             futures.push(pool.submit(formatter.next_chunk(options)));
         }
 
         // Write chunks in order as they become available.
```

### Comparing `fast-matrix-market-1.5.1/pyproject.toml` & `fast-matrix-market-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["scikit-build-core", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "fast_matrix_market"
-version = "1.5.1"
+version = "1.6.0"
 description="Fast and full-featured Matrix Market file I/O"
 readme = "README.md"
 authors = [
     { name = "Adam Lugowski"},
 ]
 requires-python = ">=3.7"
```

### Comparing `fast-matrix-market-1.5.1/src/fast_matrix_market/__init__.py` & `fast-matrix-market-1.6.0/src/fast_matrix_market/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # Copyright (C) 2022-2023 Adam Lugowski. All rights reserved.
 # Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+# SPDX-License-Identifier: BSD-2-Clause
 """
-The ultimate Matrix Market I/O library. Read and write MatrixMarket files.
+Read and write Matrix Market files.
 
 Supports sparse coo/triplet matrices, sparse scipy matrices, and numpy array dense matrices.
 """
 import io
 import os
 
 from . import _core
 from ._core import __version__, header
 
 PARALLELISM = 0
 """
-Number of threads to use. 0 means number of threads in the system.
+Number of threads to use. 0 means number of CPUs in the system.
 """
 
 ALWAYS_FIND_SYMMETRY = False
 """
-If True then equivalent to always passing find_symmetry=True to mmwrite() and write_scipy().
-This matches scipy.io.mmwrite behavior, as well as its massive performance cost.
+If True then equivalent to always passing find_symmetry=True to mmwrite().
+This matches scipy.io.mmwrite()'s behavior, as well as its performance cost.
 """
 
 _field_to_dtype = {
     "integer": "int64",
     "unsigned-integer": "uint64",
     "real": "float64",
     "complex": "complex",
@@ -332,15 +333,15 @@
         return arr, arr.shape
     else:
         (data, (rows, cols)), shape = _read_body_coo(cursor, long_type=long_type,
                                                      generalize_symmetry=generalize_symmetry)
         return (data, (rows, cols)), shape
 
 
-def read_scipy(source, parallelism=None, long_type=False):
+def mmread(source, parallelism=None, long_type=False):
     """
     Read MatrixMarket file. If the file is dense, return a 2D numpy array. Else return a SciPy sparse matrix.
 
     Interchangeable with scipy.io.mmread() but faster and supports longdouble.
 
     :param source: path to MatrixMarket file or open file-like object
     :param parallelism: number of threads to use. 0 means auto.
@@ -354,15 +355,15 @@
         return _read_body_array(cursor, long_type=long_type)
     else:
         from scipy.sparse import coo_matrix
         triplet, shape = _read_body_coo(cursor, long_type=long_type, generalize_symmetry=True)
         return coo_matrix(triplet, shape=shape)
 
 
-def write_scipy(target, a, comment=None, field=None, precision=None, symmetry=None,
+def mmwrite(target, a, comment=None, field=None, precision=None, symmetry=None,
                 parallelism=None, find_symmetry=False):
     """
     Write a matrix to a MatrixMarket file or file-like object.
 
     Interchangeable with scipy.io.mmwrite() but faster.
 
     :param target: path to MatrixMarket file or open file-like object
@@ -428,20 +429,20 @@
         else:
             _core.write_coo(cursor, a.shape, a.row, a.col, data)
         return
 
     raise ValueError("unknown matrix type: %s" % type(a))
 
 
-mmread = read_scipy
-mmwrite = write_scipy
-
-
 def mminfo(source):
     """
     Same as scipy.io.mminfo()
 
     :param source: a Matrix Market file path or an open file-like object
     :return: a tuple of (# of rows, #of columns, #of entries, "coordinate" or "array", field type, symmetry type)
     """
     h = read_header(source)
     return h.nrows, h.ncols, h.nnz, h.format, h.field, h.symmetry
+
+
+read_scipy = mmread
+write_scipy = mmwrite
```

### Comparing `fast-matrix-market-1.5.1/src/fast_matrix_market/core.cpp` & `fast-matrix-market-1.6.0/src/fast_matrix_market/core.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // Copyright (C) 2022-2023 Adam Lugowski. All rights reserved.
 // Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+// SPDX-License-Identifier: BSD-2-Clause
 
 #include <fstream>
 
 #include <pybind11/pybind11.h>
 #include <pybind11/numpy.h>
 
 #include "pystreambuf.h"
```

### Comparing `fast-matrix-market-1.5.1/src/fast_matrix_market/pystreambuf.h` & `fast-matrix-market-1.6.0/src/fast_matrix_market/pystreambuf.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+// SPDX-License-Identifier: BSD-3-Clause
 /*
 Based on https://gist.github.com/asford/544323a5da7dddad2c9174490eb5ed06
 
 Original license text
 ---------------------
 
 This component utilizes components derived from cctbx, available at
@@ -417,15 +418,15 @@
         buf_begin = reinterpret_cast<std::streamsize>(pbase());
         buf_cur = reinterpret_cast<std::streamsize>(pptr());
         buf_end = reinterpret_cast<std::streamsize>(epptr());
         farthest_pptr = (std::max)(farthest_pptr, pptr());
         upper_bound = reinterpret_cast<std::streamsize>(farthest_pptr) + 1;
       }
       else {
-           std::runtime_error(
+           throw std::runtime_error(
              "Control flow passes through branch that should be unreachable.");
       }
 
       // Sought position in "buffer coordinate"
       off_type buf_sought;
       if (way == std::ios_base::cur) {
         buf_sought = buf_cur + off;
@@ -433,15 +434,15 @@
       else if (way == std::ios_base::beg) {
         buf_sought = buf_end + (off - pos_of_buffer_end_in_py_file);
       }
       else if (way == std::ios_base::end) {
         return false;
       }
       else {
-           std::runtime_error(
+           throw std::runtime_error(
              "Control flow passes through branch that should be unreachable.");
       }
 
       // if the sought position is not in the buffer, give up
       if (buf_sought < buf_begin || buf_sought >= upper_bound) return false;
 
       // we are in wonderland
```

### Comparing `fast-matrix-market-1.5.1/tests/test_array.py` & `fast-matrix-market-1.6.0/tests/test_array.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Copyright (C) 2022-2023 Adam Lugowski. All rights reserved.
 # Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+# SPDX-License-Identifier: BSD-2-Clause
+
 from io import BytesIO, StringIO
 from pathlib import Path
 import numpy as np
 import unittest
 import scipy
 import sys
```

### Comparing `fast-matrix-market-1.5.1/tests/test_coo.py` & `fast-matrix-market-1.6.0/tests/test_coo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Copyright (C) 2022-2023 Adam Lugowski. All rights reserved.
 # Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+# SPDX-License-Identifier: BSD-2-Clause
+
 from io import BytesIO, StringIO
 from pathlib import Path
 import numpy as np
 import unittest
 import scipy
 import sys
```

### Comparing `fast-matrix-market-1.5.1/tests/test_header.py` & `fast-matrix-market-1.6.0/tests/test_header.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Copyright (C) 2022-2023 Adam Lugowski. All rights reserved.
 # Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+# SPDX-License-Identifier: BSD-2-Clause
+
 from io import BytesIO, StringIO
 import unittest
 from pathlib import Path
 import sys
 
 import fast_matrix_market as fmm
```

### Comparing `fast-matrix-market-1.5.1/tests/test_scipy.py` & `fast-matrix-market-1.6.0/tests/test_scipy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Copyright (C) 2022-2023 Adam Lugowski. All rights reserved.
 # Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+# SPDX-License-Identifier: BSD-2-Clause
+
 import warnings
 from io import BytesIO, StringIO
 from pathlib import Path
 import unittest
 import sys
 
 import numpy as np
```

### Comparing `fast-matrix-market-1.5.1/testsuite_scipy/test_scipy_suite.py` & `fast-matrix-market-1.6.0/testsuite_scipy/test_scipy_suite.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Copyright (C) 2022-2023 Adam Lugowski. All rights reserved.
 # Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
+# SPDX-License-Identifier: BSD-2-Clause
+
 """
 Run the actual SciPy test suite for scipy.io.mm* methods against fast_matrix_market.
 
 This is intended to be run in development only as SciPy may change their suite at any time.
 """
 
 # replace scipy.io.mm* methods with the fast_matrix_market equivalents
```

### Comparing `fast-matrix-market-1.5.1/PKG-INFO` & `fast-matrix-market-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-matrix-market
-Version: 1.5.1
+Version: 1.6.0
 Summary: Fast and full-featured Matrix Market file I/O
 Home-page: https://github.com/alugowski/fast_matrix_market
 Author: Adam Lugowski
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

