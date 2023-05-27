# Comparing `tmp/squander-1.8.3.tar.gz` & `tmp/squander-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squander-1.8.3.tar", last modified: Sun May 21 05:00:47 2023, max compression
+gzip compressed data, was "squander-1.8.4.tar", last modified: Sat May 27 16:26:58 2023, max compression
```

## Comparing `squander-1.8.3.tar` & `squander-1.8.4.tar`

### file list

```diff
@@ -1,195 +1,193 @@
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.295089 squander-1.8.3/.pytest_cache/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      302 2023-05-20 20:13:53.000000 squander-1.8.3/.pytest_cache/README.md
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15412 2023-05-21 04:59:59.000000 squander-1.8.3/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    35149 2023-05-20 20:06:21.000000 squander-1.8.3/LICENSE
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      121 2023-05-20 20:06:21.000000 squander-1.8.3/MANIFEST.in
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15887 2023-05-21 05:00:47.319089 squander-1.8.3/PKG-INFO
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15299 2023-05-20 20:07:48.000000 squander-1.8.3/README.md
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.295089 squander-1.8.3/cmake/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4306 2023-05-20 20:06:21.000000 squander-1.8.3/cmake/check_AVX.cmake
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.295089 squander-1.8.3/common/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6776 2023-05-20 20:06:21.000000 squander-1.8.3/common/Adam.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8316 2023-05-20 20:06:21.000000 squander-1.8.3/common/common.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5293 2023-05-20 20:06:21.000000 squander-1.8.3/common/common_DFE.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5524 2023-05-20 20:06:21.000000 squander-1.8.3/common/config_element.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    14292 2023-05-20 20:06:21.000000 squander-1.8.3/common/dot.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.299089 squander-1.8.3/common/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3441 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/Adam.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      166 2023-05-20 20:08:18.000000 squander-1.8.3/common/include/Config.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      216 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/Config.h.in
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2109 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/QGDTypes.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5357 2023-05-20 20:07:48.000000 squander-1.8.3/common/include/common.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3026 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/common_DFE.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3423 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/config_element.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7798 2023-05-20 20:07:48.000000 squander-1.8.3/common/include/dot.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9130 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/lbfgs.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2443 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/logging.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3812 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/matrix.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    13831 2023-05-20 20:07:48.000000 squander-1.8.3/common/include/matrix_base.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3752 2023-05-20 20:07:48.000000 squander-1.8.3/common/include/matrix_real.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1393 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/mpi_base.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1468 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/numpy_interface.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9234 2023-05-20 20:07:48.000000 squander-1.8.3/common/include/tolmin.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)   156010 2023-05-20 20:06:21.000000 squander-1.8.3/common/lbfgs.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2515 2023-05-20 20:06:21.000000 squander-1.8.3/common/logging.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5065 2023-05-20 20:06:21.000000 squander-1.8.3/common/matrix.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4497 2023-05-20 20:07:48.000000 squander-1.8.3/common/matrix_real.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1095 2023-05-20 20:06:21.000000 squander-1.8.3/common/mpi_base.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4808 2023-05-20 20:06:21.000000 squander-1.8.3/common/numpy_interface.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    58339 2023-05-20 20:07:48.000000 squander-1.8.3/common/tolmin.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.299089 squander-1.8.3/decomposition/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    57710 2023-05-20 20:07:48.000000 squander-1.8.3/decomposition/Decomposition_Base.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    37081 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/N_Qubit_Decomposition.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)   103422 2023-05-20 20:07:48.000000 squander-1.8.3/decomposition/N_Qubit_Decomposition_Base.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    16714 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/N_Qubit_Decomposition_Cost_Function.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    70942 2023-05-21 04:51:46.000000 squander-1.8.3/decomposition/N_Qubit_Decomposition_adaptive.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    12741 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/N_Qubit_Decomposition_custom.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    23508 2023-05-20 20:07:48.000000 squander-1.8.3/decomposition/Sub_Matrix_Decomposition.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8536 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.303089 squander-1.8.3/decomposition/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    16528 2023-05-20 20:07:48.000000 squander-1.8.3/decomposition/include/Decomposition_Base.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7166 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/include/N_Qubit_Decomposition.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15866 2023-05-20 20:07:48.000000 squander-1.8.3/decomposition/include/N_Qubit_Decomposition_Base.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5077 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/include/N_Qubit_Decomposition_Cost_Function.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8301 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/include/N_Qubit_Decomposition_adaptive.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3393 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/include/N_Qubit_Decomposition_custom.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6924 2023-05-20 20:07:48.000000 squander-1.8.3/decomposition/include/Sub_Matrix_Decomposition.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3723 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.307089 squander-1.8.3/gates/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5728 2023-05-20 20:06:21.000000 squander-1.8.3/gates/Adaptive.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4900 2023-05-20 20:06:21.000000 squander-1.8.3/gates/CH.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4937 2023-05-20 20:06:21.000000 squander-1.8.3/gates/CNOT.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5839 2023-05-20 20:06:21.000000 squander-1.8.3/gates/CRY.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4841 2023-05-20 20:06:21.000000 squander-1.8.3/gates/CZ.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7781 2023-05-20 20:06:21.000000 squander-1.8.3/gates/Composite.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    11545 2023-05-20 20:06:21.000000 squander-1.8.3/gates/Gate.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)   120998 2023-05-20 20:06:21.000000 squander-1.8.3/gates/Gates_block.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8547 2023-05-20 20:06:21.000000 squander-1.8.3/gates/ON.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6819 2023-05-20 20:06:21.000000 squander-1.8.3/gates/RX.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6815 2023-05-20 20:06:21.000000 squander-1.8.3/gates/RY.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7110 2023-05-20 20:06:21.000000 squander-1.8.3/gates/RZ.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8697 2023-05-20 20:06:21.000000 squander-1.8.3/gates/SX.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9587 2023-05-20 20:06:21.000000 squander-1.8.3/gates/SYC.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15472 2023-05-20 20:06:21.000000 squander-1.8.3/gates/U3.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8769 2023-05-20 20:06:21.000000 squander-1.8.3/gates/UN.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7950 2023-05-20 20:06:21.000000 squander-1.8.3/gates/X.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5671 2023-05-20 20:06:21.000000 squander-1.8.3/gates/Y.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5672 2023-05-20 20:06:21.000000 squander-1.8.3/gates/Z.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.307089 squander-1.8.3/gates/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3421 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/Adaptive.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2454 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/CH.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2530 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/CNOT.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3139 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/CRY.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2453 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/CZ.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3594 2023-05-20 20:06:21.000000 squander-1.8.3/gates/include/Composite.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5097 2023-05-20 20:06:21.000000 squander-1.8.3/gates/include/Gate.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15824 2023-05-20 20:06:21.000000 squander-1.8.3/gates/include/Gates_block.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3412 2023-05-20 20:06:21.000000 squander-1.8.3/gates/include/ON.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2838 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/RX.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3114 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/RY.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2834 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/RZ.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2809 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/SX.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2454 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/SYC.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6043 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/U3.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3412 2023-05-20 20:06:21.000000 squander-1.8.3/gates/include/UN.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2800 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/X.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2798 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/Y.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2798 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/Z.h
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.307089 squander-1.8.3/gates/kernels/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    23630 2023-05-20 20:06:21.000000 squander-1.8.3/gates/kernels/apply_kernel_to_input_AVX.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    32382 2023-05-20 20:06:21.000000 squander-1.8.3/gates/kernels/apply_kernel_to_state_vector_input.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.307089 squander-1.8.3/gates/kernels/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1786 2023-05-20 20:06:21.000000 squander-1.8.3/gates/kernels/include/apply_kernel_to_input_AVX.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2099 2023-05-20 20:06:21.000000 squander-1.8.3/gates/kernels/include/apply_kernel_to_state_vector_input.h
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.311089 squander-1.8.3/nn/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    18465 2023-05-20 20:07:48.000000 squander-1.8.3/nn/NN.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.311089 squander-1.8.3/nn/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5212 2023-05-20 20:07:48.000000 squander-1.8.3/nn/include/NN.h
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.311089 squander-1.8.3/optimization_engines/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9698 2023-05-20 20:06:21.000000 squander-1.8.3/optimization_engines/RL_experience.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.311089 squander-1.8.3/optimization_engines/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3549 2023-05-20 20:06:21.000000 squander-1.8.3/optimization_engines/include/RL_experience.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      123 2023-05-20 20:06:21.000000 squander-1.8.3/pyproject.toml
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.311089 squander-1.8.3/qgd_python/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       27 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/__init__.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.311089 squander-1.8.3/qgd_python/decomposition/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4472 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/decomposition/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       27 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/__init__.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7661 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    36701 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    25000 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    82737 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    14278 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    40978 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3367 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.315089 squander-1.8.3/qgd_python/decomposition/test/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        0 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/__init__.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    11024 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_Compression.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1927 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_Global_Phase.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7037 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_IBM.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1777 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_Project_Name.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5616 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_QX2.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4399 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_State_Preparation.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1656 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_Unitary.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4672 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_decomposition.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7190 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_fmo.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7018 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_heavy_hex.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6583 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_optmization_problem_combined.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4905 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_parametric_circuit.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.315089 squander-1.8.3/qgd_python/gates/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    13911 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        0 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/__init__.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8355 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_CH.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8292 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_CNOT.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8165 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_CZ.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    28668 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_Gates_Block.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8661 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_RX.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8660 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_RY.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8659 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_RZ.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7903 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_SX.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7941 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_SYC.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9186 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_U3.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7621 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_X.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8499 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_Y.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8499 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_Z.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/qgd_python/gates/test/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        0 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/__init__.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3364 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_CH.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3409 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_CNOT.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3444 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_CZ.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3466 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_RX.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3348 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_RY.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3919 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_RZ.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3278 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_SX.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3676 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_U3.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3182 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_X.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3179 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_Y.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3232 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_Z.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6878 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_gates.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/qgd_python/nn/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1332 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/nn/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       27 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/nn/__init__.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2387 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/nn/qgd_nn.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9606 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/nn/qgd_nn_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1573 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/utils.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/random_unitary/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6628 2023-05-20 20:06:21.000000 squander-1.8.3/random_unitary/Random_Orthogonal.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    11039 2023-05-20 20:06:21.000000 squander-1.8.3/random_unitary/Random_Unitary.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/random_unitary/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1927 2023-05-20 20:06:21.000000 squander-1.8.3/random_unitary/include/Random_Orthogonal.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4476 2023-05-20 20:06:21.000000 squander-1.8.3/random_unitary/include/Random_Unitary.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       38 2023-05-21 05:00:47.319089 squander-1.8.3/setup.cfg
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1898 2023-05-21 05:00:10.000000 squander-1.8.3/setup.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/squander/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1442 2023-05-20 20:06:21.000000 squander-1.8.3/squander/__init__.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/squander.egg-info/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15887 2023-05-21 05:00:47.000000 squander-1.8.3/squander.egg-info/PKG-INFO
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5181 2023-05-21 05:00:47.000000 squander-1.8.3/squander.egg-info/SOURCES.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        1 2023-05-21 05:00:47.000000 squander-1.8.3/squander.egg-info/dependency_links.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       50 2023-05-21 05:00:47.000000 squander-1.8.3/squander.egg-info/requires.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       20 2023-05-21 05:00:47.000000 squander-1.8.3/squander.egg-info/top_level.txt
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/test_standalone/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1996 2023-05-20 20:06:21.000000 squander-1.8.3/test_standalone/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6325 2023-05-20 20:06:21.000000 squander-1.8.3/test_standalone/custom_gate_structure_test.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4837 2023-05-20 20:06:21.000000 squander-1.8.3/test_standalone/decomposition_test.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15412 2023-05-27 16:25:37.000000 squander-1.8.4/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    35149 2023-05-27 16:24:34.000000 squander-1.8.4/LICENSE
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      121 2023-05-27 16:24:34.000000 squander-1.8.4/MANIFEST.in
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16207 2023-05-27 16:26:58.646819 squander-1.8.4/PKG-INFO
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15619 2023-05-27 16:24:34.000000 squander-1.8.4/README.md
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.630819 squander-1.8.4/cmake/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4306 2023-05-27 16:24:34.000000 squander-1.8.4/cmake/check_AVX.cmake
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.630819 squander-1.8.4/common/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6776 2023-05-27 16:24:34.000000 squander-1.8.4/common/Adam.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8316 2023-05-27 16:24:34.000000 squander-1.8.4/common/common.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5293 2023-05-27 16:24:34.000000 squander-1.8.4/common/common_DFE.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5524 2023-05-27 16:24:34.000000 squander-1.8.4/common/config_element.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14292 2023-05-27 16:24:34.000000 squander-1.8.4/common/dot.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.634819 squander-1.8.4/common/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3441 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/Adam.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      166 2023-05-27 16:26:35.000000 squander-1.8.4/common/include/Config.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      216 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/Config.h.in
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2109 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/QGDTypes.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5357 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/common.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3026 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/common_DFE.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3423 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/config_element.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7798 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/dot.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9130 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/lbfgs.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2443 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/logging.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3812 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/matrix.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    13831 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/matrix_base.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3752 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/matrix_real.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1393 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/mpi_base.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1468 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/numpy_interface.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9234 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/tolmin.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   156010 2023-05-27 16:24:34.000000 squander-1.8.4/common/lbfgs.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2515 2023-05-27 16:24:34.000000 squander-1.8.4/common/logging.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5065 2023-05-27 16:24:34.000000 squander-1.8.4/common/matrix.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4497 2023-05-27 16:24:34.000000 squander-1.8.4/common/matrix_real.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1095 2023-05-27 16:24:34.000000 squander-1.8.4/common/mpi_base.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4808 2023-05-27 16:24:34.000000 squander-1.8.4/common/numpy_interface.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    58339 2023-05-27 16:24:34.000000 squander-1.8.4/common/tolmin.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.634819 squander-1.8.4/decomposition/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    57710 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/Decomposition_Base.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    37081 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/N_Qubit_Decomposition.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   117800 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/N_Qubit_Decomposition_Base.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16713 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/N_Qubit_Decomposition_Cost_Function.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    70942 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/N_Qubit_Decomposition_adaptive.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    12741 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/N_Qubit_Decomposition_custom.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    23508 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/Sub_Matrix_Decomposition.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8536 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.634819 squander-1.8.4/decomposition/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16528 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/Decomposition_Base.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7166 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/N_Qubit_Decomposition.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15866 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/N_Qubit_Decomposition_Base.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5077 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/N_Qubit_Decomposition_Cost_Function.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8301 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/N_Qubit_Decomposition_adaptive.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3393 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/N_Qubit_Decomposition_custom.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6924 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/Sub_Matrix_Decomposition.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3723 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/gates/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5728 2023-05-27 16:24:34.000000 squander-1.8.4/gates/Adaptive.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4900 2023-05-27 16:24:34.000000 squander-1.8.4/gates/CH.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4937 2023-05-27 16:24:34.000000 squander-1.8.4/gates/CNOT.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5839 2023-05-27 16:24:34.000000 squander-1.8.4/gates/CRY.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4841 2023-05-27 16:24:34.000000 squander-1.8.4/gates/CZ.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7781 2023-05-27 16:24:34.000000 squander-1.8.4/gates/Composite.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11507 2023-05-27 16:24:34.000000 squander-1.8.4/gates/Gate.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   120998 2023-05-27 16:24:34.000000 squander-1.8.4/gates/Gates_block.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8547 2023-05-27 16:24:34.000000 squander-1.8.4/gates/ON.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6819 2023-05-27 16:24:34.000000 squander-1.8.4/gates/RX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6815 2023-05-27 16:24:34.000000 squander-1.8.4/gates/RY.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7110 2023-05-27 16:24:34.000000 squander-1.8.4/gates/RZ.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8697 2023-05-27 16:24:34.000000 squander-1.8.4/gates/SX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9587 2023-05-27 16:24:34.000000 squander-1.8.4/gates/SYC.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15837 2023-05-27 16:24:34.000000 squander-1.8.4/gates/U3.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8769 2023-05-27 16:24:34.000000 squander-1.8.4/gates/UN.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7950 2023-05-27 16:24:34.000000 squander-1.8.4/gates/X.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5671 2023-05-27 16:24:34.000000 squander-1.8.4/gates/Y.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5672 2023-05-27 16:24:34.000000 squander-1.8.4/gates/Z.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/gates/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3421 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/Adaptive.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2454 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/CH.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2530 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/CNOT.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3139 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/CRY.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2453 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/CZ.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3594 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/Composite.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5097 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/Gate.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15824 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/Gates_block.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3412 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/ON.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2838 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/RX.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3114 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/RY.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2834 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/RZ.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2809 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/SX.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2454 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/SYC.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6043 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/U3.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3412 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/UN.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2800 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/X.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2798 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/Y.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2798 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/Z.h
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/gates/kernels/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    23630 2023-05-27 16:24:34.000000 squander-1.8.4/gates/kernels/apply_kernel_to_input_AVX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    32382 2023-05-27 16:24:34.000000 squander-1.8.4/gates/kernels/apply_kernel_to_state_vector_input.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/gates/kernels/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1786 2023-05-27 16:24:34.000000 squander-1.8.4/gates/kernels/include/apply_kernel_to_input_AVX.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2099 2023-05-27 16:24:34.000000 squander-1.8.4/gates/kernels/include/apply_kernel_to_state_vector_input.h
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/nn/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    18465 2023-05-27 16:24:34.000000 squander-1.8.4/nn/NN.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/nn/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5212 2023-05-27 16:24:34.000000 squander-1.8.4/nn/include/NN.h
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/optimization_engines/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9698 2023-05-27 16:24:34.000000 squander-1.8.4/optimization_engines/RL_experience.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/optimization_engines/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3549 2023-05-27 16:24:34.000000 squander-1.8.4/optimization_engines/include/RL_experience.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      123 2023-05-27 16:24:34.000000 squander-1.8.4/pyproject.toml
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/qgd_python/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/__init__.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.642819 squander-1.8.4/qgd_python/decomposition/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4472 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7661 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    36701 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    25000 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    82737 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14278 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    40978 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3367 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.642819 squander-1.8.4/qgd_python/decomposition/test/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11142 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_Compression.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1927 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_Global_Phase.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7037 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_IBM.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1777 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_Project_Name.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5616 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_QX2.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4399 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_State_Preparation.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1656 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_Unitary.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4672 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_decomposition.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7190 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_fmo.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7018 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_heavy_hex.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6583 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_optmization_problem_combined.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4905 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_parametric_circuit.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.642819 squander-1.8.4/qgd_python/gates/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    13911 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8355 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_CH.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8292 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_CNOT.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8165 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_CZ.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    28668 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_Gates_Block.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8661 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_RX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8660 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_RY.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8659 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_RZ.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7903 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_SX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7941 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_SYC.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9186 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_U3.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7621 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_X.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8499 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_Y.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8499 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_Z.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/qgd_python/gates/test/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3364 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_CH.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3409 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_CNOT.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3444 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_CZ.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3466 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_RX.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3348 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_RY.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3919 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_RZ.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3278 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_SX.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3676 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_U3.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3182 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_X.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3179 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_Y.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3232 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_Z.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6878 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_gates.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/qgd_python/nn/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1332 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/nn/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/nn/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2387 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/nn/qgd_nn.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9606 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/nn/qgd_nn_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1573 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/utils.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/random_unitary/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6628 2023-05-27 16:24:34.000000 squander-1.8.4/random_unitary/Random_Orthogonal.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11039 2023-05-27 16:24:34.000000 squander-1.8.4/random_unitary/Random_Unitary.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/random_unitary/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1927 2023-05-27 16:24:34.000000 squander-1.8.4/random_unitary/include/Random_Orthogonal.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4476 2023-05-27 16:24:34.000000 squander-1.8.4/random_unitary/include/Random_Unitary.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       38 2023-05-27 16:26:58.646819 squander-1.8.4/setup.cfg
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1898 2023-05-27 16:24:49.000000 squander-1.8.4/setup.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/squander/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1442 2023-05-27 16:24:34.000000 squander-1.8.4/squander/__init__.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/squander.egg-info/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16207 2023-05-27 16:26:58.000000 squander-1.8.4/squander.egg-info/PKG-INFO
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5157 2023-05-27 16:26:58.000000 squander-1.8.4/squander.egg-info/SOURCES.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        1 2023-05-27 16:26:58.000000 squander-1.8.4/squander.egg-info/dependency_links.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       50 2023-05-27 16:26:58.000000 squander-1.8.4/squander.egg-info/requires.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       20 2023-05-27 16:26:58.000000 squander-1.8.4/squander.egg-info/top_level.txt
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/test_standalone/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1996 2023-05-27 16:24:34.000000 squander-1.8.4/test_standalone/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6325 2023-05-27 16:24:34.000000 squander-1.8.4/test_standalone/custom_gate_structure_test.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4837 2023-05-27 16:24:34.000000 squander-1.8.4/test_standalone/decomposition_test.cpp
```

### Comparing `squander-1.8.3/CMakeLists.txt` & `squander-1.8.4/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cmake_minimum_required(VERSION 3.10.2)
 
 # CMAKE to create the shared library of the quantum gate decomposition project
 
 # set the project name and version
