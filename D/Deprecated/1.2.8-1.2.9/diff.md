# Comparing `tmp/Deprecated-1.2.8.tar.gz` & `tmp/Deprecated-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Deprecated-1.2.8.tar", last modified: Sun Apr  5 20:42:15 2020, max compression
+gzip compressed data, was "dist/Deprecated-1.2.9.tar", last modified: Fri Apr 10 08:30:26 2020, max compression
```

## Comparing `Deprecated-1.2.8.tar` & `Deprecated-1.2.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/
--rw-r--r--   0 tantale    (505) staff       (20)      574 2019-11-11 15:07:20.000000 Deprecated-1.2.8/.bumpversion.cfg
--rw-r--r--   0 tantale    (505) staff       (20)      215 2019-10-02 18:18:27.000000 Deprecated-1.2.8/.editorconfig
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/.github/
--rw-r--r--   0 tantale    (505) staff       (20)     3284 2019-10-02 18:18:27.000000 Deprecated-1.2.8/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 tantale    (505) staff       (20)      837 2019-10-02 18:18:27.000000 Deprecated-1.2.8/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 tantale    (505) staff       (20)      512 2019-10-02 18:18:27.000000 Deprecated-1.2.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 tantale    (505) staff       (20)      586 2019-10-02 18:18:27.000000 Deprecated-1.2.8/.packit.yaml
--rw-r--r--   0 tantale    (505) staff       (20)      321 2019-11-11 13:45:11.000000 Deprecated-1.2.8/.travis.yml
--rw-r--r--   0 tantale    (505) staff       (20)     8931 2020-04-05 20:41:59.000000 Deprecated-1.2.8/CHANGELOG.rst
--rw-r--r--   0 tantale    (505) staff       (20)     5321 2019-10-02 18:18:27.000000 Deprecated-1.2.8/CONTRIBUTING.rst
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/Deprecated.egg-info/
--rw-r--r--   0 tantale    (505) staff       (20)     5909 2020-04-05 20:42:15.000000 Deprecated-1.2.8/Deprecated.egg-info/PKG-INFO
--rw-r--r--   0 tantale    (505) staff       (20)     1864 2020-04-05 20:42:15.000000 Deprecated-1.2.8/Deprecated.egg-info/SOURCES.txt
--rw-r--r--   0 tantale    (505) staff       (20)        1 2020-04-05 20:42:15.000000 Deprecated-1.2.8/Deprecated.egg-info/dependency_links.txt
--rw-r--r--   0 tantale    (505) staff       (20)        1 2019-10-02 19:38:33.000000 Deprecated-1.2.8/Deprecated.egg-info/not-zip-safe
--rw-r--r--   0 tantale    (505) staff       (20)      150 2020-04-05 20:42:15.000000 Deprecated-1.2.8/Deprecated.egg-info/requires.txt
--rw-r--r--   0 tantale    (505) staff       (20)       11 2020-04-05 20:42:15.000000 Deprecated-1.2.8/Deprecated.egg-info/top_level.txt
--rw-r--r--   0 tantale    (505) staff       (20)     1081 2019-10-02 18:18:27.000000 Deprecated-1.2.8/LICENSE.rst
--rw-r--r--   0 tantale    (505) staff       (20)      275 2020-04-05 20:41:59.000000 Deprecated-1.2.8/MANIFEST.in
--rw-r--r--   0 tantale    (505) staff       (20)      781 2019-10-02 18:18:27.000000 Deprecated-1.2.8/Makefile
--rw-r--r--   0 tantale    (505) staff       (20)     5909 2020-04-05 20:42:15.000000 Deprecated-1.2.8/PKG-INFO
--rw-r--r--   0 tantale    (505) staff       (20)     2144 2020-04-05 20:17:11.000000 Deprecated-1.2.8/README.md
--rw-r--r--   0 tantale    (505) staff       (20)     1433 2019-10-02 18:18:27.000000 Deprecated-1.2.8/appveyor.yml
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/deprecated/
--rw-r--r--   0 tantale    (505) staff       (20)      312 2019-11-11 15:07:20.000000 Deprecated-1.2.8/deprecated/__init__.py
--rw-r--r--   0 tantale    (505) staff       (20)     9445 2020-03-29 16:31:45.000000 Deprecated-1.2.8/deprecated/classic.py
--rw-r--r--   0 tantale    (505) staff       (20)     7286 2020-02-23 06:15:14.000000 Deprecated-1.2.8/deprecated/sphinx.py
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/docs/
--rw-r--r--   0 tantale    (505) staff       (20)      507 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/blurb.rst
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/docs/cover/
--rw-r--r--   0 tantale    (505) staff       (20)  2314143 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/cover/paper_10.jpeg
--rw-r--r--   0 tantale    (505) staff       (20)  2387620 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/cover/title-page.odg
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/docs/source/
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/docs/source/_static/
--rw-r--r--   0 tantale    (505) staff       (20)   281884 2020-02-22 18:05:50.000000 Deprecated-1.2.8/docs/source/_static/banner.png
--rw-r--r--   0 tantale    (505) staff       (20)    42764 2020-02-22 18:05:50.000000 Deprecated-1.2.8/docs/source/_static/logo-full.png
--rw-r--r--   0 tantale    (505) staff       (20)   314739 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/_static/title-page.jpg
--rw-r--r--   0 tantale    (505) staff       (20)      241 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/api.rst
--rw-r--r--   0 tantale    (505) staff       (20)       33 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/changelog.rst
--rw-r--r--   0 tantale    (505) staff       (20)     6736 2020-02-22 18:06:42.000000 Deprecated-1.2.8/docs/source/conf.py
--rw-r--r--   0 tantale    (505) staff       (20)       36 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/contributing.rst
--rw-r--r--   0 tantale    (505) staff       (20)     1125 2020-04-05 20:24:53.000000 Deprecated-1.2.8/docs/source/index.rst
--rw-r--r--   0 tantale    (505) staff       (20)     4555 2020-02-10 12:24:37.000000 Deprecated-1.2.8/docs/source/installation.rst
--rw-r--r--   0 tantale    (505) staff       (20)     3487 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/introduction.rst
--rw-r--r--   0 tantale    (505) staff       (20)       48 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/license.rst
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/docs/source/sphinx/
--rw-r--r--   0 tantale    (505) staff       (20)      336 2020-04-05 20:17:11.000000 Deprecated-1.2.8/docs/source/sphinx/calc_mean.py
--rw-r--r--   0 tantale    (505) staff       (20)      399 2020-04-05 20:17:11.000000 Deprecated-1.2.8/docs/source/sphinx/calc_mean_deco.py
--rw-r--r--   0 tantale    (505) staff       (20)      816 2020-04-05 20:17:11.000000 Deprecated-1.2.8/docs/source/sphinx/sphinx_demo.py
--rw-r--r--   0 tantale    (505) staff       (20)       53 2020-04-05 20:17:11.000000 Deprecated-1.2.8/docs/source/sphinx/use_calc_mean_deco.py
--rw-r--r--   0 tantale    (505) staff       (20)     5897 2020-04-05 20:31:25.000000 Deprecated-1.2.8/docs/source/sphinx_deco.rst
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/docs/source/tutorial/
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/docs/source/tutorial/v0/
--rw-r--r--   0 tantale    (505) staff       (20)      188 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/tutorial/v0/liberty.py
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/docs/source/tutorial/v1/
--rw-r--r--   0 tantale    (505) staff       (20)      515 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/tutorial/v1/liberty.py
--rw-r--r--   0 tantale    (505) staff       (20)      128 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/tutorial/v1/using_liberty.py
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/docs/source/tutorial/v2/
--rw-r--r--   0 tantale    (505) staff       (20)      570 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/tutorial/v2/liberty.py
--rw-r--r--   0 tantale    (505) staff       (20)      128 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/tutorial/v2/using_liberty.py
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/docs/source/tutorial/v3/
--rw-r--r--   0 tantale    (505) staff       (20)      618 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/tutorial/v3/liberty.py
--rw-r--r--   0 tantale    (505) staff       (20)      121 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/tutorial/v3/using_liberty.py
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/docs/source/tutorial/v4/
--rw-r--r--   0 tantale    (505) staff       (20)      316 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/tutorial/v4/liberty.py
--rw-r--r--   0 tantale    (505) staff       (20)      104 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/tutorial/v4/using_liberty.py
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/docs/source/tutorial/warning_ctrl/
--rw-r--r--   0 tantale    (505) staff       (20)      208 2020-02-22 17:04:29.000000 Deprecated-1.2.8/docs/source/tutorial/warning_ctrl/filter_action_demo.py
--rw-r--r--   0 tantale    (505) staff       (20)      243 2020-02-22 17:04:29.000000 Deprecated-1.2.8/docs/source/tutorial/warning_ctrl/filter_warnings_demo.py
--rw-r--r--   0 tantale    (505) staff       (20)      593 2020-02-22 17:04:29.000000 Deprecated-1.2.8/docs/source/tutorial/warning_ctrl/warning_classes_demo.py
--rw-r--r--   0 tantale    (505) staff       (20)     9511 2020-04-05 20:17:11.000000 Deprecated-1.2.8/docs/source/tutorial.rst
--rw-r--r--   0 tantale    (505) staff       (20)    15416 2019-10-02 18:18:27.000000 Deprecated-1.2.8/docs/source/white_paper.rst
--rw-r--r--   0 tantale    (505) staff       (20)      150 2020-02-23 17:51:31.000000 Deprecated-1.2.8/pyproject.toml
--rw-r--r--   0 tantale    (505) staff       (20)     1266 2019-11-11 15:07:20.000000 Deprecated-1.2.8/python-deprecated.spec
--rw-r--r--   0 tantale    (505) staff       (20)      269 2020-04-05 20:42:15.000000 Deprecated-1.2.8/setup.cfg
--rwxr-xr-x   0 tantale    (505) staff       (20)     5475 2019-11-11 15:07:20.000000 Deprecated-1.2.8/setup.py
-drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-05 20:42:15.000000 Deprecated-1.2.8/tests/
--rw-r--r--   0 tantale    (505) staff       (20)        0 2019-10-02 18:18:27.000000 Deprecated-1.2.8/tests/__init__.py
--rw-r--r--   0 tantale    (505) staff       (20)      873 2019-10-02 18:18:27.000000 Deprecated-1.2.8/tests/test.py
--rw-r--r--   0 tantale    (505) staff       (20)     6635 2020-02-22 17:04:29.000000 Deprecated-1.2.8/tests/test_deprecated.py
--rw-r--r--   0 tantale    (505) staff       (20)     4024 2019-10-27 15:35:16.000000 Deprecated-1.2.8/tests/test_deprecated_class.py
--rw-r--r--   0 tantale    (505) staff       (20)     2968 2019-10-27 15:10:11.000000 Deprecated-1.2.8/tests/test_deprecated_metaclass.py
--rw-r--r--   0 tantale    (505) staff       (20)    10109 2019-10-27 15:13:42.000000 Deprecated-1.2.8/tests/test_sphinx.py
--rw-r--r--   0 tantale    (505) staff       (20)     2220 2019-10-27 15:35:43.000000 Deprecated-1.2.8/tests/test_sphinx_class.py
--rw-r--r--   0 tantale    (505) staff       (20)     2967 2019-10-27 15:10:11.000000 Deprecated-1.2.8/tests/test_sphinx_metaclass.py
--rw-r--r--   0 tantale    (505) staff       (20)     1003 2020-02-22 17:04:29.000000 Deprecated-1.2.8/tox.ini
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/
+-rw-r--r--   0 tantale    (505) staff       (20)      573 2020-04-05 20:45:36.000000 Deprecated-1.2.9/.bumpversion.cfg
+-rw-r--r--   0 tantale    (505) staff       (20)      247 2020-04-10 07:54:34.000000 Deprecated-1.2.9/.editorconfig
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/.github/
+-rw-r--r--   0 tantale    (505) staff       (20)     3284 2019-10-02 18:18:27.000000 Deprecated-1.2.9/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 tantale    (505) staff       (20)      837 2019-10-02 18:18:27.000000 Deprecated-1.2.9/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 tantale    (505) staff       (20)      512 2019-10-02 18:18:27.000000 Deprecated-1.2.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 tantale    (505) staff       (20)      747 2020-04-10 07:54:34.000000 Deprecated-1.2.9/.packit.yml
+-rw-r--r--   0 tantale    (505) staff       (20)      321 2019-11-11 13:45:11.000000 Deprecated-1.2.9/.travis.yml
+-rw-r--r--   0 tantale    (505) staff       (20)     9268 2020-04-10 07:54:34.000000 Deprecated-1.2.9/CHANGELOG.rst
+-rw-r--r--   0 tantale    (505) staff       (20)     5321 2019-10-02 18:18:27.000000 Deprecated-1.2.9/CONTRIBUTING.rst
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/Deprecated.egg-info/
+-rw-r--r--   0 tantale    (505) staff       (20)     5946 2020-04-10 08:30:26.000000 Deprecated-1.2.9/Deprecated.egg-info/PKG-INFO
+-rw-r--r--   0 tantale    (505) staff       (20)     1863 2020-04-10 08:30:26.000000 Deprecated-1.2.9/Deprecated.egg-info/SOURCES.txt
+-rw-r--r--   0 tantale    (505) staff       (20)        1 2020-04-10 08:30:26.000000 Deprecated-1.2.9/Deprecated.egg-info/dependency_links.txt
+-rw-r--r--   0 tantale    (505) staff       (20)        1 2019-10-02 19:38:33.000000 Deprecated-1.2.9/Deprecated.egg-info/not-zip-safe
+-rw-r--r--   0 tantale    (505) staff       (20)      150 2020-04-10 08:30:26.000000 Deprecated-1.2.9/Deprecated.egg-info/requires.txt
+-rw-r--r--   0 tantale    (505) staff       (20)       11 2020-04-10 08:30:26.000000 Deprecated-1.2.9/Deprecated.egg-info/top_level.txt
+-rw-r--r--   0 tantale    (505) staff       (20)     1081 2019-10-02 18:18:27.000000 Deprecated-1.2.9/LICENSE.rst
+-rw-r--r--   0 tantale    (505) staff       (20)      275 2020-04-05 20:41:59.000000 Deprecated-1.2.9/MANIFEST.in
+-rw-r--r--   0 tantale    (505) staff       (20)      781 2019-10-02 18:18:27.000000 Deprecated-1.2.9/Makefile
+-rw-r--r--   0 tantale    (505) staff       (20)     5946 2020-04-10 08:30:26.000000 Deprecated-1.2.9/PKG-INFO
+-rw-r--r--   0 tantale    (505) staff       (20)     2144 2020-04-05 20:17:11.000000 Deprecated-1.2.9/README.md
+-rw-r--r--   0 tantale    (505) staff       (20)     1433 2019-10-02 18:18:27.000000 Deprecated-1.2.9/appveyor.yml
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/deprecated/
+-rw-r--r--   0 tantale    (505) staff       (20)      312 2020-04-05 20:45:36.000000 Deprecated-1.2.9/deprecated/__init__.py
+-rw-r--r--   0 tantale    (505) staff       (20)     9644 2020-04-10 07:53:49.000000 Deprecated-1.2.9/deprecated/classic.py
+-rw-r--r--   0 tantale    (505) staff       (20)     7286 2020-02-23 06:15:14.000000 Deprecated-1.2.9/deprecated/sphinx.py
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/docs/
+-rw-r--r--   0 tantale    (505) staff       (20)      507 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/blurb.rst
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/docs/cover/
+-rw-r--r--   0 tantale    (505) staff       (20)  2314143 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/cover/paper_10.jpeg
+-rw-r--r--   0 tantale    (505) staff       (20)  2387620 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/cover/title-page.odg
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/docs/source/
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/docs/source/_static/
+-rw-r--r--   0 tantale    (505) staff       (20)   281884 2020-02-22 18:05:50.000000 Deprecated-1.2.9/docs/source/_static/banner.png
+-rw-r--r--   0 tantale    (505) staff       (20)    42764 2020-02-22 18:05:50.000000 Deprecated-1.2.9/docs/source/_static/logo-full.png
+-rw-r--r--   0 tantale    (505) staff       (20)   314739 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/_static/title-page.jpg
+-rw-r--r--   0 tantale    (505) staff       (20)      241 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/api.rst
+-rw-r--r--   0 tantale    (505) staff       (20)       33 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/changelog.rst
+-rw-r--r--   0 tantale    (505) staff       (20)     6736 2020-04-05 20:45:36.000000 Deprecated-1.2.9/docs/source/conf.py
+-rw-r--r--   0 tantale    (505) staff       (20)       36 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/contributing.rst
+-rw-r--r--   0 tantale    (505) staff       (20)     1125 2020-04-05 20:24:53.000000 Deprecated-1.2.9/docs/source/index.rst
+-rw-r--r--   0 tantale    (505) staff       (20)     4555 2020-02-10 12:24:37.000000 Deprecated-1.2.9/docs/source/installation.rst
+-rw-r--r--   0 tantale    (505) staff       (20)     3487 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/introduction.rst
+-rw-r--r--   0 tantale    (505) staff       (20)       48 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/license.rst
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/docs/source/sphinx/
+-rw-r--r--   0 tantale    (505) staff       (20)      336 2020-04-05 20:17:11.000000 Deprecated-1.2.9/docs/source/sphinx/calc_mean.py
+-rw-r--r--   0 tantale    (505) staff       (20)      399 2020-04-05 20:17:11.000000 Deprecated-1.2.9/docs/source/sphinx/calc_mean_deco.py
+-rw-r--r--   0 tantale    (505) staff       (20)      816 2020-04-05 20:17:11.000000 Deprecated-1.2.9/docs/source/sphinx/sphinx_demo.py
+-rw-r--r--   0 tantale    (505) staff       (20)       53 2020-04-05 20:17:11.000000 Deprecated-1.2.9/docs/source/sphinx/use_calc_mean_deco.py
+-rw-r--r--   0 tantale    (505) staff       (20)     5897 2020-04-05 20:31:25.000000 Deprecated-1.2.9/docs/source/sphinx_deco.rst
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/docs/source/tutorial/
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/docs/source/tutorial/v0/
+-rw-r--r--   0 tantale    (505) staff       (20)      188 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/tutorial/v0/liberty.py
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/docs/source/tutorial/v1/
+-rw-r--r--   0 tantale    (505) staff       (20)      515 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/tutorial/v1/liberty.py
+-rw-r--r--   0 tantale    (505) staff       (20)      128 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/tutorial/v1/using_liberty.py
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/docs/source/tutorial/v2/
+-rw-r--r--   0 tantale    (505) staff       (20)      570 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/tutorial/v2/liberty.py
+-rw-r--r--   0 tantale    (505) staff       (20)      128 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/tutorial/v2/using_liberty.py
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/docs/source/tutorial/v3/
+-rw-r--r--   0 tantale    (505) staff       (20)      618 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/tutorial/v3/liberty.py
+-rw-r--r--   0 tantale    (505) staff       (20)      121 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/tutorial/v3/using_liberty.py
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/docs/source/tutorial/v4/
+-rw-r--r--   0 tantale    (505) staff       (20)      316 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/tutorial/v4/liberty.py
+-rw-r--r--   0 tantale    (505) staff       (20)      104 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/tutorial/v4/using_liberty.py
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/docs/source/tutorial/warning_ctrl/
+-rw-r--r--   0 tantale    (505) staff       (20)      208 2020-02-22 17:04:29.000000 Deprecated-1.2.9/docs/source/tutorial/warning_ctrl/filter_action_demo.py
+-rw-r--r--   0 tantale    (505) staff       (20)      243 2020-02-22 17:04:29.000000 Deprecated-1.2.9/docs/source/tutorial/warning_ctrl/filter_warnings_demo.py
+-rw-r--r--   0 tantale    (505) staff       (20)      593 2020-02-22 17:04:29.000000 Deprecated-1.2.9/docs/source/tutorial/warning_ctrl/warning_classes_demo.py
+-rw-r--r--   0 tantale    (505) staff       (20)     9511 2020-04-05 20:17:11.000000 Deprecated-1.2.9/docs/source/tutorial.rst
+-rw-r--r--   0 tantale    (505) staff       (20)    15416 2019-10-02 18:18:27.000000 Deprecated-1.2.9/docs/source/white_paper.rst
+-rw-r--r--   0 tantale    (505) staff       (20)      150 2020-02-23 17:51:31.000000 Deprecated-1.2.9/pyproject.toml
+-rw-r--r--   0 tantale    (505) staff       (20)     1266 2020-04-05 20:57:56.000000 Deprecated-1.2.9/python-deprecated.spec
+-rw-r--r--   0 tantale    (505) staff       (20)      269 2020-04-10 08:30:26.000000 Deprecated-1.2.9/setup.cfg
+-rwxr-xr-x   0 tantale    (505) staff       (20)     5523 2020-04-10 08:30:23.000000 Deprecated-1.2.9/setup.py
+drwxr-xr-x   0 tantale    (505) staff       (20)        0 2020-04-10 08:30:26.000000 Deprecated-1.2.9/tests/
+-rw-r--r--   0 tantale    (505) staff       (20)        0 2019-10-02 18:18:27.000000 Deprecated-1.2.9/tests/__init__.py
+-rw-r--r--   0 tantale    (505) staff       (20)      873 2019-10-02 18:18:27.000000 Deprecated-1.2.9/tests/test.py
+-rw-r--r--   0 tantale    (505) staff       (20)     6635 2020-02-22 17:04:29.000000 Deprecated-1.2.9/tests/test_deprecated.py
+-rw-r--r--   0 tantale    (505) staff       (20)     4024 2019-10-27 15:35:16.000000 Deprecated-1.2.9/tests/test_deprecated_class.py
+-rw-r--r--   0 tantale    (505) staff       (20)     2968 2019-10-27 15:10:11.000000 Deprecated-1.2.9/tests/test_deprecated_metaclass.py
+-rw-r--r--   0 tantale    (505) staff       (20)    10109 2019-10-27 15:13:42.000000 Deprecated-1.2.9/tests/test_sphinx.py
+-rw-r--r--   0 tantale    (505) staff       (20)     2220 2019-10-27 15:35:43.000000 Deprecated-1.2.9/tests/test_sphinx_class.py
+-rw-r--r--   0 tantale    (505) staff       (20)     2967 2019-10-27 15:10:11.000000 Deprecated-1.2.9/tests/test_sphinx_metaclass.py
+-rw-r--r--   0 tantale    (505) staff       (20)     1185 2020-04-10 07:53:24.000000 Deprecated-1.2.9/tox.ini
```

### Comparing `Deprecated-1.2.8/.bumpversion.cfg` & `Deprecated-1.2.9/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.8
+current_version = 1.2.9
 commit = True
 tag = False
 message = Prepare next version {new_version} (unreleased)
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
@@ -15,8 +15,7 @@
 [bumpversion:file:docs/source/conf.py]
 search = release = "{current_version}"
 replace = release = "{new_version}"
 
 [bumpversion:file:python-deprecated.spec]
 search = (?<=Version:\s+){current_version}
 replace = {new_version}
