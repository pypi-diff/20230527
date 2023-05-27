# Comparing `tmp/sword2vec-3.2.1b0.tar.gz` & `tmp/sword2vec-3.2.2b0-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sword2vec-3.2.1b0.tar", last modified: Sat May 27 06:27:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

