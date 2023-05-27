# Comparing `tmp/irails-1.3.30.tar.gz` & `tmp/irails-1.3.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.30.tar", last modified: Fri May 26 14:46:17 2023, max compression
+gzip compressed data, was "irails-1.3.31.tar", last modified: Sat May 27 08:52:36 2023, max compression
```

## Comparing `irails-1.3.30.tar` & `irails-1.3.31.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.421299 irails-1.3.30/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.30/MANIFEST.in
--rw-rw-rw-   0        0        0     4878 2023-05-26 14:46:17.420311 irails-1.3.30/PKG-INFO
--rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.30/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.324638 irails-1.3.30/irails/
--rw-rw-rw-   0        0        0      307 2023-05-26 14:46:02.000000 irails-1.3.30/irails/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.30/irails/_i18n.py
--rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.30/irails/_loader.py
--rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.30/irails/_utils.py
--rw-rw-rw-   0        0        0    14179 2023-05-26 14:38:40.000000 irails-1.3.30/irails/auth.py
--rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.30/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.336615 irails-1.3.30/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.339599 irails-1.3.30/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0     9284 2023-05-25 05:11:53.000000 irails-1.3.30/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.30/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10591 2023-05-25 05:11:49.000000 irails-1.3.30/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.30/irails/cbv.py
--rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.30/irails/config.py
--rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.30/irails/controller_utils.py
--rw-rw-rw-   0        0        0    24995 2023-05-26 14:01:10.000000 irails-1.3.30/irails/core.py
--rw-rw-rw-   0        0        0    20250 2023-05-25 14:04:48.000000 irails-1.3.30/irails/database.py
--rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.30/irails/log.py
--rw-rw-rw-   0        0        0     8736 2023-05-21 14:38:31.000000 irails-1.3.30/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.30/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.30/irails/midware_session.py
--rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.30/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.353682 irails-1.3.30/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.30/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.30/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.30/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.30/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.30/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.30/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.30/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.30/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.30/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.30/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.30/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.278801 irails-1.3.30/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.363883 irails-1.3.30/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.30/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.30/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.30/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.30/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.30/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.30/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.30/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.30/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.30/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.365878 irails-1.3.30/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.30/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.367873 irails-1.3.30/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.30/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.378843 irails-1.3.30/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.30/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.30/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.30/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.392806 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.30/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.30/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.30/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.30/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.282790 irails-1.3.30/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.395798 irails-1.3.30/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.30/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.30/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.30/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.30/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.397792 irails-1.3.30/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.30/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.30/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.401783 irails-1.3.30/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.287776 irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.407413 irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.413493 irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.30/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.30/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.289772 irails-1.3.30/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.415787 irails-1.3.30/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.30/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     1662 2023-05-25 10:31:13.000000 irails-1.3.30/irails/unit_test.py
--rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.30/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.332618 irails-1.3.30/irails.egg-info/
--rw-rw-rw-   0        0        0     4878 2023-05-26 14:46:16.000000 irails-1.3.30/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3185 2023-05-26 14:46:17.000000 irails-1.3.30/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 14:46:16.000000 irails-1.3.30/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-26 14:46:16.000000 irails-1.3.30/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      367 2023-05-26 14:46:16.000000 irails-1.3.30/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 14:46:16.000000 irails-1.3.30/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 14:46:17.421299 irails-1.3.30/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.30/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.513137 irails-1.3.31/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.31/MANIFEST.in
+-rw-rw-rw-   0        0        0     4878 2023-05-27 08:52:36.512140 irails-1.3.31/PKG-INFO
+-rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.31/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.408269 irails-1.3.31/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-27 08:52:24.000000 irails-1.3.31/irails/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.31/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.31/irails/_loader.py
+-rw-rw-rw-   0        0        0     5595 2023-05-27 08:18:04.000000 irails-1.3.31/irails/_utils.py
+-rw-rw-rw-   0        0        0    14149 2023-05-27 08:28:58.000000 irails-1.3.31/irails/auth.py
+-rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.31/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.417244 irails-1.3.31/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.420236 irails-1.3.31/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0     9284 2023-05-25 05:11:53.000000 irails-1.3.31/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.31/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10591 2023-05-25 05:11:49.000000 irails-1.3.31/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.31/irails/cbv.py
+-rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.31/irails/config.py
+-rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.31/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    25443 2023-05-27 08:49:15.000000 irails-1.3.31/irails/core.py
+-rw-rw-rw-   0        0        0    20988 2023-05-27 08:36:14.000000 irails-1.3.31/irails/database.py
+-rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.31/irails/log.py
+-rw-rw-rw-   0        0        0     8876 2023-05-27 05:49:02.000000 irails-1.3.31/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.31/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.31/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.31/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.434262 irails-1.3.31/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.31/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.31/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.31/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.31/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.31/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.31/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.31/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.31/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.31/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.31/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.31/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.377474 irails-1.3.31/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.448225 irails-1.3.31/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.31/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.31/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.31/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.31/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.31/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.31/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.31/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.31/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.31/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.450543 irails-1.3.31/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.31/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.451543 irails-1.3.31/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.31/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.465505 irails-1.3.31/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.31/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.31/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.31/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.481463 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.31/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.31/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.31/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.31/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.31/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.379469 irails-1.3.31/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.484455 irails-1.3.31/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.31/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.31/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.31/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.31/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.487446 irails-1.3.31/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.31/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.31/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.491438 irails-1.3.31/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.381464 irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.497541 irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.503659 irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.31/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.31/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.382461 irails-1.3.31/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.507649 irails-1.3.31/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.31/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1737 2023-05-27 08:50:04.000000 irails-1.3.31/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.31/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:52:36.415250 irails-1.3.31/irails.egg-info/
+-rw-rw-rw-   0        0        0     4878 2023-05-27 08:52:36.000000 irails-1.3.31/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3185 2023-05-27 08:52:36.000000 irails-1.3.31/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 08:52:36.000000 irails-1.3.31/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-27 08:52:36.000000 irails-1.3.31/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      367 2023-05-27 08:52:36.000000 irails-1.3.31/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-27 08:52:36.000000 irails-1.3.31/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 08:52:36.513137 irails-1.3.31/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.31/setup.py
```

### Comparing `irails-1.3.30/PKG-INFO` & `irails-1.3.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.30
+Version: 1.3.31
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.30/README.md` & `irails-1.3.31/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/_i18n.py` & `irails-1.3.31/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/_loader.py` & `irails-1.3.31/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/_utils.py` & `irails-1.3.31/irails/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -153,8 +153,18 @@
     if not _pluralizer:
         _pluralizer = inflect.engine()
     referred_name = referred_cls.__name__
     uncamelized = re.sub(r'[A-Z]',
                          lambda m: "_%s" % m.group(0).lower(),
                          referred_name)[1:]
     pluralized = _pluralizer.plural(uncamelized)