-project(CQGD VERSION 1.8.3)
+project(CQGD VERSION 1.8.4)
 
 # reuse compilation time linking for use runtime linking 
 SET(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
 
 # specify the C++ standard
 set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_STANDARD_REQUIRED True)
```

### Comparing `squander-1.8.3/LICENSE` & `squander-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/PKG-INFO` & `squander-1.8.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squander
-Version: 1.8.3
+Version: 1.8.4
 Summary: Package to decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta
 Maintainer-email: peter.rakyta@ttk.elte.hu
 License: GNU General Public License v3.0
 Keywords: test,cmake,extension
 Classifier: Intended Audience :: Developers
@@ -101,43 +101,15 @@
 
 environment variables are sufficient for successful compilation. 
 When the TBB library is installed via a python package, setting the environment variables above is not necessary.
 The SQUANDER package with C++ Python extensions can be compiled via the Python script **setup.py** located in the root directory of the SQUANDER package.
 The script automatically finds out the CBLAS library working behind the numpy package and uses it in further linking. 
 The **setup.py** script also build the C++ library of the SQUANDER package by making the appropriate CMake calls. 
 
-### Build and Install on Microsoft Windows with Microsoft Visual C++
-
-CMake must be in the path and able to find the MSVC compiler e.g.
-
-$ set PATH=%PATH%;C:\Program Files\cmake\bin
-
-Now set the TBB and BLAS folders and build via:
-
-$ set TBB_LOCATION=<Python_Folder>/LocalCache/local-packages
-
-$ set TBB_INC_DIR=%TBB_LOCATION%/Library/include
-
-$ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib
-
-$ set LIB=<BLAS_Location>/lib;<LAPACK_Location>/lib
 
-$ python setup.py build_ext -DTBB_HEADER=<TBB_Location>\Library\include\
-
-Installation merely requires copying DLL files (if they are not in the path):
-
-$ copy _skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition
-
-$ copy "%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition
-
-$ copy "%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition
-
-Verify the installation:
-
-$ python -m pytest
 
 ### Developer build
 
 
 We recommend to install the SQUANDER package in the Anaconda environment. In order to install the necessary requirements, follow the steps below:
 
 Creating new python environment: 
@@ -193,14 +165,45 @@
 
 $ pip3 install qgd-*.tar.gz
 
 issued from directory **path/to/SQUANDER/package/dist**
 (It is optional to install the ninja package which speeds up the building process by parallel compilation.)
 
 
+### Build and Install on Microsoft Windows with Microsoft Visual C++
+
+CMake must be in the path and able to find the MSVC compiler e.g.
+
+$ set PATH=%PATH%;C:\Program Files\cmake\bin
+
+Now set the TBB and BLAS folders and build via:
+
+$ set TBB_LOCATION=<Python_Folder>/LocalCache/local-packages
+
+$ set TBB_INC_DIR=%TBB_LOCATION%/Library/include
+
+$ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib
+
+$ set LIB=<BLAS_Location>/lib;<LAPACK_Location>/lib
+
+$ python setup.py build_ext -DTBB_HEADER=<TBB_Location>\Library\include\
+
+Installation merely requires copying DLL files (if they are not in the path):
+
+$ copy _skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition
+
+$ copy "%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition
+
+$ copy "%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition
+
+Verify the installation:
+
+$ python -m pytest
+
+
 ### How to use
 
 The algorithm implemented in the SQUANDER package intends to transform the given unitary into an identity matrix via a sequence of two-qubit and one-qubit gate operations applied on the unitary. 
 Thus, in order to get the decomposition of a unitary, one should rather provide the complex transpose of this unitary as the input for the SQUANDER decomposing process, as can be seen in the examples.
 
 
 ## Python Interface
@@ -221,15 +224,15 @@
         config = { 'max_outer_iterations': 1, 
                     'max_inner_iterations_agent': 25000, 
                     'max_inner_iterations_compression': 10000,
                     'max_inner_iterations' : 500,
                     'max_inner_iterations_final': 5000, 		
                     'Randomized_Radius': 0.3, 
                     'randomized_adaptive_layers': 1,
-                    'optimization_tolerance_agent': 1e-4,
+                    'optimization_tolerance_agent': 1e-2,
                     'optimization_tolerance': 1e-8,
                     'agent_num': 10}
  
 Next we initialize the decomposition class with the unitary Umtx to be decomposed. 
 
         # creating a class to decompose the unitary
         from squander import N_Qubit_Decomposition_adaptive
@@ -255,25 +258,26 @@
 We can construct an initial parameters set for the optimization by retrieving the number of free parameters. If the initial parameter set is not set, random parameters are used by default.
 
         # setting intial parameter set
         parameter_num = cDecompose.get_Parameter_Num()
         parameters = np.zeros( (parameter_num,1), dtype=np.float64 )
         cDecompose.set_Optimized_Parameters( parameters )
 
-We can use between several engines to solve the optimization problem. Here we use an evolutionary based algorithm named 'AGENTS'
+We can choose between several engines to solve the optimization problem. Here we use an evolutionary based algorithm named 'AGENTS'
 
         # setting optimizer
         cDecompose.set_Optimizer("AGENTS")
 	
 The optimization process is started by the function call	
 
         # starting the decomposition
         cDecompose.get_Initial_Circuit()
 	
 The optimization process terminates by either reaching the tolerance 'optimization_tolerance_agent' or by reaching the maximal iteration number 'max_inner_iterations_agent', or if the engines identifies a convergence to a local minimum. The SQUANDER framework enables one to continue the optimization using a different engine. In particular we set a second order gradient descend method 'BFGS' 
