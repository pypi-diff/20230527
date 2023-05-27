# Comparing `tmp/ckanext-check-link-0.1.1.tar.gz` & `tmp/ckanext-check-link-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-check-link-0.1.1.tar", last modified: Tue May  9 14:31:46 2023, max compression
+gzip compressed data, was "ckanext-check-link-0.1.1.post1.tar", last modified: Sat May 27 14:38:39 2023, max compression
```

## Comparing `ckanext-check-link-0.1.1.tar` & `ckanext-check-link-0.1.1.post1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      205 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3125 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2466 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.817529 ckanext-check-link-0.1.1/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.817529 ckanext-check-link-0.1.1/ckanext/check_link/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.817529 ckanext-check-link-0.1.1/ckanext/check_link/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      162 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/assets/script.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/assets/style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      319 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5887 2023-05-05 15:31:50.000000 ckanext-check-link-0.1.1/ckanext/check_link/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      383 2023-05-05 15:31:11.000000 ckanext-check-link-0.1.1/ckanext/check_link/helpers.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.817529 ckanext-check-link-0.1.1/ckanext/check_link/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/logic/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/ckanext/check_link/logic/action/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      131 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/logic/action/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5377 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1/ckanext/check_link/logic/action/check.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3536 2022-08-25 20:38:04.000000 ckanext-check-link-0.1.1/ckanext/check_link/logic/action/report.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1791 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3615 2022-08-25 23:59:09.000000 ckanext-check-link-0.1.1/ckanext/check_link/logic/schema.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.817529 ckanext-check-link-0.1.1/ckanext/check_link/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/ckanext/check_link/migration/check_link/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1804 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/migration/check_link/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/migration/check_link/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/migration/check_link/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/ckanext/check_link/migration/check_link/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1103 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/ckanext/check_link/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      139 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1/ckanext/check_link/model/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2365 2023-05-05 15:32:57.000000 ckanext-check-link-0.1.1/ckanext/check_link/model/report.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1138 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1/ckanext/check_link/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/ckanext/check_link/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/ckanext/check_link/templates/check_link/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      889 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/templates/check_link/base.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      712 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/templates/check_link/base_admin.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2218 2023-05-05 15:06:35.000000 ckanext-check-link-0.1.1/ckanext/check_link/templates/check_link/report.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/ckanext/check_link/templates/check_link/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1538 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/templates/check_link/snippets/report_item.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      578 2022-11-07 20:13:48.000000 ckanext-check-link-0.1.1/ckanext/check_link/templates/header.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/ckanext/check_link/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      665 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1/ckanext/check_link/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/ckanext/check_link/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/tests/logic/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/ckanext/check_link/tests/logic/action/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/tests/logic/action/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3675 2023-05-05 15:33:16.000000 ckanext-check-link-0.1.1/ckanext/check_link/tests/logic/action/test_check.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4019 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1/ckanext/check_link/tests/logic/action/test_report.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/ckanext/check_link/tests/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/ckanext/check_link/tests/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1170 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1/ckanext/check_link/tests/model/test_report.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      210 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1/ckanext/check_link/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4146 2023-05-09 14:30:50.000000 ckanext-check-link-0.1.1/ckanext/check_link/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/ckanext_check_link.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3125 2023-05-09 14:31:46.000000 ckanext-check-link-0.1.1/ckanext_check_link.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1886 2023-05-09 14:31:46.000000 ckanext-check-link-0.1.1/ckanext_check_link.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-05-09 14:31:46.000000 ckanext-check-link-0.1.1/ckanext_check_link.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      127 2023-05-09 14:31:46.000000 ckanext-check-link-0.1.1/ckanext_check_link.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-05-09 14:31:46.000000 ckanext-check-link-0.1.1/ckanext_check_link.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       54 2023-05-09 14:31:46.000000 ckanext-check-link-0.1.1/ckanext_check_link.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-05-09 14:31:46.000000 ckanext-check-link-0.1.1/ckanext_check_link.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4447 2023-05-05 15:32:15.000000 ckanext-check-link-0.1.1/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1553 2023-05-09 14:31:46.827530 ckanext-check-link-0.1.1/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      205 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3904 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3239 2023-05-27 14:37:01.000000 ckanext-check-link-0.1.1.post1/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      162 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/assets/script.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/assets/style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      319 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5879 2023-05-27 14:34:21.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      383 2023-05-05 15:31:11.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/helpers.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/action/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      131 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/action/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5377 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/action/check.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3536 2022-08-25 20:38:04.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/action/report.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1791 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3615 2022-08-25 23:59:09.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/schema.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.760222 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1804 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1103 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      139 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/model/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2365 2023-05-05 15:32:57.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/model/report.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1138 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      889 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/base.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      712 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/base_admin.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2218 2023-05-05 15:06:35.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/report.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1538 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/snippets/report_item.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      578 2022-11-07 20:13:48.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/header.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      665 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/action/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/action/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3675 2023-05-05 15:33:16.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/action/test_check.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4019 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/action/test_report.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1170 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/model/test_report.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      210 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4146 2023-05-09 14:30:50.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3904 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1886 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      127 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       54 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4447 2023-05-05 15:32:15.000000 ckanext-check-link-0.1.1.post1/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1559 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/setup.py
```

### Comparing `ckanext-check-link-0.1.1/LICENSE` & `ckanext-check-link-0.1.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/PKG-INFO` & `ckanext-check-link-0.1.1.post1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-check-link
-Version: 0.1.1
+Version: 0.1.1.post1
 Summary: Resource URL checker
 Home-page: https://github.com/DataShades/ckanext-check-link
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
@@ -109,14 +109,45 @@
 $ ckan check-link check-packages --include-draft
 
 # check only two specified packages
 $ ckan check-link check-packages pkg-id-one pkg-name-two
 
 ```
 
+### `check-resources`
+Check every resource on the portal.
+
+Scope can be narrowed via arbitary number of arguments, specifying resource's ID
+
+### `delete-reports`
+Delete check-link reports.
+
+```sh
+# delete all reports
+$ ckan check-link delete-reports
+
+# drop reports that point to an unexisting resource
+$ ckan check-link delete-reports --orphans-only
+```
+
+Scope can be narrowed via arbitary number of arguments, specifying resource's ID
+
 ## API
 
+### `check_link_url_check`
+### `check_link_resource_check`
+### `check_link_package_check`
+### `check_link_organization_check`
+### `check_link_group_check`
+### `check_link_user_check`
+### `check_link_search_check`
+
+### `check_link_report_save`
+### `check_link_report_show`
+### `check_link_report_search`
+### `check_link_report_delete`
+
 TBA
 
 ## License
 
 [AGPL](https://www.gnu.org/licenses/agpl-3.0.en.html)
```

