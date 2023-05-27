# Comparing `tmp/MDAnalysis-2.5.0.tar.gz` & `tmp/MDAnalysis-2.5.0.dev0-cp39-cp39-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDAnalysis-2.5.0.tar", last modified: Sat May 27 20:46:06 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

