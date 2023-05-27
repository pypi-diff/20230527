# Comparing `tmp/jupyter-converter-0.0.2.tar.gz` & `tmp/jupyter_converter-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-converter-0.0.2.tar", last modified: Sat May 27 19:44:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