-
```

### Comparing `Deprecated-1.2.8/.github/CODE_OF_CONDUCT.md` & `Deprecated-1.2.9/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/.github/ISSUE_TEMPLATE.md` & `Deprecated-1.2.9/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/.github/PULL_REQUEST_TEMPLATE.md` & `Deprecated-1.2.9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/.packit.yaml` & `Deprecated-1.2.9/.packit.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 00000000: 7370 6563 6669 6c65 5f70 6174 683a 2070  specfile_path: p
 00000010: 7974 686f 6e2d 6465 7072 6563 6174 6564  ython-deprecated
 00000020: 2e73 7065 630a 7379 6e63 6564 5f66 696c  .spec.synced_fil
 00000030: 6573 3a0a 2020 2d20 7079 7468 6f6e 2d64  es:.  - python-d
 00000040: 6570 7265 6361 7465 642e 7370 6563 0a20  eprecated.spec. 
-00000050: 202d 202e 7061 636b 6974 2e79 616d 6c0a   - .packit.yaml.
-00000060: 7570 7374 7265 616d 5f70 726f 6a65 6374  upstream_project
-00000070: 5f6e 616d 653a 2044 6570 7265 6361 7465  _name: Deprecate
-00000080: 640a 646f 776e 7374 7265 616d 5f70 6163  d.downstream_pac
-00000090: 6b61 6765 5f6e 616d 653a 2070 7974 686f  kage_name: pytho
-000000a0: 6e2d 6465 7072 6563 6174 6564 0a63 7265  n-deprecated.cre
-000000b0: 6174 655f 7072 3a20 6661 6c73 650a 6a6f  ate_pr: false.jo
-000000c0: 6273 3a0a 2d20 6a6f 623a 2070 726f 706f  bs:.- job: propo
-000000d0: 7365 5f64 6f77 6e73 7472 6561 6d0a 2020  se_downstream.  
-000000e0: 7472 6967 6765 723a 2072 656c 6561 7365  trigger: release
-000000f0: 0a20 206d 6574 6164 6174 613a 0a20 2020  .  metadata:.   
-00000100: 2064 6973 745f 6769 745f 6272 616e 6368   dist_git_branch
-00000110: 3a20 6d61 7374 6572 0a2d 206a 6f62 3a20  : master.- job: 
-00000120: 7072 6f70 6f73 655f 646f 776e 7374 7265  propose_downstre
-00000130: 616d 0a20 2074 7269 6767 6572 3a20 7265  am.  trigger: re
-00000140: 6c65 6173 650a 2020 6d65 7461 6461 7461  lease.  metadata
-00000150: 3a0a 2020 2020 6469 7374 5f67 6974 5f62  :.    dist_git_b
-00000160: 7261 6e63 683a 2066 3330 0a2d 206a 6f62  ranch: f30.- job
-00000170: 3a20 7072 6f70 6f73 655f 646f 776e 7374  : propose_downst
-00000180: 7265 616d 0a20 2074 7269 6767 6572 3a20  ream.  trigger: 
-00000190: 7265 6c65 6173 650a 2020 6d65 7461 6461  release.  metada
-000001a0: 7461 3a0a 2020 2020 6469 7374 5f67 6974  ta:.    dist_git
-000001b0: 5f62 7261 6e63 683a 2066 3239 0a2d 206a  _branch: f29.- j
-000001c0: 6f62 3a20 636f 7072 5f62 7569 6c64 0a20  ob: copr_build. 
-000001d0: 2074 7269 6767 6572 3a20 7075 6c6c 5f72   trigger: pull_r
-000001e0: 6571 7565 7374 0a20 206d 6574 6164 6174  equest.  metadat
-000001f0: 613a 0a20 2020 2074 6172 6765 7473 3a0a  a:.    targets:.
-00000200: 2020 2020 2d20 6665 646f 7261 2d33 302d      - fedora-30-
-00000210: 7838 365f 3634 0a20 2020 202d 2066 6564  x86_64.    - fed
-00000220: 6f72 612d 3239 2d78 3836 5f36 340a 2020  ora-29-x86_64.  
-00000230: 2020 2d20 6665 646f 7261 2d72 6177 6869    - fedora-rawhi
-00000240: 6465 2d78 3836 5f36 340a                 de-x86_64.
+00000050: 202d 202e 7061 636b 6974 2e79 6d6c 0a75   - .packit.yml.u
+00000060: 7073 7472 6561 6d5f 7072 6f6a 6563 745f  pstream_project_
+00000070: 6e61 6d65 3a20 4465 7072 6563 6174 6564  name: Deprecated
+00000080: 0a64 6f77 6e73 7472 6561 6d5f 7061 636b  .downstream_pack
+00000090: 6167 655f 6e61 6d65 3a20 7079 7468 6f6e  age_name: python
+000000a0: 2d64 6570 7265 6361 7465 640a 6372 6561  -deprecated.crea
+000000b0: 7465 5f70 723a 2066 616c 7365 0a6a 6f62  te_pr: false.job
+000000c0: 733a 0a20 202d 206a 6f62 3a20 7072 6f70  s:.  - job: prop
+000000d0: 6f73 655f 646f 776e 7374 7265 616d 0a20  ose_downstream. 
+000000e0: 2020 2074 7269 6767 6572 3a20 7265 6c65     trigger: rele
+000000f0: 6173 650a 2020 2020 6d65 7461 6461 7461  ase.    metadata
+00000100: 3a0a 2020 2020 2020 6469 7374 2d67 6974  :.      dist-git
+00000110: 2d62 7261 6e63 683a 206d 6173 7465 720a  -branch: master.
+00000120: 2020 2d20 6a6f 623a 2070 726f 706f 7365    - job: propose
+00000130: 5f64 6f77 6e73 7472 6561 6d0a 2020 2020  _downstream.    
+00000140: 7472 6967 6765 723a 2072 656c 6561 7365  trigger: release
+00000150: 0a20 2020 206d 6574 6164 6174 613a 0a20  .    metadata:. 
+00000160: 2020 2020 2064 6973 742d 6769 742d 6272       dist-git-br
+00000170: 616e 6368 3a20 6665 646f 7261 2d61 6c6c  anch: fedora-all
+00000180: 0a20 202d 206a 6f62 3a20 7072 6f70 6f73  .  - job: propos
+00000190: 655f 646f 776e 7374 7265 616d 0a20 2020  e_downstream.   
+000001a0: 2074 7269 6767 6572 3a20 7265 6c65 6173   trigger: releas
+000001b0: 650a 2020 2020 6d65 7461 6461 7461 3a0a  e.    metadata:.
+000001c0: 2020 2020 2020 6469 7374 2d67 6974 2d62        dist-git-b
+000001d0: 7261 6e63 683a 2066 3330 0a20 202d 206a  ranch: f30.  - j
+000001e0: 6f62 3a20 7072 6f70 6f73 655f 646f 776e  ob: propose_down
+000001f0: 7374 7265 616d 0a20 2020 2074 7269 6767  stream.    trigg
+00000200: 6572 3a20 7265 6c65 6173 650a 2020 2020  er: release.    
+00000210: 6d65 7461 6461 7461 3a0a 2020 2020 2020  metadata:.      
+00000220: 6469 7374 2d67 6974 2d62 7261 6e63 683a  dist-git-branch:
+00000230: 2066 3239 0a20 202d 206a 6f62 3a20 636f   f29.  - job: co
+00000240: 7072 5f62 7569 6c64 0a20 2020 2074 7269  pr_build.    tri
+00000250: 6767 6572 3a20 7075 6c6c 5f72 6571 7565  gger: pull_reque
+00000260: 7374 0a20 2020 206d 6574 6164 6174 613a  st.    metadata:
+00000270: 0a20 2020 2020 2074 6172 6765 7473 3a0a  .      targets:.
+00000280: 2020 2020 2020 2020 2d20 6665 646f 7261          - fedora
+00000290: 2d61 6c6c 0a20 2020 2020 2020 202d 2066  -all.        - f
+000002a0: 6564 6f72 612d 3330 2d78 3836 5f36 340a  edora-30-x86_64.
+000002b0: 2020 2020 2020 2020 2d20 6665 646f 7261          - fedora
+000002c0: 2d32 392d 7838 365f 3634 0a20 2020 2020  -29-x86_64.     
+000002d0: 2020 202d 2066 6564 6f72 612d 7261 7768     - fedora-rawh
+000002e0: 6964 652d 7838 365f 3634 0a              ide-x86_64.
```

### Comparing `Deprecated-1.2.8/CHANGELOG.rst` & `Deprecated-1.2.9/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,32 @@
 
     - In your ``setup.py``, you can replace the "Python-Deprecated" dependency with "Deprecated".
     - In your source code, nothing has changed, you will always use ``import deprecated``, as before.
     - I decided to keep the same version number because there is really no change in the source code
       (only in comment or documentation).
 
 