-    return pluralized
+    return pluralized
+def copy_attr(obj1:object, obj2:object,copy_none:bool=True):
+    """
+        将obj1的属性复制到obj2（如果obj2有相同的属性）。
+    """
+    for key, value in obj1.__dict__.items():
+        if hasattr(obj2, key):
+            if copy_none or value:
+                setattr(obj2, key, value)
+             
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `irails-1.3.30/irails/auth.py` & `irails-1.3.31/irails/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,360 +1,385 @@
 import base64
-import binascii
-import importlib
+
 import os
 
 import casbin
 from casbin.enforcer import Enforcer
- 
-from fastapi import FastAPI,Request,Response
-from starlette.authentication import AuthenticationBackend, AuthenticationError, SimpleUser, AuthCredentials,BaseUser
+
+from fastapi import FastAPI, Request, Response
+from starlette.authentication import AuthenticationBackend, AuthenticationError, SimpleUser, AuthCredentials, BaseUser
 from starlette.middleware.authentication import AuthenticationMiddleware
-from starlette.authentication import BaseUser,SimpleUser,UnauthenticatedUser
+from starlette.authentication import BaseUser, SimpleUser, UnauthenticatedUser
 from casbin.persist.adapters import FileAdapter
 from casbin.persist.adapter import Adapter
 # from .midware_casbin import CasbinMiddleware
- 
-from .config import config,ROOT_PATH
+
+from .config import config, ROOT_PATH
 from .log import _log
 import jwt
 from datetime import datetime, timedelta
-from typing import Optional, Tuple, Type, Union,Dict
-from ._utils import iJSONEncoder,is_datetime_format
+from typing import Optional, Tuple, Type, Union, Dict
+from ._utils import iJSONEncoder, is_datetime_format
 from ._i18n import _
-AUTH_EXPIRED='[EXPIRED]!' 
-_session_name:str = ""
+AUTH_EXPIRED = '[EXPIRED]!'
+_session_name: str = ""
+default_domain = "system"
+
 
 class DomainUser(BaseUser):
-    def __init__(self,username: str='anonymous',group:str="",domain:str="") -> None:
+    def __init__(self, username: str = 'anonymous', group: str = "", domain: str = "") -> None:
         self.username = username
         self._group = group
-        self._domain = domain
+        self._domain = domain or default_domain
         self._lang = "zh"
-        self._timezone =  'Asia/Shanghai'
+        self._timezone = 'Asia/Shanghai'
         super().__init__()
+
     @property
     def group(self):
-        return self._group 
+        return self._group
+
     @group.setter
-    def group(self,value):
+    def group(self, value):
         self._group = value
+
     @property
     def domain(self):
-        return self._domain    
+        return self._domain
+
     @domain.setter
-    def domain(self,value):
-        self._domain=value
+    def domain(self, value):
+        if not value:
+            value = default_domain
+        self._domain = value
+
     @property
     def is_authenticated(self) -> bool:
-        return self.username!='anonymous'
+        return self.username != 'anonymous'
+
     @property
     def display_name(self) -> str:
         return self.username
+
     @property
     def identity(self) -> str:
         identity = self.username
         if self._group:
             group = self._group
             if self._domain:
                 group = self._domain+"."+group
-            identity+='@'+group
+            identity += '@'+group
         return identity
+
     def __repr__(self):
         return self.identity
+
+
 class BasicUser(DomainUser):
-    def __init__(self,username: str,group:str="",domain:str="") -> None: 
-        super().__init__(username,group,domain)
-    
-class JWTUser(DomainUser): 
-    def __init__(self, username: str, token: str, payload: dict,group:str="",domain:str="") -> None: 
+    def __init__(self, username: str, group: str = "", domain: str = "") -> None:
+        super().__init__(username, group, domain)
+
+
+class JWTUser(DomainUser):
+    def __init__(self, username: str, token: str, payload: dict, group: str = "", domain: str = "") -> None:
         self.token = token
         self.payload = payload
-        super().__init__(username,group,domain) 
-     
-    
+        super().__init__(username, group, domain)
+
+
 class CasbinAuth:
-    def __init__(self,enforcer:Enforcer,session_name="user") -> None:
+    def __init__(self, enforcer: Enforcer, session_name="user") -> None:
         global _session_name
         self.enforcer = enforcer
         self.__session_name = _session_name = session_name
         pass
-    def policy(self,*args,**kwargs):
+
+    def policy(self, *args, **kwargs):
         """
         :sub(user_name or mainbody),:obj(resource or url),:act(action like 'GET','POST','DELETE')
         add or remove authorization info by :authorzie
         """
         authorize = True
         if kwargs and 'authorize' in kwargs:
             authorize = kwargs['authorize']
         if self.enforcer:
             if authorize:
-                return self.enforcer.add_policy(*args) 
+                return self.enforcer.add_policy(*args)
             else:
                 return self.enforcer.remove_policy(*args)
         raise RuntimeError("Casbin Enforcer is None")
-    def grouping(self,*args,**kwargs):
+
+    def grouping(self, *args, **kwargs):
         '''grouping(`alice`,`admin`) add `alice` to group `admin` or delete it'''
         authorize = True
         if kwargs and 'authorize' in kwargs:
             authorize = kwargs['authorize']
         if self.enforcer:
             if authorize:
                 return self.enforcer.add_grouping_policy(*args)
-            else: 
+            else:
                 return self.enforcer.remove_grouping_policy(*args)
         raise RuntimeError("Casbin Enforcer is None")
-    def is_grouping(self,*args):
+
+    def is_grouping(self, *args):
         ''' is_grouping('alice','admin')? return `alice` is belongs `admin` '''
         if self.enforcer:
             return self.enforcer.has_grouping_policy(*args)
         raise RuntimeError("Casbin Enforcer is None")
-    def _auth(self,request:Request,user:DomainUser):
+
+    def _auth(self, request: Request, user: DomainUser):
         '''
         do verity,return True means `Success` and others `Failed`
         '''
-         
-        sub = user.identity 
+
+        sub = user.identity
         path = request.url.path
         method = request.method
-        param:Tuple = (sub,user.domain,path,method,)
-          
-          
+        param: Tuple = (sub, user.domain, path, method,)
+
         return self.enforcer.enforce(*param)
-    
+
     def __get_token_from_header(self, authorization: str, prefix: str) -> str:
         """Parses the Authorization header and returns only the token"""
         try:
             scheme, token = authorization.split()
         except ValueError as e:
-            raise AuthenticationError(_('Could not separate Authorization scheme and token')) from e 
+            raise AuthenticationError(
+                _('Could not separate Authorization scheme and token')) from e
         if scheme.lower() != prefix.lower():
-            raise AuthenticationError( _('Authorization scheme %s is not supported') % {scheme})
+            raise AuthenticationError(
+                _('Authorization scheme %s is not supported') % {scheme})
         return token
-    
-    def get_user_from_request(self,request:Request,prefix:str="Bearer",is_jwt:bool=False,**kwargs) : 
+
+    def get_user_from_request(self, request: Request, prefix: str = "Bearer", is_jwt: bool = False, **kwargs):
         userobj = request.session.get(self.__session_name)
         payload = None
         username = ''
-       
-        if is_jwt:   
+
+        if is_jwt:
             username_field = kwargs['username_field']
             auth = request.headers["Authorization"] if 'Authorization' in request.headers else None
             if auth:
-                scheme, credentials = auth.split() 
-                token = self.__get_token_from_header(authorization=auth, prefix=prefix)
-                
+                scheme, credentials = auth.split()
+                token = self.__get_token_from_header(
+                    authorization=auth, prefix=prefix)
+
                 del kwargs['username_field']
                 try:
-                    payload = jwt.decode(token,**kwargs)
+                    payload = jwt.decode(token, **kwargs)
                 except jwt.InvalidTokenError as e:
-                    msg = _('token %s has been expired(%s)'%(token,e.args))
+                    msg = _('token %s has been expired(%s)' % (token, e.args))
                     _log.debug(msg)
                     request.session[self.__session_name] = None
-                    return "","",None
+                    return "", "", None
                 if is_datetime_format(payload['exp']):
                     payload['exp'] = datetime.fromisoformat(payload['exp'])
 
-
-                return  payload[username_field],token,payload
+                return payload[username_field], token, payload
             elif userobj:
                 if 'token' in userobj:
                     try:
-                        payload = jwt.decode(userobj['token'],**kwargs)
-                    except jwt.InvalidTokenError as e:#Signature has expired
+                        payload = jwt.decode(userobj['token'], **kwargs)
+                    except jwt.InvalidTokenError as e:  # Signature has expired
                         request.session[self.__session_name] = None
-                        return AUTH_EXPIRED,AUTH_EXPIRED,None
+                        return AUTH_EXPIRED, AUTH_EXPIRED, None
                         # raise AuthenticationError(str(e)) from e
-                     
-                    return  payload[username_field],userobj['token'],payload
+
+                    return payload[username_field], userobj['token'], payload
         else:
-            if userobj: 
-                return userobj,"",None
+            if userobj:
+                return userobj, "", None
             else:
                 decoded = base64.b64decode(credentials).decode("ascii")
                 username, _, password = decoded.partition(":")
                 if username:
-                    return username,password,None
-        return "","",None
-    
+                    return username, password, None
+        return "", "", None
+
+
 class AuthenticationBackend_(AuthenticationBackend):
     user_class = DomainUser
-    def create_access_token(self,**kwargs):
+
+    def create_access_token(self, **kwargs):
         raise NotImplementedError()
-    def clear_userinfo(self,request:Request):
+
+    def clear_userinfo(self, request: Request):
         raise NotImplementedError()
+
     @property
-    def casbin_auth(self)->CasbinAuth:
+    def casbin_auth(self) -> CasbinAuth:
         return _casbin_auth
-     
 
 
 class BasicAuth(AuthenticationBackend_):
-     
-    def __init__(self,**kwargs) -> None:
-         
+
+    def __init__(self, **kwargs) -> None:
+
         super().__init__()
-     
-    
-    async def authenticate(self, request:Request, **kwargs):
-        userobj,password,_ = _casbin_auth.get_user_from_request(request=request)
+
+    async def authenticate(self, request: Request, **kwargs):
+        userobj, password, _ = _casbin_auth.get_user_from_request(
+            request=request)
         if not userobj:
-            return False,None
-        if isinstance(userobj,BasicUser):
+            return False, None
+        if isinstance(userobj, BasicUser):
             user = userobj
-        elif isinstance(userobj,str): 
+        elif isinstance(userobj, str):
             user = BasicUser(userobj)
         request.scope['user'] = user
-        auth_type:str = kwargs.get("auth_type")
-        if not auth_type or auth_type.lower()=='public': 
+        auth_type: str = kwargs.get("auth_type")
+        if not auth_type or auth_type.lower() == 'public':
             return True,  user
-        result = _casbin_auth._auth(request=request,user=user)
-        
+        result = _casbin_auth._auth(request=request, user=user)
+
         return result, user
 
-         
-    def clear_userinfo(self,request:Request):
+    def clear_userinfo(self, request: Request):
         global _session_name
-        del request.session[_session_name] 
-        
-    def create_access_token(self,  user:DomainUser,**kwargs):
+        del request.session[_session_name]
+
+    def create_access_token(self,  user: DomainUser, **kwargs):
         global _session_name
-        request:Request = kwargs['request'] if 'request' in kwargs else None
+        request: Request = kwargs['request'] if 'request' in kwargs else None
         if request:
             request.session[_session_name] = user
         return None
-        
-
 
 
 class JWTAuthenticationBackend(AuthenticationBackend_):
-     
+
     def __init__(self,
                  secret_key: str,
                  algorithm: str = 'HS256',
                  prefix: str = 'Bearer',
                  username_field: str = 'username',
                  audience: Optional[str] = None,
                  options: Optional[dict] = None) -> None:
         self.secret_key = secret_key
         self.algorithm = algorithm
         self.prefix = prefix
         self.username_field = username_field
         self.audience = audience
         self.options = options or dict()
-        
-     
-    
-    async def authenticate(self, request:Request,**kwargs) -> Union[None, Tuple[AuthCredentials, JWTUser]]:
-        auth_type:str = kwargs.get("auth_type")
-
-        args = {'username_field':self.username_field, 'key':self.secret_key, 'algorithms': self.algorithm , 'audience':self.audience ,
-                                            'options':self.options }
-        user_name,token,payload = _casbin_auth.get_user_from_request(request=request,
-                                                                 prefix=self.prefix, 
-                                                                 is_jwt=True,**args)
-        if token==AUTH_EXPIRED:
+
+    async def authenticate(self, request: Request, **kwargs) -> Union[None, Tuple[AuthCredentials, JWTUser]]:
+        auth_type: str = kwargs.get("auth_type")
+
+        args = {'username_field': self.username_field, 'key': self.secret_key, 'algorithms': self.algorithm, 'audience': self.audience,
+                'options': self.options}
+        user_name, token, payload = _casbin_auth.get_user_from_request(request=request,
+                                                                       prefix=self.prefix,
+                                                                       is_jwt=True, **args)
+        if token == AUTH_EXPIRED:
             self.clear_userinfo(request)
-            return False,AUTH_EXPIRED
-        jwtuser:BasicUser = DomainUser()
-        def from_payload(payload)->JWTUser:
-            return JWTUser(username=payload[self.username_field], 
-                              token=token,
-                              group=payload['group'],
-                              domain=payload['domain'],
-                              payload=payload) 
-        if user_name or token or payload: 
+            return False, AUTH_EXPIRED
+        jwtuser: BasicUser = DomainUser()
+
+        def from_payload(payload) -> JWTUser:
+            return JWTUser(username=payload[self.username_field],
+                           token=token,
+                           group=payload['group'],
+                           domain=payload['domain'],
+                           payload=payload)
+        if user_name or token or payload:
             if payload and token:
-                jwtuser = from_payload(payload) 
+                jwtuser = from_payload(payload)
                 request.scope['user'] = jwtuser
-        
-        if  auth_type.lower()=='public': 
-            return jwtuser.is_authenticated, jwtuser 
-        elif auth_type.lower()=='none':
-            return True,jwtuser
+
+        if auth_type.lower() == 'public':
+            return jwtuser.is_authenticated, jwtuser
+        elif auth_type.lower() == 'none':
+            return True, jwtuser
         elif payload and not jwtuser.is_authenticated:
-            jwtuser = from_payload(payload) 
+            jwtuser = from_payload(payload)
             request.scope['user'] = jwtuser
-        result = _casbin_auth._auth(request=request,user=jwtuser) 
-        return result, jwtuser  
-         
-    def clear_userinfo(self,request:Request):
+        result = _casbin_auth._auth(request=request, user=jwtuser)
+        return result, jwtuser
+
+    def clear_userinfo(self, request: Request):
         global _session_name
         if _session_name in request.session:
-            del request.session[_session_name] 
-    def create_access_token(self,  user:DomainUser , expires_delta: timedelta = None,**kwargs)  :
+            del request.session[_session_name]
+
+    def create_access_token(self,  user: DomainUser, expires_delta: timedelta = None, **kwargs):
         global _session_name
         if expires_delta:
             expire = datetime.utcnow() + expires_delta
         else:
             authCfg = config.get('auth')
             if authCfg:
-                expires_delta = int(authCfg.get('expires_delta',60))
+                expires_delta = int(authCfg.get('expires_delta', 60))
             else:
                 expires_delta = 60
             expire = datetime.utcnow() + timedelta(
                 minutes=expires_delta
             )
-         
-        auth_user_obj = { 
-                          "exp": expire, 
-                          "username": user.username,
-                          "group":user.group,
-                          "domain":user.domain 
-                        }
-         
-        request:Request = kwargs['request']
-        
-        access_token = jwt.encode(auth_user_obj, self.secret_key ,self.algorithm )
-        auth_user_obj.update({"token":access_token})
+
+        auth_user_obj = {
+            "exp": expire,
+            "username": user.username,
+            "group": user.group,
+            "domain": user.domain
+        }
+
+        request: Request = kwargs['request']
+
+        access_token = jwt.encode(
+            auth_user_obj, self.secret_key, self.algorithm)
+        auth_user_obj.update({"token": access_token})
         request.session[_session_name] = auth_user_obj
         return access_token
-    
-_casbin_auth:CasbinAuth = None
 
-def init(app:FastAPI,backend:AuthenticationBackend,adapter_class:Type=None,**kwagrs)->AuthenticationBackend:
+
+_casbin_auth: CasbinAuth = None
+
+
+def init(app: FastAPI, backend: AuthenticationBackend, adapter_class: Type = None, **kwagrs) -> AuthenticationBackend:
     """
         kwargs:secret_key=KEY
     """
-    __session_name = config.get("auth").get("session_name",'user')
+    __session_name = config.get("auth").get("session_name", 'user')
     global _casbin_auth
     cfg = config.get("auth")
-    adapter_uri = kwagrs.get('adapter_uri',None)
-    
+    adapter_uri = kwagrs.get('adapter_uri', None)
+
     del kwagrs['adapter_uri']
-    model_file = cfg.get("auth_model",'./configs/casbin-model.conf') 
-    model_file = os.path.abspath(os.path.join(ROOT_PATH,model_file))   
+    model_file = cfg.get("auth_model", './configs/casbin-model.conf')
+    model_file = os.path.abspath(os.path.join(ROOT_PATH, model_file))
     if adapter_class is FileAdapter and not os.path.isabs(adapter_uri):
         adapter_uri = os.path.abspath(os.path.join(ROOT_PATH, adapter_uri))
     adapter = adapter_class(adapter_uri)
     enforcer = casbin.Enforcer(model_file, adapter)
-   
-    _casbin_auth = CasbinAuth(enforcer=enforcer,session_name=__session_name)
-    
-    return backend(**kwagrs) 
-def reload_adapter(app:FastAPI,adapter:Adapter=None):
+
+    _casbin_auth = CasbinAuth(enforcer=enforcer, session_name=__session_name)
+
+    return backend(**kwagrs)
+
+
+def reload_adapter(app: FastAPI, adapter: Adapter = None):
     cfg = config.get("auth")
-    model_file = cfg.get("auth_model",'./configs/casbin-model.conf')    
+    model_file = cfg.get("auth_model", './configs/casbin-model.conf')
     if not adapter:
-        adapter_file = cfg.get("auth_adapter",'./configs/casbin-adapter.csv')    
-        adapter = FileAdapter(adapter_file)   
-    enforcer = casbin.Enforcer(model_file, adapter) 
+        adapter_file = cfg.get("auth_adapter", './configs/casbin-adapter.csv')
+        adapter = FileAdapter(adapter_file)
+    enforcer = casbin.Enforcer(model_file, adapter)
     app.router.current_casbin_instance = enforcer
 
-def get_auth_backend(name:str)->AuthenticationBackend_: 
-    _auth_types = {'basic':BasicAuth,'jwt':JWTAuthenticationBackend}
-    return _auth_types[name] if name in  _auth_types else None
 
-def get_adapter_module(name:str)->Adapter:
+def get_auth_backend(name: str) -> AuthenticationBackend_:
+    _auth_types = {'basic': BasicAuth, 'jwt': JWTAuthenticationBackend}
+    return _auth_types[name] if name in _auth_types else None
+
+
+def get_adapter_module(name: str) -> Adapter:
     from ._loader import load_module
-    if name.lower()=='file':
+    if name.lower() == 'file':
         return FileAdapter
-    module_name= f"{name}_adapter"
+    module_name = f"{name}_adapter"
     module_dir = os.path.dirname(__file__)
-    module_dir = os.path.join(module_dir,'casbin_adapters')
-    module_path = os.path.join(module_dir, module_name + '.py') 
-    module = load_module(module_name,module_path)
-    if module and hasattr(module,'Adapter'):
-        return getattr(module,'Adapter')   
+    module_dir = os.path.join(module_dir, 'casbin_adapters')
+    module_path = os.path.join(module_dir, module_name + '.py')
+    module = load_module(module_name, module_path)
+    if module and hasattr(module, 'Adapter'):
+        return getattr(module, 'Adapter')
     else:
         raise RuntimeError(_("Can't load module:%s") % module_path)
-
```