+In order to achieve the best performance one can play around with the hyper-parameters in the map 'config'. (Optimization strategy AGENTS is good in avoiding local minima or get through flat areas of the optimization landscape. Then a gradient descend method can be used for faster convergence toward a solution.)
 
         # setting optimizer
         cDecompose.set_Optimizer("BFGS")
 
         # continue the decomposition with a second optimizer method
         cDecompose.get_Initial_Circuit()
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: squander Version: 1.8.3 Summary: Package to
+Metadata-Version: 2.1 Name: squander Version: 1.8.4 Summary: Package to
 decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta Maintainer-email: peter.rakyta@ttk.elte.hu License:
 GNU General Public License v3.0 Keywords: test,cmake,extension Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: Programming Language :: C Classifier: Programming Language :: C++
 Description-Content-Type: text/markdown License-File: LICENSE [![DOI](https://
@@ -84,31 +84,20 @@
 TBB_INC_DIR=path/to/TBB/include environment variables are sufficient for
 successful compilation. When the TBB library is installed via a python package,
 setting the environment variables above is not necessary. The SQUANDER package
 with C++ Python extensions can be compiled via the Python script **setup.py**
 located in the root directory of the SQUANDER package. The script automatically
 finds out the CBLAS library working behind the numpy package and uses it in
 further linking. The **setup.py** script also build the C++ library of the
-SQUANDER package by making the appropriate CMake calls. ### Build and Install
-on Microsoft Windows with Microsoft Visual C++ CMake must be in the path and
-able to find the MSVC compiler e.g. $ set PATH=%PATH%;C:\Program
-Files\cmake\bin Now set the TBB and BLAS folders and build via: $ set
-TBB_LOCATION=/LocalCache/local-packages $ set TBB_INC_DIR=%TBB_LOCATION%/
-Library/include $ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib $ set LIB=/lib;/
-lib $ python setup.py build_ext -DTBB_HEADER=\Library\include\ Installation
-merely requires copying DLL files (if they are not in the path): $ copy
-_skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition $ copy
-"%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition $ copy
-"%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition Verify
-the installation: $ python -m pytest ### Developer build We recommend to
-install the SQUANDER package in the Anaconda environment. In order to install
-the necessary requirements, follow the steps below: Creating new python
-environment: $ conda create -n qgd Activate the new anaconda environment $
-conda activate qgd Install dependencies: $ conda install numpy scipy pip pytest
-scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
+SQUANDER package by making the appropriate CMake calls. ### Developer build We
+recommend to install the SQUANDER package in the Anaconda environment. In order
+to install the necessary requirements, follow the steps below: Creating new
+python environment: $ conda create -n qgd Activate the new anaconda environment
+$ conda activate qgd Install dependencies: $ conda install numpy scipy pip
+pytest scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
 environment variables are set and the dependencies are installed, the
 compilation of the package can be started by the Python command: $ python3
 setup.py build_ext The command above starts the compilation of the SQUANDER C++
 library and builds the necessary C++ Python interface extensions of the
 SQUANDER package in place. After a successful build, one can register the
 SQUANDER package in the Python distribution in developer (i.e. editable) mode
 by command: $ python -m pip install -e . ### Binary distribution After the
@@ -128,35 +117,46 @@
 necessary to set the environment variables, since this script only collects the
 necessary files and pack them into a tar ball located in the directory **path/
 to/SQUANDER/package/dist**. In order to install the SQUANDER package from
 source tar ball, see the previous section discussing the initialization of the
 environment variables. The package can be compiled and installed by the command
 $ pip3 install qgd-*.tar.gz issued from directory **path/to/SQUANDER/package/
 dist** (It is optional to install the ninja package which speeds up the
-building process by parallel compilation.) ### How to use The algorithm
-implemented in the SQUANDER package intends to transform the given unitary into
-an identity matrix via a sequence of two-qubit and one-qubit gate operations
-applied on the unitary. Thus, in order to get the decomposition of a unitary,
-one should rather provide the complex transpose of this unitary as the input
-for the SQUANDER decomposing process, as can be seen in the examples. ## Python
+building process by parallel compilation.) ### Build and Install on Microsoft
+Windows with Microsoft Visual C++ CMake must be in the path and able to find
+the MSVC compiler e.g. $ set PATH=%PATH%;C:\Program Files\cmake\bin Now set the
+TBB and BLAS folders and build via: $ set TBB_LOCATION=/LocalCache/local-
+packages $ set TBB_INC_DIR=%TBB_LOCATION%/Library/include $ set
+TBB_LIB_DIR=%TBB_LOCATION%/Library/lib $ set LIB=/lib;/lib $ python setup.py
+build_ext -DTBB_HEADER=\Library\include\ Installation merely requires copying
+DLL files (if they are not in the path): $ copy _skbuild\win-amd64-3.9\cmake-
+install\bin .\qgd_python\decomposition $ copy
+"%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition $ copy
+"%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition Verify
+the installation: $ python -m pytest ### How to use The algorithm implemented
+in the SQUANDER package intends to transform the given unitary into an identity
+matrix via a sequence of two-qubit and one-qubit gate operations applied on the
+unitary. Thus, in order to get the decomposition of a unitary, one should
+rather provide the complex transpose of this unitary as the input for the
+SQUANDER decomposing process, as can be seen in the examples. ## Python
 Interface The SQUANDER package contains a Python interface allowing the access
 of the functionalities of the SQUANDER package from Python. The usage of the
 SQUANDER Python interface is demonstrated in the example files in the directory
 **examples** located in the directory **path/to/SQUANDER/package**, or in test
 files located in sub-directories of **path/to/SQUANDER/package/qgd_python/*/
 test**. ### Example code snippet Here we provide an example to use the SQUANDER
 package. The following python interface is accessible from version 1.8.0. In
 this example we use two optimization engines for the decomposition: 1. An
 evolutionary engine called AGENTS 2. Second order gradient descend algorithm
 (BFGS) Firstly we construct a Python map to set hyper-parameters during the
 gate synthesis. #Python map containing hyper-parameters config =
 { 'max_outer_iterations': 1, 'max_inner_iterations_agent': 25000,
 'max_inner_iterations_compression': 10000, 'max_inner_iterations' : 500,
 'max_inner_iterations_final': 5000, 'Randomized_Radius': 0.3,
-'randomized_adaptive_layers': 1, 'optimization_tolerance_agent': 1e-4,
+'randomized_adaptive_layers': 1, 'optimization_tolerance_agent': 1e-2,
 'optimization_tolerance': 1e-8, 'agent_num': 10} Next we initialize the
 decomposition class with the unitary Umtx to be decomposed. # creating a class
 to decompose the unitary from squander import N_Qubit_Decomposition_adaptive
 cDecompose = N_Qubit_Decomposition_adaptive( Umtx.conj().T, config=config ) The
 verbosity of the execution output can be controlled by the function call #
 setting the verbosity of the decomposition cDecompose.set_Verbose( 3 ) We
 construct the initial trial gate structure for the optimization consisting of 2
@@ -165,36 +165,40 @@
 layers to the gate structure levels = 2 for idx in range(levels):
 cDecompose.add_Adaptive_Layers()
 cDecompose.add_Finalyzing_Layer_To_Gate_Structure() We can construct an initial
 parameters set for the optimization by retrieving the number of free
 parameters. If the initial parameter set is not set, random parameters are used
 by default. # setting intial parameter set parameter_num =
 cDecompose.get_Parameter_Num() parameters = np.zeros( (parameter_num,1),
-dtype=np.float64 ) cDecompose.set_Optimized_Parameters( parameters ) We can use
-between several engines to solve the optimization problem. Here we use an
-evolutionary based algorithm named 'AGENTS' # setting optimizer
+dtype=np.float64 ) cDecompose.set_Optimized_Parameters( parameters ) We can
+choose between several engines to solve the optimization problem. Here we use
+an evolutionary based algorithm named 'AGENTS' # setting optimizer
 cDecompose.set_Optimizer("AGENTS") The optimization process is started by the
 function call # starting the decomposition cDecompose.get_Initial_Circuit() The
 optimization process terminates by either reaching the tolerance
 'optimization_tolerance_agent' or by reaching the maximal iteration number
 'max_inner_iterations_agent', or if the engines identifies a convergence to a
 local minimum. The SQUANDER framework enables one to continue the optimization
 using a different engine. In particular we set a second order gradient descend
-method 'BFGS' # setting optimizer cDecompose.set_Optimizer("BFGS") # continue
-the decomposition with a second optimizer method cDecompose.get_Initial_Circuit
-() After solving the optimization problem for the initial gate structure, we
-can initiate gate compression iterations. (This step can be omited.) # starting
-compression iterations cDecompose.Compress_Circuit() By finalizing the gate
-structure we replace the CRY gates with CNOT gates. (CRY gates with small
-rotation angle are approximately expressed with a single CNOT gate, so further
-optimization process needs to be initiated.) # finalize the gate structure
-(replace CRY gates with CNOT gates) cDecompose.Finalize_Circuit() Finally, we
-can retrieve the decomposed quantum circuit in QISKIT format. # get the
-decomposing operations quantum_circuit = cDecompose.get_Quantum_Circuit() ###
-How to cite us If you have found our work useful for your research project,
-please cite us by [1] PÃ©ter Rakyta, ZoltÃ¡n ZimborÃ¡s, Approaching the
-theoretical limit in quantum gate decomposition, Quantum 6, 710 (2022).
+method 'BFGS' In order to achieve the best performance one can play around with
+the hyper-parameters in the map 'config'. (Optimization strategy AGENTS is good
+in avoiding local minima or get through flat areas of the optimization
+landscape. Then a gradient descend method can be used for faster convergence
+toward a solution.) # setting optimizer cDecompose.set_Optimizer("BFGS") #
+continue the decomposition with a second optimizer method
+cDecompose.get_Initial_Circuit() After solving the optimization problem for the
+initial gate structure, we can initiate gate compression iterations. (This step
+can be omited.) # starting compression iterations cDecompose.Compress_Circuit()
+By finalizing the gate structure we replace the CRY gates with CNOT gates. (CRY
+gates with small rotation angle are approximately expressed with a single CNOT
+gate, so further optimization process needs to be initiated.) # finalize the
+gate structure (replace CRY gates with CNOT gates) cDecompose.Finalize_Circuit
+() Finally, we can retrieve the decomposed quantum circuit in QISKIT format. #
+get the decomposing operations quantum_circuit = cDecompose.get_Quantum_Circuit
+() ### How to cite us If you have found our work useful for your research
+project, please cite us by [1] PÃ©ter Rakyta, ZoltÃ¡n ZimborÃ¡s, Approaching
+the theoretical limit in quantum gate decomposition, Quantum 6, 710 (2022).
 [2] PÃ©ter Rakyta, ZoltÃ¡n ZimborÃ¡s, Efficient quantum gate decomposition via
 adaptive circuit compression, arXiv:2203.04426.
 [3] Peter Rakyta, Gregory Morse, Jakab NÃ¡dori, Zita Majnay-TakÃ¡cs, Oskar
 Mencer, ZoltÃ¡n ZimborÃ¡s, Highly optimized quantum circuits synthesized via
 data-flow engines, arXiv:2211.07685
```

### Comparing `squander-1.8.3/README.md` & `squander-1.8.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,43 +85,15 @@
 
 environment variables are sufficient for successful compilation. 
 When the TBB library is installed via a python package, setting the environment variables above is not necessary.
 The SQUANDER package with C++ Python extensions can be compiled via the Python script **setup.py** located in the root directory of the SQUANDER package.
 The script automatically finds out the CBLAS library working behind the numpy package and uses it in further linking. 
 The **setup.py** script also build the C++ library of the SQUANDER package by making the appropriate CMake calls. 
 
-### Build and Install on Microsoft Windows with Microsoft Visual C++
-
-CMake must be in the path and able to find the MSVC compiler e.g.
-
-$ set PATH=%PATH%;C:\Program Files\cmake\bin
-
-Now set the TBB and BLAS folders and build via:
-
-$ set TBB_LOCATION=<Python_Folder>/LocalCache/local-packages
-
-$ set TBB_INC_DIR=%TBB_LOCATION%/Library/include
-
-$ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib
-
-$ set LIB=<BLAS_Location>/lib;<LAPACK_Location>/lib
 
-$ python setup.py build_ext -DTBB_HEADER=<TBB_Location>\Library\include\
-
-Installation merely requires copying DLL files (if they are not in the path):
-
-$ copy _skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition
-
-$ copy "%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition
-
-$ copy "%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition
-
-Verify the installation:
-
-$ python -m pytest
 
 ### Developer build
 
 
 We recommend to install the SQUANDER package in the Anaconda environment. In order to install the necessary requirements, follow the steps below:
 
 Creating new python environment: 
@@ -177,14 +149,45 @@
 
 $ pip3 install qgd-*.tar.gz
 
 issued from directory **path/to/SQUANDER/package/dist**
 (It is optional to install the ninja package which speeds up the building process by parallel compilation.)
 
 
+### Build and Install on Microsoft Windows with Microsoft Visual C++
+
+CMake must be in the path and able to find the MSVC compiler e.g.
+
+$ set PATH=%PATH%;C:\Program Files\cmake\bin
+
+Now set the TBB and BLAS folders and build via:
+
+$ set TBB_LOCATION=<Python_Folder>/LocalCache/local-packages
+
+$ set TBB_INC_DIR=%TBB_LOCATION%/Library/include
+
+$ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib
+
+$ set LIB=<BLAS_Location>/lib;<LAPACK_Location>/lib
+
+$ python setup.py build_ext -DTBB_HEADER=<TBB_Location>\Library\include\
+
+Installation merely requires copying DLL files (if they are not in the path):
+
+$ copy _skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition
+
+$ copy "%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition
+
+$ copy "%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition
+
+Verify the installation:
+
+$ python -m pytest
+
+
 ### How to use
 
 The algorithm implemented in the SQUANDER package intends to transform the given unitary into an identity matrix via a sequence of two-qubit and one-qubit gate operations applied on the unitary. 
 Thus, in order to get the decomposition of a unitary, one should rather provide the complex transpose of this unitary as the input for the SQUANDER decomposing process, as can be seen in the examples.
 
 
 ## Python Interface
@@ -205,15 +208,15 @@
         config = { 'max_outer_iterations': 1, 
                     'max_inner_iterations_agent': 25000, 
                     'max_inner_iterations_compression': 10000,
                     'max_inner_iterations' : 500,
                     'max_inner_iterations_final': 5000, 		
                     'Randomized_Radius': 0.3, 
                     'randomized_adaptive_layers': 1,
-                    'optimization_tolerance_agent': 1e-4,
+                    'optimization_tolerance_agent': 1e-2,
                     'optimization_tolerance': 1e-8,
                     'agent_num': 10}
  
 Next we initialize the decomposition class with the unitary Umtx to be decomposed. 
 
         # creating a class to decompose the unitary
         from squander import N_Qubit_Decomposition_adaptive
@@ -239,25 +242,26 @@
 We can construct an initial parameters set for the optimization by retrieving the number of free parameters. If the initial parameter set is not set, random parameters are used by default.
 
         # setting intial parameter set
         parameter_num = cDecompose.get_Parameter_Num()
         parameters = np.zeros( (parameter_num,1), dtype=np.float64 )
         cDecompose.set_Optimized_Parameters( parameters )
 
-We can use between several engines to solve the optimization problem. Here we use an evolutionary based algorithm named 'AGENTS'
+We can choose between several engines to solve the optimization problem. Here we use an evolutionary based algorithm named 'AGENTS'
 
         # setting optimizer
         cDecompose.set_Optimizer("AGENTS")
 	
 The optimization process is started by the function call	
 
         # starting the decomposition
         cDecompose.get_Initial_Circuit()
 	
 The optimization process terminates by either reaching the tolerance 'optimization_tolerance_agent' or by reaching the maximal iteration number 'max_inner_iterations_agent', or if the engines identifies a convergence to a local minimum. The SQUANDER framework enables one to continue the optimization using a different engine. In particular we set a second order gradient descend method 'BFGS' 
+In order to achieve the best performance one can play around with the hyper-parameters in the map 'config'. (Optimization strategy AGENTS is good in avoiding local minima or get through flat areas of the optimization landscape. Then a gradient descend method can be used for faster convergence toward a solution.)
 
         # setting optimizer
         cDecompose.set_Optimizer("BFGS")
 
         # continue the decomposition with a second optimizer method
         cDecompose.get_Initial_Circuit()
```

#### html2text {}

```diff
@@ -76,31 +76,20 @@
 TBB_INC_DIR=path/to/TBB/include environment variables are sufficient for
 successful compilation. When the TBB library is installed via a python package,
 setting the environment variables above is not necessary. The SQUANDER package
 with C++ Python extensions can be compiled via the Python script **setup.py**
 located in the root directory of the SQUANDER package. The script automatically
 finds out the CBLAS library working behind the numpy package and uses it in
 further linking. The **setup.py** script also build the C++ library of the
-SQUANDER package by making the appropriate CMake calls. ### Build and Install
-on Microsoft Windows with Microsoft Visual C++ CMake must be in the path and
-able to find the MSVC compiler e.g. $ set PATH=%PATH%;C:\Program
-Files\cmake\bin Now set the TBB and BLAS folders and build via: $ set
-TBB_LOCATION=/LocalCache/local-packages $ set TBB_INC_DIR=%TBB_LOCATION%/
-Library/include $ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib $ set LIB=/lib;/
-lib $ python setup.py build_ext -DTBB_HEADER=\Library\include\ Installation
-merely requires copying DLL files (if they are not in the path): $ copy
-_skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition $ copy
-"%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition $ copy
-"%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition Verify
-the installation: $ python -m pytest ### Developer build We recommend to
-install the SQUANDER package in the Anaconda environment. In order to install
-the necessary requirements, follow the steps below: Creating new python
-environment: $ conda create -n qgd Activate the new anaconda environment $
-conda activate qgd Install dependencies: $ conda install numpy scipy pip pytest
-scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
+SQUANDER package by making the appropriate CMake calls. ### Developer build We
+recommend to install the SQUANDER package in the Anaconda environment. In order
+to install the necessary requirements, follow the steps below: Creating new
+python environment: $ conda create -n qgd Activate the new anaconda environment
+$ conda activate qgd Install dependencies: $ conda install numpy scipy pip
+pytest scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
 environment variables are set and the dependencies are installed, the
 compilation of the package can be started by the Python command: $ python3
 setup.py build_ext The command above starts the compilation of the SQUANDER C++
 library and builds the necessary C++ Python interface extensions of the
 SQUANDER package in place. After a successful build, one can register the
 SQUANDER package in the Python distribution in developer (i.e. editable) mode
 by command: $ python -m pip install -e . ### Binary distribution After the
@@ -120,35 +109,46 @@
 necessary to set the environment variables, since this script only collects the
 necessary files and pack them into a tar ball located in the directory **path/
 to/SQUANDER/package/dist**. In order to install the SQUANDER package from
 source tar ball, see the previous section discussing the initialization of the
 environment variables. The package can be compiled and installed by the command
 $ pip3 install qgd-*.tar.gz issued from directory **path/to/SQUANDER/package/
 dist** (It is optional to install the ninja package which speeds up the
-building process by parallel compilation.) ### How to use The algorithm
-implemented in the SQUANDER package intends to transform the given unitary into
-an identity matrix via a sequence of two-qubit and one-qubit gate operations
-applied on the unitary. Thus, in order to get the decomposition of a unitary,
-one should rather provide the complex transpose of this unitary as the input
-for the SQUANDER decomposing process, as can be seen in the examples. ## Python
+building process by parallel compilation.) ### Build and Install on Microsoft
+Windows with Microsoft Visual C++ CMake must be in the path and able to find
+the MSVC compiler e.g. $ set PATH=%PATH%;C:\Program Files\cmake\bin Now set the
+TBB and BLAS folders and build via: $ set TBB_LOCATION=/LocalCache/local-
+packages $ set TBB_INC_DIR=%TBB_LOCATION%/Library/include $ set
+TBB_LIB_DIR=%TBB_LOCATION%/Library/lib $ set LIB=/lib;/lib $ python setup.py
+build_ext -DTBB_HEADER=\Library\include\ Installation merely requires copying
+DLL files (if they are not in the path): $ copy _skbuild\win-amd64-3.9\cmake-
+install\bin .\qgd_python\decomposition $ copy
+"%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition $ copy
+"%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition Verify
+the installation: $ python -m pytest ### How to use The algorithm implemented
+in the SQUANDER package intends to transform the given unitary into an identity
+matrix via a sequence of two-qubit and one-qubit gate operations applied on the
+unitary. Thus, in order to get the decomposition of a unitary, one should
+rather provide the complex transpose of this unitary as the input for the
+SQUANDER decomposing process, as can be seen in the examples. ## Python
 Interface The SQUANDER package contains a Python interface allowing the access
 of the functionalities of the SQUANDER package from Python. The usage of the
 SQUANDER Python interface is demonstrated in the example files in the directory
 **examples** located in the directory **path/to/SQUANDER/package**, or in test
 files located in sub-directories of **path/to/SQUANDER/package/qgd_python/*/
 test**. ### Example code snippet Here we provide an example to use the SQUANDER
 package. The following python interface is accessible from version 1.8.0. In
 this example we use two optimization engines for the decomposition: 1. An
 evolutionary engine called AGENTS 2. Second order gradient descend algorithm
 (BFGS) Firstly we construct a Python map to set hyper-parameters during the
 gate synthesis. #Python map containing hyper-parameters config =
 { 'max_outer_iterations': 1, 'max_inner_iterations_agent': 25000,
 'max_inner_iterations_compression': 10000, 'max_inner_iterations' : 500,
 'max_inner_iterations_final': 5000, 'Randomized_Radius': 0.3,
-'randomized_adaptive_layers': 1, 'optimization_tolerance_agent': 1e-4,
+'randomized_adaptive_layers': 1, 'optimization_tolerance_agent': 1e-2,
 'optimization_tolerance': 1e-8, 'agent_num': 10} Next we initialize the
 decomposition class with the unitary Umtx to be decomposed. # creating a class
 to decompose the unitary from squander import N_Qubit_Decomposition_adaptive
 cDecompose = N_Qubit_Decomposition_adaptive( Umtx.conj().T, config=config ) The
 verbosity of the execution output can be controlled by the function call #
 setting the verbosity of the decomposition cDecompose.set_Verbose( 3 ) We
 construct the initial trial gate structure for the optimization consisting of 2
@@ -157,36 +157,40 @@
 layers to the gate structure levels = 2 for idx in range(levels):
 cDecompose.add_Adaptive_Layers()
 cDecompose.add_Finalyzing_Layer_To_Gate_Structure() We can construct an initial
 parameters set for the optimization by retrieving the number of free
 parameters. If the initial parameter set is not set, random parameters are used
 by default. # setting intial parameter set parameter_num =
 cDecompose.get_Parameter_Num() parameters = np.zeros( (parameter_num,1),
-dtype=np.float64 ) cDecompose.set_Optimized_Parameters( parameters ) We can use
-between several engines to solve the optimization problem. Here we use an
-evolutionary based algorithm named 'AGENTS' # setting optimizer
+dtype=np.float64 ) cDecompose.set_Optimized_Parameters( parameters ) We can
+choose between several engines to solve the optimization problem. Here we use
+an evolutionary based algorithm named 'AGENTS' # setting optimizer
 cDecompose.set_Optimizer("AGENTS") The optimization process is started by the
 function call # starting the decomposition cDecompose.get_Initial_Circuit() The
 optimization process terminates by either reaching the tolerance
 'optimization_tolerance_agent' or by reaching the maximal iteration number
 'max_inner_iterations_agent', or if the engines identifies a convergence to a
 local minimum. The SQUANDER framework enables one to continue the optimization
 using a different engine. In particular we set a second order gradient descend
