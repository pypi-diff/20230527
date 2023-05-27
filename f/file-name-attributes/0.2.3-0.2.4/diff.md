# Comparing `tmp/file-name-attributes-0.2.3.tar.gz` & `tmp/file-name-attributes-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file-name-attributes-0.2.3.tar", last modified: Mon May 22 17:00:32 2023, max compression
+gzip compressed data, was "file-name-attributes-0.2.4.tar", last modified: Sat May 27 15:17:26 2023, max compression
```

## Comparing `file-name-attributes-0.2.3.tar` & `file-name-attributes-0.2.4.tar`

### file list

```diff
@@ -1,107 +1,114 @@
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-06 18:55:15.000000 file-name-attributes-0.2.3/LICENSE
--rw-rw-r--   0 kevin     (1001) dialout     (20)       31 2023-05-07 00:42:08.000000 file-name-attributes-0.2.3/MANIFEST.in
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4367 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3702 2023-05-21 18:22:36.000000 file-name-attributes-0.2.3/README.md
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/config/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      873 2023-05-06 03:24:15.000000 file-name-attributes-0.2.3/config/config.toml
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/doc/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3783 2023-05-01 23:27:37.000000 file-name-attributes-0.2.3/doc/keys.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4316 2023-05-22 16:20:17.000000 file-name-attributes-0.2.3/pyproject.toml
--rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/setup.cfg
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/extra/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4894 2023-05-22 16:03:33.000000 file-name-attributes-0.2.3/src/extra/fnaffle.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4249 2023-05-22 15:56:18.000000 file-name-attributes-0.2.3/src/extra/make_isbn_ranges.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/file_name_attributes.egg-info/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4367 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/file_name_attributes.egg-info/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2196 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/file_name_attributes.egg-info/SOURCES.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/file_name_attributes.egg-info/dependency_links.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)       62 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/file_name_attributes.egg-info/entry_points.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)       34 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/file_name_attributes.egg-info/top_level.txt
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/fna/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3415 2023-05-22 16:11:49.000000 file-name-attributes-0.2.3/src/fna/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/util/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-22 16:12:06.000000 file-name-attributes-0.2.3/src/util/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      778 2023-05-21 18:37:39.000000 file-name-attributes-0.2.3/src/util/checksum.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      716 2023-05-21 18:37:58.000000 file-name-attributes-0.2.3/src/util/checksum_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3648 2023-05-21 20:02:21.000000 file-name-attributes-0.2.3/src/util/config.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5367 2023-05-22 13:18:46.000000 file-name-attributes-0.2.3/src/util/config_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      625 2023-05-21 19:00:38.000000 file-name-attributes-0.2.3/src/util/docsplit.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      707 2023-05-22 16:03:59.000000 file-name-attributes-0.2.3/src/util/docsplit_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      102 2023-05-22 16:04:07.000000 file-name-attributes-0.2.3/src/util/error.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2181 2023-05-21 19:04:05.000000 file-name-attributes-0.2.3/src/util/escape.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2912 2023-05-21 18:38:18.000000 file-name-attributes-0.2.3/src/util/escape_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      926 2023-05-21 19:04:45.000000 file-name-attributes-0.2.3/src/util/fearmat.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      710 2023-05-06 18:49:53.000000 file-name-attributes-0.2.3/src/util/fearmat_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1857 2023-05-22 16:13:43.000000 file-name-attributes-0.2.3/src/util/io.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2033 2023-05-21 20:01:59.000000 file-name-attributes-0.2.3/src/util/io_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3464 2023-05-22 15:48:23.000000 file-name-attributes-0.2.3/src/util/multimap.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4558 2023-05-22 13:21:05.000000 file-name-attributes-0.2.3/src/util/multimap_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1063 2023-05-22 16:04:25.000000 file-name-attributes-0.2.3/src/util/pytestutil.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1738 2023-05-22 16:05:14.000000 file-name-attributes-0.2.3/src/util/registry.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      849 2023-05-21 18:38:59.000000 file-name-attributes-0.2.3/src/util/registry_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1099 2023-05-21 20:46:41.000000 file-name-attributes-0.2.3/src/util/repr.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1408 2023-05-21 18:39:13.000000 file-name-attributes-0.2.3/src/util/repr_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     7871 2023-05-22 16:14:23.000000 file-name-attributes-0.2.3/src/util/sqlite.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4996 2023-05-22 16:15:07.000000 file-name-attributes-0.2.3/src/util/sqlite_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      438 2023-05-22 16:05:57.000000 file-name-attributes-0.2.3/src/util/typecheck.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1338 2023-05-06 18:49:53.000000 file-name-attributes-0.2.3/src/util/typecheck_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/vlju/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1788 2023-05-22 15:56:18.000000 file-name-attributes-0.2.3/src/vlju/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      401 2023-05-22 16:06:32.000000 file-name-attributes-0.2.3/src/vlju/testutil.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/vlju/types/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-22 16:15:23.000000 file-name-attributes-0.2.3/src/vlju/types/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      760 2023-05-21 18:39:37.000000 file-name-attributes-0.2.3/src/vlju/types/all.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/vlju/types/doi/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4012 2023-05-22 15:56:18.000000 file-name-attributes-0.2.3/src/vlju/types/doi/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3698 2023-05-22 12:38:34.000000 file-name-attributes-0.2.3/src/vlju/types/doi/doi_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)  1136925 2023-05-22 16:07:12.000000 file-name-attributes-0.2.3/src/vlju/types/doi/org.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/vlju/types/ean/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1691 2023-05-22 15:56:18.000000 file-name-attributes-0.2.3/src/vlju/types/ean/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2346 2023-05-21 21:36:50.000000 file-name-attributes-0.2.3/src/vlju/types/ean/ean_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3210 2023-05-22 15:56:18.000000 file-name-attributes-0.2.3/src/vlju/types/ean/isbn.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    40480 2023-05-22 15:22:32.000000 file-name-attributes-0.2.3/src/vlju/types/ean/isbn_ranges.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2463 2023-05-21 21:38:59.000000 file-name-attributes-0.2.3/src/vlju/types/ean/isbn_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      653 2023-05-22 15:56:18.000000 file-name-attributes-0.2.3/src/vlju/types/ean/ismn.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1082 2023-05-21 21:40:39.000000 file-name-attributes-0.2.3/src/vlju/types/ean/ismn_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1281 2023-05-22 15:56:18.000000 file-name-attributes-0.2.3/src/vlju/types/ean/issn.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2198 2023-05-21 21:42:02.000000 file-name-attributes-0.2.3/src/vlju/types/ean/issn_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/vlju/types/file/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1966 2023-05-22 15:56:18.000000 file-name-attributes-0.2.3/src/vlju/types/file/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1751 2023-05-21 18:40:36.000000 file-name-attributes-0.2.3/src/vlju/types/file/file_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/vlju/types/info/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      924 2023-05-22 15:56:18.000000 file-name-attributes-0.2.3/src/vlju/types/info/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      670 2023-05-21 18:40:36.000000 file-name-attributes-0.2.3/src/vlju/types/info/info_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2835 2023-05-22 16:07:37.000000 file-name-attributes-0.2.3/src/vlju/types/info/kinds.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/vlju/types/lccn/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1201 2023-05-22 15:56:18.000000 file-name-attributes-0.2.3/src/vlju/types/lccn/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1055 2023-05-21 18:40:36.000000 file-name-attributes-0.2.3/src/vlju/types/lccn/lccn_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/vlju/types/site/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2241 2023-05-22 15:56:18.000000 file-name-attributes-0.2.3/src/vlju/types/site/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1541 2023-05-22 16:15:47.000000 file-name-attributes-0.2.3/src/vlju/types/site/site_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2860 2023-05-22 12:18:47.000000 file-name-attributes-0.2.3/src/vlju/types/site/sites_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/vlju/types/uri/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8357 2023-05-22 15:56:18.000000 file-name-attributes-0.2.3/src/vlju/types/uri/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     6218 2023-05-22 13:38:50.000000 file-name-attributes-0.2.3/src/vlju/types/uri/uri_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/vlju/types/url/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      673 2023-05-22 16:16:29.000000 file-name-attributes-0.2.3/src/vlju/types/url/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      533 2023-05-21 18:40:36.000000 file-name-attributes-0.2.3/src/vlju/types/url/url_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/vlju/types/urn/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1356 2023-05-22 15:56:18.000000 file-name-attributes-0.2.3/src/vlju/types/urn/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4039 2023-05-22 16:09:09.000000 file-name-attributes-0.2.3/src/vlju/types/urn/kinds.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1087 2023-05-22 12:43:05.000000 file-name-attributes-0.2.3/src/vlju/types/urn/urn_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1760 2023-05-22 13:43:11.000000 file-name-attributes-0.2.3/src/vlju/vlju_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/vljum/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8249 2023-05-22 16:16:57.000000 file-name-attributes-0.2.3/src/vljum/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2343 2023-05-22 16:09:55.000000 file-name-attributes-0.2.3/src/vljum/m.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8973 2023-05-22 16:17:33.000000 file-name-attributes-0.2.3/src/vljum/m_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     9587 2023-05-22 16:17:59.000000 file-name-attributes-0.2.3/src/vljum/runner.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     7915 2023-05-22 16:10:31.000000 file-name-attributes-0.2.3/src/vljum/runner_test.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 17:00:32.000000 file-name-attributes-0.2.3/src/vljumap/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1197 2023-05-22 15:35:19.000000 file-name-attributes-0.2.3/src/vljumap/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    20697 2023-05-22 16:18:50.000000 file-name-attributes-0.2.3/src/vljumap/enc.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    10399 2023-05-22 16:19:22.000000 file-name-attributes-0.2.3/src/vljumap/enc_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      985 2023-05-22 16:20:09.000000 file-name-attributes-0.2.3/src/vljumap/factory.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1388 2023-05-21 23:37:25.000000 file-name-attributes-0.2.3/src/vljumap/factory_test.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1575 2023-05-22 01:56:36.000000 file-name-attributes-0.2.3/src/vljumap/vljumap_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-06 18:55:15.000000 file-name-attributes-0.2.4/LICENSE
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       31 2023-05-07 00:42:08.000000 file-name-attributes-0.2.4/MANIFEST.in
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5434 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4769 2023-05-25 13:38:58.000000 file-name-attributes-0.2.4/README.md
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/config/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      873 2023-05-06 03:24:15.000000 file-name-attributes-0.2.4/config/config.toml
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/doc/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2059 2023-05-22 21:45:38.000000 file-name-attributes-0.2.4/doc/configuration.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    10407 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/doc/fna.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4121 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/doc/keys.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4432 2023-05-26 19:58:41.000000 file-name-attributes-0.2.4/pyproject.toml
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/setup.cfg
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/extra/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4899 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/extra/fnaffle.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4378 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/extra/make_isbn_ranges.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/file_name_attributes.egg-info/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5434 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/file_name_attributes.egg-info/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2354 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/file_name_attributes.egg-info/SOURCES.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/file_name_attributes.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       62 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/file_name_attributes.egg-info/entry_points.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       34 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/file_name_attributes.egg-info/top_level.txt
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:25.000000 file-name-attributes-0.2.4/src/fna/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3415 2023-05-22 16:11:49.000000 file-name-attributes-0.2.4/src/fna/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/util/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-22 16:12:06.000000 file-name-attributes-0.2.4/src/util/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      778 2023-05-21 18:37:39.000000 file-name-attributes-0.2.4/src/util/checksum.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      716 2023-05-21 18:37:58.000000 file-name-attributes-0.2.4/src/util/checksum_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3648 2023-05-21 20:02:21.000000 file-name-attributes-0.2.4/src/util/config.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5367 2023-05-22 13:18:46.000000 file-name-attributes-0.2.4/src/util/config_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      625 2023-05-21 19:00:38.000000 file-name-attributes-0.2.4/src/util/docsplit.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      707 2023-05-22 16:03:59.000000 file-name-attributes-0.2.4/src/util/docsplit_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     9038 2023-05-26 20:01:56.000000 file-name-attributes-0.2.4/src/util/duration.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5525 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/src/util/duration_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      102 2023-05-22 16:04:07.000000 file-name-attributes-0.2.4/src/util/error.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2181 2023-05-21 19:04:05.000000 file-name-attributes-0.2.4/src/util/escape.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2912 2023-05-21 18:38:18.000000 file-name-attributes-0.2.4/src/util/escape_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      926 2023-05-21 19:04:45.000000 file-name-attributes-0.2.4/src/util/fearmat.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      710 2023-05-06 18:49:53.000000 file-name-attributes-0.2.4/src/util/fearmat_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1857 2023-05-22 16:13:43.000000 file-name-attributes-0.2.4/src/util/io.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2033 2023-05-21 20:01:59.000000 file-name-attributes-0.2.4/src/util/io_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3535 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/util/multimap.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4661 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/util/multimap_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1063 2023-05-22 16:04:25.000000 file-name-attributes-0.2.4/src/util/pytestutil.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1738 2023-05-22 16:05:14.000000 file-name-attributes-0.2.4/src/util/registry.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      849 2023-05-21 18:38:59.000000 file-name-attributes-0.2.4/src/util/registry_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1099 2023-05-21 20:46:41.000000 file-name-attributes-0.2.4/src/util/repr.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1408 2023-05-21 18:39:13.000000 file-name-attributes-0.2.4/src/util/repr_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8073 2023-05-26 20:00:25.000000 file-name-attributes-0.2.4/src/util/sqlite.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4994 2023-05-26 19:15:36.000000 file-name-attributes-0.2.4/src/util/sqlite_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      438 2023-05-22 16:05:57.000000 file-name-attributes-0.2.4/src/util/typecheck.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1338 2023-05-06 18:49:53.000000 file-name-attributes-0.2.4/src/util/typecheck_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1788 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      401 2023-05-22 16:06:32.000000 file-name-attributes-0.2.4/src/vlju/testutil.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-22 16:15:23.000000 file-name-attributes-0.2.4/src/vlju/types/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      830 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/src/vlju/types/all.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/doi/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3999 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vlju/types/doi/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3698 2023-05-22 12:38:34.000000 file-name-attributes-0.2.4/src/vlju/types/doi/doi_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)  1136925 2023-05-22 16:07:12.000000 file-name-attributes-0.2.4/src/vlju/types/doi/org.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/ean/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1691 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/ean/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2346 2023-05-21 21:36:50.000000 file-name-attributes-0.2.4/src/vlju/types/ean/ean_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3210 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/ean/isbn.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    40480 2023-05-22 15:22:32.000000 file-name-attributes-0.2.4/src/vlju/types/ean/isbn_ranges.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2463 2023-05-21 21:38:59.000000 file-name-attributes-0.2.4/src/vlju/types/ean/isbn_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      653 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/ean/ismn.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1082 2023-05-21 21:40:39.000000 file-name-attributes-0.2.4/src/vlju/types/ean/ismn_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1281 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/ean/issn.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2198 2023-05-21 21:42:02.000000 file-name-attributes-0.2.4/src/vlju/types/ean/issn_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/file/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1967 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vlju/types/file/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1751 2023-05-21 18:40:36.000000 file-name-attributes-0.2.4/src/vlju/types/file/file_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/info/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      924 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/info/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      670 2023-05-21 18:40:36.000000 file-name-attributes-0.2.4/src/vlju/types/info/info_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2835 2023-05-22 16:07:37.000000 file-name-attributes-0.2.4/src/vlju/types/info/kinds.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/lccn/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1201 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/lccn/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1055 2023-05-21 18:40:36.000000 file-name-attributes-0.2.4/src/vlju/types/lccn/lccn_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/site/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2241 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/site/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1541 2023-05-22 16:15:47.000000 file-name-attributes-0.2.4/src/vlju/types/site/site_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2860 2023-05-22 12:18:47.000000 file-name-attributes-0.2.4/src/vlju/types/site/sites_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/timestamp/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      874 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vlju/types/timestamp/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1244 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/src/vlju/types/timestamp/timestamp_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/uri/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8357 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/uri/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     6218 2023-05-22 13:38:50.000000 file-name-attributes-0.2.4/src/vlju/types/uri/uri_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/url/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      673 2023-05-22 16:16:29.000000 file-name-attributes-0.2.4/src/vlju/types/url/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      533 2023-05-21 18:40:36.000000 file-name-attributes-0.2.4/src/vlju/types/url/url_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vlju/types/urn/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1356 2023-05-22 15:56:18.000000 file-name-attributes-0.2.4/src/vlju/types/urn/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4039 2023-05-22 16:09:09.000000 file-name-attributes-0.2.4/src/vlju/types/urn/kinds.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1054 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vlju/types/urn/urn_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1760 2023-05-22 13:43:11.000000 file-name-attributes-0.2.4/src/vlju/vlju_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vljum/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8442 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vljum/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2570 2023-05-23 22:07:37.000000 file-name-attributes-0.2.4/src/vljum/m.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     9087 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vljum/m_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    10520 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/src/vljum/runner.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8326 2023-05-25 00:54:41.000000 file-name-attributes-0.2.4/src/vljum/runner_test.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-27 15:17:26.000000 file-name-attributes-0.2.4/src/vljumap/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1197 2023-05-22 15:35:19.000000 file-name-attributes-0.2.4/src/vljumap/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    20714 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vljumap/enc.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    10428 2023-05-25 00:54:42.000000 file-name-attributes-0.2.4/src/vljumap/enc_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1342 2023-05-23 21:58:33.000000 file-name-attributes-0.2.4/src/vljumap/factory.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1742 2023-05-23 22:02:05.000000 file-name-attributes-0.2.4/src/vljumap/factory_test.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1575 2023-05-22 01:56:36.000000 file-name-attributes-0.2.4/src/vljumap/vljumap_test.py
```

### Comparing `file-name-attributes-0.2.3/LICENSE` & `file-name-attributes-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/PKG-INFO` & `file-name-attributes-0.2.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,15 @@
-Metadata-Version: 2.1
-Name: file-name-attributes
-Version: 0.2.3
-Summary: Manage key/value metadata in file names.
-License: MIT License
-Project-URL: repository, https://codeberg.org/datatravelandexperiments/fna
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # fna
 