+v1.2.9 (2020-04-10)
+===================
+
+Bug fix release
+
+Fix
+---
+
+- Fix #20: Set the :func:`warnings.warn` stacklevel to 2 if the Python implementation is `PyPy <https://www.pypy.org/>`_.
+
+- Fix packit configuration: use ``dist-git-branch: fedora-all``.
+
+Other
+-----
+
+- Change the Tox configuration to run tests on PyPy v2.7 and 3.6.
+
+
 v1.2.8 (2020-04-05)
 ===================
 
 Bug fix release
 
 Fix
 ---
```

### Comparing `Deprecated-1.2.8/CONTRIBUTING.rst` & `Deprecated-1.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/Deprecated.egg-info/PKG-INFO` & `Deprecated-1.2.9/Deprecated.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Deprecated
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python @deprecated decorator to deprecate old python classes, functions or methods.
 Home-page: https://github.com/tantale/deprecated
 Author: Laurent LAPORTE
 Author-email: tantale.solutions@gmail.com
 License: MIT
 Project-URL: Documentation, https://deprecated.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/tantale/deprecated
@@ -161,8 +161,9 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
+Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `Deprecated-1.2.8/Deprecated.egg-info/SOURCES.txt` & `Deprecated-1.2.9/Deprecated.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .bumpversion.cfg
 .editorconfig
-.packit.yaml
+.packit.yml
 .travis.yml
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE.rst
 MANIFEST.in
 Makefile
 README.md
```