-method 'BFGS' # setting optimizer cDecompose.set_Optimizer("BFGS") # continue
-the decomposition with a second optimizer method cDecompose.get_Initial_Circuit
-() After solving the optimization problem for the initial gate structure, we
-can initiate gate compression iterations. (This step can be omited.) # starting
-compression iterations cDecompose.Compress_Circuit() By finalizing the gate
-structure we replace the CRY gates with CNOT gates. (CRY gates with small
-rotation angle are approximately expressed with a single CNOT gate, so further
-optimization process needs to be initiated.) # finalize the gate structure
-(replace CRY gates with CNOT gates) cDecompose.Finalize_Circuit() Finally, we
-can retrieve the decomposed quantum circuit in QISKIT format. # get the
-decomposing operations quantum_circuit = cDecompose.get_Quantum_Circuit() ###
-How to cite us If you have found our work useful for your research project,
-please cite us by [1] PÃ©ter Rakyta, ZoltÃ¡n ZimborÃ¡s, Approaching the
-theoretical limit in quantum gate decomposition, Quantum 6, 710 (2022).
+method 'BFGS' In order to achieve the best performance one can play around with
+the hyper-parameters in the map 'config'. (Optimization strategy AGENTS is good
+in avoiding local minima or get through flat areas of the optimization
+landscape. Then a gradient descend method can be used for faster convergence
+toward a solution.) # setting optimizer cDecompose.set_Optimizer("BFGS") #
+continue the decomposition with a second optimizer method
+cDecompose.get_Initial_Circuit() After solving the optimization problem for the
+initial gate structure, we can initiate gate compression iterations. (This step
+can be omited.) # starting compression iterations cDecompose.Compress_Circuit()
+By finalizing the gate structure we replace the CRY gates with CNOT gates. (CRY
+gates with small rotation angle are approximately expressed with a single CNOT
+gate, so further optimization process needs to be initiated.) # finalize the
+gate structure (replace CRY gates with CNOT gates) cDecompose.Finalize_Circuit
+() Finally, we can retrieve the decomposed quantum circuit in QISKIT format. #
+get the decomposing operations quantum_circuit = cDecompose.get_Quantum_Circuit
+() ### How to cite us If you have found our work useful for your research
+project, please cite us by [1] PÃ©ter Rakyta, ZoltÃ¡n ZimborÃ¡s, Approaching
+the theoretical limit in quantum gate decomposition, Quantum 6, 710 (2022).
 [2] PÃ©ter Rakyta, ZoltÃ¡n ZimborÃ¡s, Efficient quantum gate decomposition via
 adaptive circuit compression, arXiv:2203.04426.
 [3] Peter Rakyta, Gregory Morse, Jakab NÃ¡dori, Zita Majnay-TakÃ¡cs, Oskar
 Mencer, ZoltÃ¡n ZimborÃ¡s, Highly optimized quantum circuits synthesized via
 data-flow engines, arXiv:2211.07685