### Comparing `irails-1.3.30/irails/base_controller.py` & `irails-1.3.31/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc` & `irails-1.3.31/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.31/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.31/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/cbv.py` & `irails-1.3.31/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/config.py` & `irails-1.3.31/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/controller_utils.py` & `irails-1.3.31/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/core.py` & `irails-1.3.31/irails/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .log import _log,set_logger
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import RedirectResponse,JSONResponse,ORJSONResponse
 from . import midware
 from . import auth
 from . import database
 from ._loader import _load_apps
-from ._utils import get_controller_name,get_snaked_name
+from ._utils import get_controller_name,get_snaked_name,copy_attr
 
 from ._i18n import _
 
 
 __is_debug=config.get('debug',False)
 
 def singleton(cls):
@@ -44,20 +44,26 @@
         self.__casbin_auth:auth.AuthenticationBackend_ = None 
         self._data_engine:database.Engine = None
         self.__user_auth_url=""
         self.__public_auth_url=""
         self.__app_views_dirs = {} 
         self.routers_map = {}
         self.__apps_dirs = []
-        self.auth_class = None
+        self.auth_user_class:auth.DomainUser = None
         super().__init__(**kwargs)
-    def new_user(self,username:str)->auth.DomainUser:
-        if not self.auth_class:
+
+    def new_user(self,user:Union[database.Base,str])->auth.DomainUser:
+        if not self.auth_user_class:
             raise RuntimeError('application.auth_class is None')
