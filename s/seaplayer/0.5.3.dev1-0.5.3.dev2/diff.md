# Comparing `tmp/seaplayer-0.5.3.dev1.tar.gz` & `tmp/seaplayer-0.5.3.dev2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.5.3.dev1.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

