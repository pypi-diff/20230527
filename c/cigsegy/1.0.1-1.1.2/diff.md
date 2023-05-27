# Comparing `tmp/cigsegy-1.0.1.tar.gz` & `tmp/cigsegy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cigsegy-1.0.1.tar", last modified: Thu Feb 16 11:03:14 2023, max compression
+gzip compressed data, was "dist/cigsegy-1.1.2.tar", last modified: Sat May 27 10:07:05 2023, max compression
```

## Comparing `cigsegy-1.0.1.tar` & `cigsegy-1.1.2.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 jtli      (1002) cig       (1016)        0 2023-02-16 11:03:13.000000 cigsegy-1.0.1/
--rw-r--r--   0 jtli      (1002) cig       (1016)      292 2023-02-16 11:03:13.000000 cigsegy-1.0.1/PKG-INFO
--rw-r--r--   0 jtli      (1002) cig       (1016)      133 2022-12-23 07:37:49.000000 cigsegy-1.0.1/MANIFEST.in
--rw-r--r--   0 jtli      (1002) cig       (1016)       38 2023-02-16 11:03:13.000000 cigsegy-1.0.1/setup.cfg
-drwxr-xr-x   0 jtli      (1002) cig       (1016)        0 2023-02-16 11:03:13.000000 cigsegy-1.0.1/src/
--rw-r--r--   0 jtli      (1002) cig       (1016)    34551 2023-02-16 10:59:35.000000 cigsegy-1.0.1/src/segy.cpp
-drwxr-xr-x   0 jtli      (1002) cig       (1016)        0 2023-02-16 11:03:13.000000 cigsegy-1.0.1/src/include/
--rw-r--r--   0 jtli      (1002) cig       (1016)    59848 2023-02-16 10:59:35.000000 cigsegy-1.0.1/src/include/mio.hpp
--rw-r--r--   0 jtli      (1002) cig       (1016)    10823 2023-02-16 10:59:35.000000 cigsegy-1.0.1/src/include/segy.h
--rw-r--r--   0 jtli      (1002) cig       (1016)     6011 2023-02-16 10:59:35.000000 cigsegy-1.0.1/src/include/progressbar.hpp
--rw-r--r--   0 jtli      (1002) cig       (1016)    11927 2023-02-16 10:59:35.000000 cigsegy-1.0.1/src/include/utils.h
-drwxr-xr-x   0 jtli      (1002) cig       (1016)        0 2023-02-16 11:03:13.000000 cigsegy-1.0.1/python/
--rw-r--r--   0 jtli      (1002) cig       (1016)     4396 2023-02-16 11:00:10.000000 cigsegy-1.0.1/python/tools.py
--rw-r--r--   0 jtli      (1002) cig       (1016)      427 2023-02-16 11:00:10.000000 cigsegy-1.0.1/python/__init__.py
--rw-r--r--   0 jtli      (1002) cig       (1016)      666 2023-02-16 11:00:10.000000 cigsegy-1.0.1/python/setup.py
--rw-r--r--   0 jtli      (1002) cig       (1016)     9674 2023-02-16 11:00:10.000000 cigsegy-1.0.1/python/PySegy.cpp
--rw-r--r--   0 jtli      (1002) cig       (1016)       46 2023-02-16 11:03:11.000000 cigsegy-1.0.1/python/version.py
--rw-r--r--   0 jtli      (1002) cig       (1016)     8641 2023-02-16 11:00:10.000000 cigsegy-1.0.1/python/cigsegy.pyi
--rw-r--r--   0 jtli      (1002) cig       (1016)     1066 2022-12-23 07:10:47.000000 cigsegy-1.0.1/LICENSE
--rw-r--r--   0 jtli      (1002) cig       (1016)      114 2022-12-23 07:44:04.000000 cigsegy-1.0.1/pyproject.toml
--rw-r--r--   0 jtli      (1002) cig       (1016)     1962 2023-02-16 11:01:24.000000 cigsegy-1.0.1/setup.py
-drwxr-xr-x   0 jtli      (1002) cig       (1016)        0 2023-02-16 11:03:13.000000 cigsegy-1.0.1/include/
-drwxr-xr-x   0 jtli      (1002) cig       (1016)        0 2023-02-16 11:03:13.000000 cigsegy-1.0.1/include/fmt/
--rw-r--r--   0 jtli      (1002) cig       (1016)   118325 2022-12-23 07:10:47.000000 cigsegy-1.0.1/include/fmt/format.h
--rw-r--r--   0 jtli      (1002) cig       (1016)    19898 2022-12-23 07:10:47.000000 cigsegy-1.0.1/include/fmt/compile.h
--rw-r--r--   0 jtli      (1002) cig       (1016)    11858 2022-12-23 07:10:47.000000 cigsegy-1.0.1/include/fmt/ranges.h
--rw-r--r--   0 jtli      (1002) cig       (1016)    50189 2022-12-23 07:10:47.000000 cigsegy-1.0.1/include/fmt/format-inl.h
--rw-r--r--   0 jtli      (1002) cig       (1016)     4607 2022-12-23 07:10:47.000000 cigsegy-1.0.1/include/fmt/ostream.h
--rw-r--r--   0 jtli      (1002) cig       (1016)     2870 2022-12-23 07:10:47.000000 cigsegy-1.0.1/include/fmt/locale.h
--rw-r--r--   0 jtli      (1002) cig       (1016)    21823 2022-12-23 07:10:47.000000 cigsegy-1.0.1/include/fmt/printf.h
--rw-r--r--   0 jtli      (1002) cig       (1016)    50435 2022-12-23 07:10:47.000000 cigsegy-1.0.1/include/fmt/core.h
--rw-r--r--   0 jtli      (1002) cig       (1016)    34822 2022-12-23 07:10:47.000000 cigsegy-1.0.1/include/fmt/chrono.h
--rw-r--r--   0 jtli      (1002) cig       (1016)     9025 2022-12-23 07:10:47.000000 cigsegy-1.0.1/include/fmt/posix.h
--rw-r--r--   0 jtli      (1002) cig       (1016)    22421 2022-12-23 07:10:47.000000 cigsegy-1.0.1/include/fmt/color.h
-drwxr-xr-x   0 jtli      (1002) cig       (1016)        0 2023-02-16 11:03:13.000000 cigsegy-1.0.1/cigsegy.egg-info/
--rw-r--r--   0 jtli      (1002) cig       (1016)      292 2023-02-16 11:03:12.000000 cigsegy-1.0.1/cigsegy.egg-info/PKG-INFO
--rw-r--r--   0 jtli      (1002) cig       (1016)        6 2023-02-16 11:03:12.000000 cigsegy-1.0.1/cigsegy.egg-info/requires.txt
--rw-r--r--   0 jtli      (1002) cig       (1016)        1 2023-02-16 11:03:12.000000 cigsegy-1.0.1/cigsegy.egg-info/dependency_links.txt
--rw-r--r--   0 jtli      (1002) cig       (1016)       24 2023-02-16 11:03:12.000000 cigsegy-1.0.1/cigsegy.egg-info/top_level.txt
--rw-r--r--   0 jtli      (1002) cig       (1016)      636 2023-02-16 11:03:12.000000 cigsegy-1.0.1/cigsegy.egg-info/SOURCES.txt
+drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.649687 cigsegy-1.1.2/
+-rw-r--r--   0 roger     (1000) roger     (1000)     1066 2023-05-27 10:03:26.000000 cigsegy-1.1.2/LICENSE
+-rw-r--r--   0 roger     (1000) roger     (1000)      133 2023-05-27 10:03:07.000000 cigsegy-1.1.2/MANIFEST.in
+-rw-rw-r--   0 roger     (1000) roger     (1000)      264 2023-05-27 10:07:05.645687 cigsegy-1.1.2/PKG-INFO
+drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.645687 cigsegy-1.1.2/cigsegy.egg-info/
+-rw-rw-r--   0 roger     (1000) roger     (1000)      264 2023-05-27 10:07:05.000000 cigsegy-1.1.2/cigsegy.egg-info/PKG-INFO
+-rw-rw-r--   0 roger     (1000) roger     (1000)      606 2023-05-27 10:07:05.000000 cigsegy-1.1.2/cigsegy.egg-info/SOURCES.txt
+-rw-rw-r--   0 roger     (1000) roger     (1000)        1 2023-05-27 10:07:05.000000 cigsegy-1.1.2/cigsegy.egg-info/dependency_links.txt
+-rw-rw-r--   0 roger     (1000) roger     (1000)        8 2023-05-27 10:07:05.000000 cigsegy-1.1.2/cigsegy.egg-info/top_level.txt
+drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.645687 cigsegy-1.1.2/include/
+drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.645687 cigsegy-1.1.2/include/fmt/
+-rw-r--r--   0 roger     (1000) roger     (1000)    34822 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/chrono.h
+-rw-r--r--   0 roger     (1000) roger     (1000)    22421 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/color.h
+-rw-r--r--   0 roger     (1000) roger     (1000)    19898 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/compile.h
+-rw-r--r--   0 roger     (1000) roger     (1000)    50435 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/core.h
+-rw-r--r--   0 roger     (1000) roger     (1000)    50189 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/format-inl.h
+-rw-r--r--   0 roger     (1000) roger     (1000)   118325 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/format.h
+-rw-r--r--   0 roger     (1000) roger     (1000)     2870 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/locale.h
+-rw-r--r--   0 roger     (1000) roger     (1000)     4607 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/ostream.h
+-rw-r--r--   0 roger     (1000) roger     (1000)     9025 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/posix.h
+-rw-r--r--   0 roger     (1000) roger     (1000)    21823 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/printf.h
+-rw-r--r--   0 roger     (1000) roger     (1000)    11858 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/ranges.h
+-rw-r--r--   0 roger     (1000) roger     (1000)      114 2023-05-27 10:03:36.000000 cigsegy-1.1.2/pyproject.toml
+drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.645687 cigsegy-1.1.2/python/
+-rw-r--r--   0 roger     (1000) roger     (1000)    12791 2023-05-27 09:54:05.000000 cigsegy-1.1.2/python/PySegy.cpp
+-rw-r--r--   0 roger     (1000) roger     (1000)      427 2023-05-27 09:54:05.000000 cigsegy-1.1.2/python/__init__.py
+-rw-r--r--   0 roger     (1000) roger     (1000)    10680 2023-05-27 09:54:05.000000 cigsegy-1.1.2/python/cigsegy.pyi
+-rw-r--r--   0 roger     (1000) roger     (1000)      695 2023-05-27 09:54:05.000000 cigsegy-1.1.2/python/setup.py
+-rw-r--r--   0 roger     (1000) roger     (1000)    11284 2023-05-27 09:54:05.000000 cigsegy-1.1.2/python/tools.py
+-rw-r--r--   0 roger     (1000) roger     (1000)       79 2023-05-27 10:07:05.000000 cigsegy-1.1.2/python/version.py
+-rw-rw-r--   0 roger     (1000) roger     (1000)       38 2023-05-27 10:07:05.649687 cigsegy-1.1.2/setup.cfg
+-rw-r--r--   0 roger     (1000) roger     (1000)     2281 2023-05-27 09:54:05.000000 cigsegy-1.1.2/setup.py
+drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.645687 cigsegy-1.1.2/src/
+drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.645687 cigsegy-1.1.2/src/include/
+-rw-r--r--   0 roger     (1000) roger     (1000)    59855 2023-05-27 09:54:04.000000 cigsegy-1.1.2/src/include/mio.hpp
+-rw-r--r--   0 roger     (1000) roger     (1000)     6009 2023-05-27 09:54:04.000000 cigsegy-1.1.2/src/include/progressbar.hpp
+-rw-r--r--   0 roger     (1000) roger     (1000)     6496 2023-05-27 09:54:04.000000 cigsegy-1.1.2/src/include/segy.h
+-rw-r--r--   0 roger     (1000) roger     (1000)    17167 2023-05-27 09:54:04.000000 cigsegy-1.1.2/src/include/utils.h
+-rw-r--r--   0 roger     (1000) roger     (1000)    37107 2023-05-27 09:54:04.000000 cigsegy-1.1.2/src/segy.cpp
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cigsegy-1.0.1/src/segy.cpp` & `cigsegy-1.1.2/src/segy.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,26 @@
 #include "segy.h"
 #include <chrono>
 #include <cstring>
 #define FMT_HEADER_ONLY
 #include <fmt/format.h>
 #include <stdexcept>
 