```

### Comparing `squander-1.8.3/cmake/check_AVX.cmake` & `squander-1.8.4/cmake/check_AVX.cmake`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/Adam.cpp` & `squander-1.8.4/common/Adam.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/common.cpp` & `squander-1.8.4/common/common.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/common_DFE.cpp` & `squander-1.8.4/common/common_DFE.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/config_element.cpp` & `squander-1.8.4/common/config_element.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/dot.cpp` & `squander-1.8.4/common/dot.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/Adam.h` & `squander-1.8.4/common/include/Adam.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/QGDTypes.h` & `squander-1.8.4/common/include/QGDTypes.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/common.h` & `squander-1.8.4/common/include/common.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/common_DFE.h` & `squander-1.8.4/common/include/common_DFE.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/config_element.h` & `squander-1.8.4/common/include/config_element.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/dot.h` & `squander-1.8.4/common/include/dot.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/lbfgs.h` & `squander-1.8.4/common/include/lbfgs.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/logging.h` & `squander-1.8.4/common/include/logging.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/matrix.h` & `squander-1.8.4/common/include/matrix.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/matrix_base.h` & `squander-1.8.4/common/include/matrix_base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/matrix_real.h` & `squander-1.8.4/common/include/matrix_real.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/mpi_base.h` & `squander-1.8.4/common/include/mpi_base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/numpy_interface.h` & `squander-1.8.4/common/include/numpy_interface.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/include/tolmin.h` & `squander-1.8.4/common/include/tolmin.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/lbfgs.cpp` & `squander-1.8.4/common/lbfgs.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/logging.cpp` & `squander-1.8.4/common/logging.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/matrix.cpp` & `squander-1.8.4/common/matrix.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/matrix_real.cpp` & `squander-1.8.4/common/matrix_real.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/mpi_base.cpp` & `squander-1.8.4/common/mpi_base.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/numpy_interface.cpp` & `squander-1.8.4/common/numpy_interface.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/common/tolmin.cpp` & `squander-1.8.4/common/tolmin.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/Decomposition_Base.cpp` & `squander-1.8.4/decomposition/Decomposition_Base.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/N_Qubit_Decomposition.cpp` & `squander-1.8.4/decomposition/N_Qubit_Decomposition.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/N_Qubit_Decomposition_Base.cpp` & `squander-1.8.4/decomposition/N_Qubit_Decomposition_Base.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,53 @@
 static double DFE_time = 0.0;
 static double CPU_time = 0.0;
 
 
 extern "C" int LAPACKE_dgesv( 	int  matrix_layout, int n, int nrhs, double *a, int lda, int *ipiv, double *b, int ldb); 	
 
 
+
+/**
+@brief ???????????????
+@return ???????????
+*/
+double HS_partial_optimization_problem( Matrix_real parameters, void* void_params) {
+
+    double* params = (double*)void_params;
+
+    return params[0]*sin(2*parameters[0] + params[1]) + params[2]*sin(parameters[0] + params[3] ) + params[4];
+}
+
+
+/**
+@brief ???????????????
+@return ???????????
+*/
+void HS_partial_optimization_problem_grad( Matrix_real parameters, void* void_params, Matrix_real& grad) {
+
+
+    double* params = (double*)void_params;
+    grad[0] = 2*params[0]*cos(2*parameters[0] + params[1]) + params[2]*cos(parameters[0] + params[3] );
+
+}
+
+
+/**
+@brief ???????????????
+@return ???????????
+*/
+void HS_partial_optimization_problem_combined( Matrix_real parameters, void* void_params, double* f0, Matrix_real& grad) {
+
+    *f0 = HS_partial_optimization_problem( parameters, void_params );
+    HS_partial_optimization_problem_grad( parameters, void_params, grad);
+
+
+}
+
+
 /**
 @brief Nullary constructor of the class.
 @return An instance of the class
 */
 N_Qubit_Decomposition_Base::N_Qubit_Decomposition_Base() {
 
     // logical value. Set true if finding the minimum number of gate layers is required (default), or false when the maximal number of two-qubit gates is used (ideal for general unitaries).
@@ -376,14 +415,21 @@
 /**
 @brief Call to solve layer by layer the optimization problem via the COSINE algorithm. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
 @param solution_guess Array containing the solution guess.
 */
 void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_COSINE( int num_of_parameters, Matrix_real& solution_guess) {
 
+
+        if ( cost_fnc != FROBENIUS_NORM ) {
+            std::string err("N_Qubit_Decomposition_Base::solve_layer_optimization_problem_COSINE: Only cost function 0 is implemented");
+            throw err;
+        }
+
+
 #ifdef __DFE__
         if ( qbit_num >= 5 && get_accelerator_num() > 0 ) {
             upload_Umtx_to_DFE();
         }
 #endif
 
 
@@ -426,45 +472,60 @@
         
 
         // the array storing the optimized parameters
         Matrix_real solution_guess_tmp_mtx = Matrix_real( num_of_parameters, 1 );
         memcpy(solution_guess_tmp_mtx.get_data(), optimized_parameters_mtx.get_data(), num_of_parameters*sizeof(double) );
 
         int agent_num;
-        if ( config.count("agent_num") > 0 ) { 
+        if ( config.count("agent_num_cosine") > 0 ) { 
+             long long value;                   
+             config["agent_num_cosine"].get_property( value );  
+             agent_num = (int) value;
+        }
+        else if ( config.count("agent_num") > 0 ) { 
              long long value;                   
              config["agent_num"].get_property( value );  
              agent_num = (int) value;
         }
         else {
             agent_num = 64;
         }
 
 
         long long max_inner_iterations_loc;
-        if ( config.count("max_inner_iterations") > 0 ) {
+        if ( config.count("max_inner_iterations_cosine") > 0 ) {
+             config["max_inner_iterations_cosine"].get_property( max_inner_iterations_loc );  
+        }
+        else if ( config.count("max_inner_iterations") > 0 ) {
              config["max_inner_iterations"].get_property( max_inner_iterations_loc );  
         }
         else {
             max_inner_iterations_loc = max_inner_iterations;
         }
         
         
         long long export_circuit_2_binary_loc;
-        if ( config.count("export_circuit_2_binary") > 0 ) {
+        if ( config.count("export_circuit_2_binary_cosine") > 0 ) {
+             config["export_circuit_2_binary_cosine"].get_property( export_circuit_2_binary_loc );  
+        }
+        else if ( config.count("export_circuit_2_binary") > 0 ) {
              config["export_circuit_2_binary"].get_property( export_circuit_2_binary_loc );  
         }
         else {
             export_circuit_2_binary_loc = 0;
         }        
 
 
         double optimization_tolerance_loc;
-        if ( config.count("optimization_tolerance") > 0 ) {
-             config["optimization_tolerance"].get_property( optimization_tolerance_loc );  
+        if ( config.count("optimization_tolerance_cosine") > 0 ) {
+             config["optimization_tolerance_cosine"].get_property( optimization_tolerance_loc );  
+        }
+        else if ( config.count("optimization_tolerance") > 0 ) {
+             double value;
+             config["optimization_tolerance"].get_property( optimization_tolerance_loc );
         }
         else {
             optimization_tolerance_loc = optimization_tolerance;
         }
 
 
 
@@ -744,27 +805,34 @@
 @brief Call to solve layer by layer the optimization problem via the AGENT algorithm. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
 @param solution_guess Array containing the solution guess.
 */
 void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_AGENTS( int num_of_parameters, Matrix_real& solution_guess) {
 
 
+
+        if ( (cost_fnc != FROBENIUS_NORM) && (cost_fnc != HILBERT_SCHMIDT_TEST) ) {
+            std::string err("N_Qubit_Decomposition_Base::solve_layer_optimization_problem_AGENTS: Only cost functions 0 and 3 are implemented");
+            throw err;
+        }
+
 #ifdef __DFE__
         if ( qbit_num >= 5 && get_accelerator_num() > 0 ) {
             upload_Umtx_to_DFE();
         }
 #endif
 
 
 
         if (gates.size() == 0 ) {
             return;
         }
 
 
+        double M_PI_quarter = M_PI/4;
         double M_PI_half = M_PI/2;
         double M_PI_double = M_PI*2;
 
         if (solution_guess.size() == 0 ) {
             solution_guess = Matrix_real(num_of_parameters,1);
             std::uniform_real_distribution<> distrib_real(0, M_PI_double); 
             for ( int idx=0; idx<num_of_parameters; idx++) {
@@ -804,39 +872,57 @@
 
         int max_inner_iterations_loc;
         if ( config.count("max_inner_iterations_agent") > 0 ) {
              long long value;
              config["max_inner_iterations_agent"].get_property( value );
              max_inner_iterations_loc = (int) value;
         }
+        else if ( config.count("max_inner_iterations") > 0 ) {
+             long long value;
+             config["max_inner_iterations"].get_property( value );
+             max_inner_iterations_loc = (int) value;
+        }
         else {
             max_inner_iterations_loc = max_inner_iterations;
         }
 
 
         double optimization_tolerance_loc;
         if ( config.count("optimization_tolerance_agent") > 0 ) {
              double value;
              config["optimization_tolerance_agent"].get_property( optimization_tolerance_loc );
         }
+        else if ( config.count("optimization_tolerance") > 0 ) {
+             double value;
+             config["optimization_tolerance"].get_property( optimization_tolerance_loc );
+        }
         else {
             optimization_tolerance_loc = optimization_tolerance;
         }
+
         
         long long export_circuit_2_binary_loc;
-        if ( config.count("export_circuit_2_binary") > 0 ) {
+        if ( config.count("export_circuit_2_binary_agent") > 0 ) {
+             config["export_circuit_2_binary_agent"].get_property( export_circuit_2_binary_loc );  
+        }
+        else if ( config.count("export_circuit_2_binary") > 0 ) {
              config["export_circuit_2_binary"].get_property( export_circuit_2_binary_loc );  
         }
         else {
             export_circuit_2_binary_loc = 0;
         }            
 
         
         int agent_lifetime_loc;
-        if ( config.count("agent_lifetime") > 0 ) {
+        if ( config.count("agent_lifetime_agent") > 0 ) {
+             long long agent_lifetime_loc_tmp;
+             config["agent_lifetime_agent"].get_property( agent_lifetime_loc_tmp );  
+             agent_lifetime_loc = (int)agent_lifetime_loc_tmp;
+        }
+        else if ( config.count("agent_lifetime") > 0 ) {
              long long agent_lifetime_loc_tmp;
              config["agent_lifetime"].get_property( agent_lifetime_loc_tmp );  
              agent_lifetime_loc = (int)agent_lifetime_loc_tmp;
         }
         else {
             agent_lifetime_loc = 1000;
         }        
@@ -847,26 +933,34 @@
         sstream << "max_inner_iterations: " << max_inner_iterations_loc << std::endl;
         sstream << "agent_lifetime_loc: " << agent_lifetime_loc << std::endl;
         print(sstream, 2); 
 
         double agent_randomization_rate = 0.2;
         
         int agent_num;
-        if ( config.count("agent_num") > 0 ) { 
+        if ( config.count("agent_num_agent") > 0 ) { 
+             long long value;                   
+             config["agent_num_agent"].get_property( value );  
+             agent_num = (int) value;
+        }
+        else if ( config.count("agent_num") > 0 ) { 
              long long value;                   
              config["agent_num"].get_property( value );  
              agent_num = (int) value;
         }
         else {
             agent_num = 64;
         }
 
 
         double agent_exploration_rate = 0.2;
-        if ( config.count("agent_exploration_rate") > 0 ) {
+        if ( config.count("agent_exploration_rate_agent") > 0 ) {
+             config["agent_exploration_rate_agent"].get_property( agent_exploration_rate );
+        }
+        else if ( config.count("agent_exploration_rate") > 0 ) {
              config["agent_exploration_rate"].get_property( agent_exploration_rate );
         }
         
         sstream.str("");
         sstream << "AGENTS: number of agents " << agent_num << std::endl;
         sstream << "AGENTS: exploration_rate " << agent_exploration_rate << std::endl;
         sstream << "AGENTS: lifetime " << agent_lifetime_loc << std::endl;
@@ -950,16 +1044,18 @@
         current_minimum_agents = optimization_problem_batched( solution_guess_mtx_agents );
 
 
         // arrays to store some parameter values needed to be restored later
         Matrix_real parameter_value_save_agents( agent_num, 1 );    
        
         // arrays to store the cost functions at shifted parameters
-        Matrix_real f0_shifted_pi2_agents( agent_num, 1 );
-        Matrix_real f0_shifted_pi_agents( agent_num, 1 );                 
+        Matrix_real f0_shifted_pi2_agents;
+        Matrix_real f0_shifted_pi_agents;                 
+        Matrix_real f0_shifted_pi4_agents;    
+        Matrix_real f0_shifted_3pi2_agents;           
        
 
 
    
         // CPU time
         CPU_time += (tbb::tick_count::now() - t0_CPU).seconds();       
        
@@ -997,79 +1093,229 @@
 #ifdef __MPI__  
             }
                   
             MPI_Bcast( (void*)param_idx_agents.get_data(), agent_num, MPI_INT, 0, MPI_COMM_WORLD);
             MPI_Bcast( (void*)parameter_value_save_agents.get_data(), agent_num, MPI_DOUBLE, 0, MPI_COMM_WORLD);            
 #endif        
                       
-                      
-            // calsulate the cist functions at shifted parameter values
-            for(int agent_idx=0; agent_idx<agent_num; agent_idx++) { 
-                Matrix_real solution_guess_mtx_agent = solution_guess_mtx_agents[ agent_idx ]; 
-                solution_guess_mtx_agent[param_idx_agents[agent_idx]] += M_PI_half;                
-            }   
+                 
+            if ( cost_fnc == FROBENIUS_NORM ) {
+                                      
+                // calsulate the cist functions at shifted parameter values
+                for(int agent_idx=0; agent_idx<agent_num; agent_idx++) { 
+                    Matrix_real solution_guess_mtx_agent = solution_guess_mtx_agents[ agent_idx ]; 
+                    solution_guess_mtx_agent[param_idx_agents[agent_idx]] += M_PI_half;                
+                }   
             
-            // CPU time              
-            CPU_time += (tbb::tick_count::now() - t0_CPU).seconds();  
+                // CPU time              
+                CPU_time += (tbb::tick_count::now() - t0_CPU).seconds();  
             
-            // calculate batched cost function                 
-            f0_shifted_pi2_agents = optimization_problem_batched( solution_guess_mtx_agents );              
+                // calculate batched cost function                 
+                f0_shifted_pi2_agents = optimization_problem_batched( solution_guess_mtx_agents );              
             
-            // CPU time
-            t0_CPU = tbb::tick_count::now();                                         
+                // CPU time
+                t0_CPU = tbb::tick_count::now();                                         
                         
 
-            for(int agent_idx=0; agent_idx<agent_num; agent_idx++) { 
-                Matrix_real solution_guess_mtx_agent = solution_guess_mtx_agents[ agent_idx ];             
-                solution_guess_mtx_agent[param_idx_agents[agent_idx]] += M_PI_half;
-            }  
+                for(int agent_idx=0; agent_idx<agent_num; agent_idx++) { 
+                    Matrix_real solution_guess_mtx_agent = solution_guess_mtx_agents[ agent_idx ];             
+                    solution_guess_mtx_agent[param_idx_agents[agent_idx]] += M_PI_half;
+                }  
             
-            // CPU time             
-            CPU_time += (tbb::tick_count::now() - t0_CPU).seconds();        
+                // CPU time             
+                CPU_time += (tbb::tick_count::now() - t0_CPU).seconds();        
             
-            // calculate batched cost function                         
-            f0_shifted_pi_agents = optimization_problem_batched( solution_guess_mtx_agents );             
+                // calculate batched cost function                         
+                f0_shifted_pi_agents = optimization_problem_batched( solution_guess_mtx_agents );             
                 
                                                      
-            // CPU time                                      
-            t0_CPU = tbb::tick_count::now();                                  
+                // CPU time                                      
+                t0_CPU = tbb::tick_count::now();                                  
             
          
-            // determine the parameters of the cosine function and determine the parameter shift at the minimum
-            for ( int agent_idx=0; agent_idx<agent_num; agent_idx++ ) {
+                // determine the parameters of the cosine function and determine the parameter shift at the minimum
+                for ( int agent_idx=0; agent_idx<agent_num; agent_idx++ ) {
 
-                double current_minimum_agent = current_minimum_agents[agent_idx];         
-                double f0_shifted_pi         = f0_shifted_pi_agents[agent_idx];
-                double f0_shifted_pi2        = f0_shifted_pi2_agents[agent_idx];                                                  
+                    double current_minimum_agent = current_minimum_agents[agent_idx];         
+                    double f0_shifted_pi         = f0_shifted_pi_agents[agent_idx];
+                    double f0_shifted_pi2        = f0_shifted_pi2_agents[agent_idx];                                                  
             
 
-                double A_times_cos = (current_minimum_agent-f0_shifted_pi)/2;
-                double offset      = (current_minimum_agent+f0_shifted_pi)/2;
+                    double A_times_cos = (current_minimum_agent-f0_shifted_pi)/2;
+                    double offset      = (current_minimum_agent+f0_shifted_pi)/2;
 
-                double A_times_sin = offset - f0_shifted_pi2;
+                    double A_times_sin = offset - f0_shifted_pi2;
 
-                double phi0 = atan2( A_times_sin, A_times_cos);
+                    double phi0 = atan2( A_times_sin, A_times_cos);
 
 
-                double parameter_shift = phi0 > 0 ? M_PI-phi0 : -phi0-M_PI;
+                    double parameter_shift = phi0 > 0 ? M_PI-phi0 : -phi0-M_PI;
+                    double amplitude = sqrt(A_times_sin*A_times_sin + A_times_cos*A_times_cos);
 		
+
+
+                    //update  the parameter vector
+                    Matrix_real& solution_guess_mtx_agent                    = solution_guess_mtx_agents[ agent_idx ];  
+                    solution_guess_mtx_agent[param_idx_agents[ agent_idx ]] = parameter_value_save_agents[ agent_idx ] + parameter_shift; 
+
+                    current_minimum_agents[agent_idx] = offset - amplitude;
+                    
+                }
+                
+            }  
+            else if ( cost_fnc == HILBERT_SCHMIDT_TEST){
+           
+                
+                // calsulate the cist functions at shifted parameter values
+                for(int agent_idx=0; agent_idx<agent_num; agent_idx++) { 
+                    Matrix_real solution_guess_mtx_agent = solution_guess_mtx_agents[ agent_idx ]; 
+                    solution_guess_mtx_agent[param_idx_agents[agent_idx]] += M_PI_quarter;                
+                }   
+            
+                // CPU time              
+                CPU_time += (tbb::tick_count::now() - t0_CPU).seconds();  
+            
+                // calculate batched cost function                 
+                f0_shifted_pi4_agents = optimization_problem_batched( solution_guess_mtx_agents );              
+            
+                // CPU time
+                t0_CPU = tbb::tick_count::now();                                         
+                        
+
+                for(int agent_idx=0; agent_idx<agent_num; agent_idx++) { 
+                    Matrix_real solution_guess_mtx_agent = solution_guess_mtx_agents[ agent_idx ];             
+                    solution_guess_mtx_agent[param_idx_agents[agent_idx]] += M_PI_quarter;
+                }  
+            
+                // CPU time             
+                CPU_time += (tbb::tick_count::now() - t0_CPU).seconds();        
+            
+                // calculate batched cost function                         
+                f0_shifted_pi2_agents = optimization_problem_batched( solution_guess_mtx_agents );             
+                          
+                
+                                                     
+                // CPU time                                      
+                t0_CPU = tbb::tick_count::now(); 
+                
+                
+                for(int agent_idx=0; agent_idx<agent_num; agent_idx++) { 
+                    Matrix_real solution_guess_mtx_agent = solution_guess_mtx_agents[ agent_idx ];             
+                    solution_guess_mtx_agent[param_idx_agents[agent_idx]] += M_PI_half;
+                }  
+            
+                // CPU time             
+                CPU_time += (tbb::tick_count::now() - t0_CPU).seconds();        
+            
+                // calculate batched cost function                         
+                f0_shifted_pi_agents = optimization_problem_batched( solution_guess_mtx_agents );             
+                
+                                                     
+                // CPU time                                      
+                t0_CPU = tbb::tick_count::now();    
+                
+                for(int agent_idx=0; agent_idx<agent_num; agent_idx++) { 
+                    Matrix_real solution_guess_mtx_agent = solution_guess_mtx_agents[ agent_idx ];             
+                    solution_guess_mtx_agent[param_idx_agents[agent_idx]] += M_PI_half;
+                }  
+            
+                // CPU time             
+                CPU_time += (tbb::tick_count::now() - t0_CPU).seconds();        
+            
+                // calculate batched cost function                         
+                f0_shifted_3pi2_agents = optimization_problem_batched( solution_guess_mtx_agents );             
+                
+                                                     
+                // CPU time                                      
+                t0_CPU = tbb::tick_count::now();  
+		                
+                
+                // determine the parameters of the cosine function and determine the parameter shift at the minimum
+                for ( int agent_idx=0; agent_idx<agent_num; agent_idx++ ) {
+
+                    double current_minimum_agent = current_minimum_agents[agent_idx];         
+                    double f0_shifted_pi4        = f0_shifted_pi4_agents[agent_idx];                    
+                    double f0_shifted_pi2        = f0_shifted_pi2_agents[agent_idx];                    
+                    double f0_shifted_pi         = f0_shifted_pi_agents[agent_idx];                   
+                    double f0_shifted_3pi2       = f0_shifted_3pi2_agents[agent_idx];   
+/*                                                                              
+                    f(p)          = kappa*sin(2p+xi) + gamma*sin(p+phi) + offset
+                    f(p + pi/4)   = kappa*cos(2p+xi) + gamma*sin(p+pi/4+phi) + offset
+                    f(p + pi/2)   = -kappa*sin(2p+xi) + gamma*cos(p+phi) + offset
+                    f(p + pi)     = kappa*sin(2p+xi) - gamma*sin(p+phi) + offset
+                    f(p + 3*pi/2) = -kappa*sin(2p+xi) - gamma*cos(p+phi) + offset
+*/
+
+                    double f1 = current_minimum_agent -  f0_shifted_pi;
+                    double f2 = f0_shifted_pi2 - f0_shifted_3pi2;
+
+                    double gamma = sqrt( f1*f1 + f2*f2 )*0.5;
+                    //print( "gamma: ", gamma )
+
+                    double varphi = atan2( f1, f2) - parameter_value_save_agents[ agent_idx ];
+                    //print( "varphi: ", varphi )
+
+                    double offset = 0.25*(current_minimum_agent +  f0_shifted_pi + f0_shifted_pi2 + f0_shifted_3pi2);
+                    double f3     = 0.5*(current_minimum_agent +  f0_shifted_pi - 2*offset);
+                    double f4     = f0_shifted_pi4 - offset - gamma*sin(parameter_value_save_agents[ agent_idx ]+M_PI_quarter+varphi);
+
+
+                    double kappa = sqrt( f3*f3 + f4*f4);
+                    //print( "kappa: ", kappa )
+
+                    double xi = atan2( f3, f4) - 2*parameter_value_save_agents[ agent_idx ];
+                    //print( "xi: ", xi )
+
+
+
+                    double params[5];
+                    params[0] = kappa;
+                    params[1] = xi + 2*parameter_value_save_agents[ agent_idx ];
+                    params[2] = gamma;
+                    params[3] = varphi + parameter_value_save_agents[ agent_idx ];
+                    params[4] = offset;
+                    Problem p(1, -100, 100, HS_partial_optimization_problem, HS_partial_optimization_problem_grad, HS_partial_optimization_problem_combined, (void*)&params);
+                    
+
+                    double f; 
+                    Matrix_real parameter_shift(1,1);
+                    if ( abs(gamma) > abs(kappa) ) {
+                        parameter_shift[0] = 3*M_PI/2 - varphi - parameter_value_save_agents[ agent_idx ];                        
+                    }
+                    else {
+                        parameter_shift[0] = 3*M_PI/4 - xi/2 - parameter_value_save_agents[ agent_idx ]/2;
+                        
+
+                    }
+                   
+                    parameter_shift[0] = std::fmod( parameter_shift[0], M_PI_double);    
+                                                 
+                    Tolmin tolmin(&p);                                                 
+                    f = tolmin.Solve(parameter_shift, false, 10);
 		
-                //update  the parameter vector
-                Matrix_real& solution_guess_mtx_agent                    = solution_guess_mtx_agents[ agent_idx ];                             
-                solution_guess_mtx_agent[param_idx_agents[ agent_idx ]] = parameter_value_save_agents[ agent_idx ] + parameter_shift; 
+                    //update  the parameter vector
+                    Matrix_real& solution_guess_mtx_agent                   = solution_guess_mtx_agents[ agent_idx ];                             
+                    solution_guess_mtx_agent[param_idx_agents[ agent_idx ]] = parameter_value_save_agents[ agent_idx ] + parameter_shift[0]; 
 
+                    current_minimum_agents[agent_idx] = f;
+                    
+                }                                                                                                                         
                 
             }
+    
+
+                
+            
                
             // CPU time                                                     
             CPU_time += (tbb::tick_count::now() - t0_CPU).seconds();
             
-            
-            // determine the current minimum  at the shifted parameters        
-            current_minimum_agents = optimization_problem_batched( solution_guess_mtx_agents ); 
+          
+            // determine the current minimum  at the shifted parameters  
+            //current_minimum_agents = optimization_problem_batched( solution_guess_mtx_agents ); 
 
   
             // CPU time                                        
             t0_CPU = tbb::tick_count::now();        
 
 
             // generate random numbers to manage the behavior of the agents
@@ -1134,15 +1380,15 @@
                
                 
                 Matrix_real& solution_guess_mtx_agent = solution_guess_mtx_agents[ agent_idx ];                             
 
                 // look for the best agent periodicaly
                 if ( iter_idx % agent_lifetime_loc == 0 )
                 {
-                             
+                            
                     if ( current_minimum_agent <= current_minimum ) {
 
                         most_successfull_agent = agent_idx;
                     
                         // export the parameters of the curremt, most successful agent
                         memcpy(optimized_parameters_mtx.get_data(), solution_guess_mtx_agent.get_data(), num_of_parameters*sizeof(double) );
 
@@ -1179,15 +1425,16 @@
                                 current_minimum_agents[ agent_idx ] = current_minimum_agents[ most_successfull_agent ];
                                 memcpy( solution_guess_mtx_agent.get_data(), solution_guess_mtx_agents[ most_successfull_agent ].get_data(), solution_guess_mtx_agent.size()*sizeof(double) );
 
                             
                                 random_num = random_numbers[ agent_idx*random_numbers.stride + 1 ];
                             
                                 if ( random_num < agent_randomization_rate ) {
-                                    randomize_parameters( optimized_parameters_mtx, solution_guess_mtx_agent, radius  );                              
+                                    randomize_parameters( optimized_parameters_mtx, solution_guess_mtx_agent, current_minimum  );  
+                                    current_minimum_agents[agent_idx] = optimization_problem( solution_guess_mtx_agent );                             
                                 }     
 
                        
                             }
                             else {
                                 // keep the current state  of the agent                    
                             }
@@ -1217,14 +1464,15 @@
                             
                         if ( std::abs( current_minimum_mean - current_minimum) < 1e-7  && var_current_minimum < 1e-7 ) {
                             std::stringstream sstream;
                             sstream << "AGENTS, iterations converged to "<< current_minimum << std::endl;
                             print(sstream, 0); 
                             terminate_optimization = true;
                         }                    
+
                    }   
                     
 
                     
                 }   
 
 
@@ -1251,19 +1499,20 @@
             if ( terminate_optimization ) {                   
                 break;                    
             }      
         
         }
 
 
-
         tbb::tick_count optimization_end = tbb::tick_count::now();
         optimization_time  = optimization_time + (optimization_end-optimization_start).seconds();
+        sstream.str("");
         sstream << "AGENTS time: " << adam_time << ", pure DFE time:  " << pure_DFE_time << " " << current_minimum << std::endl;
 
+        print(sstream, 0); 
 }
 
 
 
 /**
 @brief Call to solve layer by layer the optimization problem via the AGENT COMBINED algorithm. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
@@ -1298,15 +1547,15 @@
 @param num_of_parameters Number of parameters to be optimized
 @param solution_guess Array containing the solution guess.
 */
 void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_ADAM_BATCHED( int num_of_parameters, Matrix_real& solution_guess) {
 
 
 #ifdef __DFE__
-        if ( qbit_num >= 2 && get_accelerator_num() > 0 ) {
+        if ( qbit_num >= 5 && get_accelerator_num() > 0 ) {
             upload_Umtx_to_DFE();
         }
 #endif
 
 
 
         if (gates.size() == 0 ) {
@@ -1342,33 +1591,63 @@
         memcpy(solution_guess_tmp.get_data(), solution_guess.get_data(), num_of_parameters*sizeof(double) );
 
         Matrix_real grad_mtx = Matrix_real( num_of_parameters, 1 );
         //solution_guess_tmp_mtx.print_matrix();
 
 
         long long max_inner_iterations_loc;
-        if ( config.count("max_inner_iterations_agent") > 0 ) {
-             config["max_inner_iterations_agent"].get_property( max_inner_iterations_loc );  
+        if ( config.count("max_inner_iterations_adam_batched") > 0 ) {
+             config["max_inner_iterations_adam_batched"].get_property( max_inner_iterations_loc );  
+        }
+        if ( config.count("max_inner_iterations") > 0 ) {
+             config["max_inner_iterations"].get_property( max_inner_iterations_loc );  
         }
         else {
             max_inner_iterations_loc = max_inner_iterations;
         }
-        
+
+        long long iteration_threshold_of_randomization_loc;
+        if ( config.count("randomization_threshold_adam") > 0 ) {
+            config["randomization_threshold_adam"].get_property( iteration_threshold_of_randomization_loc );  
+        }
+        else if ( config.count("randomization_threshold") > 0 ) {
+            config["randomization_threshold"].get_property( iteration_threshold_of_randomization_loc );  
+        }
+        else {
+            iteration_threshold_of_randomization_loc = iteration_threshold_of_randomization;
+        }
+
         
         long long export_circuit_2_binary_loc;
-        if ( config.count("export_circuit_2_binary") > 0 ) {
+        if ( config.count("export_circuit_2_binary_adam") > 0 ) {
+             config["export_circuit_2_binary_adam"].get_property( export_circuit_2_binary_loc );  
+        }
+        else if ( config.count("export_circuit_2_binary") > 0 ) {
              config["export_circuit_2_binary"].get_property( export_circuit_2_binary_loc );  
         }
         else {
             export_circuit_2_binary_loc = 0;
         }            
 
+        double optimization_tolerance_loc;
+        if ( config.count("optimization_tolerance_adam_batched") > 0 ) {
+             double value;
+             config["optimization_tolerance_adam_batched"].get_property( optimization_tolerance_loc );
+        }
+        else if ( config.count("optimization_tolerance") > 0 ) {
+             double value;
+             config["optimization_tolerance"].get_property( optimization_tolerance_loc );
+        }
+        else {
+            optimization_tolerance_loc = optimization_tolerance;
+        }
+
         double f0 = DBL_MAX;
         std::stringstream sstream;
-        sstream << "iter_max: " << max_inner_iterations_loc << ", randomization threshold: " << iteration_threshold_of_randomization << ", randomization radius: " << radius << std::endl;
+        sstream << "iter_max: " << max_inner_iterations_loc << ", randomization threshold: " << iteration_threshold_of_randomization_loc << std::endl;
         print(sstream, 2); 
 
         int ADAM_status = 0;
 
 
 
         Matrix Umtx_orig = Umtx;
@@ -1436,41 +1715,35 @@
 
                     Matrix matrix_new = get_transformed_matrix( optimized_parameters_mtx, gates.begin(), gates.size(), Umtx );
 
                     std::stringstream sstream;
                     sstream << "ADAM: processed iterations " << (double)iter_idx/max_inner_iterations_loc*100;
                     sstream << "\%, current minimum:" << current_minimum << ", pure cost function:" << get_cost_function(matrix_new, trace_offset) << std::endl;
                     print(sstream, 0);   
-                    
-                    if ( export_circuit_2_binary_loc > 0 ) {
-                        std::string filename("initial_circuit_iteration.binary");
-                        if (project_name != "") { 
-                            filename=project_name+ "_"  +filename;
-                        }
-                        export_gate_list_to_binary(optimized_parameters_mtx, this, filename, verbose);
-                    }
+                    std::string filename("initial_circuit_iteration.binary");
+                    export_gate_list_to_binary(optimized_parameters_mtx, this, filename, verbose);
 
                 }
 
 //std::cout << grad_norm  << std::endl;
-                if (f0 < optimization_tolerance || random_shift_count > random_shift_count_max ) {
+                if (f0 < optimization_tolerance_loc || random_shift_count > random_shift_count_max ) {
                     break;
                 }
 
 
 
                 // calculate the gradient norm
                 double norm = 0.0;
                 for ( int grad_idx=0; grad_idx<num_of_parameters; grad_idx++ ) {
                     norm += grad_mtx[grad_idx]*grad_mtx[grad_idx];
                 }
                 norm = std::sqrt(norm);
                     
 
-                if ( sub_iter_idx> iteration_threshold_of_randomization || ADAM_status != 0 ) {
+                if ( sub_iter_idx> iteration_threshold_of_randomization_loc || ADAM_status != 0 ) {
 
                     //random_shift_count++;
                     sub_iter_idx = 0;
                     random_shift_count++;
                     current_minimum_hold = current_minimum;   
 
 
@@ -1579,45 +1852,58 @@
 
         int ADAM_status = 0;
 
         int randomization_successful = 0;
 
 
         long long max_inner_iterations_loc;
-        if ( config.count("max_inner_iterations") > 0 ) {
+        if ( config.count("max_inner_iterations_adam") > 0 ) {
+            config["max_inner_iterations_adam"].get_property( max_inner_iterations_loc );         
+        }
+        else if ( config.count("max_inner_iterations") > 0 ) {
             config["max_inner_iterations"].get_property( max_inner_iterations_loc );         
         }
         else {
             max_inner_iterations_loc =max_inner_iterations;
         }
 
         long long iteration_threshold_of_randomization_loc;
-        if ( config.count("randomization_threshold") > 0 ) {
+        if ( config.count("randomization_threshold_adam") > 0 ) {
+            config["randomization_threshold_adam"].get_property( iteration_threshold_of_randomization_loc );  
+        }
+        else if ( config.count("randomization_threshold") > 0 ) {
             config["randomization_threshold"].get_property( iteration_threshold_of_randomization_loc );  
         }
         else {
             iteration_threshold_of_randomization_loc = iteration_threshold_of_randomization;
         }
         
         long long export_circuit_2_binary_loc;
-        if ( config.count("export_circuit_2_binary") > 0 ) {
+        if ( config.count("export_circuit_2_binary_adam") > 0 ) {
+             config["export_circuit_2_binary_adam"].get_property( export_circuit_2_binary_loc );  
+        }
+        else if ( config.count("export_circuit_2_binary") > 0 ) {
              config["export_circuit_2_binary"].get_property( export_circuit_2_binary_loc );  
         }
         else {
             export_circuit_2_binary_loc = 0;
         }            
         
         
         double optimization_tolerance_loc;
-        if ( config.count("optimization_tolerance") > 0 ) {
+        if ( config.count("optimization_tolerance_adam") > 0 ) {
+             config["optimization_tolerance_adam"].get_property( optimization_tolerance_loc );  
+        }
+        else if ( config.count("optimization_tolerance") > 0 ) {
              config["optimization_tolerance"].get_property( optimization_tolerance_loc );  
         }
         else {
             optimization_tolerance_loc = optimization_tolerance;
-        }        
+        }       
+ 
 
 
         double f0 = DBL_MAX;
         std::stringstream sstream;
         sstream << "max_inner_iterations: " << max_inner_iterations_loc << ", randomization threshold: " << iteration_threshold_of_randomization_loc << ", randomization radius: " << radius << std::endl;
         print(sstream, 2); 
         
@@ -1806,15 +2092,18 @@
         }
 
         // random generator of real numbers   
         std::uniform_real_distribution<> distrib_real(0.0, 2*M_PI);
 
         // maximal number of inner iterations overriden by config
         long long max_inner_iterations_loc;
-        if ( config.count("max_inner_iterations") > 0 ) {
+        if ( config.count("max_inner_iterations_bfgs") > 0 ) {
+            config["max_inner_iterations_bfgs"].get_property( max_inner_iterations_loc );         
+        }
+        else if ( config.count("max_inner_iterations") > 0 ) {
             config["max_inner_iterations"].get_property( max_inner_iterations_loc );         
         }
         else {
             max_inner_iterations_loc =max_inner_iterations;
         }
 
 
@@ -1916,33 +2205,42 @@
         std::uniform_real_distribution<> distrib_real(0.0, 2*M_PI);
 
         // random generator of integers   
         std::uniform_int_distribution<> distrib_int(0, 5000);  
 
 
         long long max_inner_iterations_loc;
-        if ( config.count("max_inner_iterations") > 0 ) {
+        if ( config.count("max_inner_iterations_bfgs2") > 0 ) {
+            config["max_inner_iterations_bfgs2"].get_property( max_inner_iterations_loc );  
+        }
+        else if ( config.count("max_inner_iterations") > 0 ) {
             config["max_inner_iterations"].get_property( max_inner_iterations_loc );  
         }
         else {
             max_inner_iterations_loc =max_inner_iterations;
         }
 
 
         long long export_circuit_2_binary_loc;
-        if ( config.count("export_circuit_2_binary") > 0 ) {
+        if ( config.count("export_circuit_2_binary_bfgs2") > 0 ) {
+             config["export_circuit_2_binary_bfgs2"].get_property( export_circuit_2_binary_loc );  
+        }
+        else if ( config.count("export_circuit_2_binary") > 0 ) {
              config["export_circuit_2_binary"].get_property( export_circuit_2_binary_loc );  
         }
         else {
             export_circuit_2_binary_loc = 0;
         }    
         
 
         long long iteration_threshold_of_randomization_loc;
-        if ( config.count("randomization_threshold") > 0 ) {
+        if ( config.count("randomization_threshold_bfgs2") > 0 ) {
+            config["randomization_threshold_bfgs2"].get_property( iteration_threshold_of_randomization_loc );  
+        }
+        else if ( config.count("randomization_threshold") > 0 ) {
             config["randomization_threshold"].get_property( iteration_threshold_of_randomization_loc );  
         }
         else {
             iteration_threshold_of_randomization_loc = iteration_threshold_of_randomization;
         }
 
         std::stringstream sstream;
@@ -2205,15 +2503,15 @@
         }
         else if ( cost_fnc == FROBENIUS_NORM_CORRECTION2 ) {
             for ( int idx=0; idx<parameters_vec.size(); idx++ ) {
                 cost_fnc_mtx[idx] = 1-(trace_DFE_mtx[idx*3] + std::sqrt(prev_cost_fnv_val)*(trace_DFE_mtx[idx*3+1]*correction1_scale + trace_DFE_mtx[idx*3+2]*correction2_scale))/Umtx.cols;
             }
         }
         else {
-            std::string err("N_Qubit_Decomposition_Base::optimization_problem_batched: Cost function variant not implmented.");
+            std::string err("N_Qubit_Decomposition_Base::optimization_problem_batched: Cost function variant not implmented for DFE.");
             throw err;
         }
```