-        return self.auth_class(username=username)
+        if isinstance(user,str):
+            return self.auth_user_class(username=user)
+        elif isinstance(user,database.Base):
+            userobj = self.auth_user_class(user.name)
+            copy_attr(user,userobj,False)
+            return userobj
      
     @property
     def app_views_dirs(self)->Dict:
         return self.__app_views_dirs
     @app_views_dirs.setter
     def app_views_dirs(self,key,value):
         self.__app_views_dirs[key]=value
@@ -165,15 +171,15 @@
 
 def __init_auth(app,auth_type:str,casbin_adapter_class,__adapter_uri):
     
     
     auth_class = auth.get_auth_backend(auth_type)
     if not auth_class:
         raise RuntimeError(_("%s auth type not support") % auth_type)
-    application.auth_class = auth_class.user_class
+    application.auth_user_class = auth_class.user_class
     
     secret_key = config.get("auth").get(f"secret_key","")
     kwargs = {'secret_key':secret_key,'adapter_uri':__adapter_uri} 
     return auth.init(app=app, backend = auth_class,adapter_class=casbin_adapter_class, **kwargs)
 
 
 def api_router(path:str="", version:str="",**allargs):  
@@ -378,27 +384,46 @@
             application.routers_map[funcname] = {'path':r.path,'methods':methods,'doc':doc_map,'auth':auth_type,"endpoint":r.endpoint}
       
     _log.info(_("static files mouting..."))
     midware.init(app=application,debug=__is_debug)
 
 def check_db_migrate():
     db_cfg = config.get("database")
