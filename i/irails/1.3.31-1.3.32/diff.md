# Comparing `tmp/irails-1.3.31.tar.gz` & `tmp/irails-1.3.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.31.tar", last modified: Sat May 27 08:52:36 2023, max compression
+gzip compressed data, was "irails-1.3.32.tar", last modified: Sat May 27 12:10:09 2023, max compression
```

## Comparing `irails-1.3.31.tar` & `irails-1.3.32.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.513137 irails-1.3.31/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.31/MANIFEST.in
--rw-rw-rw-   0        0        0     4878 2023-05-27 08:52:36.512140 irails-1.3.31/PKG-INFO
--rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.31/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.408269 irails-1.3.31/irails/
--rw-rw-rw-   0        0        0      307 2023-05-27 08:52:24.000000 irails-1.3.31/irails/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.31/irails/_i18n.py
--rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.31/irails/_loader.py
--rw-rw-rw-   0        0        0     5595 2023-05-27 08:18:04.000000 irails-1.3.31/irails/_utils.py
--rw-rw-rw-   0        0        0    14149 2023-05-27 08:28:58.000000 irails-1.3.31/irails/auth.py
--rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.31/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.417244 irails-1.3.31/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.420236 irails-1.3.31/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0     9284 2023-05-25 05:11:53.000000 irails-1.3.31/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.31/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10591 2023-05-25 05:11:49.000000 irails-1.3.31/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.31/irails/cbv.py
--rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.31/irails/config.py
--rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.31/irails/controller_utils.py
--rw-rw-rw-   0        0        0    25443 2023-05-27 08:49:15.000000 irails-1.3.31/irails/core.py
--rw-rw-rw-   0        0        0    20988 2023-05-27 08:36:14.000000 irails-1.3.31/irails/database.py
--rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.31/irails/log.py
--rw-rw-rw-   0        0        0     8876 2023-05-27 05:49:02.000000 irails-1.3.31/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.31/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.31/irails/midware_session.py
--rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.31/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.434262 irails-1.3.31/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.31/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.31/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.31/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.31/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.31/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.31/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.31/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.31/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.31/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.31/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.31/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.377474 irails-1.3.31/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.448225 irails-1.3.31/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.31/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.31/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.31/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.31/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.31/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.31/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.31/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.31/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.31/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.450543 irails-1.3.31/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.31/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.451543 irails-1.3.31/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.31/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.465505 irails-1.3.31/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.31/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.31/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.31/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.481463 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.31/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.31/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.31/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.31/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.379469 irails-1.3.31/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.484455 irails-1.3.31/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.31/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.31/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.31/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.31/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.487446 irails-1.3.31/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.31/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.31/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.491438 irails-1.3.31/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.381464 irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.497541 irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.503659 irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.31/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.31/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.382461 irails-1.3.31/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.507649 irails-1.3.31/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.31/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     1737 2023-05-27 08:50:04.000000 irails-1.3.31/irails/unit_test.py
--rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.31/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.415250 irails-1.3.31/irails.egg-info/
--rw-rw-rw-   0        0        0     4878 2023-05-27 08:52:36.000000 irails-1.3.31/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3185 2023-05-27 08:52:36.000000 irails-1.3.31/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 08:52:36.000000 irails-1.3.31/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-27 08:52:36.000000 irails-1.3.31/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      367 2023-05-27 08:52:36.000000 irails-1.3.31/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-27 08:52:36.000000 irails-1.3.31/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 08:52:36.513137 irails-1.3.31/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.31/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.050382 irails-1.3.32/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.32/MANIFEST.in
+-rw-rw-rw-   0        0        0     4878 2023-05-27 12:10:09.050382 irails-1.3.32/PKG-INFO
+-rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.32/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.947497 irails-1.3.32/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-27 12:09:57.000000 irails-1.3.32/irails/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.32/irails/_i18n.py
+-rw-rw-rw-   0        0        0     3959 2023-05-27 11:52:24.000000 irails-1.3.32/irails/_loader.py
+-rw-rw-rw-   0        0        0     5595 2023-05-27 08:18:04.000000 irails-1.3.32/irails/_utils.py
+-rw-rw-rw-   0        0        0    14149 2023-05-27 08:28:58.000000 irails-1.3.32/irails/auth.py
+-rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.32/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.958473 irails-1.3.32/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.962458 irails-1.3.32/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0     9284 2023-05-25 05:11:53.000000 irails-1.3.32/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.32/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10591 2023-05-25 05:11:49.000000 irails-1.3.32/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.32/irails/cbv.py
+-rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.32/irails/config.py
+-rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.32/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    26026 2023-05-27 10:48:38.000000 irails-1.3.32/irails/core.py
+-rw-rw-rw-   0        0        0    20988 2023-05-27 08:36:14.000000 irails-1.3.32/irails/database.py
+-rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.32/irails/log.py
+-rw-rw-rw-   0        0        0     8876 2023-05-27 05:49:02.000000 irails-1.3.32/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.32/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.32/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4219 2023-05-27 10:24:12.000000 irails-1.3.32/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.975468 irails-1.3.32/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.32/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.32/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.32/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.32/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.32/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.32/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.32/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.32/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.32/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.32/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.32/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.912676 irails-1.3.32/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.989292 irails-1.3.32/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.32/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.32/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.32/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.32/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.32/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.32/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.32/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.32/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.32/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.992277 irails-1.3.32/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.32/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.993275 irails-1.3.32/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.32/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.005241 irails-1.3.32/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.32/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.32/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.32/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.019209 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.32/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.32/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.32/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.32/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.917102 irails-1.3.32/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.023194 irails-1.3.32/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.32/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.32/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.32/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.32/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.026193 irails-1.3.32/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.32/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.32/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.030174 irails-1.3.32/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.920096 irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.036191 irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.043179 irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.32/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.32/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.922094 irails-1.3.32/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.045907 irails-1.3.32/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.32/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1737 2023-05-27 08:50:04.000000 irails-1.3.32/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.32/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.956476 irails-1.3.32/irails.egg-info/
+-rw-rw-rw-   0        0        0     4878 2023-05-27 12:10:08.000000 irails-1.3.32/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3185 2023-05-27 12:10:08.000000 irails-1.3.32/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 12:10:08.000000 irails-1.3.32/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-27 12:10:08.000000 irails-1.3.32/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      367 2023-05-27 12:10:08.000000 irails-1.3.32/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-27 12:10:08.000000 irails-1.3.32/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 12:10:09.050382 irails-1.3.32/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.32/setup.py
```

### Comparing `irails-1.3.31/PKG-INFO` & `irails-1.3.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.31
+Version: 1.3.32
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.31/README.md` & `irails-1.3.32/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/_i18n.py` & `irails-1.3.32/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/_utils.py` & `irails-1.3.32/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/auth.py` & `irails-1.3.32/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/base_controller.py` & `irails-1.3.32/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc` & `irails-1.3.32/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.32/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.32/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/cbv.py` & `irails-1.3.32/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/config.py` & `irails-1.3.32/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/controller_utils.py` & `irails-1.3.32/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/core.py` & `irails-1.3.32/irails/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,27 +44,31 @@
         self.__casbin_auth:auth.AuthenticationBackend_ = None 
         self._data_engine:database.Engine = None
         self.__user_auth_url=""
         self.__public_auth_url=""
         self.__app_views_dirs = {} 
         self.routers_map = {}
         self.__apps_dirs = []