### Comparing `Deprecated-1.2.8/LICENSE.rst` & `Deprecated-1.2.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/Makefile` & `Deprecated-1.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/PKG-INFO` & `Deprecated-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Deprecated
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python @deprecated decorator to deprecate old python classes, functions or methods.
 Home-page: https://github.com/tantale/deprecated
 Author: Laurent LAPORTE
 Author-email: tantale.solutions@gmail.com
 License: MIT
 Project-URL: Documentation, https://deprecated.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/tantale/deprecated
@@ -161,8 +161,9 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
+Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `Deprecated-1.2.8/README.md` & `Deprecated-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/appveyor.yml` & `Deprecated-1.2.9/appveyor.yml`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/deprecated/classic.py` & `Deprecated-1.2.9/deprecated/classic.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,32 @@
 Classic ``@deprecated`` decorator to deprecate old python classes, functions or methods.
 
 .. _The Warnings Filter: https://docs.python.org/3/library/warnings.html#the-warnings-filter
 """
 import functools
 import inspect
 import warnings
+import platform
 
 import wrapt
 
 try:
-    # If the c extension for wrapt was compiled and wrapt/_wrappers.pyd exists, then the
+    # If the C extension for wrapt was compiled and wrapt/_wrappers.pyd exists, then the
     # stack level that should be passed to warnings.warn should be 2. However, if using
     # a pure python wrapt, a extra stacklevel is required.
     import wrapt._wrappers
 
-    _stacklevel = 2
+    _routine_stacklevel = 2
+    _class_stacklevel = 2
 except ImportError:
-    _stacklevel = 3
+    _routine_stacklevel = 3
+    if platform.python_implementation() == "PyPy":
+        _class_stacklevel = 2
+    else:
+        _class_stacklevel = 3
 
 string_types = (type(b''), type(u''))
 
 
 class ClassicAdapter(wrapt.AdapterFactory):
     """
     Classic adapter -- *for advanced usage only*