-    if __is_debug and db_cfg:
+    if not db_cfg:return
+    if __is_debug :
         _log.info(_("checking database migrations...."))
     try:
             
         alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
         uri = db_cfg.get("uri")
         if uri:
             database.check_migration(application.data_engine,uri,alembic_ini)
     except database.InitDbError as e:
         raise
     except Exception as e:
         _log.disabled = False
         _log.error(e.args)
+def check_init_auth(db_cfg):
+    # Initializing the authentication system
+    auth_type = config.get("auth", None)
+    _casbin_adapter_class = None
+    _adapter_uri: str = None
+    if auth_type:
+        auth_type = auth_type.get("type")
+        if auth_type:
+            # Get the adapter type from the configuration
+            __type_casbin_adapter = config.get("auth").get("casbin_adapter", "file")
+            _casbin_adapter_class = auth.get_adapter_module(__type_casbin_adapter)
+            _adapter_uri = config.get("auth").get("adapter_uri")
+            if not _adapter_uri:
+                _adapter_uri = db_cfg.get('uri')
+            # Raise an error if the adapter is not supported
+            if not _casbin_adapter_class:
+                raise RuntimeError(_("Not support %s ,Adapter config error in auth.casbin_adapter") % __type_casbin_adapter)
+    return auth_type,_adapter_uri,_casbin_adapter_class
 def generate_mvc_app():
     global __is_debug
      
     application.title = _project_name
     
     
     