+#ifdef WIN32
+#include <fcntl.h>
+#include <io.h>
+#define open _open
+#define lseek _lseek
+#define close _close
+#define write _write
+#define O_RDWR _O_RDWR
+#define O_CREAT _O_CREAT
+#define O_TRUNC _O_TRUNC
+#endif
+
 #include "mio.hpp"
 #include "progressbar.hpp"
 #include "utils.h"
 
 namespace segy {
 
 SegyIO::SegyIO(const std::string &segyname) {
@@ -59,33 +71,34 @@
 SegyIO::~SegyIO() {
   if (m_source.is_mapped()) {
     m_source.unmap();
   }
 }
 
 void SegyIO::setInlineLocation(int loc) {
-  if (loc != 5 && loc != 9 && loc != 189) {
-    fmt::print("[Warning]: You set a unusual inline field: {}, the best choice "
-               "is setting it as 189 or 5 or 9.\n",
-               loc);
-  }
+  // if (loc != 5 && loc != 9 && loc != 189) {
+  //   fmt::print("[Warning]: You set a unusual inline field: {}, the best
+  //   choice "
+  //              "is setting it as 189 or 5 or 9.\n",
+  //              loc);
+  // }
   if (loc <= 0) {
     throw std::runtime_error("Invalid location (must > 0)");
   }
   m_metaInfo.inline_field = loc;
   isScan = false;
 }
 
 void SegyIO::setCrosslineLocation(int loc) {
-  if (loc != 193 && loc != 17 && loc != 21) {
-    fmt::print(
-        "[Warning]: You set a unusual crossline field: {}, the best choice "
-        "is set it as 193 or 17 or 21.\n",
-        loc);
-  }
+  // if (loc != 193 && loc != 17 && loc != 21) {
+  //   fmt::print(
+  //       "[Warning]: You set a unusual crossline field: {}, the best choice "
+  //       "is set it as 193 or 17 or 21.\n",
+  //       loc);
+  // }
   if (loc <= 0) {
     throw std::runtime_error("Invalid location (must > 0)");
   }
   m_metaInfo.crossline_field = loc;
   isScan = false;
 }
 
@@ -111,14 +124,33 @@
   if (loc <= 0) {
     throw std::runtime_error("Invalid location (must > 0)");
   }
   m_metaInfo.Y_field = loc;
   isScan = false;
 }
 
+void SegyIO::setInlineStep(int step) {
+  if (step <= 0) {
+    throw std::runtime_error("Invalid inline step (must > 0)");
+  }
+  m_metaInfo.inline_step = step;
+}
+
+void SegyIO::setCrosslineStep(int step) {
+  if (step <= 0) {
+    throw std::runtime_error("Invalid crossline step (must > 0)");
+  }
+  m_metaInfo.crossline_step = step;
+}
+
+void SegyIO::setSteps(int istep, int xstep) {
+  setInlineStep(istep);
+  setCrosslineStep(xstep);
+}
+
 void SegyIO::setFillNoValue(float noValue) {
   m_metaInfo.fillNoValue = noValue;
   isScan = false;
 }
 
 void SegyIO::setSampleInterval(int dt) {
   if (dt <= 0) {
@@ -185,14 +217,21 @@
   m_metaInfo.sizeX = swap_endian(binary_header->trace_length);
   m_metaInfo.sample_interval = swap_endian(binary_header->sample_interval);
   m_metaInfo.trace_count =
       (m_source.size() - kTextualHeaderSize - kBinaryHeaderSize) /
       (kTraceHeaderSize + m_metaInfo.sizeX * sizeof(float));
 }
 
+void SegyIO::get_TraceInfo(int n, int *traceinfo) {
+  if (m_metaInfo.trace_count <= n || n < 0) {
+    throw std::runtime_error("the trace number must be in [0, ntrace-1)");
+  }
+  _get_TraceInfo(n, *reinterpret_cast<TraceInfo *>(traceinfo));
+}
+
 void SegyIO::scan() {
   if (!isReadSegy) {
     throw std::runtime_error(
         "'scan()' function only used in reading segy mode.");
   }
 
   isScan = true;
@@ -207,30 +246,37 @@
   if (m_metaInfo.X_field == 0) {
     m_metaInfo.X_field = kDefaultXField;
   }
   if (m_metaInfo.Y_field == 0) {
     m_metaInfo.Y_field = kDefaultYField;
   }
 
+  if (m_metaInfo.inline_step <= 0) {
+    m_metaInfo.inline_step = 1;
+  }
+  if (m_metaInfo.crossline_step <= 0) {
+    m_metaInfo.crossline_step = 1;
+  }
+
   // get sizeZ, i.e. line_count
   int trace_size = m_metaInfo.sizeX * sizeof(float) + kTraceHeaderSize;
   const char *start = m_source.data() + kTextualHeaderSize + kBinaryHeaderSize;
   m_metaInfo.start_time = swap_endian(
       *reinterpret_cast<const int16_t *>(start + kTStartTimeField - 1));
   m_metaInfo.scalar = swap_endian(
       *reinterpret_cast<const int16_t *>(start + kTScalarField - 1));
 
   // line x: ... trace1
   // line x+1: trace2 ...
   TraceInfo trace1{}, trace2{};
-  get_TraceInfo(start, trace1);
-  get_TraceInfo(start + static_cast<uint64_t>(m_metaInfo.trace_count - 1) *
-                            trace_size,
-                trace2);
-  m_metaInfo.sizeZ = trace2.inline_num - trace1.inline_num + 1;
+  _get_TraceInfo(0, trace1);
+  _get_TraceInfo(m_metaInfo.trace_count - 1, trace2);
+
+  m_metaInfo.sizeZ =
+      (trace2.inline_num - trace1.inline_num) / m_metaInfo.inline_step + 1;
   m_metaInfo.min_inline = trace1.inline_num;
   m_metaInfo.max_inline = trace2.inline_num;
 
   // init this two field
   m_metaInfo.min_crossline = trace1.crossline_num;
   m_metaInfo.max_crossline = trace2.crossline_num;
 
@@ -245,87 +291,96 @@
       m_metaInfo.trace_count % m_metaInfo.sizeZ == 0 ? true : false;
   m_lineInfo.resize(m_metaInfo.sizeZ);
 
   // fill m_lineInfo
   int jump = m_metaInfo.trace_count / m_metaInfo.sizeZ;
   m_metaInfo.sizeY = jump;
   int64_t itrace = 0;
-  get_TraceInfo(start, trace2);
+  _get_TraceInfo(0, trace2);
   for (int i = 0; i < m_metaInfo.sizeZ - 1; i++) {
     m_lineInfo[i].trace_start = itrace;
     m_lineInfo[i].line_num = trace2.inline_num;
     m_lineInfo[i].count = 1;
 
     if (trace2.crossline_num < m_metaInfo.min_crossline) {
       m_metaInfo.min_crossline = trace2.crossline_num;
     }
 
     itrace += jump;
-    get_TraceInfo(start + itrace * trace_size, trace2);
-    get_TraceInfo(start + (itrace - 1) * trace_size, trace1);
+    if (itrace >= m_metaInfo.trace_count) {
+      jump -= (itrace - m_metaInfo.trace_count + 1);
+      itrace = m_metaInfo.trace_count - 1;
+    }
+
+    _get_TraceInfo(itrace, trace2);
+    _get_TraceInfo(itrace - 1, trace1);
 
     if (trace2.inline_num == m_lineInfo[i].line_num) {
       m_metaInfo.isNormalSegy = false;
-      while (trace2.inline_num != m_lineInfo[i].line_num + 1 &&
+      while (trace2.inline_num !=
+                 m_lineInfo[i].line_num + m_metaInfo.inline_step &&
              itrace < m_metaInfo.trace_count &&
              m_metaInfo.sizeY <= kMaxSizeOneDimemsion) {
         itrace++;
         jump++;
         if (jump > kMaxSizeOneDimemsion || itrace >= m_metaInfo.trace_count) {
           throw std::runtime_error(
               "inline/crossline location is wrong, use "
               "'setInlineLocation(loc)'/'setCrosslineLocation(loc)' to set");
         }
-        get_TraceInfo(start + itrace * trace_size, trace2);
-      }
-      if (jump > m_metaInfo.sizeY) {
-        m_metaInfo.sizeY = jump;
+        _get_TraceInfo(itrace, trace2);
       }
+      // if (jump > m_metaInfo.sizeY) {
+      //   m_metaInfo.sizeY = jump;
+      // }
     } else if (trace1.inline_num > m_lineInfo[i].line_num) {
       m_metaInfo.isNormalSegy = false;
       while (trace1.inline_num != m_lineInfo[i].line_num && itrace > 0 &&
              jump > 0) {
         itrace--;
         jump--;
         if (jump <= 0 || itrace <= 0) {
           throw std::runtime_error(
               "inline/crossline location is wrong, use "
               "'setInlineLocation(loc)'/'setCrosslineLocation(loc)' to set");
         }
         trace2 = trace1;
-        get_TraceInfo(start + (itrace - 1) * trace_size, trace1);
+        _get_TraceInfo(itrace - 1, trace1);
       }
     }
 
-    if (trace2.inline_num == m_lineInfo[i].line_num + 1 &&
+    m_metaInfo.sizeY = m_metaInfo.max_crossline - m_metaInfo.min_crossline + 1;
+
+    if (trace2.inline_num == m_lineInfo[i].line_num + m_metaInfo.inline_step &&
         trace1.inline_num == m_lineInfo[i].line_num) {
       if (trace1.crossline_num > m_metaInfo.max_crossline) {
         m_metaInfo.max_crossline = trace1.crossline_num;
       }
       m_lineInfo[i].trace_end = itrace - 1;
       m_lineInfo[i].count = itrace - m_lineInfo[i].trace_start;
     } else {
-      throw std::runtime_error("Cannot analysis this segy file");
+      throw std::runtime_error("Cannot analysis this segy file, "
+                               "may inline step != 1");
     }
   }
 
   // the last line
   m_lineInfo[m_metaInfo.sizeZ - 1].trace_start = itrace;
   m_lineInfo[m_metaInfo.sizeZ - 1].line_num = trace2.inline_num;
   m_lineInfo[m_metaInfo.sizeZ - 1].trace_end = m_metaInfo.trace_count - 1;
   m_lineInfo[m_metaInfo.sizeZ - 1].count = m_metaInfo.trace_count - itrace;
 
   // cal x, y interval
-  get_TraceInfo(start, trace1);
-  get_TraceInfo(start + m_lineInfo[0].trace_end * trace_size, trace2);
+  _get_TraceInfo(0, trace1);
+  _get_TraceInfo(m_lineInfo[0].trace_end, trace2);
   m_metaInfo.Y_interval = std::sqrt(std::pow(trace2.X - trace1.X, 2) +
                                     std::pow(trace2.Y - trace1.Y, 2)) /
                           m_lineInfo[0].count;
   int num = m_metaInfo.trace_count > 10 ? 10 : m_metaInfo.trace_count - 1;
-  get_TraceInfo(start + m_lineInfo[num].trace_start * trace_size, trace2);
+  _get_TraceInfo(m_lineInfo[num].trace_start, trace2);
   m_metaInfo.Z_interval =
       std::sqrt(std::pow(trace2.X - trace1.X, 2) +
                 std::pow(trace2.Y - trace1.Y, 2) -
                 std::pow((trace2.crossline_num - trace1.crossline_num) *
                              m_metaInfo.Y_interval,
                          2)) /
       (trace2.inline_num - trace1.inline_num);
@@ -368,43 +423,44 @@
                                ? static_cast<uint64_t>(iZ) * m_metaInfo.sizeY
                                : m_lineInfo[iZ].trace_start;
     const char *sourceline = source + trace_start * trace_size;
     bool normal = true;
     if (!m_metaInfo.isNormalSegy) {
       normal = m_lineInfo[iZ].count == m_metaInfo.sizeY ? true : false;
       if (!normal) {
-        int dst_crossline = m_metaInfo.min_crossline + startY;
+        int dst_crossline =
+            m_metaInfo.min_crossline + startY * m_metaInfo.crossline_step;
         while (getCrossline(sourceline + istart * trace_size,
                             m_metaInfo.crossline_field) > dst_crossline &&
                istart > 0) {
           istart--;
         }
       }
     }
 
     for (int iY = startY; iY < endY; iY++) {
       float *dsttrace = dstline + (iY - startY) * sizeX;
-      if (normal || getCrossline(sourceline + istart * trace_size,
-                                 m_metaInfo.crossline_field) ==
-                        (m_metaInfo.min_crossline + iY)) {
+      if (normal ||
+          getCrossline(sourceline + istart * trace_size,
+                       m_metaInfo.crossline_field) ==
+              (m_metaInfo.min_crossline + iY * m_metaInfo.crossline_step)) {
         memcpy(dsttrace, sourceline + istart * trace_size + offset,
                sizeX * sizeof(float));
         for (int iX = 0; iX < sizeX; iX++) {
           if (m_metaInfo.data_format == 1) {
             dsttrace[iX] = ibm_to_ieee(dsttrace[iX], true);
           } else if (m_metaInfo.data_format == 5) {
             dsttrace[iX] = swap_endian(dsttrace[iX]);
           } else {
             throw std::runtime_error("Unsuport sample format");
           }
         }
         istart++;
       } else {
-        std::fill(dsttrace, dstline + (iY - startY + 1) * sizeX,
-                  m_metaInfo.fillNoValue);
+        std::fill(dsttrace, dsttrace + sizeX, m_metaInfo.fillNoValue);
       }
     }
     // #pragma omp critical
     bar.update();
   }
   fmt::print("\n");
 
@@ -467,21 +523,21 @@
     if (write(fd, "", 1) < 0) {
       throw std::runtime_error("create file failed");
     }
     if (need_size > kMaxLSeekSize) {
       need_size -= kMaxLSeekSize;
     }
   }
+  close(fd);
 
   std::error_code error;
-  mio::mmap_sink rw_mmap = mio::make_mmap_sink(fd, error);
+  mio::mmap_sink rw_mmap = mio::make_mmap_sink(binary_out_name, error);
   if (error) {
     throw std::runtime_error("mmap fail when write data");
   }
-  close(fd);
   // or need split into serveral chunks?
   read(reinterpret_cast<float *>(rw_mmap.data()));
   rw_mmap.unmap();
 }
 
 std::string SegyIO::metaInfo() {
   if (!isScan && isReadSegy) {
@@ -500,24 +556,27 @@
                      ? m_metaInfo.Z_interval * m_metaInfo.scalar
                      : m_metaInfo.Z_interval / -m_metaInfo.scalar;
   }
 
   std::string dformat = m_metaInfo.data_format == 1
                             ? "4-bytes IBM floating-point"
                             : "4-bytes IEEE floating-point";
-  return fmt::format(
-      "shape: (n-time, n-crossline, n-inline) = ({}, {}, {})\nsample interval: "
-      "{}, data format code: {}\ninline "
-      "start: {}, crossline start: {}\nX interval: {:.1f}, Y interval: {:.1f}, "
-      "time "
-      "start: {}\nIs regular file (no missing traces): {}",
-      m_metaInfo.sizeX, m_metaInfo.sizeY, m_metaInfo.sizeZ,
-      m_metaInfo.sample_interval, dformat, m_metaInfo.min_inline,
-      m_metaInfo.min_crossline, Y_interval, Z_interval, m_metaInfo.start_time,
-      m_metaInfo.isNormalSegy);
+  return fmt::format("shape: (n-time, n-crossline, n-inline) = ({}, {}, {})\n"
+                     "sample interval: {}, data format code: {}\n"
+                     "inline start: {}, crossline start: {}\n"
+                     "X interval: {:.1f}, Y interval: {:.1f}, time start: {}\n"
+                     "inline field: {}, crossline field: {}\n"
+                     "inline step: {}, crossline step: {}\n"
+                     "Is regular file (no missing traces): {}",
+                     m_metaInfo.sizeX, m_metaInfo.sizeY, m_metaInfo.sizeZ,
+                     m_metaInfo.sample_interval, dformat, m_metaInfo.min_inline,
+                     m_metaInfo.min_crossline, Y_interval, Z_interval,
+                     m_metaInfo.start_time, m_metaInfo.inline_field,
+                     m_metaInfo.crossline_field, m_metaInfo.inline_step,
+                     m_metaInfo.crossline_step, m_metaInfo.isNormalSegy);
 }
 
 std::string SegyIO::textual_header() {
   if (!isReadSegy && m_sink.size() < kTextualHeaderSize) {
     throw std::runtime_error(
         "No textual header, because this is not a segy "
         "file (read mode) or you don't create textual header (create mode)");
@@ -567,21 +626,21 @@
     if (write(fd, "", 1) < 0) {
       throw std::runtime_error("create file failed");
     }
     if (need_size > kMaxLSeekSize) {
       need_size -= kMaxLSeekSize;
     }
   }
+  close(fd);
 
   std::error_code error;
-  mio::mmap_sink rw_mmap = mio::make_mmap_sink(fd, error);
+  mio::mmap_sink rw_mmap = mio::make_mmap_sink(segy_out_name, error);
   if (error) {
     throw std::runtime_error("mmap fail when write data");
   }
-  close(fd);
 
   write_textual_header(rw_mmap.data(), segy_out_name);
   write_binary_header(rw_mmap.data() + kTextualHeaderSize);
   TraceHeader trace_header{};
   initTraceHeader(&trace_header);
   char *dst = rw_mmap.data() + kTextualHeaderSize + kBinaryHeaderSize;
   char *dstline = dst;
@@ -808,43 +867,45 @@
   const char *source = m_source.data() + kTextualHeaderSize + kBinaryHeaderSize;
   int32_t trace_size = m_metaInfo.sizeX * sizeof(float) + kTraceHeaderSize;
   progressbar bar(100);
   for (int i = 0; i < m_metaInfo.trace_count; i++) {
     if (i % (m_metaInfo.trace_count / 100) == 0) {
       bar.update();
     }
-    get_TraceInfo(source + i * trace_size,
-                  *reinterpret_cast<TraceInfo *>(header));
+    _get_TraceInfo(i, *reinterpret_cast<TraceInfo *>(header));
     memcpy(data, source + kTraceHeaderSize, m_metaInfo.sizeX * sizeof(float));
     for (int j = 0; j < m_metaInfo.sizeX; j++) {
       if (m_metaInfo.data_format == 1) {
         data[j] = ibm_to_ieee(data[j], true);
       } else {
         data[j] = swap_endian(data[j]);
       }
     }
     data += m_metaInfo.sizeX;
     header += 4;
   }
 }
 
-void read(const std::string &segy_name, float *dst, int iline, int xline) {
+void read(const std::string &segy_name, float *dst, int iline, int xline,
+          int istep, int xstep) {
   SegyIO segy_data(segy_name);
   segy_data.setInlineLocation(iline);
   segy_data.setCrosslineLocation(xline);
+  segy_data.setSteps(istep, xstep);
   segy_data.scan();
   segy_data.read(dst);
   segy_data.close_file();
 }
 
 void tofile(const std::string &segy_name, const std::string &out_name,
-            int iline, int xline) {
+            int iline, int xline, int istep, int xstep) {
   SegyIO segy_data(segy_name);
   segy_data.setInlineLocation(iline);
   segy_data.setCrosslineLocation(xline);
+  segy_data.setSteps(istep, xstep);
   segy_data.scan();
   segy_data.tofile(out_name);
   segy_data.close_file();
 }
 
 void read_ignore_header(const std::string &segy_name, float *dst, int sizeX,
                         int sizeY, int sizeZ, int format) {
@@ -864,18 +925,19 @@
   segy_data.tofile(out_name);
   segy_data.close_file();
 }
 
 void create_by_sharing_header(const std::string &segy_name,
                               const std::string &header_segy, const float *src,
                               int sizeX, int sizeY, int sizeZ, int iline,
-                              int xline) {
+                              int xline, int istep, int xstep) {
   SegyIO header(header_segy);
   header.setInlineLocation(iline);
   header.setCrosslineLocation(xline);
+  header.setSteps(istep, xstep);
   header.scan();
   auto line_info = header.line_info();
   auto meta_info = header.get_metaInfo();
   auto trace_count = header.trace_count();
   header.close_file();
 
   if (meta_info.sizeY != sizeY || meta_info.sizeZ != sizeZ ||
@@ -898,21 +960,21 @@
     if (write(fd, "", 1) < 0) {
       throw std::runtime_error("create file failed");
     }
     if (need_size > kMaxLSeekSize) {
       need_size -= kMaxLSeekSize;
     }
   }
+  close(fd);
 
   std::error_code error;
-  mio::mmap_sink rw_mmap = mio::make_mmap_sink(fd, error);
+  mio::mmap_sink rw_mmap = mio::make_mmap_sink(segy_name, error);
   if (error) {
     throw std::runtime_error("mmap fail when write data");
   }
-  close(fd);
 
   mio::mmap_source m_source;
   m_source.map(header_segy, error);
   if (error) {
     throw std::runtime_error("Cannot mmap segy file");
   }
 
@@ -963,8 +1025,28 @@
   }
   fmt::print("\n");
 
   m_source.unmap();
   rw_mmap.unmap();
 }
 
+// if src is very huge, memmap it
+void create_by_sharing_header(const std::string &segy_name,
+                              const std::string &header_segy,
+                              const std::string &src_file, int sizeX, int sizeY,
+                              int sizeZ, int iline, int xline, int istep,
+                              int xstep) {
+  mio::mmap_source m_src;
+  std::error_code error;
+  m_src.map(src_file, error);
+  if (error) {
+    throw std::runtime_error("Cannot mmap segy file");
+  }
+
+  const float *src = reinterpret_cast<const float *>(m_src.data());
+  create_by_sharing_header(segy_name, header_segy, src, sizeX, sizeY, sizeZ,
+                           iline, xline, istep, xstep);
+
+  m_src.unmap();
+}
+
 } // namespace segy
```

### Comparing `cigsegy-1.0.1/src/include/mio.hpp` & `cigsegy-1.1.2/src/include/mio.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -790,15 +790,15 @@
 
 /** Returns the 4 lower bytes of an 8-byte integer. */
 inline DWORD int64_low(int64_t n) noexcept
 {
     return n & 0xffffffff;
 }
 
-std::wstring s_2_ws(const std::string& s)
+inline std::wstring s_2_ws(const std::string& s)
 {
     if (s.empty())
         return{};
     const auto s_length = static_cast<int>(s.length());
     auto buf = std::vector<wchar_t>(s_length);
     const auto wide_char_count = MultiByteToWideChar(CP_UTF8, 0, s.c_str(), s_length, buf.data(), s_length);
     return std::wstring(buf.data(), wide_char_count);
```

### Comparing `cigsegy-1.0.1/src/include/progressbar.hpp` & `cigsegy-1.1.2/src/include/progressbar.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -134,24 +134,24 @@
       output << "0%";
   }
   update_is_called = true;
 
   int perc = 0;
 
   // compute percentage, if did not change, do nothing and return
-  perc = progress * 100. / (n_cycles - 1);
+  perc = progress * 100 / (n_cycles - 1);
   if (perc < last_perc)
     return;
 
   // update percentage each unit
   if (perc == last_perc + 1) {
     // erase the correct  number of characters
     if (perc <= 10)
       output << "\b\b" << perc << '%';
-    else if (perc > 10 and perc < 100)
+    else if (perc > 10 && perc < 100)
       output << "\b\b\b" << perc << '%';
     else if (perc == 100)
       output << "\b\b\b" << perc << '%';
   }
   if (do_show_bar == true) {
     // update bar every ten units
     if (perc % 2 == 0) {
```

### Comparing `cigsegy-1.0.1/python/setup.py` & `cigsegy-1.1.2/python/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,16 +9,16 @@
             _bdist_wheel.finalize_options(self)
             self.root_is_pure = False
 except ImportError:
     bdist_wheel = None
 
 setup(
     name='cigsegy',
-    version='1.0.1',
+    version='1.1.2',
     description=
     'A tool for segy-format file reading and segy-format creating from binary file',
     author='roger',
     url='https://github.com/JintaoLee-Roger/cigsegy',
     license='MIT',
     cmdclass={'bdist_wheel': bdist_wheel},
     packages=find_packages(),
-    package_data={'': ['*.so']})
+    package_data={'': ['*.so', '*.dylib', '*.pyd', '*.pyi']})
```

### Comparing `cigsegy-1.0.1/python/PySegy.cpp` & `cigsegy-1.1.2/python/PySegy.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -8,39 +8,64 @@
 ** @Version: 1.0
 ** @Description :
 *********************************************************************/
 
 #include "segy.h"
 #include <pybind11/numpy.h>
 #include <pybind11/pybind11.h>
-#include <utility>
+#include <stdexcept>
 
 namespace py = pybind11;
 
 class Pysegy : public segy::SegyIO {
 public:
   using segy::SegyIO::create;
   using segy::SegyIO::read;
   using segy::SegyIO::read_cross_slice;
   using segy::SegyIO::read_inline_slice;
   using segy::SegyIO::read_time_slice;
   using segy::SegyIO::read_trace;
   using segy::SegyIO::SegyIO;
 
+  py::array_t<int> get_traceInfo(int n);
+  py::array_t<int> get_traceInfo(int beg, int end);
+
   py::array_t<float> read(int startZ, int endZ, int startY, int endY,
                           int startX, int endX);
   py::array_t<float> read();
   py::array_t<float> read_inline_slice(int iZ);
   py::array_t<float> read_cross_slice(int iY);
   py::array_t<float> read_time_slice(int iX);
   py::array_t<float> read_trace(int iZ, int iY);
 
   void create(const std::string &segy_out_name, const py::array_t<float> &src);
 };
 
+py::array_t<int> Pysegy::get_traceInfo(int n) {
+  py::array_t<int> traceinfo(4);
+  int *ptr = static_cast<int *>(traceinfo.request().ptr);
+  get_TraceInfo(n, ptr);
+  return traceinfo;
+}
+
+py::array_t<int> Pysegy::get_traceInfo(int beg, int end) {
+  if (beg < 0 || beg >= trace_count() || end <= beg || end > trace_count()) {
+    throw std::runtime_error("Invalid index");
+  }
+  int n = end - beg;
+  py::array_t<int> traceinfo({n, 4});
+  int *ptr = static_cast<int *>(traceinfo.request().ptr);
+
+  for (int i = beg; i < end; i++) {
+    get_TraceInfo(i, ptr);
+    ptr += 4;
+  }
+  return traceinfo;
+}
+
 // Be careful the order of the dimensions
 // In segy, X (time) is the first, but when you read into python,
 // Z (inline) is the first. If need change it to X first,
 // use data.transpose() in python
 py::array_t<float> Pysegy::read(int startZ, int endZ, int startY, int endY,
                                 int startX, int endX) {
 
@@ -111,42 +136,58 @@
   float *ptr = static_cast<float *>(buff.ptr);
   create(segy_out_name, ptr);
 }
 
 void create_by_sharing_header(const std::string &segy_name,
                               const std::string &header_segy,
                               const py::array_t<float> &src, int iline = 189,
-                              int xline = 193) {
+                              int xline = 193, int istep = 1, int xstep = 1) {
   auto buff = src.request();
   if (buff.ndim != 3) {
     throw std::runtime_error("Input data must be a 3D data.");
   }
 
   auto r = src.unchecked<3>();
   float *ptr = static_cast<float *>(buff.ptr);
 
   segy::create_by_sharing_header(segy_name, header_segy, ptr, r.shape(2),
-                                 r.shape(1), r.shape(0), iline, xline);
+                                 r.shape(1), r.shape(0), iline, xline, istep,
+                                 xstep);
+}
+
+void create_by_sharing_header(const std::string &segy_name,
+                              const std::string &header_segy,
+                              const std::string &src_file,
+                              const py::sequence &shape, int iline = 189,
+                              int xline = 193, int istep = 1, int xstep = 1) {
+  if (shape.size() != 3) {
+    throw std::runtime_error("dimensions must be 3");
+  }
+  segy::create_by_sharing_header(
+      segy_name, header_segy, src_file, py::cast<int>(shape[2]),
+      py::cast<int>(shape[1]), py::cast<int>(shape[0]), iline, xline, istep,
+      xstep);
 }
 
 py::array_t<float> fromfile_ignore_header(const std::string &segy_name,
                                           int sizeZ, int sizeY, int sizeX,
                                           int format = 5) {
   py::array_t<float> out({sizeZ, sizeY, sizeX});
   auto buff = out.request();
   float *ptr = static_cast<float *>(buff.ptr);
   segy::read_ignore_header(segy_name, ptr, sizeX, sizeY, sizeZ, format);
   return out;
 }
 
 py::array_t<float> fromfile(const std::string &segy_name, int iline = 189,
-                            int xline = 193) {
+                            int xline = 193, int istep = 1, int xstep = 1) {
   Pysegy segy_data(segy_name);
   segy_data.setInlineLocation(iline);
   segy_data.setCrosslineLocation(xline);
+  segy_data.setSteps(istep, xstep);
   segy_data.scan();
   py::array_t<float> out = segy_data.read();
 
   return out;
 }
 
 std::pair<py::array_t<float>, py::array_t<int>>
@@ -177,19 +218,27 @@
 using overload_cast_ = pybind11::detail::overload_cast_impl<Args...>;
 
 PYBIND11_MODULE(cigsegy, m) {
   py::class_<Pysegy>(m, "Pysegy")
       .def(py::init<std::string>())
       .def(py::init<int, int, int>())
       .def(py::init<std::string, int, int, int>())
+      .def("trace_cout", &Pysegy::trace_count)
+      .def("get_traceInfo", overload_cast_<int>()(&Pysegy::get_traceInfo),
+           py::arg("n"))
+      .def("get_traceInfo", overload_cast_<int, int>()(&Pysegy::get_traceInfo),
+           py::arg("beg"), py::arg("end"))
       .def("setInlineLocation", &Pysegy::setInlineLocation, py::arg("iline"))
       .def("setCrosslineLocation", &Pysegy::setCrosslineLocation,
            py::arg("xline"))
       .def("setXLocation", &Pysegy::setXLocation, py::arg("xfield"))
       .def("setYLocation", &Pysegy::setYLocation, py::arg("yfield"))
+      .def("setInlineStep", &Pysegy::setInlineStep, py::arg("step"))
+      .def("setCrosslineStep", &Pysegy::setCrosslineStep, py::arg("step"))
+      .def("setSteps", &Pysegy::setSteps, py::arg("istep"), py::arg("xstep"))
       .def("setFillNoValue", &Pysegy::setFillNoValue, py::arg("fills"))
       .def("scan", &Pysegy::scan)
       .def("tofile", &Pysegy::tofile, py::arg("binary_out_name"))
       .def("read", overload_cast_<>()(&Pysegy::read), "read hole volume")
       .def("read",
            overload_cast_<int, int, int, int, int, int>()(&Pysegy::read),
            "read with index", py::arg("startZ"), py::arg("endZ"),
@@ -209,38 +258,57 @@
       .def("setStartTime", &Pysegy::setStartTime, py::arg("start_time"))
       .def("setXInterval", &Pysegy::setXInterval, py::arg("dx"))
       .def("setYInterval", &Pysegy::setYInterval, py::arg("dy"))
       .def("setMinInline", &Pysegy::setMinInline, py::arg("minInline"))
       .def("setMinCrossline", &Pysegy::setMinCrossline, py::arg("minXline"))
       .def("textual_header", &Pysegy::textual_header)
       .def("metaInfo", &Pysegy::metaInfo)
-      .def("create", overload_cast_<const std::string &>()(&Pysegy::create),
+ //     .def("create", overload_cast_<const std::string &>()(&Pysegy::create),
+ //          "create a segy", py::arg("segy_out_name"))
+ //     .def("create",
+ //          overload_cast_<const std::string &,
+ //                         const pybind11::array_t<float> &>()(&Pysegy::create),
+ //          "create a segy from memory", py::arg("segy_out_name"),
+ //          py::arg("src"))
+      .def("create", static_cast<void (Pysegy::*)(const std::string &)>(&Pysegy::create),
            "create a segy", py::arg("segy_out_name"))
       .def("create",
-           overload_cast_<const std::string &,
-                          const pybind11::array_t<float> &>()(&Pysegy::create),
+          static_cast<void (Pysegy::*)(const std::string&, const py::array_t<float>&)>(&Pysegy::create),
            "create a segy from memory", py::arg("segy_out_name"),
            py::arg("src"))
       .def("set_size", &Pysegy::set_size, py::arg("sizeX"), py::arg("sizeY"),
            py::arg("sizeZ"))
       .def("close_file", &Pysegy::close_file);
 
   m.def("fromfile_ignore_header", &fromfile_ignore_header,
         "read by ignoring header and specify shape", py::arg("segy_name"),
         py::arg("sizeZ"), py::arg("sizeY"), py::arg("sizeX"),
         py::arg("format") = 5);
   m.def("fromfile", &fromfile, "read from a file", py::arg("segy_name"),
-        py::arg("iline") = 189, py::arg("xline") = 193);
+        py::arg("iline") = 189, py::arg("xline") = 193, py::arg("istep") = 1,
+        py::arg("xstep") = 1);
   m.def("tofile_ignore_header", &segy::tofile_ignore_header,
         "convert to binary file by ignoring header and specify shape",
         py::arg("segy_name"), py::arg("out_name"), py::arg("sizeX"),
         py::arg("sizeY"), py::arg("sizeZ"), py::arg("format") = 5);
   m.def("tofile", &segy::tofile, "convert to binary file", py::arg("segy_name"),
-        py::arg("out_name"), py::arg("iline") = 189, py::arg("xline") = 193);
+        py::arg("out_name"), py::arg("iline") = 189, py::arg("xline") = 193,
+        py::arg("istep") = 1, py::arg("xstep") = 1);
   m.def("collect", &collect, "colloct all trace (data and location)",
         py::arg("segy_in"), py::arg("iline") = 189, py::arg("xline") = 193,
         py::arg("xfield") = 73, py::arg("yfield") = 77);
-  m.def("create_by_sharing_header", &create_by_sharing_header,
+  m.def("create_by_sharing_header",
+        overload_cast_<const std::string &, const std::string &,
+                       const py::array_t<float> &, int, int, int, int>()(
+            &create_by_sharing_header),
         "create a segy file using a existed segy header", py::arg("segy_name"),
         py::arg("header_segy"), py::arg("src"), py::arg("iline") = 189,
-        py::arg("xline") = 193);
+        py::arg("xline") = 193, py::arg("istep") = 1, py::arg("xstep") = 1);
+  m.def("create_by_sharing_header",
+        overload_cast_<const std::string &, const std::string &,
+                       const std::string &, const py::sequence &, int, int, int,
+                       int>()(&create_by_sharing_header),
+        "create a segy file using a existed segy header", py::arg("segy_name"),
+        py::arg("header_segy"), py::arg("src_file"), py::arg("shape"),
+        py::arg("iline") = 189, py::arg("xline") = 193, py::arg("istep") = 1,
+        py::arg("xstep") = 1);
 }
```

### Comparing `cigsegy-1.0.1/python/cigsegy.pyi` & `cigsegy-1.1.2/python/cigsegy.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import typing
 import numpy
 
 _Shape = typing.Tuple[int, ...]
 
 __all__ = [
     "Pysegy", "fromfile", "fromfile_ignore_header", "tofile",
-    "tofile_ignore_header", "collect"
+    "tofile_ignore_header", "collect", "create_by_sharing_header"
 ]
 
 
 class Pysegy():
 
     @typing.overload
     def __init__(self, segy_name: str) -> None:
@@ -205,27 +205,61 @@
         """
 
     def close_file(self) -> None:
         """
         close mmap for reading mode
         """
 
+    def setInlineStep(self, step: int) -> None:
+        """
+        set inline step
+        """
+
+    def setCrosslineStep(self, step: int) -> None:
+        """
+        set inline step
+        """
+
+    def setSteps(self, istep: int, xstep: int) -> None:
+        """
+        set inline and crossline step
+        """
+
+    def get_traceInfo(self, n: int) -> numpy.ndarray[int]:
+        """
+        get ndarray: [iline, xline, x, y]
+        """
+
+    def get_traceInfo(self, beg: int, end: int) -> numpy.ndarray[int]:
+        """
+        get traceinfo from beg to end traces: [beg, end)
+        """
+
+    def trace_count(self) -> int:
+        """
+        get the total traces
+        """
+
     pass
 
 
 def fromfile(segy_name: str,
              iline: int = 189,
-             xline: int = 193) -> numpy.ndarray[numpy.float32]:
+             xline: int = 193,
+             istep: int = 1,
+             xstep: int = 1) -> numpy.ndarray[numpy.float32]:
     """
     reading from a segy file.
 
     Parameters:
     - segy_name: the input segy file name
     - iline: the inline number field in each trace header
     - xline: the crossline number field in each trace header
+    - istep: the step of inline numbers
+    - xstep: the step of crossline numbers
     """
 
 
 def fromfile_ignore_header(segy_name: str,
                            sizeZ: int,
                            sizeY: int,
                            sizeX: int,
@@ -241,23 +275,27 @@
     - format: the data format code, 1 for 4 bytes IBM float, 5 for 4 bytes IEEE float
     """
 
 
 def tofile(segy_name: str,
            out_name: str,
            iline: int = 189,
-           xline: int = 193) -> None:
+           xline: int = 193,
+           istep: int = 1,
+           xstep: int = 1) -> None:
     """
     convert a segy file to a binary file
 
     Parameters:
     - segy_name: the input segy file name
     - out_name: the output binary file name
     - iline: the inline number field in each trace header
     - xline: the crossline number field in each trace header
+    - istep: the step of inline numbers
+    - xstep: the step of crossline numbers
     """
 
 
 def tofile_ignore_header(segy_name: str,
                          out_name: str,
                          sizeX: int,
                          sizeY: int,
@@ -302,18 +340,45 @@
     """
 
 
 def create_by_sharing_header(segy_name: str,
                              header_segy: str,
                              src: numpy.ndarray[numpy.float32],
                              iline: int = 189,
-                             xline: int = 193):
+                             xline: int = 193,
+                             istep: int = 1,
+                             xstep: int = 1) -> None:
     """
     create a segy and its header is from an existed segy.
 
     Parameters:
     - segy_name: str, the out segy name
     - header_segy: str, the header segy file
     - src: numpy.ndarray, source data
     - iline: int, the inline number field of header segy
     - xline: int, the crossline number field of header segy
+    - istep: the step of inline numbers
+    - xstep: the step of crossline numbers
+    """
+
+
+def create_by_sharing_header(segy_name: str,
+                             header_segy: str,
+                             src_file: str,
+                             shape: tuple or list,
+                             iline: int = 189,
+                             xline: int = 193,
+                             istep: int = 1,
+                             xstep: int = 1) -> None:
+    """
+    create a segy and its header is from an existed segy.
+
+    Parameters:
+    - segy_name: str, the out segy name
+    - header_segy: str, the header segy file
+    - src_file: source data file
+    - shape: tuple or list, like: (sizeZ, sizeY, sizeX) or (iline, xline, nt)
+    - iline: int, the inline number field of header segy
+    - xline: int, the crossline number field of header segy
+    - istep: the step of inline numbers
+    - xstep: the step of crossline numbers
     """
```

### Comparing `cigsegy-1.0.1/LICENSE` & `cigsegy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cigsegy-1.0.1/setup.py` & `cigsegy-1.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import os, sys
 import subprocess
+
 from pathlib import Path
-from setuptools import setup
 
 from pybind11.setup_helpers import Pybind11Extension, build_ext
-
+from setuptools import setup
+from distutils.ccompiler import get_default_compiler
 
 fmt_root = '.'
+for v in sys.argv:
+    if v.startswith('--fmt_root='):
+        sys.argv.remove(v)
+        # fmt_root = v.removeprefix('--fmt_root=')
+        fmt_root = v[11:]
+        break
 
 cwd = Path(__file__).resolve().parent
 
 package_name = "cigsegy"
-version = "1.0.1"
+version = "1.1.2"
 git_hash = "unknown"
 
 try:
     git_hash = (subprocess.check_output(["git", "rev-parse", "HEAD"],
                                         cwd=cwd).decode().strip())
 except (FileNotFoundError, subprocess.CalledProcessError):
     pass
@@ -34,21 +41,23 @@
 def get_extensions():
     # add segy
     ext_modules = []
     sources = ['src/segy.cpp', 'python/PySegy.cpp']
     include_dirs = ['src/include']
     if fmt_root:
         include_dirs.append(str(Path(fmt_root) / 'include'))
-    extra_compile_args = ["-std=c++11", "-Wall"]
+    if get_default_compiler() == 'msvc':
+        extra_compile_args = ['/wd4244', '/wd4996', '/wd4819']
+    else:
+        extra_compile_args = ["-std=c++11", "-Wall", "-O3"]
     extra_link_args = []
     # extra_link_args = ['-lfmt']
-    extra_compile_args += ["-O3"]
 
     ext_modules.append(
-        Pybind11Extension(name=f'{package_name}/{package_name}',
+        Pybind11Extension(name=f'{package_name}.{package_name}',
                           sources=[str(s) for s in sources],
                           include_dirs=include_dirs,
                           extra_compile_args=extra_compile_args,
                           extra_link_args=extra_link_args))
 
     return ext_modules
 
@@ -57,15 +66,15 @@
     name=package_name,
     version=version,
     description=
     'A tool for segy-format file reading and segy-format creating from binary file',
     author='roger',
     url='https://github.com/JintaoLee-Roger/cigsegy',
     license='MIT',
-    install_requires=['numpy'],
+    # install_requires=['numpy'],
     python_requires=">=3.6",
     ext_modules=get_extensions(),
     cmdclass={"build_ext": build_ext},
     packages=['cigsegy'],
     package_dir={'cigsegy': 'python'},
     include_package_data=True,
     exclude_package_data={'cigsegy': ['*.cpp', '*.txt', 'setup.py']})
```

### Comparing `cigsegy-1.0.1/include/fmt/format.h` & `cigsegy-1.1.2/include/fmt/format.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.0.1/include/fmt/compile.h` & `cigsegy-1.1.2/include/fmt/compile.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.0.1/include/fmt/ranges.h` & `cigsegy-1.1.2/include/fmt/ranges.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.0.1/include/fmt/format-inl.h` & `cigsegy-1.1.2/include/fmt/format-inl.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.0.1/include/fmt/ostream.h` & `cigsegy-1.1.2/include/fmt/ostream.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.0.1/include/fmt/locale.h` & `cigsegy-1.1.2/include/fmt/locale.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.0.1/include/fmt/printf.h` & `cigsegy-1.1.2/include/fmt/printf.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.0.1/include/fmt/core.h` & `cigsegy-1.1.2/include/fmt/core.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.0.1/include/fmt/chrono.h` & `cigsegy-1.1.2/include/fmt/chrono.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.0.1/include/fmt/posix.h` & `cigsegy-1.1.2/include/fmt/posix.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.0.1/include/fmt/color.h` & `cigsegy-1.1.2/include/fmt/color.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.0.1/cigsegy.egg-info/SOURCES.txt` & `cigsegy-1.1.2/cigsegy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 pyproject.toml
 setup.py
 cigsegy.egg-info/PKG-INFO
 cigsegy.egg-info/SOURCES.txt
 cigsegy.egg-info/dependency_links.txt
-cigsegy.egg-info/requires.txt
 cigsegy.egg-info/top_level.txt
 include/fmt/chrono.h
 include/fmt/color.h
 include/fmt/compile.h
 include/fmt/core.h
 include/fmt/format-inl.h
 include/fmt/format.h
```