@@ -154,21 +160,21 @@
             old_new1 = wrapped.__new__
 
             def wrapped_cls(cls, *args, **kwargs):
                 msg = self.get_deprecated_msg(wrapped, None)
                 with warnings.catch_warnings():
                     if self.action:
                         warnings.simplefilter(self.action, self.category)
-                    warnings.warn(msg, category=self.category, stacklevel=_stacklevel)
+                    warnings.warn(msg, category=self.category, stacklevel=_class_stacklevel)
                 if old_new1 is object.__new__:
                     return old_new1(cls)
                 # actually, we don't know the real signature of *old_new1*
-                return old_new1(*args, **kwargs)
+                return old_new1(cls, *args, **kwargs)
 
-            wrapped.__new__ = classmethod(wrapped_cls)
+            wrapped.__new__ = staticmethod(wrapped_cls)
 
         return wrapped
 
 
 def deprecated(*args, **kwargs):
     """
     This is a decorator which can be used to mark functions
@@ -267,15 +273,15 @@
 
             @wrapt.decorator(adapter=adapter)
             def wrapper_function(wrapped_, instance_, args_, kwargs_):
                 msg = adapter.get_deprecated_msg(wrapped_, instance_)
                 with warnings.catch_warnings():
                     if action:
                         warnings.simplefilter(action, category)
-                    warnings.warn(msg, category=category, stacklevel=_stacklevel)
+                    warnings.warn(msg, category=category, stacklevel=_routine_stacklevel)
                 return wrapped_(*args_, **kwargs_)
 
             return wrapper_function(wrapped)
 
         else:
             raise TypeError(repr(type(wrapped)))
```

### Comparing `Deprecated-1.2.8/deprecated/sphinx.py` & `Deprecated-1.2.9/deprecated/sphinx.py`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/cover/paper_10.jpeg` & `Deprecated-1.2.9/docs/cover/paper_10.jpeg`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/cover/title-page.odg` & `Deprecated-1.2.9/docs/cover/title-page.odg`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/_static/banner.png` & `Deprecated-1.2.9/docs/source/_static/banner.png`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/_static/logo-full.png` & `Deprecated-1.2.9/docs/source/_static/logo-full.png`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/_static/title-page.jpg` & `Deprecated-1.2.9/docs/source/_static/title-page.jpg`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/conf.py` & `Deprecated-1.2.9/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 author = 'Marcos CARDOSO & Laurent LAPORTE'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = "1.2.8"
+release = "1.2.9"
 # The short X.Y version.
 version = release.rpartition('.')[0]
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
```

### Comparing `Deprecated-1.2.8/docs/source/index.rst` & `Deprecated-1.2.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/installation.rst` & `Deprecated-1.2.9/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/introduction.rst` & `Deprecated-1.2.9/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/sphinx/sphinx_demo.py` & `Deprecated-1.2.9/docs/source/sphinx/sphinx_demo.py`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/sphinx_deco.rst` & `Deprecated-1.2.9/docs/source/sphinx_deco.rst`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/tutorial/v1/liberty.py` & `Deprecated-1.2.9/docs/source/tutorial/v1/liberty.py`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/tutorial/v2/liberty.py` & `Deprecated-1.2.9/docs/source/tutorial/v2/liberty.py`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/tutorial/v3/liberty.py` & `Deprecated-1.2.9/docs/source/tutorial/v3/liberty.py`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/tutorial/warning_ctrl/warning_classes_demo.py` & `Deprecated-1.2.9/docs/source/tutorial/warning_ctrl/warning_classes_demo.py`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/tutorial.rst` & `Deprecated-1.2.9/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/docs/source/white_paper.rst` & `Deprecated-1.2.9/docs/source/white_paper.rst`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/python-deprecated.spec` & `Deprecated-1.2.9/python-deprecated.spec`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 %global srcname Deprecated
 %global pkgname deprecated
 
 Name:           python-%{pkgname}
-Version:        1.2.8
+Version:        1.2.9
 Release:        2%{?dist}
 Summary:        Python decorator to deprecate old python classes, functions or methods
 License:        MIT
 URL:            https://github.com/tantale/%{pkgname}
 Source0:        https://files.pythonhosted.org/packages/source/D/%{srcname}/%{srcname}-%{version}.tar.gz
 BuildArch:      noarch
 
@@ -38,12 +38,12 @@
 %license LICENSE.rst
 %doc README.md
 %{python3_sitelib}/%{pkgname}/
 %{python3_sitelib}/%{srcname}-%{version}-*.egg-info/
 
 
 %changelog
-* Fri Jul 26 2019 Petr Hracek <phracek@redhat.com> - 1.2.8-2
+* Fri Jul 26 2019 Petr Hracek <phracek@redhat.com> - 1.2.6-2
 - Fix python3_sitelib issue
 
-* Fri Jul 26 2019 Petr Hracek <phracek@redhat.com> - 1.2.8-1
+* Fri Jul 26 2019 Petr Hracek <phracek@redhat.com> - 1.2.6-1
 - Initial package
```

### Comparing `Deprecated-1.2.8/setup.py` & `Deprecated-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,26 +139,27 @@
   <https://github.com/tantale/deprecated/zipball/master#egg=Deprecated-dev>`_
 
 """
 from setuptools import setup
 
 setup(
     name='Deprecated',
-    version='1.2.8',
+    version='1.2.9',
     url='https://github.com/tantale/deprecated',
     project_urls={
         "Documentation": "https://deprecated.readthedocs.io/en/latest/",
         "Source": "https://github.com/tantale/deprecated",
         "Bug Tracker": "https://github.com/tantale/deprecated/issues",
     },
     license='MIT',
     author='Laurent LAPORTE',  # since v1.1.0
     author_email='tantale.solutions@gmail.com',
     description='Python @deprecated decorator to deprecate old python classes, functions or methods.',
     long_description=__doc__,
+    long_description_content_type="text/x-rst",
     keywords='deprecate,deprecated,deprecation,warning,warn,decorator',
     packages=['deprecated'],
     install_requires=['wrapt < 2, >= 1.10'],
     zip_safe=False,
     include_package_data=True,
     platforms='any',
     classifiers=[
```

### Comparing `Deprecated-1.2.8/tests/test.py` & `Deprecated-1.2.9/tests/test.py`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/tests/test_deprecated.py` & `Deprecated-1.2.9/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/tests/test_deprecated_class.py` & `Deprecated-1.2.9/tests/test_deprecated_class.py`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/tests/test_deprecated_metaclass.py` & `Deprecated-1.2.9/tests/test_deprecated_metaclass.py`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/tests/test_sphinx.py` & `Deprecated-1.2.9/tests/test_sphinx.py`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/tests/test_sphinx_class.py` & `Deprecated-1.2.9/tests/test_sphinx_class.py`

 * *Files identical despite different names*

### Comparing `Deprecated-1.2.8/tests/test_sphinx_metaclass.py` & `Deprecated-1.2.9/tests/test_sphinx_metaclass.py`

 * *Files identical despite different names*