### Comparing `ckanext-check-link-0.1.1/README.md` & `ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: ckanext-check-link
+Version: 0.1.1.post1
+Summary: Resource URL checker
+Home-page: https://github.com/DataShades/ckanext-check-link
+Author: Sergey Motornyuk
+Author-email: sergey.motornyuk@linkdigital.com.au
+License: AGPL
+Keywords: CKAN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Tests](https://github.com/DataShades/ckanext-check-link/workflows/Tests/badge.svg?branch=main)](https://github.com/DataShades/ckanext-check-link/actions)
 
 # ckanext-check-link
 
 Link checker for CKAN.
 
 Provides API, CLI commands, and views for:
@@ -91,14 +109,45 @@
 $ ckan check-link check-packages --include-draft
 
 # check only two specified packages
 $ ckan check-link check-packages pkg-id-one pkg-name-two
 
 ```
 
+### `check-resources`
+Check every resource on the portal.
+
+Scope can be narrowed via arbitary number of arguments, specifying resource's ID
+
+### `delete-reports`
+Delete check-link reports.
+
+```sh
+# delete all reports
+$ ckan check-link delete-reports
+
+# drop reports that point to an unexisting resource
+$ ckan check-link delete-reports --orphans-only
+```
+
+Scope can be narrowed via arbitary number of arguments, specifying resource's ID
+
 ## API
 
+### `check_link_url_check`
+### `check_link_resource_check`
+### `check_link_package_check`
+### `check_link_organization_check`
+### `check_link_group_check`
+### `check_link_user_check`
+### `check_link_search_check`
+
+### `check_link_report_save`
+### `check_link_report_show`
+### `check_link_report_search`
+### `check_link_report_delete`
+
 TBA
 
 ## License
 
 [AGPL](https://www.gnu.org/licenses/agpl-3.0.en.html)
```

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/cli.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     "-t", "--timeout", default=10, help="Request timeout", type=click.FloatRange(0)
 )
 @click.argument("ids", nargs=-1)
 def check_resources(ids: tuple[str, ...], delay: float, timeout: float):
     """Check every resource on the portal.
 
     Scope can be narrowed via arbitary number of arguments, specifying
-    resource's ID or name.
+    resource's ID.
     """
     user = tk.get_action("get_site_user")({"ignore_auth": True}, {})
     context = {"user": user["name"]}
 
     check = tk.get_action("check_link_resource_check")
     q = model.Session.query(model.Resource.id).filter_by(state="active")
     if ids:
```

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/logic/action/check.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/action/check.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/logic/action/report.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/action/report.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/logic/auth.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/logic/schema.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/migration/check_link/alembic.ini` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/migration/check_link/env.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/model/report.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/model/report.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/plugin.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/templates/check_link/base.html` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/base.html`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/templates/check_link/base_admin.html` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/base_admin.html`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/templates/check_link/report.html` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/report.html`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/templates/check_link/snippets/report_item.html` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/snippets/report_item.html`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/templates/header.html` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/header.html`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/tests/conftest.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/tests/logic/action/test_check.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/action/test_check.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/tests/logic/action/test_report.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/action/test_report.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/tests/model/test_report.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/model/test_report.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext/check_link/views.py` & `ckanext-check-link-0.1.1.post1/ckanext/check_link/views.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/ckanext_check_link.egg-info/SOURCES.txt` & `ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/pyproject.toml` & `ckanext-check-link-0.1.1.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1/setup.cfg` & `ckanext-check-link-0.1.1.post1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-check-link
-version = 0.1.1
+version = 0.1.1.post1
 description = Resource URL checker
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-check-link
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

### Comparing `ckanext-check-link-0.1.1/setup.py` & `ckanext-check-link-0.1.1.post1/setup.py`

 * *Files identical despite different names*