### Comparing `squander-1.8.3/decomposition/N_Qubit_Decomposition_Cost_Function.cpp` & `squander-1.8.4/decomposition/N_Qubit_Decomposition_Cost_Function.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,16 @@
 @return Returns the cost function
 */
 double get_hilbert_schmidt_test(Matrix& matrix){
     
     double d = 1.0/matrix.cols;
     double cost_function = 0.0;
     QGD_Complex16 ret = get_trace(matrix);
-    cost_function = 1.0-d*d*ret.real*ret.real-d*d*ret.imag*ret.imag;
+    cost_function = 1.0-d*d*(ret.real*ret.real+ret.imag*ret.imag);
+
     return cost_function;
 }
 
 /**
 @brief Call co calculate the Hilbert Schmidt testof the optimization process, and the first correction to the cost finction according to https://arxiv.org/pdf/2210.09191.pdf
 @param matrix The square shaped complex matrix from which the cost function is calculated.
 @param qbit_num The number of qubits
```

### Comparing `squander-1.8.3/decomposition/N_Qubit_Decomposition_adaptive.cpp` & `squander-1.8.4/decomposition/N_Qubit_Decomposition_adaptive.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/N_Qubit_Decomposition_custom.cpp` & `squander-1.8.4/decomposition/N_Qubit_Decomposition_custom.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/Sub_Matrix_Decomposition.cpp` & `squander-1.8.4/decomposition/Sub_Matrix_Decomposition.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp` & `squander-1.8.4/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/include/Decomposition_Base.h` & `squander-1.8.4/decomposition/include/Decomposition_Base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/include/N_Qubit_Decomposition.h` & `squander-1.8.4/decomposition/include/N_Qubit_Decomposition.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/include/N_Qubit_Decomposition_Base.h` & `squander-1.8.4/decomposition/include/N_Qubit_Decomposition_Base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/include/N_Qubit_Decomposition_Cost_Function.h` & `squander-1.8.4/decomposition/include/N_Qubit_Decomposition_Cost_Function.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/include/N_Qubit_Decomposition_adaptive.h` & `squander-1.8.4/decomposition/include/N_Qubit_Decomposition_adaptive.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/include/N_Qubit_Decomposition_custom.h` & `squander-1.8.4/decomposition/include/N_Qubit_Decomposition_custom.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/include/Sub_Matrix_Decomposition.h` & `squander-1.8.4/decomposition/include/Sub_Matrix_Decomposition.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h` & `squander-1.8.4/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/Adaptive.cpp` & `squander-1.8.4/gates/Adaptive.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/CH.cpp` & `squander-1.8.4/gates/CH.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/CNOT.cpp` & `squander-1.8.4/gates/CNOT.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/CRY.cpp` & `squander-1.8.4/gates/CRY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/CZ.cpp` & `squander-1.8.4/gates/CZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/Composite.cpp` & `squander-1.8.4/gates/Composite.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/Gate.cpp` & `squander-1.8.4/gates/Gate.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
 #ifdef USE_AVX
 
     if ( qbit_num < 4 ) {
         apply_kernel_to_input_AVX_small(u3_1qbit, input, deriv, target_qbit, control_qbit, matrix_size);
         return;
     }
-    else if ( qbit_num < 6 || (qbit_num < 10 && input.cols < 32) ) {
+    else if ( qbit_num < 10) {
         apply_kernel_to_input_AVX(u3_1qbit, input, deriv, target_qbit, control_qbit, matrix_size);
         return;
      }
     else {
         apply_kernel_to_input_AVX_parallel(u3_1qbit, input, deriv, target_qbit, control_qbit, matrix_size);
         return;
      }
```

### Comparing `squander-1.8.3/gates/Gates_block.cpp` & `squander-1.8.4/gates/Gates_block.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/ON.cpp` & `squander-1.8.4/gates/ON.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/RX.cpp` & `squander-1.8.4/gates/RX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/RY.cpp` & `squander-1.8.4/gates/RY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/RZ.cpp` & `squander-1.8.4/gates/RZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/SX.cpp` & `squander-1.8.4/gates/SX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/SYC.cpp` & `squander-1.8.4/gates/SYC.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/U3.cpp` & `squander-1.8.4/gates/U3.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -538,28 +538,35 @@
         print(sstream, 1);	   
     }
 #endif // DEBUG
 
 
     double cos_theta = cos(ThetaOver2);
     double sin_theta = sin(ThetaOver2);
-
+    double cos_phi = cos(Phi);
+    double sin_phi = sin(Phi);
+    double cos_lambda = cos(Lambda);
+    double sin_lambda = sin(Lambda);
 
     // the 1,1 element
     u3_1qbit[0].real = cos_theta;
     u3_1qbit[0].imag = 0;
     // the 1,2 element
-    u3_1qbit[1].real = -cos(Lambda)*sin_theta;
-    u3_1qbit[1].imag = -sin(Lambda)*sin_theta;
+    u3_1qbit[1].real = -cos_lambda*sin_theta;
+    u3_1qbit[1].imag = -sin_lambda*sin_theta;
     // the 2,1 element
-    u3_1qbit[2].real = cos(Phi)*sin_theta;
-    u3_1qbit[2].imag = sin(Phi)*sin_theta;
+    u3_1qbit[2].real = cos_phi*sin_theta;
+    u3_1qbit[2].imag = sin_phi*sin_theta;
     // the 2,2 element
-    u3_1qbit[3].real = cos(Phi+Lambda)*cos_theta;
-    u3_1qbit[3].imag = sin(Phi+Lambda)*cos_theta;
+    //cos(a+b)=cos(a)cos(b)-sin(a)sin(b)
+    //sin(a+b)=sin(a)cos(b)+cos(a)sin(b)
+    u3_1qbit[3].real = (cos_phi*cos_lambda-sin_phi*sin_lambda)*cos_theta;
+    u3_1qbit[3].imag = (sin_phi*cos_lambda+cos_phi*sin_lambda)*cos_theta;
+    //u3_1qbit[3].real = cos(Phi+Lambda)*cos_theta;
+    //u3_1qbit[3].imag = sin(Phi+Lambda)*cos_theta;
 
 
     return u3_1qbit;
 
 }
```

### Comparing `squander-1.8.3/gates/UN.cpp` & `squander-1.8.4/gates/UN.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/X.cpp` & `squander-1.8.4/gates/X.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/Y.cpp` & `squander-1.8.4/gates/Y.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/Z.cpp` & `squander-1.8.4/gates/Z.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/Adaptive.h` & `squander-1.8.4/gates/include/Adaptive.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/CH.h` & `squander-1.8.4/gates/include/CH.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/CNOT.h` & `squander-1.8.4/gates/include/CNOT.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/CRY.h` & `squander-1.8.4/gates/include/CRY.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/CZ.h` & `squander-1.8.4/gates/include/CZ.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/Composite.h` & `squander-1.8.4/gates/include/Composite.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/Gate.h` & `squander-1.8.4/gates/include/Gate.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/Gates_block.h` & `squander-1.8.4/gates/include/Gates_block.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/ON.h` & `squander-1.8.4/gates/include/ON.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/RX.h` & `squander-1.8.4/gates/include/RX.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/RY.h` & `squander-1.8.4/gates/include/RY.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/RZ.h` & `squander-1.8.4/gates/include/RZ.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/SX.h` & `squander-1.8.4/gates/include/SX.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/SYC.h` & `squander-1.8.4/gates/include/SYC.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/U3.h` & `squander-1.8.4/gates/include/U3.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/UN.h` & `squander-1.8.4/gates/include/UN.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/X.h` & `squander-1.8.4/gates/include/X.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/Y.h` & `squander-1.8.4/gates/include/Y.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/include/Z.h` & `squander-1.8.4/gates/include/Z.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/kernels/apply_kernel_to_input_AVX.cpp` & `squander-1.8.4/gates/kernels/apply_kernel_to_input_AVX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/kernels/apply_kernel_to_state_vector_input.cpp` & `squander-1.8.4/gates/kernels/apply_kernel_to_state_vector_input.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/kernels/include/apply_kernel_to_input_AVX.h` & `squander-1.8.4/gates/kernels/include/apply_kernel_to_input_AVX.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/gates/kernels/include/apply_kernel_to_state_vector_input.h` & `squander-1.8.4/gates/kernels/include/apply_kernel_to_state_vector_input.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/nn/NN.cpp` & `squander-1.8.4/nn/NN.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/nn/include/NN.h` & `squander-1.8.4/nn/include/NN.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/optimization_engines/RL_experience.cpp` & `squander-1.8.4/optimization_engines/RL_experience.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/optimization_engines/include/RL_experience.h` & `squander-1.8.4/optimization_engines/include/RL_experience.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/CMakeLists.txt` & `squander-1.8.4/qgd_python/decomposition/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py` & `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp` & `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py` & `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp` & `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py` & `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp` & `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py` & `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/test/test_Compression.py` & `squander-1.8.4/qgd_python/decomposition/test/test_Compression.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
         # generate config structure
         config = { 'max_outer_iterations': 10, 
 		'max_inner_iterations': 300000, 	
 		'max_inner_iterations_compression': 10000, 
 		'max_inner_iterations_final': 1000, 	
 	        'randomized_adaptive_layers': 1,
+	        'export_circuit_2_binary': 1,
 		'optimization_tolerance': 1e-8 }
 
         
         
 
         # creating a class to decompose the unitary
         cDecompose = N_Qubit_Decomposition_adaptive( Umtx.conj().T, config=config )
@@ -134,14 +135,15 @@
         
         # generate config structure
         config = { 'max_outer_iterations': 10, 
 		'max_inner_iterations': 300000, 	
 		'max_inner_iterations_compression': 10000, 
 		'max_inner_iterations_final': 1000, 	
 	        'randomized_adaptive_layers': 1,
+	        'export_circuit_2_binary': 1,
 		'optimization_tolerance': 1e-8 }
 
 
         # creating a class to decompose the unitary
         cDecompose = N_Qubit_Decomposition_adaptive( Umtx.conj().T, config=config )
 
 
@@ -207,14 +209,15 @@
 
         # generate config structure
         config = { 'max_outer_iterations': 10, 
 		'max_inner_iterations': 300000, 	
 		'max_inner_iterations_compression': 10000, 
 		'max_inner_iterations_final': 1000, 	
 	        'randomized_adaptive_layers': 1,
+	        'export_circuit_2_binary': 1,
 		'optimization_tolerance': 1e-8 }
         
 
         # creating a class to decompose the unitary
         cDecompose = N_Qubit_Decomposition_adaptive( Umtx.conj().T, config=config )
 
 
@@ -277,14 +280,15 @@
 		'max_inner_iterations_compression': 10000,
 		'max_inner_iterations' : 500,
 		'max_inner_iterations_final': 5000, 		
 		'Randomized_Radius': 0.3, 
                 'randomized_adaptive_layers': 1,
 		'optimization_tolerance_agent': 1e-4,
 		'optimization_tolerance': 1e-5,
+
                 'agent_num': 10}
 
         # creating a class to decompose the unitary
         cDecompose = N_Qubit_Decomposition_adaptive( Umtx.conj().T, config=config )
 
 
         # setting the verbosity of the decomposition
```

### Comparing `squander-1.8.3/qgd_python/decomposition/test/test_Global_Phase.py` & `squander-1.8.4/qgd_python/decomposition/test/test_Global_Phase.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/test/test_IBM.py` & `squander-1.8.4/qgd_python/decomposition/test/test_IBM.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/test/test_Project_Name.py` & `squander-1.8.4/qgd_python/decomposition/test/test_Project_Name.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/test/test_QX2.py` & `squander-1.8.4/qgd_python/decomposition/test/test_QX2.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/test/test_State_Preparation.py` & `squander-1.8.4/qgd_python/decomposition/test/test_State_Preparation.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/test/test_Unitary.py` & `squander-1.8.4/qgd_python/decomposition/test/test_Unitary.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/test/test_decomposition.py` & `squander-1.8.4/qgd_python/decomposition/test/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/test/test_fmo.py` & `squander-1.8.4/qgd_python/decomposition/test/test_fmo.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/test/test_heavy_hex.py` & `squander-1.8.4/qgd_python/decomposition/test/test_heavy_hex.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/test/test_optmization_problem_combined.py` & `squander-1.8.4/qgd_python/decomposition/test/test_optmization_problem_combined.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/decomposition/test/test_parametric_circuit.py` & `squander-1.8.4/qgd_python/decomposition/test/test_parametric_circuit.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/CMakeLists.txt` & `squander-1.8.4/qgd_python/gates/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/qgd_CH.cpp` & `squander-1.8.4/qgd_python/gates/qgd_CH.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/qgd_CNOT.cpp` & `squander-1.8.4/qgd_python/gates/qgd_CNOT.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/qgd_CZ.cpp` & `squander-1.8.4/qgd_python/gates/qgd_CZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/qgd_Gates_Block.cpp` & `squander-1.8.4/qgd_python/gates/qgd_Gates_Block.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/qgd_RX.cpp` & `squander-1.8.4/qgd_python/gates/qgd_RX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/qgd_RY.cpp` & `squander-1.8.4/qgd_python/gates/qgd_RY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/qgd_RZ.cpp` & `squander-1.8.4/qgd_python/gates/qgd_RZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/qgd_SX.cpp` & `squander-1.8.4/qgd_python/gates/qgd_SX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/qgd_SYC.cpp` & `squander-1.8.4/qgd_python/gates/qgd_SYC.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/qgd_U3.cpp` & `squander-1.8.4/qgd_python/gates/qgd_U3.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/qgd_X.cpp` & `squander-1.8.4/qgd_python/gates/qgd_X.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/qgd_Y.cpp` & `squander-1.8.4/qgd_python/gates/qgd_Y.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/qgd_Z.cpp` & `squander-1.8.4/qgd_python/gates/qgd_Z.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/test/test_CH.py` & `squander-1.8.4/qgd_python/gates/test/test_CH.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/test/test_CNOT.py` & `squander-1.8.4/qgd_python/gates/test/test_CNOT.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/test/test_CZ.py` & `squander-1.8.4/qgd_python/gates/test/test_CZ.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/test/test_RX.py` & `squander-1.8.4/qgd_python/gates/test/test_RX.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/test/test_RY.py` & `squander-1.8.4/qgd_python/gates/test/test_RY.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/test/test_RZ.py` & `squander-1.8.4/qgd_python/gates/test/test_RZ.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/test/test_SX.py` & `squander-1.8.4/qgd_python/gates/test/test_SX.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/test/test_U3.py` & `squander-1.8.4/qgd_python/gates/test/test_U3.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/test/test_X.py` & `squander-1.8.4/qgd_python/gates/test/test_X.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/test/test_Y.py` & `squander-1.8.4/qgd_python/gates/test/test_Y.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/test/test_Z.py` & `squander-1.8.4/qgd_python/gates/test/test_Z.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/gates/test/test_gates.py` & `squander-1.8.4/qgd_python/gates/test/test_gates.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/nn/CMakeLists.txt` & `squander-1.8.4/qgd_python/nn/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/nn/qgd_nn.py` & `squander-1.8.4/qgd_python/nn/qgd_nn.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/nn/qgd_nn_Wrapper.cpp` & `squander-1.8.4/qgd_python/nn/qgd_nn_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/qgd_python/utils.py` & `squander-1.8.4/qgd_python/utils.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/random_unitary/Random_Orthogonal.cpp` & `squander-1.8.4/random_unitary/Random_Orthogonal.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/random_unitary/Random_Unitary.cpp` & `squander-1.8.4/random_unitary/Random_Unitary.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/random_unitary/include/Random_Orthogonal.h` & `squander-1.8.4/random_unitary/include/Random_Orthogonal.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/random_unitary/include/Random_Unitary.h` & `squander-1.8.4/random_unitary/include/Random_Unitary.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/setup.py` & `squander-1.8.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 setup(
     name="squander",
     packages=find_packages(
         exclude=(
             "test_standalone", "test_standalone.*",
         )
     ),
-    version='1.8.3',
+    version='1.8.4',
     url="https://github.com/rakytap/sequential-quantum-gate-decomposer", 
     maintainer="Peter Rakyta",
     maintainer_email="peter.rakyta@ttk.elte.hu",
     include_package_data=True,
     install_requires=[
         "setuptools>=40.8.0",
         "wheel",
```

### Comparing `squander-1.8.3/squander/__init__.py` & `squander-1.8.4/squander/__init__.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/squander.egg-info/PKG-INFO` & `squander-1.8.4/squander.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squander
-Version: 1.8.3
+Version: 1.8.4
 Summary: Package to decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta
 Maintainer-email: peter.rakyta@ttk.elte.hu
 License: GNU General Public License v3.0
 Keywords: test,cmake,extension
 Classifier: Intended Audience :: Developers
@@ -101,43 +101,15 @@
 
 environment variables are sufficient for successful compilation. 
 When the TBB library is installed via a python package, setting the environment variables above is not necessary.
 The SQUANDER package with C++ Python extensions can be compiled via the Python script **setup.py** located in the root directory of the SQUANDER package.
 The script automatically finds out the CBLAS library working behind the numpy package and uses it in further linking. 
 The **setup.py** script also build the C++ library of the SQUANDER package by making the appropriate CMake calls. 
 
-### Build and Install on Microsoft Windows with Microsoft Visual C++
-
-CMake must be in the path and able to find the MSVC compiler e.g.
-
-$ set PATH=%PATH%;C:\Program Files\cmake\bin
-
-Now set the TBB and BLAS folders and build via:
-
-$ set TBB_LOCATION=<Python_Folder>/LocalCache/local-packages
-
-$ set TBB_INC_DIR=%TBB_LOCATION%/Library/include
-
-$ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib
-
-$ set LIB=<BLAS_Location>/lib;<LAPACK_Location>/lib
 
-$ python setup.py build_ext -DTBB_HEADER=<TBB_Location>\Library\include\
-
-Installation merely requires copying DLL files (if they are not in the path):
-
-$ copy _skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition
-
-$ copy "%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition
-
-$ copy "%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition
-
-Verify the installation:
-
-$ python -m pytest
 
 ### Developer build
 
 
 We recommend to install the SQUANDER package in the Anaconda environment. In order to install the necessary requirements, follow the steps below:
 
 Creating new python environment: 
@@ -193,14 +165,45 @@
 
 $ pip3 install qgd-*.tar.gz
 
 issued from directory **path/to/SQUANDER/package/dist**
 (It is optional to install the ninja package which speeds up the building process by parallel compilation.)
 
 
+### Build and Install on Microsoft Windows with Microsoft Visual C++
+
+CMake must be in the path and able to find the MSVC compiler e.g.
+
+$ set PATH=%PATH%;C:\Program Files\cmake\bin
+
+Now set the TBB and BLAS folders and build via:
+
+$ set TBB_LOCATION=<Python_Folder>/LocalCache/local-packages
+
+$ set TBB_INC_DIR=%TBB_LOCATION%/Library/include
+
+$ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib
+
+$ set LIB=<BLAS_Location>/lib;<LAPACK_Location>/lib
+
+$ python setup.py build_ext -DTBB_HEADER=<TBB_Location>\Library\include\
+
+Installation merely requires copying DLL files (if they are not in the path):
+
+$ copy _skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition
+
+$ copy "%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition
+
+$ copy "%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition
+
+Verify the installation:
+
+$ python -m pytest
+
+
 ### How to use
 
 The algorithm implemented in the SQUANDER package intends to transform the given unitary into an identity matrix via a sequence of two-qubit and one-qubit gate operations applied on the unitary. 
 Thus, in order to get the decomposition of a unitary, one should rather provide the complex transpose of this unitary as the input for the SQUANDER decomposing process, as can be seen in the examples.
 
 
 ## Python Interface
@@ -221,15 +224,15 @@
         config = { 'max_outer_iterations': 1, 
                     'max_inner_iterations_agent': 25000, 
                     'max_inner_iterations_compression': 10000,
                     'max_inner_iterations' : 500,
                     'max_inner_iterations_final': 5000, 		
                     'Randomized_Radius': 0.3, 
                     'randomized_adaptive_layers': 1,
-                    'optimization_tolerance_agent': 1e-4,
+                    'optimization_tolerance_agent': 1e-2,
                     'optimization_tolerance': 1e-8,
                     'agent_num': 10}
  
 Next we initialize the decomposition class with the unitary Umtx to be decomposed. 
 
         # creating a class to decompose the unitary
         from squander import N_Qubit_Decomposition_adaptive
@@ -255,25 +258,26 @@
 We can construct an initial parameters set for the optimization by retrieving the number of free parameters. If the initial parameter set is not set, random parameters are used by default.
 
         # setting intial parameter set
         parameter_num = cDecompose.get_Parameter_Num()
         parameters = np.zeros( (parameter_num,1), dtype=np.float64 )
         cDecompose.set_Optimized_Parameters( parameters )
 
-We can use between several engines to solve the optimization problem. Here we use an evolutionary based algorithm named 'AGENTS'
+We can choose between several engines to solve the optimization problem. Here we use an evolutionary based algorithm named 'AGENTS'
 
         # setting optimizer
         cDecompose.set_Optimizer("AGENTS")
 	
 The optimization process is started by the function call	
 
         # starting the decomposition
         cDecompose.get_Initial_Circuit()
 	
 The optimization process terminates by either reaching the tolerance 'optimization_tolerance_agent' or by reaching the maximal iteration number 'max_inner_iterations_agent', or if the engines identifies a convergence to a local minimum. The SQUANDER framework enables one to continue the optimization using a different engine. In particular we set a second order gradient descend method 'BFGS' 
+In order to achieve the best performance one can play around with the hyper-parameters in the map 'config'. (Optimization strategy AGENTS is good in avoiding local minima or get through flat areas of the optimization landscape. Then a gradient descend method can be used for faster convergence toward a solution.)
 
         # setting optimizer
         cDecompose.set_Optimizer("BFGS")
 
         # continue the decomposition with a second optimizer method
         cDecompose.get_Initial_Circuit()
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: squander Version: 1.8.3 Summary: Package to
+Metadata-Version: 2.1 Name: squander Version: 1.8.4 Summary: Package to
 decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta Maintainer-email: peter.rakyta@ttk.elte.hu License:
 GNU General Public License v3.0 Keywords: test,cmake,extension Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: Programming Language :: C Classifier: Programming Language :: C++
 Description-Content-Type: text/markdown License-File: LICENSE [![DOI](https://
@@ -84,31 +84,20 @@
 TBB_INC_DIR=path/to/TBB/include environment variables are sufficient for
 successful compilation. When the TBB library is installed via a python package,
 setting the environment variables above is not necessary. The SQUANDER package
 with C++ Python extensions can be compiled via the Python script **setup.py**
 located in the root directory of the SQUANDER package. The script automatically
 finds out the CBLAS library working behind the numpy package and uses it in
 further linking. The **setup.py** script also build the C++ library of the
-SQUANDER package by making the appropriate CMake calls. ### Build and Install
-on Microsoft Windows with Microsoft Visual C++ CMake must be in the path and
-able to find the MSVC compiler e.g. $ set PATH=%PATH%;C:\Program
-Files\cmake\bin Now set the TBB and BLAS folders and build via: $ set
-TBB_LOCATION=/LocalCache/local-packages $ set TBB_INC_DIR=%TBB_LOCATION%/
-Library/include $ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib $ set LIB=/lib;/
-lib $ python setup.py build_ext -DTBB_HEADER=\Library\include\ Installation
-merely requires copying DLL files (if they are not in the path): $ copy
-_skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition $ copy
-"%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition $ copy
-"%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition Verify
-the installation: $ python -m pytest ### Developer build We recommend to
-install the SQUANDER package in the Anaconda environment. In order to install
-the necessary requirements, follow the steps below: Creating new python
-environment: $ conda create -n qgd Activate the new anaconda environment $
-conda activate qgd Install dependencies: $ conda install numpy scipy pip pytest
-scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
+SQUANDER package by making the appropriate CMake calls. ### Developer build We
+recommend to install the SQUANDER package in the Anaconda environment. In order
+to install the necessary requirements, follow the steps below: Creating new
+python environment: $ conda create -n qgd Activate the new anaconda environment
+$ conda activate qgd Install dependencies: $ conda install numpy scipy pip
+pytest scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
 environment variables are set and the dependencies are installed, the
 compilation of the package can be started by the Python command: $ python3
 setup.py build_ext The command above starts the compilation of the SQUANDER C++
 library and builds the necessary C++ Python interface extensions of the
 SQUANDER package in place. After a successful build, one can register the
 SQUANDER package in the Python distribution in developer (i.e. editable) mode
 by command: $ python -m pip install -e . ### Binary distribution After the
@@ -128,35 +117,46 @@
 necessary to set the environment variables, since this script only collects the
 necessary files and pack them into a tar ball located in the directory **path/
 to/SQUANDER/package/dist**. In order to install the SQUANDER package from
 source tar ball, see the previous section discussing the initialization of the
 environment variables. The package can be compiled and installed by the command
 $ pip3 install qgd-*.tar.gz issued from directory **path/to/SQUANDER/package/
 dist** (It is optional to install the ninja package which speeds up the
-building process by parallel compilation.) ### How to use The algorithm
-implemented in the SQUANDER package intends to transform the given unitary into
-an identity matrix via a sequence of two-qubit and one-qubit gate operations
-applied on the unitary. Thus, in order to get the decomposition of a unitary,
-one should rather provide the complex transpose of this unitary as the input
-for the SQUANDER decomposing process, as can be seen in the examples. ## Python
+building process by parallel compilation.) ### Build and Install on Microsoft
+Windows with Microsoft Visual C++ CMake must be in the path and able to find
+the MSVC compiler e.g. $ set PATH=%PATH%;C:\Program Files\cmake\bin Now set the
+TBB and BLAS folders and build via: $ set TBB_LOCATION=/LocalCache/local-
+packages $ set TBB_INC_DIR=%TBB_LOCATION%/Library/include $ set
+TBB_LIB_DIR=%TBB_LOCATION%/Library/lib $ set LIB=/lib;/lib $ python setup.py
+build_ext -DTBB_HEADER=\Library\include\ Installation merely requires copying
+DLL files (if they are not in the path): $ copy _skbuild\win-amd64-3.9\cmake-
+install\bin .\qgd_python\decomposition $ copy
+"%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition $ copy
+"%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition Verify
+the installation: $ python -m pytest ### How to use The algorithm implemented
+in the SQUANDER package intends to transform the given unitary into an identity
+matrix via a sequence of two-qubit and one-qubit gate operations applied on the
+unitary. Thus, in order to get the decomposition of a unitary, one should
+rather provide the complex transpose of this unitary as the input for the
+SQUANDER decomposing process, as can be seen in the examples. ## Python
 Interface The SQUANDER package contains a Python interface allowing the access
 of the functionalities of the SQUANDER package from Python. The usage of the
 SQUANDER Python interface is demonstrated in the example files in the directory
 **examples** located in the directory **path/to/SQUANDER/package**, or in test
 files located in sub-directories of **path/to/SQUANDER/package/qgd_python/*/
 test**. ### Example code snippet Here we provide an example to use the SQUANDER
 package. The following python interface is accessible from version 1.8.0. In
 this example we use two optimization engines for the decomposition: 1. An
 evolutionary engine called AGENTS 2. Second order gradient descend algorithm
 (BFGS) Firstly we construct a Python map to set hyper-parameters during the
 gate synthesis. #Python map containing hyper-parameters config =
 { 'max_outer_iterations': 1, 'max_inner_iterations_agent': 25000,
 'max_inner_iterations_compression': 10000, 'max_inner_iterations' : 500,
 'max_inner_iterations_final': 5000, 'Randomized_Radius': 0.3,
-'randomized_adaptive_layers': 1, 'optimization_tolerance_agent': 1e-4,
+'randomized_adaptive_layers': 1, 'optimization_tolerance_agent': 1e-2,
 'optimization_tolerance': 1e-8, 'agent_num': 10} Next we initialize the
 decomposition class with the unitary Umtx to be decomposed. # creating a class
 to decompose the unitary from squander import N_Qubit_Decomposition_adaptive
 cDecompose = N_Qubit_Decomposition_adaptive( Umtx.conj().T, config=config ) The
 verbosity of the execution output can be controlled by the function call #
 setting the verbosity of the decomposition cDecompose.set_Verbose( 3 ) We
 construct the initial trial gate structure for the optimization consisting of 2