+        self.__apps = {}
         self.auth_user_class:auth.DomainUser = None
         super().__init__(**kwargs)
 
     def new_user(self,user:Union[database.Base,str])->auth.DomainUser:
         if not self.auth_user_class:
             raise RuntimeError('application.auth_class is None')
         if isinstance(user,str):
             return self.auth_user_class(username=user)
         elif isinstance(user,database.Base):
             userobj = self.auth_user_class(user.name)
             copy_attr(user,userobj,False)
             return userobj
-     
+    @property
+    def apps(self)->Dict:
+        return self.__apps
+    
     @property
     def app_views_dirs(self)->Dict:
         return self.__app_views_dirs
     @app_views_dirs.setter
     def app_views_dirs(self,key,value):
         self.__app_views_dirs[key]=value
     @property
@@ -196,24 +200,24 @@
     caller_file = caller_frame.f_code.co_filename
     relative_path = caller_file.replace(ROOT_PATH,"")
     if relative_path.count(os.sep)>2:
         app_dir = os.sep.join(relative_path.split(os.sep)[:-2]) # os.path.dirname(os.path.dirname(relative_path)).replace(os.sep,"")
     else:
         raise RuntimeError(_("app dir must in apps dir"))
      
-
+    app_name = os.path.basename(app_dir)
     def format_path(p,v):
         if p and not p.startswith("/"):
             raise RuntimeError(_("route path must start with '/',%s is not alowed!") % p)
         if p and  '{controller}' not in p :
             p += '/{controller}' 
             p += '/{version}' if v else ''
         if v and not path:
             p = "/{controller}/{version}"