@@ -411,30 +436,15 @@
     
     _register_controllers()
 
     
     _log.info(_("checking database configure..."))
     db_cfg = check_init_database()
 
-    # Initializing the authentication system
-    auth_type = config.get("auth", None)
-    _casbin_adapter_class = None
-    _adapter_uri: str = None
-    if auth_type:
-        auth_type = auth_type.get("type")
-        if auth_type:
-            # Get the adapter type from the configuration
-            __type_casbin_adapter = config.get("auth").get("casbin_adapter", "file")
-            _casbin_adapter_class = auth.get_adapter_module(__type_casbin_adapter)
-            _adapter_uri = config.get("auth").get("adapter_uri")
-            if not _adapter_uri:
-                _adapter_uri = db_cfg.get('uri')
-            # Raise an error if the adapter is not supported
-            if not _casbin_adapter_class:
-                raise RuntimeError(_("Not support %s ,Adapter config error in auth.casbin_adapter") % __type_casbin_adapter)
+    auth_type,_adapter_uri,_casbin_adapter_class=check_init_auth(db_cfg)
     if __is_debug:
         # Check for database migrations
         check_db_migrate()
     # Initialize the authentication system if the adapter class and URI are present
     from .log import set_logger
     set_logger(_log,check_level=True)
     _log.info(_("init casbin auth system..."))
