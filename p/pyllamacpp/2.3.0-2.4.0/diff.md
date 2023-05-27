# Comparing `tmp/pyllamacpp-2.3.0.tar.gz` & `tmp/pyllamacpp-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllamacpp-2.3.0.tar", last modified: Sat May 20 01:09:11 2023, max compression
+gzip compressed data, was "pyllamacpp-2.4.0.tar", last modified: Sat May 27 02:19:28 2023, max compression
```

## Comparing `pyllamacpp-2.3.0.tar` & `pyllamacpp-2.4.0.tar`

### file list

```diff
@@ -1,123 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.236014 pyllamacpp-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-20 01:09:11.236014 pyllamacpp-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/
--rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/baby-llama/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/baby-llama/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/benchmark/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/embedding/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/main/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/main/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/perplexity/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/perplexity/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/quantize/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/quantize/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/quantize-stats/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/quantize-stats/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/save-load-state/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/save-load-state/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/pocs/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/pocs/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/pocs/vdot/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/pocs/vdot/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/scripts/build-info.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.224013 pyllamacpp-2.3.0/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.236014 pyllamacpp-2.3.0/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/pyllamacpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.236014 pyllamacpp-2.3.0/pyllamacpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-20 01:09:11.000000 pyllamacpp-2.3.0/pyllamacpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-20 01:09:11.000000 pyllamacpp-2.3.0/pyllamacpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 01:09:11.000000 pyllamacpp-2.3.0/pyllamacpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 01:09:11.000000 pyllamacpp-2.3.0/pyllamacpp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 01:09:10.000000 pyllamacpp-2.3.0/pyllamacpp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 01:09:11.000000 pyllamacpp-2.3.0/pyllamacpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 01:09:11.236014 pyllamacpp-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.236014 pyllamacpp-2.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/src/llama.cpp_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43672 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/src/main.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/baby-llama/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/baby-llama/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/benchmark/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/embedding/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/main/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/perplexity/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/quantize/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/quantize/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/quantize-stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/quantize-stats/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/save-load-state/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/save-load-state/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/server/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/pocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/pocs/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/pocs/vdot/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/pocs/vdot/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/scripts/build-info.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.233762 pyllamacpp-2.4.0/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/pyllamacpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/pyllamacpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-05-27 02:19:28.000000 pyllamacpp-2.4.0/pyllamacpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-27 02:19:28.000000 pyllamacpp-2.4.0/pyllamacpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:19:28.000000 pyllamacpp-2.4.0/pyllamacpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 02:19:28.000000 pyllamacpp-2.4.0/pyllamacpp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:19:27.000000 pyllamacpp-2.4.0/pyllamacpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 02:19:28.000000 pyllamacpp-2.4.0/pyllamacpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/src/llama.cpp_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43672 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/src/main.h
```

### Comparing `pyllamacpp-2.3.0/CMakeLists.txt` & `pyllamacpp-2.4.0/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # fix  "undefined reference to `pthread_join'" in github action
 set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread")
 
 add_subdirectory(pybind11)
 add_subdirectory(llama.cpp)
 # add_subdirectory(ggml)
 
-file (GLOB CPP_FILES "llama.cpp/*.cpp")
+file (GLOB CPP_FILES "llama.cpp/llama.cpp")
 file (GLOB C_FILES "llama.cpp/ggml.c")
 file (GLOB H_FILES "llama.cpp/ggml.h" "llama.cpp/llama.h")
 
 # ---------------------------------------------------------------------------------------------