+- [Introduction](#introduction)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Configuration](#configuration)
+- [Implementation](#implementation)
+
 ## Introduction
 
 ### The problem
 
 Many types of files have associated metadata, e.g. title and creators, but
 there is no universal way to record this. Some file formats contain metadata
 fields, but not all do. Some file systems provide for metadata tagging,
@@ -40,22 +27,35 @@
 This tool, `fna` (for ‘File Name Attributes’) helps automate managing
 key-value pairs in file names.
 
 For certain keys, the values can have associated semantics beyond their text.
 For example, ISBNs can be normalized to ISBN-13 and have their checksums
 corrected.
 
+## Installation
+
+The easiest (?) way to install `fna` is from
+[PyPi](https://pypi.org/project/file-name-attributes/) using `pip`.
+Depending on your system, one of the following may work:
+
+- `pip install file-name-attributes`
+- `pip install --user file-name-attributes`
+- `pipx install file-name-attributes`
+- `python -m pip install file-name-attributes`
+
 ## Usage
 
 By default, `fna` follows a subcommand familiar from tools like `git`, except
 that it's typical to chain multiple subcommands in a single invocation.
 
 Run `fna help` to get a list of subcommands, and `fna help ‹subcommand›`
 for information on a particular subcommand.
 
+See [doc/fna.md](doc/fna.md) for more information.
+
 (More complicated operations are possible using Python expressions rather
 than the subcommands, but this is not yet stable or documented.)
 
 ### Examples
 
 This example uses two subcommands, `file`, which takes a file name as
 argument, and `add`, which takes key and value as arguments:
@@ -77,29 +77,43 @@
 ```
 $ fna file '/tmp/My Book.pdf' add isbn 1234567890 json encode
 {"title": ["My Book"], "isbn": ["9781234567897"]}
 ```
 
 ## Configuration
 
-`fna` tries to read `vlju/config.toml` or  `fna/config.toml` from XDG locations
-(e.g. `$HOME/.config/`). The former is shared by all tools using the Vlju
+Unless otherwise directed by a command line option,
+`fna` tries to read `vlju/config.toml` or `fna/config.toml`
+from XDG locations (e.g. `$HOME/.config/`).
+The former is shared by all tools using the Vlju
 library, while the latter applies only to the `fna` command.
 
 This file can define keys and classes associated with web sites,
 mapping from a compact ID to a URL. (The other direction does not yet exist.)
 The distribution file `config/config.toml` contains some examples.
 
+See [doc/configuration.md](doc/configuration.md) for more information.
+
 ## Implementation
 
+The current public home for `fna` is
+[https://codeberg.org/datatravelandexperiments/fna](https://codeberg.org/datatravelandexperiments/fna)
+
 `fna` is written in Python primarily because (in the original version) the
 standard library `shlex` module provided input file tokenization ‘for free’
 (sometimes free is expensive). It was originally written in Python 2 circa
 2010, and substantially revised in 2023.
 
+`fna` aims for 100% unit test coverage (outside of `extra/`)
+and full type annotation (outside of unit tests).
+
+### src/util
+
+Code that does not depend on `vlju`, and could be useful in unrelated projects.
+
 ### src/vlju
 
 `vlju.Vlju` (pronounced ‘value’) is the base data type for attribute
 values. Every `Vlju` has a string representation. Many subclasses have
 additional internal structure; e.g. the `ISBN` subclass handles 10- and
 13-digit ISBNs including their checksums.
 
@@ -121,15 +135,14 @@
 
 `src/vljum` can depend on `src/vljumap`, `src/vlju` and `src/util`.
 
 ### src/fna
 
 The command line tool `fna`.
 
-## TODO
+### TODO
 
-- Better documentation.
-- Logging options.
 - Better error handling. Too much still just raises exceptions.
 - Investigate constructing SiteBase values from URL strings.
-
-<!-- vim:set textwidth=79: -->
+  Config would probably contain REs with named groups.
+- Document operation with `-[EFx]`.
+- Logging options?
```

### Comparing `file-name-attributes-0.2.3/config/config.toml` & `file-name-attributes-0.2.4/config/config.toml`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/pyproject.toml` & `file-name-attributes-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "file-name-attributes"
-version = "0.2.3"
+version = "0.2.4"
 description = "Manage key/value metadata in file names."
 license.text = "MIT License"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
@@ -89,15 +89,15 @@
 pythonpath = ["src"]
 addopts = "--tb=native"
 
 [tool.ruff]
 src = ["src"]
 namespace-packages = ["src/extra"]
 line-length = 80
-allowed-confusables = ["‘", "’", "–", "—", "‹", "›", "ı"]
+allowed-confusables = ["‘", "’", "–", "—", "‹", "›", "ı", "′", "″"]
 select = ["ALL"]
 ignore = [
     "ANN002",   # missing-type-args: Nah.
     "ANN003",   # missing-type-kwargs: Nah.
     "ANN101", 	# missing-type-self: Nah.
     "ANN102",   # missing-type-cls: Nah.
     "ERA",      # eradicate: Complains about yapf: directives.
@@ -125,14 +125,15 @@
 [tool.ruff.isort]
 lines-after-imports = 1
 lines-between-types = 1
 
 [tool.ruff.per-file-ignores]
 "*_test.py" = [
     "ANN001", "ANN201", "ANN202",   # type annotations tbd
+    "PLC1901",  # testing for specific results
     "S101",     # assert
 ]
 "src/vlju/types/doi/org.py" = ["Q000"]
 "src/vlju/types/ean/isbn_ranges.py" = ["E501"]
 
 [tool.ruff.pylint]
 max-args = 8
@@ -146,13 +147,13 @@
 coalesce_brackets = true
 column_limit = 80
 dedent_closing_brackets = false
 indent_dictionary_value = true
 join_multiple_lines = false
 spaces_around_default_or_named_assign = false
 spaces_around_subscript_colon = true
-spaces_before_comment = 2
+spaces_before_comment = [17, 21, 25, 29, 33, 37, 41, 45, 49, 53, 57, 61, 65, 69]
 split_before_bitwise_operator = true
 split_before_arithmetic_operator = true
 split_before_dot = true
 split_before_expression_after_opening_paren = true
 split_complex_comprehension = true
```

### Comparing `file-name-attributes-0.2.3/src/extra/fnaffle.py` & `file-name-attributes-0.2.4/src/extra/fnaffle.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                 if not dst.exists():
                     if not args.dryrun:
                         dst.mkdir(parents=True)
                     if args.dryrun or args.verbose:
                         print(f'{dst}: created')
                 if not args.dryrun:
                     try:
-                        m.dir(dst).rename()
+                        m.with_dir(dst).rename()
                     except FileExistsError as e:
                         print(f'{cmd}: file exists: {e}')
                 if args.dryrun or args.verbose:
                     print(f'{dst}: {file}')
             elif args.verbose:
                 print(f'no match for {file}')
     except Exception as e:
```

### Comparing `file-name-attributes-0.2.3/src/extra/make_isbn_ranges.py` & `file-name-attributes-0.2.4/src/extra/make_isbn_ranges.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import datetime
 import logging
 import pathlib
 import pprint
 import sys
 import xml.etree.ElementTree as ElT
 
+from collections.abc import MutableSequence
 from pathlib import Path
 from typing import TextIO
 
 from vlju.types.ean.isbn import RangeAgencies, Ranges
 
 class RangesFromXml(Ranges):
     """Load ranges from an XML file."""
@@ -29,21 +30,24 @@
         lengths: list[int] = []
         self.agencies: RangeAgencies = {}
         for rg in root.iter('RegistrationGroups'):
             for g in rg.iter('Group'):
                 self._load_group(g, starts, lengths, self.agencies)
         super().__init__(array.array('Q', starts), array.array('I', lengths))
 
-    def _load_group(self, g: ElT.Element, starts: array.array,
-                    lengths: array.array, agencies: RangeAgencies) -> None:
+    def _load_group(self, g: ElT.Element, starts: MutableSequence[int],
+                    lengths: MutableSequence[int],
+                    agencies: RangeAgencies) -> None:
         s_prefix = g.findtext('Prefix')
         assert s_prefix is not None
         s_compact_prefix = s_prefix.replace('-', '')
         ts_prefix: tuple[str, ...] = tuple(s_prefix.split('-'))
-        agencies[ts_prefix] = g.findtext('Agency')
+        agency = g.findtext('Agency')
+        if agency:
+            agencies[ts_prefix] = agency
         ti_prefix_length: tuple[int, ...] = tuple(map(len, ts_prefix))
         remaining = 12 - sum(ti_prefix_length)
         logging.debug('prefix %s %s + %d', s_prefix, ti_prefix_length,
                       remaining)
 
         for r in g.iter('Rule'):
             s_range = r.findtext('Range')
```

### Comparing `file-name-attributes-0.2.3/src/file_name_attributes.egg-info/PKG-INFO` & `file-name-attributes-0.2.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-name-attributes
-Version: 0.2.3
+Version: 0.2.4
 Summary: Manage key/value metadata in file names.
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/fna
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,20 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fna
 
+- [Introduction](#introduction)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Configuration](#configuration)
+- [Implementation](#implementation)
+
 ## Introduction
 
 ### The problem
 
 Many types of files have associated metadata, e.g. title and creators, but
 there is no universal way to record this. Some file formats contain metadata
 fields, but not all do. Some file systems provide for metadata tagging,
@@ -40,22 +46,35 @@
 This tool, `fna` (for ‘File Name Attributes’) helps automate managing
 key-value pairs in file names.
 
 For certain keys, the values can have associated semantics beyond their text.
 For example, ISBNs can be normalized to ISBN-13 and have their checksums
 corrected.
 
+## Installation
+
+The easiest (?) way to install `fna` is from
+[PyPi](https://pypi.org/project/file-name-attributes/) using `pip`.
+Depending on your system, one of the following may work:
+
+- `pip install file-name-attributes`
+- `pip install --user file-name-attributes`
+- `pipx install file-name-attributes`
+- `python -m pip install file-name-attributes`
+
 ## Usage
 
 By default, `fna` follows a subcommand familiar from tools like `git`, except
 that it's typical to chain multiple subcommands in a single invocation.
 
 Run `fna help` to get a list of subcommands, and `fna help ‹subcommand›`
 for information on a particular subcommand.
 
+See [doc/fna.md](doc/fna.md) for more information.
+
 (More complicated operations are possible using Python expressions rather
 than the subcommands, but this is not yet stable or documented.)
 
 ### Examples
 
 This example uses two subcommands, `file`, which takes a file name as
 argument, and `add`, which takes key and value as arguments:
@@ -77,29 +96,43 @@
 ```
 $ fna file '/tmp/My Book.pdf' add isbn 1234567890 json encode
 {"title": ["My Book"], "isbn": ["9781234567897"]}
 ```
 
 ## Configuration
 
-`fna` tries to read `vlju/config.toml` or  `fna/config.toml` from XDG locations
-(e.g. `$HOME/.config/`). The former is shared by all tools using the Vlju
+Unless otherwise directed by a command line option,
+`fna` tries to read `vlju/config.toml` or `fna/config.toml`
+from XDG locations (e.g. `$HOME/.config/`).
+The former is shared by all tools using the Vlju
 library, while the latter applies only to the `fna` command.
 
 This file can define keys and classes associated with web sites,
 mapping from a compact ID to a URL. (The other direction does not yet exist.)
 The distribution file `config/config.toml` contains some examples.
 
+See [doc/configuration.md](doc/configuration.md) for more information.
+
 ## Implementation
 
+The current public home for `fna` is
+[https://codeberg.org/datatravelandexperiments/fna](https://codeberg.org/datatravelandexperiments/fna)
+
 `fna` is written in Python primarily because (in the original version) the
 standard library `shlex` module provided input file tokenization ‘for free’
 (sometimes free is expensive). It was originally written in Python 2 circa
 2010, and substantially revised in 2023.
 
+`fna` aims for 100% unit test coverage (outside of `extra/`)
+and full type annotation (outside of unit tests).
+
+### src/util
+
+Code that does not depend on `vlju`, and could be useful in unrelated projects.
+
 ### src/vlju
 
 `vlju.Vlju` (pronounced ‘value’) is the base data type for attribute
 values. Every `Vlju` has a string representation. Many subclasses have
 additional internal structure; e.g. the `ISBN` subclass handles 10- and
 13-digit ISBNs including their checksums.
 
@@ -121,15 +154,14 @@
 
 `src/vljum` can depend on `src/vljumap`, `src/vlju` and `src/util`.
 
 ### src/fna
 
 The command line tool `fna`.
 
-## TODO
+### TODO
 
-- Better documentation.
-- Logging options.
 - Better error handling. Too much still just raises exceptions.
 - Investigate constructing SiteBase values from URL strings.
-
-<!-- vim:set textwidth=79: -->
+  Config would probably contain REs with named groups.
+- Document operation with `-[EFx]`.
+- Logging options?
```

### Comparing `file-name-attributes-0.2.3/src/file_name_attributes.egg-info/SOURCES.txt` & `file-name-attributes-0.2.4/src/file_name_attributes.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 config/config.toml
-doc/keys.txt
+doc/configuration.md
+doc/fna.md
+doc/keys.md
 src/extra/fnaffle.py
 src/extra/make_isbn_ranges.py
 src/file_name_attributes.egg-info/PKG-INFO
 src/file_name_attributes.egg-info/SOURCES.txt
 src/file_name_attributes.egg-info/dependency_links.txt
 src/file_name_attributes.egg-info/entry_points.txt
 src/file_name_attributes.egg-info/top_level.txt
@@ -15,14 +17,16 @@
 src/util/__init__.py
 src/util/checksum.py
 src/util/checksum_test.py
 src/util/config.py
 src/util/config_test.py
 src/util/docsplit.py
 src/util/docsplit_test.py
+src/util/duration.py
+src/util/duration_test.py
 src/util/error.py
 src/util/escape.py
 src/util/escape_test.py
 src/util/fearmat.py
 src/util/fearmat_test.py
 src/util/io.py
 src/util/io_test.py
@@ -60,14 +64,16 @@
 src/vlju/types/info/info_test.py
 src/vlju/types/info/kinds.py
 src/vlju/types/lccn/__init__.py
 src/vlju/types/lccn/lccn_test.py
 src/vlju/types/site/__init__.py
 src/vlju/types/site/site_test.py
 src/vlju/types/site/sites_test.py
+src/vlju/types/timestamp/__init__.py
+src/vlju/types/timestamp/timestamp_test.py
 src/vlju/types/uri/__init__.py
 src/vlju/types/uri/uri_test.py
 src/vlju/types/url/__init__.py
 src/vlju/types/url/url_test.py
 src/vlju/types/urn/__init__.py
 src/vlju/types/urn/kinds.py
 src/vlju/types/urn/urn_test.py
```

### Comparing `file-name-attributes-0.2.3/src/fna/__init__.py` & `file-name-attributes-0.2.4/src/fna/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/checksum.py` & `file-name-attributes-0.2.4/src/util/checksum.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/checksum_test.py` & `file-name-attributes-0.2.4/src/util/checksum_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/config.py` & `file-name-attributes-0.2.4/src/util/config.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/config_test.py` & `file-name-attributes-0.2.4/src/util/config_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/docsplit.py` & `file-name-attributes-0.2.4/src/util/docsplit.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/docsplit_test.py` & `file-name-attributes-0.2.4/src/util/docsplit_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/escape.py` & `file-name-attributes-0.2.4/src/util/escape.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/escape_test.py` & `file-name-attributes-0.2.4/src/util/escape_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/fearmat.py` & `file-name-attributes-0.2.4/src/util/fearmat.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/fearmat_test.py` & `file-name-attributes-0.2.4/src/util/fearmat_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/io.py` & `file-name-attributes-0.2.4/src/util/io.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/io_test.py` & `file-name-attributes-0.2.4/src/util/io_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/multimap.py` & `file-name-attributes-0.2.4/src/util/multimap.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     """Multi-valued dictionary."""
 
     def __init__(self) -> None:
         self.data: defaultdict[K, list[V]] = defaultdict(list[V])
 
     def __eq__(self, other: object) -> bool:
         # pylint:disable=unidiomatic-typecheck
-        return (type(self) == type(other)) and (self.data == other.data)
+        if isinstance(other, MultiMap):
+            return (type(self) == type(other)) and (self.data == other.data)
+        return False
 
     def __getitem__(self, k: K) -> list[V]:
         return self.data[k]
 
     def __delitem__(self, k: K) -> None:
         if k in self.data:
             del self.data[k]
@@ -87,15 +89,15 @@
         return default
 
     def top(self, k: K) -> V | None:
         if self.data[k]:
             return self.data[k][-1]
         return None
 
-    def extend(self, other: Self) -> Self:
+    def extend(self, other: 'MultiMap') -> Self:
         for k, v in other.pairs():
             self.add(k, v)
         return self
 
     def sortkeys(self, keys: Iterable[K] | None = None) -> Self:
         """Put the map keys in alphabetical order, or specified order."""
         if keys is None:
```

### Comparing `file-name-attributes-0.2.3/src/util/multimap_test.py` & `file-name-attributes-0.2.4/src/util/multimap_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,20 @@
 
 def test_multimap_eq():
     d = mk(CASES_KEY_LIST)
     e = mk(CASES_KEY_LIST)
     assert d is not e
     assert d == e
 
+def test_multimap_ne():
+    d = mk(CASES_KEY_LIST)
+    e = mk({})
+    assert d != e
+    assert d != 1
+
 def test_multimap_getitem():
     d = mk(CASES_KEY_LIST)
     assert d['issn'] == ['1351-5381']
     assert d['none'] == []
 
 def test_multimap_get():
     d = mk(CASES_KEY_LIST)
```

### Comparing `file-name-attributes-0.2.3/src/util/pytestutil.py` & `file-name-attributes-0.2.4/src/util/pytestutil.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/registry.py` & `file-name-attributes-0.2.4/src/util/registry.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/registry_test.py` & `file-name-attributes-0.2.4/src/util/registry_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/repr.py` & `file-name-attributes-0.2.4/src/util/repr.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/repr_test.py` & `file-name-attributes-0.2.4/src/util/repr_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/util/sqlite.py` & `file-name-attributes-0.2.4/src/util/sqlite.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,62 +117,67 @@
               on_conflict: str | None = None,
               **kwargs) -> Self:
         """
         Insert into a table.
 
         `kwargs` consists of column-value pairs.
 
-        Although this is not intended to handle untrusted arguments,
-        we take precautions against injection, since table and column
-        names must be part of the query string:
+        This is intended as a shorthand to be used with hard-coded keys,
+        for example:
+
+            db.store(users', user=u, password=p)
+
+        However, due to splatting, it is possible that this function could
+        be (mis)used with untrusted arguments. Therefore, we take precautions
+        against injection, since table and column names must be part of the
+        query string:
 
         - Verify that the supplied table and column names are actually
           existing table and column names in the database.
         - Quote table and column names.
         - Use generated parameter names.
         """
         columns = kwargs.keys()
         self.check_table_columns(table, kwargs.keys())
         p = BoundParameters(kwargs)
         q = (
-            f'INSERT INTO {quote_id(table)}'  # noqa: S608
+            f'INSERT INTO {quote_id(table)}'                # noqa: S608
             f' ({",".join(quote_id(c) for c in columns)})'
             f' VALUES ({",".join(f":{k}" for k in p.value)})')
         if on_conflict:
             q += ' ON CONFLICT ' + on_conflict
         self.connection().execute(q, p.value)
         return self
 
-    def load(self,
-             table: str,
-             columns: Iterable[str] | None = None,
-             **kwargs) -> Cursor:
+    def load(self, table: str, *args: str, **kwargs) -> Cursor:
         """
         Read from a table.
 
+        `args` consists of column names to be returned.
+
         `kwargs` consists of column-value pairs that become `WHERE`
         conditions on the select.
 
         Although this is not intended to handle untrusted arguments,
         we take precautions against injection, since table and column
         names must be part of the query string:
 
         - Verify that the supplied table and column names are actually
           existing table and column names in the database.
         - Quote table and column names.
         - Use generated parameter names.
         """
         check_columns = set(kwargs.keys())
-        if columns is None:
-            cols = '*'
+        if args:
+            check_columns |= set(args)
+            cols = ','.join(quote_id(c) for c in args)
         else:
-            check_columns |= set(columns)
-            cols = ','.join(quote_id(c) for c in columns)
+            cols = '*'
         self.check_table_columns(table, check_columns)
-        q = f'SELECT {cols} FROM {quote_id(table)}'  # noqa: S608
+        q = f'SELECT {cols} FROM {quote_id(table)}'     # noqa: S608
         if not kwargs:
             return self.connection().execute(q)
         p = BoundParameters(kwargs)
         q += ' WHERE ' + ' AND '.join(f'{p.column[k]} = :{k}' for k in p.value)
         return self.connection().execute(q, p.value)
 
     def check_table_columns(self, table: str, columns: Iterable[str]) -> None:
@@ -211,15 +216,15 @@
 def quote_id(s: str) -> str:
     return '"' + s.replace('"', '""') + '"'
 
 class BoundParameters:
     """Sanitization of bound parameters."""
 
     column: dict[str, str]  # Map from parameter name to quoted column name.
-    value: dict[str, Any]  # Map from parameter name to value.
+    value: dict[str, Any]   # Map from parameter name to value.
 
     def __init__(self, column_value: dict[str, Any]) -> None:
         self.column = {}
         self.value = {}
         for i, k in enumerate(column_value):
             p = f'p{i}'
             self.column[p] = quote_id(k)
```

### Comparing `file-name-attributes-0.2.3/src/util/sqlite_test.py` & `file-name-attributes-0.2.4/src/util/sqlite_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         cur = db.load('test')
         row = cur.fetchone()
         assert row in rows
         row = cur.fetchone()
         assert row in rows
         assert cur.fetchone() is None
 
-        cur = db.load('test', ['value'], key=1)
+        cur = db.load('test', 'value', key=1)
         assert cur.fetchone() == (42, )
         assert cur.fetchone() is None
 
 def test_database_execute_unnamed_parameters():
     with KeyValueDatabase() as db:
         db.execute('INSERT INTO test VALUES (1, ?), (2, ?);', 23, 42)
         cur = db.execute('SELECT * FROM test WHERE key=?;', 2)
```

### Comparing `file-name-attributes-0.2.3/src/util/typecheck_test.py` & `file-name-attributes-0.2.4/src/util/typecheck_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/__init__.py` & `file-name-attributes-0.2.4/src/vlju/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/all.py` & `file-name-attributes-0.2.4/src/vlju/types/all.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 from vlju.types.ean import EAN13
 from vlju.types.ean.isbn import ISBN
 from vlju.types.ean.ismn import ISMN
 from vlju.types.ean.issn import ISSN
 from vlju.types.file import File
 from vlju.types.info import Info
 from vlju.types.lccn import LCCN
+from vlju.types.timestamp import Timestamp
 from vlju.types.uri import URI
 from vlju.types.url import URL
 from vlju.types.urn import URN
 
 # yapf: disable
 VLJU_TYPES: dict[str, type[Vlju]] = {
     'doi':      DOI,
     'ean':      EAN13,
     'file':     File,
     'info':     Info,
     'isbn':     ISBN,
     'ismn':     ISMN,
     'issn':     ISSN,
     'lccn':     LCCN,
+    't':        Timestamp,
     'uri':      URI,
     'url':      URL,
     'urn':      URN,
 }
 # yapf: enable
```

### Comparing `file-name-attributes-0.2.3/src/vlju/types/doi/__init__.py` & `file-name-attributes-0.2.4/src/vlju/types/doi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,19 +108,18 @@
                 'fragment': self.fragment(),
             })
         raise self.cast_param_error(t)
 
     # URI overrides:
 
     def __eq__(self, other: object) -> bool:
-        try:
+        if isinstance(other, DOI):
             return (self._prefix == other._prefix  # noqa: SLF001
                     and self._suffix == other._suffix)  # noqa: SLF001
-        except AttributeError:
-            return False
+        return False
 
     def authority(self) -> Authority:
         return self._i[self._kind]
 
     def sauthority(self) -> str:
         return self._kind
```

### Comparing `file-name-attributes-0.2.3/src/vlju/types/doi/doi_test.py` & `file-name-attributes-0.2.4/src/vlju/types/doi/doi_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/doi/org.py` & `file-name-attributes-0.2.4/src/vlju/types/doi/org.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/ean/__init__.py` & `file-name-attributes-0.2.4/src/vlju/types/ean/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/ean/ean_test.py` & `file-name-attributes-0.2.4/src/vlju/types/ean/ean_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/ean/isbn.py` & `file-name-attributes-0.2.4/src/vlju/types/ean/isbn.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/ean/isbn_ranges.py` & `file-name-attributes-0.2.4/src/vlju/types/ean/isbn_ranges.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/ean/isbn_test.py` & `file-name-attributes-0.2.4/src/vlju/types/ean/isbn_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/ean/ismn.py` & `file-name-attributes-0.2.4/src/vlju/types/ean/ismn.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/ean/ismn_test.py` & `file-name-attributes-0.2.4/src/vlju/types/ean/ismn_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/ean/issn.py` & `file-name-attributes-0.2.4/src/vlju/types/ean/issn.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/ean/issn_test.py` & `file-name-attributes-0.2.4/src/vlju/types/ean/issn_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/file/__init__.py` & `file-name-attributes-0.2.4/src/vlju/types/file/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 'ap': self._ap,
             })
         raise self.cast_param_error(t)
 
     # Vlju overrides:
 
     def __eq__(self, other: object) -> bool:
-        if isinstance(other, URI):
+        if isinstance(other, File):
             return self._file == other._file  # noqa: SLF001
         return False
 
     def __str__(self) -> str:
         return str(self._file)
 
     def __repr__(self) -> str:
```

### Comparing `file-name-attributes-0.2.3/src/vlju/types/file/file_test.py` & `file-name-attributes-0.2.4/src/vlju/types/file/file_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/info/__init__.py` & `file-name-attributes-0.2.4/src/vlju/types/info/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/info/info_test.py` & `file-name-attributes-0.2.4/src/vlju/types/info/info_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/info/kinds.py` & `file-name-attributes-0.2.4/src/vlju/types/info/kinds.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/lccn/__init__.py` & `file-name-attributes-0.2.4/src/vlju/types/lccn/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/lccn/lccn_test.py` & `file-name-attributes-0.2.4/src/vlju/types/lccn/lccn_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/site/__init__.py` & `file-name-attributes-0.2.4/src/vlju/types/site/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/site/site_test.py` & `file-name-attributes-0.2.4/src/vlju/types/site/site_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/site/sites_test.py` & `file-name-attributes-0.2.4/src/vlju/types/site/sites_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/uri/__init__.py` & `file-name-attributes-0.2.4/src/vlju/types/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/uri/uri_test.py` & `file-name-attributes-0.2.4/src/vlju/types/uri/uri_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/url/__init__.py` & `file-name-attributes-0.2.4/src/vlju/types/url/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/url/url_test.py` & `file-name-attributes-0.2.4/src/vlju/types/url/url_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/urn/__init__.py` & `file-name-attributes-0.2.4/src/vlju/types/urn/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/urn/kinds.py` & `file-name-attributes-0.2.4/src/vlju/types/urn/kinds.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vlju/types/urn/urn_test.py` & `file-name-attributes-0.2.4/src/vlju/types/urn/urn_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     assert str(u3) == 'urn:kind:v/%3F/a/%23/l/(u)/e?+r?=q'
     assert u3.spath() == 'v/%3F/a/%23/l/(u)/e'
     assert u3.scheme() == 'urn'
     assert u3.authority() == Authority('kind')
     assert u3.sauthority() == 'kind'
     assert u3.query() is None
     assert u3.fragment() is None
-    assert u3.sfragment() == ''  # noqa: compare-to-empty-string
+    assert u3.sfragment() == ''
 
     u4 = copy.copy(u3)
     assert u4 is not u3
     assert u4 == u3
     assert str(u4) == 'urn:kind:v/%3F/a/%23/l/(u)/e?+r?=q'
 
     v = Vlju('v')
```

### Comparing `file-name-attributes-0.2.3/src/vlju/vlju_test.py` & `file-name-attributes-0.2.4/src/vlju/vlju_test.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vljum/__init__.py` & `file-name-attributes-0.2.4/src/vljum/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from collections import defaultdict
 from collections.abc import Mapping, MutableMapping
 from pathlib import Path
 from typing import Any, Self, TextIO
 
 import util.io
 
+from util.error import Error
 from util.registry import Registry
 from vlju.types.all import URI, URL, File, Vlju
 from vljumap import VljuFactory, VljuMap, enc
 
 VljuArg = Vlju | str | None
 EncoderArg = enc.Encoder | str | None
 FactoryArg = VljuFactory | str | None
@@ -28,16 +29,17 @@
 
     def __init__(self, i: VljuMap | File | Path | str | object = None) -> None:
         super().__init__()
         self.factory = copy.copy(self.default_registry['factory'])
         self.encoder = copy.copy(self.default_registry['encoder'])
         self.decoder = copy.copy(self.default_registry['decoder'])
         self.mode = copy.copy(self.default_registry['mode'])
-        self.original_path: Path
-        self.modified_path: Path
+        self._original_path: Path
+        self._current_dir: Path
+        self._current_suffix: str
         self._set_path(Path())
         if i is not None:
             if isinstance(i, VljuMap):
                 self.extend(i)
             elif isinstance(i, File):
                 self.file(i.filename())
             elif isinstance(i, Path):
@@ -80,15 +82,15 @@
         return self.submap(args)
 
     def file(self,
              s: str | Path,
              decoder: EncoderArg = None,
              factory: FactoryArg = None) -> Self:
         self._set_path(s)
-        self.decoder.get(decoder).decode(self, self.original_path.stem,
+        self.decoder.get(decoder).decode(self, self._original_path.stem,
                                          self.factory.get(factory))
         return self
 
     def order(self, *args: str) -> Self:
         return self.sortkeys(args or None)
 
     def read(self,
@@ -107,42 +109,45 @@
         if v is None:
             del self[k]
             return self
         super().remove(k, self._vlju(k, v, factory))
         return self
 
     def rename(self, encoder: EncoderArg = None, mode: ModeArg = None) -> Self:
-        self.modified_path = self.filename(encoder, self.mode.get(mode))
-        if self.modified_path.exists():
-            if self.modified_path.samefile(self.original_path):
+        if self._original_path == Path():
+            message = 'no file to rename'
+            raise Error(message)
+        modified_path = self.filename(encoder, self.mode.get(mode))
+        if modified_path.exists():
+            if modified_path.samefile(self._original_path):
                 return self
-            raise FileExistsError(self.modified_path)
-        self.original_path.rename(self.modified_path)
-        self.original_path = self.modified_path
+            raise FileExistsError(modified_path)
+        self._original_path.rename(modified_path)
+        self._set_path(modified_path)
         return self
 
     def reset(self,
               k: str,
               v: VljuArg = None,
               factory: FactoryArg = None) -> Self:
         del self[k]
         return self.add(k, v, factory)
 
     def sort(self, *args: str, mode: ModeArg = None) -> Self:
         return self.sortvalues(args or None,
                                lambda v: v.get(self.mode.get(mode)))
 
     def with_dir(self, s: str | Path) -> Self:
-        self.modified_path = Path(s) / self.modified_path.name
+        self._current_dir = Path(s)
         return self
 
     def with_suffix(self, suffix: str) -> Self:
         if not suffix.startswith('.'):
             suffix = '.' + suffix
-        self.modified_path = self.modified_path.with_suffix(suffix)
+        self._current_suffix = suffix
         return self
 
     def write(self,
               file: util.io.PathLike = '-',
               encoder: EncoderArg = None,
               mode: ModeArg = None) -> Self:
         with util.io.open_output(file, sys.stdout) as f:
@@ -152,16 +157,14 @@
     def z(self, file: TextIO = sys.stderr) -> Self:  # pragma: no coverage
         print(repr(self), file=file)
         return self
 
     # String reductions.
 
     def __str__(self) -> str:
-        if self.modified_path == Path():
-            return self.encode()
         return str(self.filename())
 
     def lv(self) -> str:
         return self.encode(mode='long')
 
     def encode(self, encoder: EncoderArg = None, mode: ModeArg = None) -> str:
         return self.encoder.get(encoder).encode(self, self.mode.get(mode))
@@ -180,19 +183,25 @@
         return self._url(URI).encode(encoder)
 
     def url(self, encoder: EncoderArg = 'value') -> str:
         return self._url(URL).encode(encoder)
 
     # Filename reduction.
 
+    def original(self) -> Path:
+        return self._original_path
+
     def filename(self,
                  encoder: EncoderArg = None,
                  mode: ModeArg = None) -> Path:
-        return self.modified_path.with_stem(
-            self.encode(encoder, self.mode.get(mode)))
+        e = self.encode(encoder, self.mode.get(mode))
+        if not e:
+            message = 'no file name'
+            raise Error(message)
+        return (self._current_dir / e).with_suffix(self._current_suffix)
 
     # Vlju reduction.
 
     def first(self, k: str | type[Vlju]) -> Vlju:
         if isinstance(k, str):
             if k in self:
                 return self[k][0]
@@ -203,19 +212,20 @@
         return Vlju('')
 
     # Helpers.
 
     def _set_path(self, s: str | Path) -> Self:
         if isinstance(s, str):
             s = Path(s)
-        self.original_path = s
-        self.modified_path = s
+        self._original_path = s
+        self._current_dir = s.parent
+        self._current_suffix = s.suffix
         return self
 
-    def _url(self, cls: type[Vlju]) -> Self:
+    def _url(self, cls: type) -> Self:
         # Try hard to get URIs/URLs from the current map.
         out = type(self)()
         strings: list[tuple[str, str]] = []
         for k, v in self.pairs():
             try:
                 u = cls(v)
             except TypeError:
@@ -242,15 +252,14 @@
         elif isinstance(v, str):
             _, r = self.factory.get(factory)(k, v)
         else:
             r = v
         return r
 
     def __repr__(self) -> str:
-        return (f'{type(self).__name__}'
-                f'({dict(self.data)!r},path={self.modified_path})')
+        return f'{type(self).__name__}({dict(self.data)!r})'
 
     @classmethod
     def configure_options(cls, options: Mapping[str, Any]) -> None:
         for r in cls.default_registry:
             if (v := options.get(r)) is not None:
                 cls.default_registry[r].set_default(v)
```

### Comparing `file-name-attributes-0.2.3/src/vljum/m.py` & `file-name-attributes-0.2.4/src/vljum/m.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,49 +6,54 @@
 from typing import Any
 
 from util.registry import Registry
 from vlju.types.all import VLJU_TYPES, Vlju
 from vlju.types.site import site_class
 from vljum import VljuM
 from vljumap import enc
-from vljumap.factory import MappedFactory, default_factory
+from vljumap.factory import LooseMappedFactory, MappedFactory, default_factory
 
 V = Vlju
 
 class M(VljuM):
     """Configured subclass of VljuM."""
 
     raw_factory = default_factory
-    typed_factory = MappedFactory(VLJU_TYPES)
+    strict_factory = MappedFactory(VLJU_TYPES)
+    loose_factory = LooseMappedFactory(VLJU_TYPES)
     default_registry = {
         'factory':
             Registry().update({
                 'raw': raw_factory,
-                'typed': typed_factory,
-            }).set_default('typed'),
+                'typed': loose_factory,
+                'loose': loose_factory,
+                'strict': strict_factory,
+            }).set_default('loose'),
         'encoder':
             Registry().update(enc.encoder).set_default('v3'),
         'decoder':
             Registry().update(enc.decoder).set_default('v3'),
         'mode':
             Registry().update({
                 k: k
                 for k in ('short', 'long', 'repr')
             }).set_default('short'),
     }
 
     @classmethod
     def configure_sites(cls, site: Mapping[str, Mapping[str, Any]]) -> None:
         for k, s in site.items():
-            cls.typed_factory.setitem(k, site_class(**s))
+            scls = site_class(**s)
+            cls.strict_factory.setitem(k, scls)
+            cls.loose_factory.setitem(k, scls)
 
     @classmethod
     def exports(cls) -> dict[str, Any]:
         x = EXPORTS.copy()
-        for k, v in cls.typed_factory.kmap.items():
+        for k, v in cls.strict_factory.kmap.items():
             x[k] = v
             x[v.__name__] = v
         return x
 
     @classmethod
     def evaluate(cls,
                  s: str,
```

### Comparing `file-name-attributes-0.2.3/src/vljum/m_test.py` & `file-name-attributes-0.2.4/src/vljum/m_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from copy import deepcopy
 from io import StringIO
 from pathlib import Path
 
 import pytest
 
+from util.error import Error
 from util.registry import Registry
 from vlju.testutil import CastParams
 from vlju.types.all import ISBN, URL, File
 from vljum.m import M, V
 
 class TstVlju(V):
     """Vlju subclass for testing."""
@@ -28,27 +29,27 @@
     N.configure_options({'decoder': 'v2', 'encoder': 'v1'})
     m = N().decode('{key=value; isbn=1234567890}')
     assert m.encode() == '[key=value,isbn=9781234567897]'
 
 def test_configure_sites():
 
     class N(M):
-        typed_factory = deepcopy(M.typed_factory)
+        strict_factory = deepcopy(M.strict_factory)
         default_registry = deepcopy(M.default_registry)
-        default_registry['factory'] = Registry().set_default(typed_factory)
+        default_registry['factory'] = Registry().set_default(strict_factory)
 
     N.configure_sites({
         'test': {
             'name': 'SiteTest',
             'scheme': 'http',
             'host': 'example.com',
             'path': 'a/{x}/b',
         },
     })
-    pprint.pp(M.typed_factory.kmap)
+    pprint.pp(M.strict_factory.kmap)
     m = N().decode('[test=123]').z()
     assert m.url() == 'http://example.com/a/123/b'
 
 def test_m_construct_vljumap():
     m = M().add('key', 'value').add('key', 'two')
     mm = M(m)
     assert mm.encode() == '[key=value; key=two]'
@@ -56,28 +57,28 @@
 def test_m_construct_file():
     m = M(File('/blah/Title [isbn=1234567890].pdf'))
     assert m.encode('keyvalue') == 'title: Title\nisbn: 9781234567897'
 
 def test_m_construct_path():
     p = Path('/blah/Title [isbn=1234567890].pdf')
     m = M(p)
-    assert m.encode() == ''  # noqa: compare-to-empty-string
-    assert m.original_path == p
+    assert m.encode() == ''
+    assert m.original() == p
 
 def test_m_construct_str():
     m = M('Title [isbn=1234567890]')
     assert m.encode('keyvalue') == 'title: Title\nisbn: 9781234567897'
 
 def test_m_construct_cast_params():
     m = M(CastParams(None, {'a': V('42')}))
     assert str(m) == '[a=42]'
 
 def test_m_construct_cast_params_with_path():
     p = Path('/blah/Title [isbn=1234567890].pdf')
-    m = M(CastParams(p, {'a': V('42')}))
+    m = M(CastParams(str(p), {'a': V('42')}))
     assert str(m.filename()) == '/blah/[a=42].pdf'
 
 def test_m_construct_other():
     with pytest.raises(TypeError):
         _ = M(1)
 
 def test_m_add_string():
@@ -88,15 +89,15 @@
     m = M().add('key', TstVlju('value'))
     assert m.encode() == '[key=value]'
     assert isinstance(m['key'][0], TstVlju)
 
 def test_m_add_none():
     m = M().add('key')
     assert m.encode() == '[key]'
-    assert str(m['key'][0]) == ''  # noqa: compare-to-empty-string
+    assert str(m['key'][0]) == ''
 
 def test_m_add_explicit_factory():
     m = M().add('isbn', '1234567897', tst_vlju_factory)
     assert m.encode() == '[isbn=1234567897]'
     assert isinstance(m['isbn'][0], TstVlju)
 
 def test_m_add_implicit_factory():
@@ -107,34 +108,39 @@
     m = M().decode('[key=value; isbn=1234567890]')
     assert m.keys() == {'key', 'isbn'}
     assert str(m['key'][0]) == 'value'
     assert str(m['isbn'][0]) == '9781234567897'
 
 def test_m_dir():
     m = M().file('/blah/f.pdf').with_dir('/etc')
-    assert m.modified_path == Path('/etc/f.pdf')
+    assert m.filename() == Path('/etc/f.pdf')
 
 def test_m_extract():
     m = M().decode('[key=value; x=1; isbn=1234567890]').extract('key', 'isbn')
     assert m.keys() == {'key', 'isbn'}
     assert str(m['key'][0]) == 'value'
     assert str(m['isbn'][0]) == '9781234567897'
 
 def test_m_file():
     p = '/blah/Title [isbn=1234567890].pdf'
     m = M().file(p)
-    assert m.original_path == Path(p)
+    assert m.original() == Path(p)
     assert str(m) == '/blah/Title [isbn=9781234567897].pdf'
 
 def test_m_filename():
     p = '/blah/[isbn=1234567890].pdf'
     m = M().file(p).add('title', 'Title')
-    assert m.original_path == Path(p)
+    assert m.original() == Path(p)
     assert m.filename() == Path('/blah/Title [isbn=9781234567897].pdf')
 
+def test_m_filename_empty():
+    m = M()
+    with pytest.raises(Error):
+        _ = m.filename()
+
 def test_m_first_key():
     m = M().decode('[y=1; y=2; x=a]')
     v = m.first('y')
     assert str(v) == '1'
 
 def test_m_first_type():
     m = M().decode('[isbn=1234567890; isbn=9876543210; x=a]')
@@ -167,26 +173,26 @@
 
 def test_m_order_all():
     m = M().decode('[z=1; y=2; x=a]').order()
     assert str(m) == '[x=a; y=2; z=1]'
 
 def test_m_q():
     m = M().add('key', 'one')
-    assert m.q() == ''  # noqa: compare-to-empty-string
+    assert m.q() == ''
 
 def test_m_read():
     f = StringIO('[key=value; isbn=1234567890]')
     m = M().read(f)
     assert str(m) == '[key=value; isbn=9781234567897]'
 
 def test_m_rename(monkeypatch):
     p = Path('/blah/[isbn=1234567890].jpeg')
     q = Path('/home/sfc/Title [isbn=9781234567897].jpg')
     m = M().file(p)
-    assert m.original_path == p
+    assert m.original() == p
 
     def mk_mock_rename():
         d = {}
 
         def mock(self, target):
             d['src'] = self
             d['dst'] = target
@@ -194,18 +200,23 @@
 
         return (mock, d)
 
     mock_rename, result = mk_mock_rename()
     monkeypatch.setattr(Path, 'rename', mock_rename)
 
     m.with_dir('/home/sfc').with_suffix('jpg').add('title', 'Title').rename()
-    assert m.original_path == q
+    assert m.original() == q
     assert result['src'] == p
     assert result['dst'] == q
 
+def test_m_rename_no_original():
+    m = M()
+    with pytest.raises(Error, match='no file'):
+        m.rename()
+
 def test_m_rename_exists(monkeypatch):
     m = M().file('/etc/passwd')
     monkeypatch.setattr(Path, 'exists', lambda _: True)
     monkeypatch.setattr(Path, 'samefile', lambda _1, _2: False)
     with pytest.raises(FileExistsError):
         m.rename()
 
@@ -241,21 +252,21 @@
     m = M().add('isbn', '1234567890')
     assert str(m) == '[isbn=9781234567897]'
     m.encoder.set_default('keyvalue')
     assert str(m) == 'isbn: 9781234567897'
 
 def test_m_suffix():
     m = M().file('/blah/f.pdf').with_suffix('jpg')
-    assert m.original_path == Path('/blah/f.pdf')
-    assert m.modified_path == Path('/blah/f.jpg')
+    assert m.original() == Path('/blah/f.pdf')
+    assert m.filename() == Path('/blah/f.jpg')
 
 def test_m_suffix_dot():
     m = M().file('/blah/f.pdf').with_suffix('.jpg')
-    assert m.original_path == Path('/blah/f.pdf')
-    assert m.modified_path == Path('/blah/f.jpg')
+    assert m.original() == Path('/blah/f.pdf')
+    assert m.filename() == Path('/blah/f.jpg')
 
 def test_m_uri():
     m = M().decode('[a=1; doi=10.1234,56-78; v=foo/bar]')
     assert m.uri() == ('info:doi/10.1234/56-78\n'
                        'http://foo/bar')
 
 def test_m_url():
@@ -266,22 +277,22 @@
     f = StringIO()
     M().add('key', 'one').write(f)
     assert f.getvalue() == '[key=one]'
 
 def test_m_to_file():
     p = '/blah/[isbn=1234567890].pdf'
     m = M().file(p).add('title', 'Title')
-    assert m.original_path == Path(p)
+    assert m.original() == Path(p)
     f = File(m)
     assert str(f) == '/blah/Title [isbn=9781234567897].pdf'
 
 def test_m_to_url():
     p = '/blah/[isbn=1234567890].pdf'
     m = M().file(p).add('title', 'Title')
-    assert m.original_path == Path(p)
+    assert m.original() == Path(p)
     f = URL(m)
     assert str(f) == 'file:///blah/Title%20%5Bisbn=9781234567897%5D.pdf'
 
 def test_m_to_other():
     with pytest.raises(TypeError):
         _ = M().cast_params(int)
```

### Comparing `file-name-attributes-0.2.3/src/vljum/runner.py` & `file-name-attributes-0.2.4/src/vljum/runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,14 +63,30 @@
         Synopsis: add ‹key› ‹value›
         """
         key = self.need(f'{cmd}: expected key')
         val = self.need(f'{cmd}: expected value')
         self.m.add(key, val)
         self.report = True
 
+    def command_compare(self, _: str) -> None:
+        """
+        Print the original and current encoded file name if they differ.
+
+        Encodes using the current active encoder.
+        This can be used as a ‘dry run’ for `rename`.
+
+        Synopsis: compare
+        """
+        original = self.m.original()
+        current = self.m.filename()
+        if current != original:
+            print(original)
+            print(current)
+        self.report = False
+
     def command_decode(self, cmd: str) -> None:
         """
         Decode a string.
 
         Decodes using the current active decoder.
 
         Synopsis: decode ‹string›
@@ -96,14 +112,19 @@
         Synopsis: delete ‹key›[,‹key›]*
         """
         for key in self.need(f'{cmd}: expected keys').split(','):
             self.m.remove(key)
         self.report = True
 
     def command_dir(self, cmd: str) -> None:
+        """
+        Set the directory associated with a file name.
+
+        Synopsis: dir ‹directory›
+        """
         self.m.with_dir(self.need(f'{cmd}: expected directory'))
         self.report = True
 
     def command_encode(self, _: str) -> None:
         """
         Encode and prints the current attributes.
 
@@ -231,14 +252,23 @@
         """
         key = self.need(f'{cmd}: expected key')
         val = self.need(f'{cmd}: expected value')
         self.m.remove(key, val)
         self.report = True
 
     def command_rename(self, _: str) -> None:
+        """
+        Rename a file.
+
+        If attributes, directory, or suffix have changed since the
+        file name decoding, rename the original file according
+        to the current state.
+
+        Synopsis: rename
+        """
         self.m.rename()
         self.report = False
 
     def command_set(self, cmd: str) -> None:
         """
         Set an attribute.
 
@@ -262,14 +292,19 @@
         if t == '--all':
             self.m.sort()
         else:
             self.m.sort(*t.split(','))
         self.report = True
 
     def command_suffix(self, cmd: str) -> None:
+        """
+        Set the suffix associated with a file name.
+
+        Synopsis: suffix ‹ext›
+        """
         self.m.with_suffix(self.need(f'{cmd}: expected suffix'))
         self.report = True
 
     def command_uri(self, _: str) -> None:
         """
         Print attribute URI(s).
```

### Comparing `file-name-attributes-0.2.3/src/vljum/runner_test.py` & `file-name-attributes-0.2.4/src/vljum/runner_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,26 @@
     assert r.m.encode() == MK_V3
 
 def test_runner_command_add():
     r = mk(MK_IN)
     r.runs('add y 7 set y 8 add y 9 set x 7')
     assert r.m.encode() == '[z=Z; z=Y; y=8; y=9; x=7]'
 
+def test_runner_command_compare_different(capsys):
+    r = mk(args=['sfc', 'file', D1SFC, 'order', 'a,isbn,edition', 'quiet'])
+    r.runs('v3 compare')
+    assert capsys.readouterr().out == f'{D1SFC}\n{D1V3}\n'
+    assert not r.report
+
+def test_runner_command_compare_same(capsys):
+    r = mk(args=['file', D1V3, 'quiet'])
+    r.runs('compare')
+    assert capsys.readouterr().out == ''
+    assert not r.report
+
 def test_runner_command_decode():
     r = mk()
     r.run(['decode', MK_V3])
     assert r.m == vljum.m.M().add_pairs(MK_IN)
 
 def test_runner_command_decoder():
     r = mk()
```

### Comparing `file-name-attributes-0.2.3/src/vljumap/__init__.py` & `file-name-attributes-0.2.4/src/vljumap/__init__.py`

 * *Files identical despite different names*

### Comparing `file-name-attributes-0.2.3/src/vljumap/enc.py` & `file-name-attributes-0.2.4/src/vljumap/enc.py`

 * *Files 0% similar despite different names*

```diff
@@ -523,15 +523,15 @@
   Attributes are encoded as shell arrays (ksh, bash).
   Decoding is not implemented.
 """
 
 def shell_encode(n: VljuMap, mode: str | None = None) -> str:
     r = []
     for k, vlist in n.get_lists(mode):
-        v = ' '.join(shlex.quote(v) for v in vlist)
+        v = ' '.join(shlex.quote(v) for v in vlist if v is not None)
         r.append(f'{k}=({v})')
     return '\n'.join(r)
 
 sh = _register_encoder(
     Encoder('sh', shell_encode, _unimplemented_decode, SHELL_DESC,
             SHELL_DESCRIPTION))
```

### Comparing `file-name-attributes-0.2.3/src/vljumap/enc_test.py` & `file-name-attributes-0.2.4/src/vljumap/enc_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,34 +178,34 @@
         'v3': ('Mr. Book [a=Paul Penman; a=Writer, W; lccn=89-456]'),
         'v2': ('Mr. Book {a=Paul Penman;a=Writer, W;lccn=89-456}'),
         'v1': ('Paul Penman; Writer, W: Mr. Book [lccn=89-456]'),
         'v0': ('Paul Penman; Writer, W: Mr. Book lccn=89-456'),
     },
 }
 
-CASES_MVE_ENCODE = [(CASES[c]['MAP'], v, CASES[c][v])
-                    for c in CASES
-                    for v in set(CASES[c].keys()) - {'MAP' }]
+CASES_MVE_ENCODE = [(d['MAP'], v, d[v])
+                    for d in CASES.values()
+                    for v in set(d.keys()) - {'MAP'}]
 
 @pytest.mark.parametrize(('m', 'v', 'e'), CASES_MVE_ENCODE)
 def test_encode(m, v, e):
     if v in enc.encoder:
-        assert enc.encoder[v].encode(m) == e
+        assert enc.encoder[v].encode(m, None) == e
 
 CASES_MVE_DECODE = filter(lambda t: t[1] not in ('sfc', 'sh', 'v0', 'value'),
                           CASES_MVE_ENCODE)
 
 @pytest.mark.parametrize(('m', 'v', 'e'), CASES_MVE_DECODE)
 def test_decode(m, v, e):
     if v in enc.encoder:
         assert enc.encoder[v].decode(VljuMap(), e, TstEncVlju.factory) == m
 
 def test_v3_encode_doi():
     m = VljuMap().add('doi', DOI('10.12345/67890'))
-    assert enc.v3.encode(m) == '[doi=10.12345,67890]'
+    assert enc.v3.encode(m, None) == '[doi=10.12345,67890]'
 
 def test_v3_decode_title_only():
     v = enc.v3.decode(VljuMap(), 'Title', TstEncVlju.factory)['title'][0]
     assert str(v) == 'Title'
 
 def test_v3_decode_missing_close():
     with pytest.warns(UserWarning, match='Expected'):
@@ -238,29 +238,29 @@
     assert enc.sfc.decode(VljuMap(), CASES['C']['sfc'],
                           TstEncVlju.factory) == CASES['C']['MAP']
     assert enc.sfc.decode(VljuMap(), CASES['D']['sfc'],
                           TstEncVlju.factory) == CASES['D']['MAP'].submap(
                               ['title', 'a', 'isbn', 'edition', 'date'])
 
 def test_json_encode():
-    assert enc.json.encode(CASES['A']['MAP']) == CASES['A']['json']
-    assert enc.json.encode(CASES['B']['MAP']) == CASES['B']['json']
-    assert enc.json.encode(CASES['C']['MAP']) == CASES['C']['json']
-    assert enc.json.encode(CASES['D']['MAP']) == CASES['D']['json']
+    assert enc.json.encode(CASES['A']['MAP'], None) == CASES['A']['json']
+    assert enc.json.encode(CASES['B']['MAP'], None) == CASES['B']['json']
+    assert enc.json.encode(CASES['C']['MAP'], None) == CASES['C']['json']
+    assert enc.json.encode(CASES['D']['MAP'], None) == CASES['D']['json']
 
 def test_json_decode():
     assert enc.json.decode(VljuMap(), CASES['D']['json2'],
                            TstEncVlju.factory) == CASES['D']['MAP']
 
 def test_keyvalue_decode():
     assert enc.keyvalue.decode(VljuMap(), CASES['D']['keyvalue'] + '\n',
                                TstEncVlju.factory) == CASES['D']['MAP']
 
 def test_sh_encode():
-    assert enc.sh.encode(CASES['D']['MAP']) == CASES['D']['sh']
+    assert enc.sh.encode(CASES['D']['MAP'], None) == CASES['D']['sh']
 
 def test_can_encode():
     assert enc.v3.can_encode()
     assert enc.sh.can_encode()
 
 def test_can_decode():
     assert enc.v3.can_decode()
```

### Comparing `file-name-attributes-0.2.3/src/vljumap/factory.py` & `file-name-attributes-0.2.4/src/vljumap/factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,7 +30,17 @@
 
     def __call__(self, k: str, v: str) -> tuple[str, Vlju]:
         try:
             return (k, self.kmap.get(k, self.default)(v))
         except Exception as e:  # noqa: blind-except
             msg = f'{k} {v}'
             raise FactoryError(msg) from e
+
+class LooseMappedFactory(MappedFactory):
+    """VljuFactory that maps keys for Vlju types, and reverts to default."""
+
+    def __call__(self, k: str, v: str) -> tuple[str, Vlju]:
+        try:
+            value = self.kmap.get(k, self.default)(v)
+        except Exception:  # noqa: blind-except
+            value = self.default(v)
+        return (k, value)
```

### Comparing `file-name-attributes-0.2.3/src/vljumap/factory_test.py` & `file-name-attributes-0.2.4/src/vljumap/factory_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,34 @@
 
 from util.pytestutil import it2p
 from vlju import Vlju
 from vlju.types.ean import EAN13
 from vlju.types.ean.isbn import ISBN
 from vlju.types.ean.ismn import ISMN
 from vlju.types.ean.issn import ISSN
-from vljumap.factory import FactoryError, MappedFactory
+from vljumap.factory import FactoryError, LooseMappedFactory, MappedFactory
 
 # yapf: disable
 CASES = [
     ('key',     'cls',  'value'),
     ('ean13',   EAN13,  '4534530128942'),
     ('isbn',    ISBN,   '9780804429573'),
     ('ismn',    ISMN,   '9790692006282'),
     ('issn',    ISSN,   '9771351538009'),
 ]
 # yapf: enable
 
 @pytest.fixture(name='factory')
-def fixture_factory():
+def fixture_mapped_factory():
     return MappedFactory({key: cls for key, cls, _ in CASES}, Vlju)
 
+@pytest.fixture(name='loose_factory')
+def fixture_loose_factory():
+    return LooseMappedFactory({key: cls for key, cls, _ in CASES}, Vlju)
+
 @pytest.mark.parametrize(*it2p(CASES))
 def test_mapped_factory(factory, key, cls, value):
     k, v = factory(key, value)
     assert k == key
     assert str(v) == value
     assert type(v) == cls   # pylint: disable=unidiomatic-typecheck
 
@@ -39,8 +43,13 @@
 def test_mapped_factory_setitem(factory):
     factory.setitem('isbn', EAN13)
     _, v = factory('isbn', '9780804429573')
     assert type(v) == EAN13  # pylint: disable=unidiomatic-typecheck
 
 def test_mapped_factory_catch(factory):
     with pytest.raises(FactoryError):
-        _ = factory('isbn', 1)
+        _ = factory('isbn', '123')
+
+def test_loose_mapped_factory(loose_factory):
+    _, v = loose_factory('isbn', '123')
+    assert type(v) == Vlju  # pylint: disable=unidiomatic-typecheck
+    assert str(v) == '123'
```

### Comparing `file-name-attributes-0.2.3/src/vljumap/vljumap_test.py` & `file-name-attributes-0.2.4/src/vljumap/vljumap_test.py`

 * *Files identical despite different names*