-        app_name = os.path.basename(app_dir)
+        
         return p.replace("{app}",app_name)
     path = format_path(path,version) 
      
     abs_path = os.path.join(ROOT_PATH,app_dir.lstrip(os.sep))
 
     if os.path.dirname(abs_path) not in application.apps_dirs:
         application.apps_dirs.append(os.path.dirname(abs_path))
@@ -222,16 +226,18 @@
     
     
     
     
     def _wapper(targetController):  
         _name = app_dir.replace(os.sep,".").lstrip(".") + "." + targetController.__name__ + "@" + version 
         _controller_hash = f"{_name}" 
-        if not _controller_hash in __all_controller__:
-            __all_controller__[_controller_hash] = {'label':'new','obj': _controllerBase}
+        if not app_name in __all_controller__:
+            __all_controller__[app_name]={}
+        if _controller_hash not in __all_controller__[app_name]: 
+            __all_controller__[app_name][_controller_hash]= {'label':'new','obj': _controllerBase}
 
         class puppetController( targetController ,_controllerBase ): 
             '''puppet class inherited by the User defined controller class '''
             def __init__(self,**kwags) -> None: 
                 
                 super().__init__()
             def _user_logout(self,msg=_('you are successed logout!'),redirect:str="/"):
@@ -355,37 +361,41 @@
 def get_wrapped_endpoint(func):
     ret = func
     while hasattr(ret,'__wrapped__'):
         ret = getattr(ret,'__wrapped__')
     return ret
 def _register_controllers():
     global __is_debug
-    all_routers = []
-    all_routers_map = {}
-    for hash,dict_obj in __all_controller__.items():
-
-        if dict_obj['label'] == 'new':
-            if __is_debug:  
-                _log.info(hash+" mountting...")
-            all_routers.append(register_controllers_to_app(application, dict_obj['obj']))
-            dict_obj['label'] = 'mounted'
-
-    for router in all_routers:
-        for r in router.routes:
-            funcname = str(r.endpoint).split('<function ')[1].split(" at ")[0] 
-            end_point_abs = get_wrapped_endpoint(r.endpoint)
-            auth_type = getattr(end_point_abs,AUTH_KEY) if hasattr(end_point_abs,AUTH_KEY) else 'None'
-            doc_map =  get_docs(r.description) if hasattr(r,'description') else {}
-            if hasattr(r,'methods'):
-                methods = r.methods
-            else:
-                methods = r.name
-            if __is_debug:  
-                _log.info((str(methods),r.path,funcname) )
-            application.routers_map[funcname] = {'path':r.path,'methods':methods,'doc':doc_map,'auth':auth_type,"endpoint":r.endpoint}
+   
+    for app_name in __all_controller__:
+        for hash,dict_obj in __all_controller__[app_name].items():
+           
+            if dict_obj['label'] == 'new':
+                if __is_debug:  
+                    _log.info(hash+" mountting...")
+                app_router = register_controllers_to_app(application, dict_obj['obj'])
+                
+                application.apps[app_name]['router'] = app_router
+                dict_obj['label'] = 'mounted'
+
+             
+                for r in app_router.routes:
+                    funcname = str(r.endpoint).split('<function ')[1].split(" at ")[0] 
+                    end_point_abs = get_wrapped_endpoint(r.endpoint)
+                    auth_type = getattr(end_point_abs,AUTH_KEY) if hasattr(end_point_abs,AUTH_KEY) else 'None'
+                    doc_map =  get_docs(r.description) if hasattr(r,'description') else {}
+                    if hasattr(r,'methods'):
+                        methods = r.methods
+                    else:
+                        methods = r.name
+                    if __is_debug:  
+                        _log.info((str(methods),r.path,funcname) )
+                    if not 'route_map' in application.apps[app_name]: 
+                        application.apps[app_name]['route_map']={}
+                    application.apps[app_name]['route_map'][funcname] = {'path':r.path,'methods':methods,'doc':doc_map,'auth':auth_type,"endpoint":r.endpoint}
       
     _log.info(_("static files mouting..."))
     midware.init(app=application,debug=__is_debug)
 
 def check_db_migrate():
     db_cfg = config.get("database")
     if not db_cfg:return