```

### Comparing `pyllamacpp-2.3.0/LICENSE` & `pyllamacpp-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/PKG-INFO` & `pyllamacpp-2.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python bindings for llama.cpp
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
 Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyLLaMACpp
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
+[![Downloads](https://static.pepy.tech/badge/pyllamacpp)](https://pepy.tech/project/pyllamacpp)
 
 Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp)
 
 
 <p align="center">
   <img src="./docs/demo.gif">
 </p>
@@ -59,14 +60,22 @@
 However, the compilation process of `llama.cpp` is taking into account the architecture of the target `CPU`, 
 so you might need to build it from source:
 
 ```shell
 pip install git+https://github.com/abdeladim-s/pyllamacpp.git
 ```
 
+:warning: **Note**
+
+[This PR](https://github.com/ggerganov/llama.cpp/pull/1405) introduced some breaking changes.
+If you want to use older models, use version `2.2.0`:
+```bash
+pip install pyllamacpp==2.2.0
+```
+
 # CLI 
 
 You can run the following simple command line interface to test the package once it is installed:
 
 ```shell
 pyllamacpp path/to/ggml/model
 ```
@@ -185,18 +194,22 @@
 
 <blockquote>
 
 **Supported models:**
 
 - [X] LLaMA 🦙
 - [X] [Alpaca](https://github.com/ggerganov/llama.cpp#instruction-mode-with-alpaca)
+- [X] [GPT4All](https://github.com/ggerganov/llama.cpp#using-gpt4all)
 - [X] [Chinese LLaMA / Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
 - [X] [Vigogne (French)](https://github.com/bofenghuang/vigogne)
 - [X] [Vicuna](https://github.com/ggerganov/llama.cpp/discussions/643#discussioncomment-5533894)
 - [X] [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/)
+- [X] [OpenBuddy 🐶 (Multilingual)](https://github.com/OpenBuddy/OpenBuddy)
+- [X] [Pygmalion 7B / Metharme 7B](#using-pygmalion-7b--metharme-7b)
+- [X] [WizardLM](https://github.com/nlpxucan/WizardLM)
 
 </blockquote>
 
 # Advanced usage
 For advanced users, you can access the [llama.cpp C-API](https://github.com/ggerganov/llama.cpp/blob/master/llama.h) functions directly to make your own logic.
 All functions from `llama.h` are exposed with the binding module [`_pyllamacpp`](https://abdeladim-s.github.io/pyllamacpp/#_pyllamacpp).
```

### Comparing `pyllamacpp-2.3.0/README.md` & `pyllamacpp-2.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # PyLLaMACpp
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
+[![Downloads](https://static.pepy.tech/badge/pyllamacpp)](https://pepy.tech/project/pyllamacpp)
 
 Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp)
 
 
 <p align="center">
   <img src="./docs/demo.gif">
 </p>
@@ -46,14 +47,22 @@
 However, the compilation process of `llama.cpp` is taking into account the architecture of the target `CPU`, 
 so you might need to build it from source:
 
 ```shell
 pip install git+https://github.com/abdeladim-s/pyllamacpp.git
 ```
 
+:warning: **Note**
+
+[This PR](https://github.com/ggerganov/llama.cpp/pull/1405) introduced some breaking changes.
+If you want to use older models, use version `2.2.0`:
+```bash
+pip install pyllamacpp==2.2.0
+```
+
 # CLI 
 
 You can run the following simple command line interface to test the package once it is installed:
 
 ```shell
 pyllamacpp path/to/ggml/model
 ```
@@ -172,18 +181,22 @@
 
 <blockquote>
 
 **Supported models:**
 
 - [X] LLaMA 🦙
 - [X] [Alpaca](https://github.com/ggerganov/llama.cpp#instruction-mode-with-alpaca)
+- [X] [GPT4All](https://github.com/ggerganov/llama.cpp#using-gpt4all)
 - [X] [Chinese LLaMA / Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
 - [X] [Vigogne (French)](https://github.com/bofenghuang/vigogne)
 - [X] [Vicuna](https://github.com/ggerganov/llama.cpp/discussions/643#discussioncomment-5533894)
 - [X] [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/)
+- [X] [OpenBuddy 🐶 (Multilingual)](https://github.com/OpenBuddy/OpenBuddy)
+- [X] [Pygmalion 7B / Metharme 7B](#using-pygmalion-7b--metharme-7b)
+- [X] [WizardLM](https://github.com/nlpxucan/WizardLM)
 
 </blockquote>
 
 # Advanced usage
 For advanced users, you can access the [llama.cpp C-API](https://github.com/ggerganov/llama.cpp/blob/master/llama.h) functions directly to make your own logic.
 All functions from `llama.h` are exposed with the binding module [`_pyllamacpp`](https://abdeladim-s.github.io/pyllamacpp/#_pyllamacpp).
```

### Comparing `pyllamacpp-2.3.0/llama.cpp/CMakeLists.txt` & `pyllamacpp-2.4.0/llama.cpp/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -33,48 +33,52 @@
 
 
 #
 # Option list
 #
 
 # general
-option(LLAMA_STATIC                 "llama: static link libraries"                          OFF)
-option(LLAMA_NATIVE                 "llama: enable -march=native flag"                      OFF)
-option(LLAMA_LTO                    "llama: enable link time optimization"                  OFF)
+option(LLAMA_STATIC                     "llama: static link libraries"                          OFF)
+option(LLAMA_NATIVE                     "llama: enable -march=native flag"                      OFF)
+option(LLAMA_LTO                        "llama: enable link time optimization"                  OFF)
 
 # debug
-option(LLAMA_ALL_WARNINGS           "llama: enable all compiler warnings"                   ON)
-option(LLAMA_ALL_WARNINGS_3RD_PARTY "llama: enable all compiler warnings in 3rd party libs" OFF)
-option(LLAMA_GPROF                  "llama: enable gprof"                                   OFF)
+option(LLAMA_ALL_WARNINGS               "llama: enable all compiler warnings"                   ON)
+option(LLAMA_ALL_WARNINGS_3RD_PARTY     "llama: enable all compiler warnings in 3rd party libs" OFF)
+option(LLAMA_GPROF                      "llama: enable gprof"                                   OFF)
 
 # sanitizers
-option(LLAMA_SANITIZE_THREAD        "llama: enable thread sanitizer"                        OFF)
-option(LLAMA_SANITIZE_ADDRESS       "llama: enable address sanitizer"                       OFF)
-option(LLAMA_SANITIZE_UNDEFINED     "llama: enable undefined sanitizer"                     OFF)
+option(LLAMA_SANITIZE_THREAD            "llama: enable thread sanitizer"                        OFF)
+option(LLAMA_SANITIZE_ADDRESS           "llama: enable address sanitizer"                       OFF)
+option(LLAMA_SANITIZE_UNDEFINED         "llama: enable undefined sanitizer"                     OFF)
 
 # instruction set specific
-option(LLAMA_AVX                    "llama: enable AVX"                                     ON)
-option(LLAMA_AVX2                   "llama: enable AVX2"                                    ON)
-option(LLAMA_AVX512                 "llama: enable AVX512"                                  OFF)
-option(LLAMA_AVX512_VBMI            "llama: enable AVX512-VBMI"                             OFF)
-option(LLAMA_AVX512_VNNI            "llama: enable AVX512-VNNI"                             OFF)
-option(LLAMA_FMA                    "llama: enable FMA"                                     ON)
+option(LLAMA_AVX                        "llama: enable AVX"                                     ON)
+option(LLAMA_AVX2                       "llama: enable AVX2"                                    ON)
+option(LLAMA_AVX512                     "llama: enable AVX512"                                  OFF)
+option(LLAMA_AVX512_VBMI                "llama: enable AVX512-VBMI"                             OFF)
+option(LLAMA_AVX512_VNNI                "llama: enable AVX512-VNNI"                             OFF)
+option(LLAMA_FMA                        "llama: enable FMA"                                     ON)
 # in MSVC F16C is implied with AVX2/AVX512
 if (NOT MSVC)
-    option(LLAMA_F16C               "llama: enable F16C"                                    ON)
+    option(LLAMA_F16C                   "llama: enable F16C"                                    ON)
 endif()
 
 # 3rd party libs
-option(LLAMA_ACCELERATE             "llama: enable Accelerate framework"                    ON)
-option(LLAMA_OPENBLAS               "llama: use OpenBLAS"                                   OFF)
-option(LLAMA_CUBLAS                 "llama: use cuBLAS"                                     OFF)
-option(LLAMA_CLBLAST                "llama: use CLBlast"                                    OFF)
-
-option(LLAMA_BUILD_TESTS            "llama: build tests"    ${LLAMA_STANDALONE})
-option(LLAMA_BUILD_EXAMPLES         "llama: build examples" ${LLAMA_STANDALONE})
+option(LLAMA_ACCELERATE                 "llama: enable Accelerate framework"                    ON)
+option(LLAMA_BLAS                       "llama: use BLAS"                                       OFF)
+option(LLAMA_BLAS_VENDOR                "llama: BLA_VENDOR from https://cmake.org/cmake/help/latest/module/FindBLAS.html#blas-lapack-vendors" Generic)
+option(LLAMA_CUBLAS                     "llama: use cuBLAS"                                     OFF)
+set(LLAMA_CUDA_DMMV_X "32" CACHE STRING "llama: x stride for dmmv CUDA kernels")
+set(LLAMA_CUDA_DMMV_Y "1" CACHE STRING  "llama: y block size for dmmv CUDA kernels")
+option(LLAMA_CLBLAST                    "llama: use CLBlast"                                    OFF)
+
+option(LLAMA_BUILD_TESTS                "llama: build tests"    ${LLAMA_STANDALONE})
+option(LLAMA_BUILD_EXAMPLES             "llama: build examples" ${LLAMA_STANDALONE})
+option(LLAMA_BUILD_SERVER               "llama: build server example"                           OFF)
 
 #
 # Build info header
 #
 
 # Generate initial build-info.h
 include(${CMAKE_CURRENT_SOURCE_DIR}/scripts/build-info.cmake)
@@ -141,44 +145,36 @@
         add_compile_definitions(GGML_USE_ACCELERATE)
         set(LLAMA_EXTRA_LIBS ${LLAMA_EXTRA_LIBS} ${ACCELERATE_FRAMEWORK})
     else()
         message(WARNING "Accelerate framework not found")
     endif()
 endif()
 
-if (LLAMA_OPENBLAS)
+if (LLAMA_BLAS)
     if (LLAMA_STATIC)
         set(BLA_STATIC ON)
     endif()
-
-    set(BLA_VENDOR OpenBLAS)
+    if ($(CMAKE_VERSION) VERSION_GREATER_EQUAL 3.22)
+        set(BLA_SIZEOF_INTEGER 8)
+    endif()
+    set(BLA_VENDOR ${LLAMA_BLAS_VENDOR})
     find_package(BLAS)
     if (BLAS_FOUND)
-        message(STATUS "OpenBLAS found")
+        message(STATUS "BLAS found, Libraries: ${BLAS_LIBRARIES}")
 
+        add_compile_options(${BLAS_LINKER_FLAGS})
         add_compile_definitions(GGML_USE_OPENBLAS)
-        add_link_options(${BLAS_LIBRARIES})
-        set(LLAMA_EXTRA_LIBS ${LLAMA_EXTRA_LIBS} openblas)
+        set(LLAMA_EXTRA_LIBS ${LLAMA_EXTRA_LIBS} ${BLAS_LIBRARIES})
 
-        # find header file
-        set(OPENBLAS_INCLUDE_SEARCH_PATHS
-            /usr/include
-            /usr/include/openblas
-            /usr/include/openblas-base
-            /usr/local/include
-            /usr/local/include/openblas
-            /usr/local/include/openblas-base
-            /opt/OpenBLAS/include
-            $ENV{OpenBLAS_HOME}
-            $ENV{OpenBLAS_HOME}/include
-            )
-        find_path(OPENBLAS_INC NAMES cblas.h PATHS ${OPENBLAS_INCLUDE_SEARCH_PATHS})
-        add_compile_options(-I${OPENBLAS_INC})
+        message("${BLAS_LIBRARIES} ${BLAS_INCLUDE_DIRS}")
+        include_directories(${BLAS_INCLUDE_DIRS})
     else()
-        message(WARNING "OpenBLAS not found")
+        message(WARNING "BLAS not found, please refer to "
+        "https://cmake.org/cmake/help/latest/module/FindBLAS.html#blas-lapack-vendors"
+        " to set correct LLAMA_BLAS_VENDOR")
     endif()
 endif()
 
 if (LLAMA_CUBLAS)
     cmake_minimum_required(VERSION 3.17)
 
     find_package(CUDAToolkit)
@@ -186,14 +182,16 @@
         message(STATUS "cuBLAS found")
 
         enable_language(CUDA)
 
         set(GGML_CUDA_SOURCES ggml-cuda.cu ggml-cuda.h)
 
         add_compile_definitions(GGML_USE_CUBLAS)
+        add_compile_definitions(GGML_CUDA_DMMV_X=${LLAMA_CUDA_DMMV_X})
+        add_compile_definitions(GGML_CUDA_DMMV_Y=${LLAMA_CUDA_DMMV_Y})
 
         if (LLAMA_STATIC)
             set(LLAMA_EXTRA_LIBS ${LLAMA_EXTRA_LIBS} CUDA::cudart_static CUDA::cublas_static CUDA::cublasLt_static)
         else()
             set(LLAMA_EXTRA_LIBS ${LLAMA_EXTRA_LIBS} CUDA::cudart CUDA::cublas CUDA::cublasLt)
         endif()
 
@@ -203,15 +201,15 @@
 endif()
 
 if (LLAMA_CLBLAST)
     find_package(CLBlast)
     if (CLBlast_FOUND)
         message(STATUS "CLBlast found")
 
-        set(GGML_OPENCL_SOURCES ggml-opencl.c ggml-opencl.h)
+        set(GGML_OPENCL_SOURCES ggml-opencl.cpp ggml-opencl.h)
 
         add_compile_definitions(GGML_USE_CLBLAST)
 
         set(LLAMA_EXTRA_LIBS ${LLAMA_EXTRA_LIBS} clblast)
     else()
         message(WARNING "CLBlast not found")
     endif()
```

### Comparing `pyllamacpp-2.3.0/llama.cpp/scripts/build-info.cmake` & `pyllamacpp-2.4.0/llama.cpp/scripts/build-info.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/llama.cpp/tests/CMakeLists.txt` & `pyllamacpp-2.4.0/llama.cpp/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/CMakeLists.txt` & `pyllamacpp-2.4.0/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/LICENSE` & `pyllamacpp-2.4.0/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/attr.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/buffer_info.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/cast.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/chrono.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/complex.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/class.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/common.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/descr.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/init.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/internals.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/type_caster_base.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/typeid.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/eigen.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/embed.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/eval.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/functional.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/gil.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/iostream.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/numpy.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/operators.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/options.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/pybind11.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/pytypes.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/stl/filesystem.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/stl.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/include/pybind11/stl_bind.h` & `pyllamacpp-2.4.0/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tests/CMakeLists.txt` & `pyllamacpp-2.4.0/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tests/test_embed/CMakeLists.txt` & `pyllamacpp-2.4.0/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tools/FindCatch.cmake` & `pyllamacpp-2.4.0/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tools/FindEigen3.cmake` & `pyllamacpp-2.4.0/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tools/FindPythonLibsNew.cmake` & `pyllamacpp-2.4.0/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tools/check-style.sh` & `pyllamacpp-2.4.0/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tools/cmake_uninstall.cmake.in` & `pyllamacpp-2.4.0/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tools/libsize.py` & `pyllamacpp-2.4.0/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tools/make_changelog.py` & `pyllamacpp-2.4.0/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tools/pybind11Common.cmake` & `pyllamacpp-2.4.0/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tools/pybind11Config.cmake.in` & `pyllamacpp-2.4.0/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tools/pybind11NewTools.cmake` & `pyllamacpp-2.4.0/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tools/pybind11Tools.cmake` & `pyllamacpp-2.4.0/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tools/setup_global.py.in` & `pyllamacpp-2.4.0/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pybind11/tools/setup_main.py.in` & `pyllamacpp-2.4.0/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pyllamacpp/_logger.py` & `pyllamacpp-2.4.0/pyllamacpp/_logger.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pyllamacpp/cli.py` & `pyllamacpp-2.4.0/pyllamacpp/cli.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pyllamacpp/model.py` & `pyllamacpp-2.4.0/pyllamacpp/model.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pyllamacpp/utils.py` & `pyllamacpp-2.4.0/pyllamacpp/utils.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pyllamacpp/webui.py` & `pyllamacpp-2.4.0/pyllamacpp/webui.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/pyllamacpp.egg-info/PKG-INFO` & `pyllamacpp-2.4.0/pyllamacpp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python bindings for llama.cpp
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
 Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyLLaMACpp
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
+[![Downloads](https://static.pepy.tech/badge/pyllamacpp)](https://pepy.tech/project/pyllamacpp)
 
 Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp)
 
 
 <p align="center">
   <img src="./docs/demo.gif">
 </p>
@@ -59,14 +60,22 @@
 However, the compilation process of `llama.cpp` is taking into account the architecture of the target `CPU`, 
 so you might need to build it from source:
 
 ```shell
 pip install git+https://github.com/abdeladim-s/pyllamacpp.git
 ```
 
+:warning: **Note**
+
+[This PR](https://github.com/ggerganov/llama.cpp/pull/1405) introduced some breaking changes.
+If you want to use older models, use version `2.2.0`:
+```bash
+pip install pyllamacpp==2.2.0
+```
+
 # CLI 
 
 You can run the following simple command line interface to test the package once it is installed:
 
 ```shell
 pyllamacpp path/to/ggml/model
 ```
@@ -185,18 +194,22 @@
 
 <blockquote>
 
 **Supported models:**
 
 - [X] LLaMA 🦙
 - [X] [Alpaca](https://github.com/ggerganov/llama.cpp#instruction-mode-with-alpaca)
+- [X] [GPT4All](https://github.com/ggerganov/llama.cpp#using-gpt4all)
 - [X] [Chinese LLaMA / Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
 - [X] [Vigogne (French)](https://github.com/bofenghuang/vigogne)
 - [X] [Vicuna](https://github.com/ggerganov/llama.cpp/discussions/643#discussioncomment-5533894)
 - [X] [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/)
+- [X] [OpenBuddy 🐶 (Multilingual)](https://github.com/OpenBuddy/OpenBuddy)
+- [X] [Pygmalion 7B / Metharme 7B](#using-pygmalion-7b--metharme-7b)
+- [X] [WizardLM](https://github.com/nlpxucan/WizardLM)
 
 </blockquote>
 
 # Advanced usage
 For advanced users, you can access the [llama.cpp C-API](https://github.com/ggerganov/llama.cpp/blob/master/llama.h) functions directly to make your own logic.
 All functions from `llama.h` are exposed with the binding module [`_pyllamacpp`](https://abdeladim-s.github.io/pyllamacpp/#_pyllamacpp).
```

### Comparing `pyllamacpp-2.3.0/pyllamacpp.egg-info/SOURCES.txt` & `pyllamacpp-2.4.0/pyllamacpp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 llama.cpp/examples/benchmark/CMakeLists.txt
 llama.cpp/examples/embedding/CMakeLists.txt
 llama.cpp/examples/main/CMakeLists.txt
 llama.cpp/examples/perplexity/CMakeLists.txt
 llama.cpp/examples/quantize/CMakeLists.txt
 llama.cpp/examples/quantize-stats/CMakeLists.txt
 llama.cpp/examples/save-load-state/CMakeLists.txt
+llama.cpp/examples/server/CMakeLists.txt
 llama.cpp/pocs/CMakeLists.txt
 llama.cpp/pocs/vdot/CMakeLists.txt
 llama.cpp/scripts/build-info.cmake
 llama.cpp/tests/CMakeLists.txt
 pybind11/CMakeLists.txt
 pybind11/LICENSE
 pybind11/include/pybind11/attr.h
```

### Comparing `pyllamacpp-2.3.0/pyproject.toml` & `pyllamacpp-2.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/setup.py` & `pyllamacpp-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,21 +121,21 @@
         subprocess.run(
             ["cmake", "--build", ".", *build_args], cwd=build_temp, check=True
         )
 
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
+long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyllamacpp",
-    version="2.3.0",
+    version="2.4.0",
     author="Abdeladim Sadiki",
     description="Python bindings for llama.cpp",
     long_description=long_description,
     ext_modules=[CMakeExtension("_pyllamacpp")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     # extras_require={"test": ["pytest>=6.0"]},
```

### Comparing `pyllamacpp-2.3.0/src/llama.cpp_LICENSE` & `pyllamacpp-2.4.0/src/llama.cpp_LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/src/main.cpp` & `pyllamacpp-2.4.0/src/main.cpp`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.3.0/src/main.h` & `pyllamacpp-2.4.0/src/main.h`

 * *Files identical despite different names*