```

### Comparing `irails-1.3.30/irails/database.py` & `irails-1.3.31/irails/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,14 +350,31 @@
             else:
                 for row in rows:
                     session.delete(row)
             cnt = len(rows)
             session.commit()
             return cnt
     @classmethod
+    def restore(self,model:Union[Type,Base],*args,**kwargs):
+        '''Undelete . set is_deleted field False '''
+        with self.get_session() as session:
+            if isinstance(model,Base):
+                if hasattr(model,is_deleted_field): 
+                    setattr(model,is_deleted_field,False)
+                    return model
+            else: 
+                query = session.query(model).filter(*args).filter_by(**kwargs)
+                rows = query.all()
+                if hasattr(model,is_deleted_field): 
+                    for row in rows:
+                        setattr(row,is_deleted_field,False)   
+                cnt = len(rows)
+                 
+                return cnt
+    @classmethod
     def real_delete(self,model:Base,*args,**kwargs):
         '''Real delete rows in database'''
         with self.get_session() as session: 
             query = session.query(model).filter(*args).filter_by(**kwargs)
             cnt = 0
             for obj in query:
                 session.delete(obj)
```

### Comparing `irails-1.3.30/irails/log.py` & `irails-1.3.31/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/midware.py` & `irails-1.3.31/irails/midware.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,22 +79,25 @@
         static_paths = app.app_views_dirs
     for _dir  in  static_paths: 
         
         _url:str = static_paths[_dir] 
         if not _url.startswith('/'):
             _url='/'+_url
         _dir = os.path.normpath(_dir)