@@ -419,22 +429,21 @@
             # Raise an error if the adapter is not supported
             if not _casbin_adapter_class:
                 raise RuntimeError(_("Not support %s ,Adapter config error in auth.casbin_adapter") % __type_casbin_adapter)
     return auth_type,_adapter_uri,_casbin_adapter_class
 def generate_mvc_app():
     global __is_debug
      
-    application.title = _project_name
-    
-    
-    
+    application.title = _project_name 
     
     _log.info(_("loading irails apps..."))
-    loaded,unloaded=_load_apps(debug=__is_debug) 
+    loaded,unloaded=_load_apps(debug=__is_debug,application=application) 
+
     _log.info(_('Load Apps Completed,%s loaded,%s unloaded') %(loaded,unloaded))  
+
     if not len(__all_controller__)>0:
         raise RuntimeError(_("not found any controller class"))
     
     _register_controllers()
 
     
     _log.info(_("checking database configure..."))
```

### Comparing `irails-1.3.31/irails/database.py` & `irails-1.3.32/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/log.py` & `irails-1.3.32/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/midware.py` & `irails-1.3.32/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/midware_casbin.py` & `irails-1.3.32/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/midware_session.py` & `irails-1.3.32/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/mvc_router.py` & `irails-1.3.32/irails/mvc_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     #     def add_api_route(self, path: str, endpoint: Callable[..., Any], **kwargs: Any) -> None:
     #         if kwargs.get("response_model") is None:
     #             kwargs["response_model"] = get_type_hints(endpoint).get("return")
     #         return super().add_api_route(path, endpoint, **kwargs)
         
 def register_controllers_to_app(app: FastAPI,
-                                controller_base: Type[ControllerBase]) -> None:
+                                controller_base: Type[ControllerBase]) -> InferringRouter:
     """
     Registers all the api routes inside child controllers of the base
     controller.
 
 
     Args:
       app: FastAPI: root FastAPI app
```

### Comparing `irails-1.3.31/irails/scripts/_app.py` & `irails-1.3.32/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/_controller.py` & `irails-1.3.32/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/_i18n.py` & `irails-1.3.32/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/_migrate.py` & `irails-1.3.32/irails/scripts/_migrate.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/_model.py` & `irails-1.3.32/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/_project.py` & `irails-1.3.32/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/_run.py` & `irails-1.3.32/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/_shell.py` & `irails-1.3.32/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/_test.py` & `irails-1.3.32/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/main.py` & `irails-1.3.32/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.32/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/app/home.tpl` & `irails-1.3.32/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/app/model.jinja` & `irails-1.3.32/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.32/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.32/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.32/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.32/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.32/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.32/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.32/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.32/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.32/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.32/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/unit_test.py` & `irails-1.3.32/irails/unit_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails/view.py` & `irails-1.3.32/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/irails.egg-info/PKG-INFO` & `irails-1.3.32/irails.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.31
+Version: 1.3.32
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.31/irails.egg-info/SOURCES.txt` & `irails-1.3.32/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.31/setup.py` & `irails-1.3.32/setup.py`

 * *Files identical despite different names*