@@ -165,36 +165,40 @@
 layers to the gate structure levels = 2 for idx in range(levels):
 cDecompose.add_Adaptive_Layers()
 cDecompose.add_Finalyzing_Layer_To_Gate_Structure() We can construct an initial
 parameters set for the optimization by retrieving the number of free
 parameters. If the initial parameter set is not set, random parameters are used
 by default. # setting intial parameter set parameter_num =
 cDecompose.get_Parameter_Num() parameters = np.zeros( (parameter_num,1),
-dtype=np.float64 ) cDecompose.set_Optimized_Parameters( parameters ) We can use
-between several engines to solve the optimization problem. Here we use an
-evolutionary based algorithm named 'AGENTS' # setting optimizer
+dtype=np.float64 ) cDecompose.set_Optimized_Parameters( parameters ) We can
+choose between several engines to solve the optimization problem. Here we use
+an evolutionary based algorithm named 'AGENTS' # setting optimizer
 cDecompose.set_Optimizer("AGENTS") The optimization process is started by the
 function call # starting the decomposition cDecompose.get_Initial_Circuit() The
 optimization process terminates by either reaching the tolerance
 'optimization_tolerance_agent' or by reaching the maximal iteration number
 'max_inner_iterations_agent', or if the engines identifies a convergence to a
 local minimum. The SQUANDER framework enables one to continue the optimization
 using a different engine. In particular we set a second order gradient descend