-        if _url=='/':
-            __roots[_dir] = _url
+        if os.path.exists(_dir):
+            if _url=='/':
+                __roots[_dir] = _url
+            else:
+                if not _url.endswith("/"):_url+="/"
+                _url = _url.lower()
+                if debug:
+                    _log.info(f"StaticDir:{_dir} mounted: {_url}")
+                app.mount(_url,MvcStaticFiles(directory=_dir),name=_dir)       
         else:
-            if not _url.endswith("/"):_url+="/"
-            _url = _url.lower()
-            if debug:
-                _log.info(f"StaticDir:{_dir} mounted: {_url}")
-            app.mount(_url,MvcStaticFiles(directory=_dir),name=_dir)       
+            _log.warn(f"StaticDir:{_dir} do not exists!")
     #mount public resources
     public_dir =  config.get("public_dir") 
     public_dir = os.path.abspath(os.path.join(ROOT_PATH,public_dir))
     if not os.path.exists(public_dir):
         os.makedirs(public_dir) 
     app.mount('/public/',  MvcStaticFiles(directory=public_dir), name='public')
```

### Comparing `irails-1.3.30/irails/midware_casbin.py` & `irails-1.3.31/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/midware_session.py` & `irails-1.3.31/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/mvc_router.py` & `irails-1.3.31/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/_app.py` & `irails-1.3.31/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/_controller.py` & `irails-1.3.31/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/_i18n.py` & `irails-1.3.31/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/_migrate.py` & `irails-1.3.31/irails/scripts/_migrate.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/_model.py` & `irails-1.3.31/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/_project.py` & `irails-1.3.31/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/_run.py` & `irails-1.3.31/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/_shell.py` & `irails-1.3.31/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/_test.py` & `irails-1.3.31/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/main.py` & `irails-1.3.31/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.31/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/app/home.tpl` & `irails-1.3.31/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/app/model.jinja` & `irails-1.3.31/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.31/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.31/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.31/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.31/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.31/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.31/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.31/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.31/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.31/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.31/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.31/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails/unit_test.py` & `irails-1.3.31/irails/unit_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 class ServiceTest(_BaseUnitTest):
     def __init__(self,*args,**kwargv) -> None:
         super().__init__(*args,**kwargv)
         from .config import config
         from ._loader import _load_apps
         from irails.database import Service,engine,Session,init_database
         from irails.database import check_migration
-         
+        from irails.core import check_init_auth
         # _load_apps()
         if not hasattr(ServiceTest,'engine'):
             db_cfg = config.get("database")
             db_uri = db_cfg.get("uri")
             alembic_ini = db_cfg.get("alembic_ini")
             ServiceTest.engine = init_database(db_uri,debug=True,cfg = db_cfg)
+            check_init_auth(db_cfg)
             if ServiceTest.engine:
                 check_migration(engine=ServiceTest.engine,uri= db_uri,alembic_ini= alembic_ini )
             ServiceTest.service = Service
```

### Comparing `irails-1.3.30/irails/view.py` & `irails-1.3.31/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/irails.egg-info/PKG-INFO` & `irails-1.3.31/irails.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.30
+Version: 1.3.31
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.30/irails.egg-info/SOURCES.txt` & `irails-1.3.31/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.30/setup.py` & `irails-1.3.31/setup.py`

 * *Files identical despite different names*