-method 'BFGS' # setting optimizer cDecompose.set_Optimizer("BFGS") # continue
-the decomposition with a second optimizer method cDecompose.get_Initial_Circuit
-() After solving the optimization problem for the initial gate structure, we
-can initiate gate compression iterations. (This step can be omited.) # starting
-compression iterations cDecompose.Compress_Circuit() By finalizing the gate
-structure we replace the CRY gates with CNOT gates. (CRY gates with small
-rotation angle are approximately expressed with a single CNOT gate, so further
-optimization process needs to be initiated.) # finalize the gate structure
-(replace CRY gates with CNOT gates) cDecompose.Finalize_Circuit() Finally, we
-can retrieve the decomposed quantum circuit in QISKIT format. # get the
-decomposing operations quantum_circuit = cDecompose.get_Quantum_Circuit() ###
-How to cite us If you have found our work useful for your research project,
-please cite us by [1] PÃ©ter Rakyta, ZoltÃ¡n ZimborÃ¡s, Approaching the
-theoretical limit in quantum gate decomposition, Quantum 6, 710 (2022).
+method 'BFGS' In order to achieve the best performance one can play around with
+the hyper-parameters in the map 'config'. (Optimization strategy AGENTS is good
+in avoiding local minima or get through flat areas of the optimization
+landscape. Then a gradient descend method can be used for faster convergence
+toward a solution.) # setting optimizer cDecompose.set_Optimizer("BFGS") #
+continue the decomposition with a second optimizer method
+cDecompose.get_Initial_Circuit() After solving the optimization problem for the
+initial gate structure, we can initiate gate compression iterations. (This step
+can be omited.) # starting compression iterations cDecompose.Compress_Circuit()
+By finalizing the gate structure we replace the CRY gates with CNOT gates. (CRY
+gates with small rotation angle are approximately expressed with a single CNOT
+gate, so further optimization process needs to be initiated.) # finalize the
+gate structure (replace CRY gates with CNOT gates) cDecompose.Finalize_Circuit
+() Finally, we can retrieve the decomposed quantum circuit in QISKIT format. #
+get the decomposing operations quantum_circuit = cDecompose.get_Quantum_Circuit
+() ### How to cite us If you have found our work useful for your research
+project, please cite us by [1] PÃ©ter Rakyta, ZoltÃ¡n ZimborÃ¡s, Approaching
+the theoretical limit in quantum gate decomposition, Quantum 6, 710 (2022).
 [2] PÃ©ter Rakyta, ZoltÃ¡n ZimborÃ¡s, Efficient quantum gate decomposition via
 adaptive circuit compression, arXiv:2203.04426.
 [3] Peter Rakyta, Gregory Morse, Jakab NÃ¡dori, Zita Majnay-TakÃ¡cs, Oskar
 Mencer, ZoltÃ¡n ZimborÃ¡s, Highly optimized quantum circuits synthesized via
 data-flow engines, arXiv:2211.07685
```

### Comparing `squander-1.8.3/squander.egg-info/SOURCES.txt` & `squander-1.8.4/squander.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 CMakeLists.txt
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
-.pytest_cache/README.md
 cmake/check_AVX.cmake
 common/Adam.cpp
 common/common.cpp
 common/common_DFE.cpp
 common/config_element.cpp
 common/dot.cpp
 common/lbfgs.cpp
```

### Comparing `squander-1.8.3/test_standalone/CMakeLists.txt` & `squander-1.8.4/test_standalone/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/test_standalone/custom_gate_structure_test.cpp` & `squander-1.8.4/test_standalone/custom_gate_structure_test.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.3/test_standalone/decomposition_test.cpp` & `squander-1.8.4/test_standalone/decomposition_test.cpp`

 * *Files identical despite different names*

