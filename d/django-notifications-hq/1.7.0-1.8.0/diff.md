# Comparing `tmp/django-notifications-hq-1.7.0.tar.gz` & `tmp/django-notifications-hq-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-notifications-hq-1.7.0.tar", last modified: Tue Mar  1 19:30:21 2022, max compression
+gzip compressed data, was "django-notifications-hq-1.8.0.tar", last modified: Sat May 27 16:25:26 2023, max compression
```

## Comparing `django-notifications-hq-1.7.0.tar` & `django-notifications-hq-1.8.0.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.863474 django-notifications-hq-1.7.0/
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)     1076 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/AUTHORS.txt
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)     5397 2022-03-01 19:28:01.000000 django-notifications-hq-1.7.0/CHANGELOG.rst
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)     1563 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/LICENSE.txt
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      124 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/MANIFEST.in
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)    18685 2022-03-01 19:30:21.863474 django-notifications-hq-1.7.0/PKG-INFO
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)    17580 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/README.rst
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.855474 django-notifications-hq-1.7.0/django_notifications_hq.egg-info/
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)    18685 2022-03-01 19:30:21.000000 django-notifications-hq-1.7.0/django_notifications_hq.egg-info/PKG-INFO
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)     2065 2022-03-01 19:30:21.000000 django-notifications-hq-1.7.0/django_notifications_hq.egg-info/SOURCES.txt
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)        1 2022-03-01 19:30:21.000000 django-notifications-hq-1.7.0/django_notifications_hq.egg-info/dependency_links.txt
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)       68 2022-03-01 19:30:21.000000 django-notifications-hq-1.7.0/django_notifications_hq.egg-info/requires.txt
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)       14 2022-03-01 19:30:21.000000 django-notifications-hq-1.7.0/django_notifications_hq.egg-info/top_level.txt
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.859474 django-notifications-hq-1.7.0/notifications/
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)      406 2022-03-01 19:28:01.000000 django-notifications-hq-1.7.0/notifications/__init__.py
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)      706 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/admin.py
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)      404 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/apps.py
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.859474 django-notifications-hq-1.7.0/notifications/base/
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)        0 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/base/__init__.py
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)      440 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/base/admin.py
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)    10693 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/base/models.py
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.859474 django-notifications-hq-1.7.0/notifications/migrations/
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)     2201 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/migrations/0001_initial.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      595 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/migrations/0002_auto_20150224_1134.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      446 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/migrations/0003_notification_data.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      420 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/migrations/0004_auto_20150826_1508.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      532 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/migrations/0005_auto_20160504_1520.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      947 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/migrations/0006_indexes.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      458 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/migrations/0007_add_timestamp_index.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      469 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/migrations/0008_index_together_recipient_unread.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)        0 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/migrations/__init__.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      293 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/models.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      403 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/settings.py
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)      119 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/signals.py
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.855474 django-notifications-hq-1.7.0/notifications/static/
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.863474 django-notifications-hq-1.7.0/notifications/static/notifications/
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)     2616 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/static/notifications/notify.js
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.855474 django-notifications-hq-1.7.0/notifications/templates/
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.863474 django-notifications-hq-1.7.0/notifications/templates/notifications/
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      130 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/templates/notifications/list.html
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      655 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/templates/notifications/notice.html
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      220 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/templates/notifications/test_tags.html
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.863474 django-notifications-hq-1.7.0/notifications/templatetags/
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)        0 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/templatetags/__init__.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)     3441 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/templatetags/notifications_tags.py
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.863474 django-notifications-hq-1.7.0/notifications/tests/
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)        0 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/tests/__init__.py
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.863474 django-notifications-hq-1.7.0/notifications/tests/sample_notifications/
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)       95 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/tests/sample_notifications/__init__.py
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)      272 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/tests/sample_notifications/admin.py
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)      204 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/tests/sample_notifications/apps.py
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.863474 django-notifications-hq-1.7.0/notifications/tests/sample_notifications/migrations/
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)     2720 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/tests/sample_notifications/migrations/0001_initial.py
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)        0 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/tests/sample_notifications/migrations/__init__.py
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)      270 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/tests/sample_notifications/models.py
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.863474 django-notifications-hq-1.7.0/notifications/tests/sample_notifications/templatetags/
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)        0 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/tests/sample_notifications/templatetags/__init__.py
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)       67 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/tests/sample_notifications/templatetags/notifications_tags.py
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)      701 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/tests/sample_notifications/tests.py
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)     2108 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/tests/settings.py
-drwxrwxr-x   0 nemesis   (1000) nemesis   (1000)        0 2022-03-01 19:30:21.863474 django-notifications-hq-1.7.0/notifications/tests/templates/
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      489 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/tests/templates/test_live.html
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)    27140 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/tests/tests.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)     1821 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/tests/urls.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      909 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/tests/views.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)     1338 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/urls.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)      267 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/notifications/utils.py
--rw-rw-r--   0 nemesis   (1000) nemesis   (1000)     7702 2021-12-26 20:36:28.000000 django-notifications-hq-1.7.0/notifications/views.py
--rw-r--r--   0 nemesis   (1000) nemesis   (1000)       67 2022-03-01 19:30:21.863474 django-notifications-hq-1.7.0/setup.cfg
--rwxr-xr-x   0 nemesis   (1000) nemesis   (1000)     2363 2020-02-21 21:01:43.000000 django-notifications-hq-1.7.0/setup.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.876377 django-notifications-hq-1.8.0/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1076 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/AUTHORS.txt
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     6241 2023-05-25 23:39:54.000000 django-notifications-hq-1.8.0/CHANGELOG.md
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1563 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/LICENSE.txt
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      122 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/MANIFEST.in
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)    17791 2023-05-27 16:25:26.876621 django-notifications-hq-1.8.0/PKG-INFO
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)    16575 2023-05-27 16:25:07.000000 django-notifications-hq-1.8.0/README.md
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.847517 django-notifications-hq-1.8.0/django_notifications_hq.egg-info/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)    17791 2023-05-27 16:25:26.000000 django-notifications-hq-1.8.0/django_notifications_hq.egg-info/PKG-INFO
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     2089 2023-05-27 16:25:26.000000 django-notifications-hq-1.8.0/django_notifications_hq.egg-info/SOURCES.txt
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        1 2023-05-27 16:25:26.000000 django-notifications-hq-1.8.0/django_notifications_hq.egg-info/dependency_links.txt
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)       68 2023-05-27 16:25:26.000000 django-notifications-hq-1.8.0/django_notifications_hq.egg-info/requires.txt
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)       14 2023-05-27 16:25:26.000000 django-notifications-hq-1.8.0/django_notifications_hq.egg-info/top_level.txt
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.854563 django-notifications-hq-1.8.0/notifications/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      406 2023-05-27 15:14:58.000000 django-notifications-hq-1.8.0/notifications/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1038 2023-05-25 23:26:46.000000 django-notifications-hq-1.8.0/notifications/admin.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      499 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/apps.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.856813 django-notifications-hq-1.8.0/notifications/base/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/base/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      440 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/base/admin.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)    13483 2023-05-25 23:34:36.000000 django-notifications-hq-1.8.0/notifications/base/models.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1416 2023-05-24 00:22:47.000000 django-notifications-hq-1.8.0/notifications/helpers.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.838961 django-notifications-hq-1.8.0/notifications/locale/
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.839106 django-notifications-hq-1.8.0/notifications/locale/ru/
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.857813 django-notifications-hq-1.8.0/notifications/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     3489 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.863992 django-notifications-hq-1.8.0/notifications/migrations/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     2201 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/migrations/0001_initial.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      595 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/migrations/0002_auto_20150224_1134.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      446 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/migrations/0003_notification_data.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      420 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/migrations/0004_auto_20150826_1508.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      532 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/migrations/0005_auto_20160504_1520.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      947 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/migrations/0006_indexes.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      458 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/migrations/0007_add_timestamp_index.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      469 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/migrations/0008_index_together_recipient_unread.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/migrations/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      826 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/models.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      427 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/settings.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      119 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/signals.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.839674 django-notifications-hq-1.8.0/notifications/templates/
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.865714 django-notifications-hq-1.8.0/notifications/templates/notifications/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      130 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/templates/notifications/list.html
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      655 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/templates/notifications/notice.html
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      220 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/templates/notifications/test_tags.html
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.866666 django-notifications-hq-1.8.0/notifications/templatetags/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/templatetags/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     4193 2023-05-26 00:53:42.000000 django-notifications-hq-1.8.0/notifications/templatetags/notifications_tags.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.870346 django-notifications-hq-1.8.0/notifications/tests/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/tests/__init__.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.873151 django-notifications-hq-1.8.0/notifications/tests/sample_notifications/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)       95 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/tests/sample_notifications/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      272 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/tests/sample_notifications/admin.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      204 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/tests/sample_notifications/apps.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.874463 django-notifications-hq-1.8.0/notifications/tests/sample_notifications/migrations/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     2720 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/tests/sample_notifications/migrations/0001_initial.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/tests/sample_notifications/migrations/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      270 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/tests/sample_notifications/models.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.875246 django-notifications-hq-1.8.0/notifications/tests/sample_notifications/templatetags/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/tests/sample_notifications/templatetags/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)       67 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/tests/sample_notifications/templatetags/notifications_tags.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1791 2023-05-25 23:35:16.000000 django-notifications-hq-1.8.0/notifications/tests/sample_notifications/tests.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     2128 2023-05-27 14:58:13.000000 django-notifications-hq-1.8.0/notifications/tests/settings.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-27 16:25:26.875777 django-notifications-hq-1.8.0/notifications/tests/templates/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      507 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/tests/templates/test_live.html
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)    28778 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.0/notifications/tests/tests.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1821 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/tests/urls.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      909 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/tests/views.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1338 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/urls.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      267 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.0/notifications/utils.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     6142 2023-05-27 14:09:18.000000 django-notifications-hq-1.8.0/notifications/views.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)       67 2023-05-27 16:25:26.877509 django-notifications-hq-1.8.0/setup.cfg
+-rwxr-xr-x   0 alvaro.mariano   (501) staff       (20)     2418 2023-05-27 16:25:18.000000 django-notifications-hq-1.8.0/setup.py
```

### Comparing `django-notifications-hq-1.7.0/AUTHORS.txt` & `django-notifications-hq-1.8.0/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.7.0/CHANGELOG.rst` & `django-notifications-hq-1.8.0/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,162 +1,175 @@
-Changelog
-=========
+# Changelog
 
+## 1.8.0
 
-1.7.0
------
+  - Added support for Django 4.1
+  - Dropped support for Django < 3.2 and Python < 3.7
+  - Added indexes for GenericForeignKey fields in AbstractNotificationModel (see https://docs.djangoproject.com/en/4.1/ref/contrib/contenttypes/#generic-relations)
+  - new setting 'CACHE_TIMEOUT' to cache certain result such as "notifications.unread().count".
+  (a timeout value of 0 won’t cache anything).
+  - #263 Fix vunerability in views
+  - #233 Adds methods to convert to human readable type
+  - Translate project all strings
+
+## 1.7.0
+
+  - Added support for Django 3.2 and Django 4.0
+  - Fixed bug on IE11 for using `forEach` in notify.js
+
+## 1.6.0
+
+  - Added support to Django up to version 3.0
+  - Added `AbstractNotification` model
+  - Added prefetch for actor field in admin
+  - Added never\_cache to some views to avoid no-update bug
+
+## 1.5
+
+Now all configs for the app are made inside the dictionary
+*DJANGO\_NOTIFICATION\_CONFIG* in *settings.py*.
+
+Default configs: `` `Python DJANGO_NOTIFICATIONS_CONFIG = {
+'PAGINATE_BY': 20, 'USE_JSONFIELD': False, 'SOFT_DELETE': False,
+'NUM_TO_FETCH': 10, } ``\`
+
+  - Improve code quality. (@AlvaroLQueiroz)
+  - Improve url patterns and remove duplicated code. (@julianogouveia)
+  - Added a view for show all notifications. \#205 (@AlvaroLQueiroz)
+  - Added a new tag to verify if an user has unread notifications. \#164
+    (@AlvaroLQueiroz)
+  - Improve documentation. (@pandabearcoder)
+  - Fix pagination in list views. \#69 (@AlvaroLQueiroz)
+  - Improve test matrix. (@AlvaroLQueiroz)
+
+## 1.4
+
+  - Adds support for django 2.0.0 (@jphamcsp and @nemesisdesign).
+  - Adds database index for some fields (@nemesisdesign).
+  - Changes the ID-based selection to a class-based selection in the
+    methods
+    \_\_[live\_notify\_badge](THIS%20VERSION%20HAS%20BREAKING%20CHANGES__:)
+    and \_\_live\_notify\_list\_\_ (@AlvaroLQueiroz).
+  - Now extra data and slug are returned on
+    \_\_live\_unread\_notification\_list\_\_ API (@AlvaroLQueiroz).
+  - Fix documentation issues (@archatas, @yaoelvon and @AlvaroLQueiroz).
+
+## 1.3
+
+  - Redirect to unread view after mark as read. (@osminogin)
+  - Django 1.10 compability. (@osminogin)
+  - Django Admin overhead reduction by removing the need to carry all
+    recipients users. (@theromis)
+  - Added option to mark as read in
+    \_\_live\_unread\_notification\_list\_\_ endpoint. (@osminogin)
+  - Fixed parameter name error in README.rst: there is no
+    \_\_api\_url\_name\_\_ parameter, the correct name is
+    \_\_api\_name\_\_ (@ikkebr)
+  - Added \_\_sent()\_\_, \_\_unsent()\_\_, \_\_mark\_as\_sent()\_\_ and
+    \_\_mark\_as\_unsent()\_\_ methods in the queryset. (@theromis)
+  - \_\_notify.send()\_\_ now returns the list of saved Notifications
+    instances. (@satyanash)
+  - Now \_\_recipient\_\_ can be a User queryset. (@AlvaroLQueiroz)
+  - Fix XMLHttpRequest onready event handler. (@AlvaroLQueiroz)
+
+## 1.2
+
+  - Django 1.9 template tag compatibility: due to `register.simple_tag`
+    automatically espacing `unsafe_html` in Django 1.9, it is now
+    recommended to use format\_html (@ikkebr)
+  - Fixed parameter name error in README.rst: there is no to\_fetch
+    parameter, the correct name is fetch (@ikkebr)
+  - Add missing migration (@marcgibbons)
+  - Minor documentation correction (@tkwon, @zhang-z)
+  - Return updated count in QuerySet (@zhang-z)
+
+## 1.1
+
+  - Custom now() invocation got overlooked by PR \#113 (@yangyuvo)
+  - Added sentinals for unauthenticated users, preventing a 500 error
+    (@LegoStormtroopr)
+  - Fix: Mark All As read fails if soft-deleted \#126 (@zhang-z)
 
-- Added support for Django 3.2 and Django 4.0
-- Fixed bug on IE11 for using ``forEach`` in notify.js
-
-1.6.0
------
-
-- Added support to Django up to version 3.0
-- Added ``AbstractNotification`` model
-- Added prefetch for actor field in admin
-- Added never_cache to some views to avoid no-update bug
-
-1.5
-----
-__THIS VERSION HAS BREAKING CHANGES__:
-Now all configs for the app are made inside the dictionary *DJANGO_NOTIFICATION_CONFIG* in *settings.py*.
-
-Default configs:
-```Python
-DJANGO_NOTIFICATION_CONFIG = {
-    'PAGINATE_BY': 20,
-    'USE_JSONFIELD': False,
-    'SOFT_DELETE': False,
-    'NUM_TO_FETCH': 10,
-}
-```
-
-- Improve code quality. (@AlvaroLQueiroz)
-- Improve url patterns and remove duplicated code. (@julianogouveia)
-- Added a view for show all notifications. #205 (@AlvaroLQueiroz)
-- Added a new tag to verify if an user has unread notifications. #164 (@AlvaroLQueiroz)
-- Improve documentation. (@pandabearcoder)
-- Fix pagination in list views. #69 (@AlvaroLQueiroz)
-- Improve test matrix. (@AlvaroLQueiroz)
-
-1.4
-----
-
-- Adds support for django 2.0.0 (@jphamcsp and @nemesisdesign).
-- Adds database index for some fields (@nemesisdesign).
-- Changes the ID-based selection to a class-based selection in the methods __live_notify_badge__ and __live_notify_list__ (@AlvaroLQueiroz).
-- Now extra data and slug are returned on __live_unread_notification_list__ API (@AlvaroLQueiroz).
-- Fix documentation issues (@archatas, @yaoelvon and @AlvaroLQueiroz).
-
-1.3
------
-
-- Redirect to unread view after mark as read. (@osminogin)
-- Django 1.10 compability. (@osminogin)
-- Django Admin overhead reduction by removing the need to carry all recipients users. (@theromis)
-- Added option to mark as read in __live_unread_notification_list__ endpoint. (@osminogin)
-- Fixed parameter name error in README.rst: there is no __api_url_name__ parameter, the correct name is __api_name__ (@ikkebr)
-- Added __sent()__, __unsent()__, __mark_as_sent()__ and __mark_as_unsent()__ methods in the queryset. (@theromis)
-- __notify.send()__ now returns the list of saved Notifications instances. (@satyanash)
-- Now __recipient__ can be a User queryset. (@AlvaroLQueiroz)
-- Fix XMLHttpRequest onready event handler. (@AlvaroLQueiroz)
-
-1.2
------
-
-- Django 1.9 template tag compatibility: due to ``register.simple_tag`` automatically espacing ``unsafe_html`` in Django 1.9, it is now recommended to use format_html (@ikkebr)
-- Fixed parameter name error in README.rst: there is no to_fetch parameter, the correct name is fetch (@ikkebr)
-- Add missing migration (@marcgibbons)
-- Minor documentation correction (@tkwon, @zhang-z)
-- Return updated count in QuerySet (@zhang-z)
-
-1.1
------
-
-- Custom now() invocation got overlooked by PR #113 (@yangyuvo)
-- Added sentinals for unauthenticated users, preventing a 500 error (@LegoStormtroopr)
-- Fix: Mark All As read fails if soft-deleted #126 (@zhang-z)
-
-1.0
------
+## 1.0
 
 The first major version that requires Django 1.7+.
 
-- Drop support for Django 1.6 and below (@zhang-z)
-- Django 1.9 compability (@illing2005)
-- Now depends on Django built-in migration facility, "south_migrations" dependence was removed (@zhang-z)
-- Make django-notification compatible with django-model-utils >= 2.4 ( #87, #88, #90 ) (@zhang-z)
-- Fix a RemovedInDjango110Warning in unittest (@zhang-z)
-- Fix pep8 & use setuptools (@areski)
-- Fix typo- in doc (@areski, @zhang-z)
-- Add app_name in urls.py (@zhang-z)
-- Use Django's vendored copy of six (@funkybob)
-- Tidy with flake8 (@funkybob)
-- Remove custom now() function (@funkybob, @yangyubo)
-- notify.send() accepts User or Group (@Evidlo)
-
-0.8.0
------
-
-0.8 is the last major version supports Django 1.4~1.6, version 0.8.0 will go into bugfix mode, no new features will be accepted.
-
-- Bugfixes for live-updater, and added a live tester page (@LegoStormtroopr)
-- Class-based classes (@alazaro)
-- Fixed urls in tests (@alazaro)
-- Added app_label to Notification model in order to fix a Django 1.9 deprecation warning (@Heldroe)
-- django-model-utils compatible issue (must >=2.0.3 and <2.4) (@zhang-z)
-- Reliable setup.py versioning (@yangyubo)
-
-0.7.1
------
-
-- Able to pass level when adding notification (@Arthur)
-- Fix deprecation notice in Django 1.8 (@ashokfernandez)
-- Fix Python 3 support for notification model (@philroche)
-- Bugfix for wrong user unread notification count (@Geeknux)
-- A simple javascript API for live-updating specific fields within a django template (@LegoStormtroopr)
-- Add missing migration for Notification model (@shezadkhan137)
-
-0.7.0
------
-
-- Add filters and displays to Django model Admin
-- Support Django 1.8, compatible with both django-south (django < 1.7) and built-in schema migration (django >= 1.7)
-- Compatible with Python 3
-- Test fixtures, and integrated with travis-ci
-
-0.6.2
------
-
-- Fix README.rst reStructuredText syntax format
-- Use relative imports
-- Add contributors to AUTHORS.txt
-
-0.6.1
------
-
-- Add support for custom user model
-- mark_as_unread
-- Require django-model-utils >= 2.0.3
-- Use different `now` function according to the `USE_TZ` setting
+  - Drop support for Django 1.6 and below (@zhang-z)
+  - Django 1.9 compability (@illing2005)
+  - Now depends on Django built-in migration facility,
+    "south\_migrations" dependence was removed (@zhang-z)
+  - Make django-notification compatible with django-model-utils \>= 2.4
+    ( \#87, \#88, \#90 ) (@zhang-z)
+  - Fix a RemovedInDjango110Warning in unittest (@zhang-z)
+  - Fix pep8 & use setuptools (@areski)
+  - Fix typo- in doc (@areski, @zhang-z)
+  - Add app\_name in urls.py (@zhang-z)
+  - Use Django's vendored copy of six (@funkybob)
+  - Tidy with flake8 (@funkybob)
+  - Remove custom now() function (@funkybob, @yangyubo)
+  - notify.send() accepts User or Group (@Evidlo)
+
+## 0.8.0
+
+0.8 is the last major version supports Django 1.4\~1.6, version 0.8.0
+will go into bugfix mode, no new features will be accepted.
+
+  - Bugfixes for live-updater, and added a live tester page
+    (@LegoStormtroopr)
+  - Class-based classes (@alazaro)
+  - Fixed urls in tests (@alazaro)
+  - Added app\_label to Notification model in order to fix a Django 1.9
+    deprecation warning (@Heldroe)
+  - django-model-utils compatible issue (must \>=2.0.3 and \<2.4)
+    (@zhang-z)
+  - Reliable setup.py versioning (@yangyubo)
+
+## 0.7.1
+
+  - Able to pass level when adding notification (@Arthur)
+  - Fix deprecation notice in Django 1.8 (@ashokfernandez)
+  - Fix Python 3 support for notification model (@philroche)
+  - Bugfix for wrong user unread notification count (@Geeknux)
+  - A simple javascript API for live-updating specific fields within a
+    django template (@LegoStormtroopr)
+  - Add missing migration for Notification model (@shezadkhan137)
+
+## 0.7.0
+
+  - Add filters and displays to Django model Admin
+  - Support Django 1.8, compatible with both django-south (django \<
+    1.7) and built-in schema migration (django \>= 1.7)
+  - Compatible with Python 3
+  - Test fixtures, and integrated with travis-ci
+
+## 0.6.2
+
+  - Fix README.rst reStructuredText syntax format
+  - Use relative imports
+  - Add contributors to AUTHORS.txt
+
+## 0.6.1
+
+  - Add support for custom user model
+  - mark\_as\_unread
+  - Require django-model-utils \>= 2.0.3
+  - Use different <span class="title-ref">now</span> function according
+    to the <span class="title-ref">USE\_TZ</span> setting
 
-0.6.0
------
+## 0.6.0
 
-- Improve documentation
-- Add unicode support at admin panel or shell
+  - Improve documentation
+  - Add unicode support at admin panel or shell
 
-0.5.5
------
+## 0.5.5
 
 Support for arbitrary data attribute.
 
-0.5.1
------
+## 0.5.1
 
 Fix package descriptions and doc links.
 
-0.5
----
+## 0.5
 
-First version based on `django-activity-stream <https://github.com/justquick/django-activity-stream>`_ v0.4.3
+First version based on
+[django-activity-stream](https://github.com/justquick/django-activity-stream)
+v0.4.3
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-notifications-hq-1.7.0/LICENSE.txt` & `django-notifications-hq-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.7.0/README.rst` & `django-notifications-hq-1.8.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,1099 +1,1112 @@
-00000000: 6060 646a 616e 676f 2d6e 6f74 6966 6963  ``django-notific
-00000010: 6174 696f 6e73 6060 2044 6f63 756d 656e  ations`` Documen
-00000020: 7461 7469 6f6e 0a3d 3d3d 3d3d 3d3d 3d3d  tation.=========
-00000030: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000040: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  ==============..
-00000050: 0a7c 6275 696c 642d 7374 6174 7573 7c20  .|build-status| 
-00000060: 7c63 6f76 6572 616c 6c73 7c0a 0a60 646a  |coveralls|..`dj
-00000070: 616e 676f 2d6e 6f74 6966 6963 6174 696f  ango-notificatio
-00000080: 6e73 203c 6874 7470 733a 2f2f 6769 7468  ns <https://gith
-00000090: 7562 2e63 6f6d 2f64 6a61 6e67 6f2d 6e6f  ub.com/django-no
-000000a0: 7469 6669 6361 7469 6f6e 732f 646a 616e  tifications/djan
-000000b0: 676f 2d6e 6f74 6966 6963 6174 696f 6e73  go-notifications
-000000c0: 3e60 5f20 6973 2061 2047 6974 4875 6220  >`_ is a GitHub 
-000000d0: 6e6f 7469 6669 6361 7469 6f6e 2061 6c69  notification ali
-000000e0: 6b65 2061 7070 2066 6f72 2044 6a61 6e67  ke app for Djang
-000000f0: 6f2c 2069 7420 7761 7320 6465 7269 7665  o, it was derive
-00000100: 6420 6672 6f6d 2060 646a 616e 676f 2d61  d from `django-a
-00000110: 6374 6976 6974 792d 7374 7265 616d 203c  ctivity-stream <
-00000120: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000130: 6f6d 2f6a 7573 7471 7569 636b 2f64 6a61  om/justquick/dja
-00000140: 6e67 6f2d 6163 7469 7669 7479 2d73 7472  ngo-activity-str
-00000150: 6561 6d3e 605f 0a0a 5468 6520 6d61 6a6f  eam>`_..The majo
-00000160: 7220 6469 6666 6572 656e 6365 2062 6574  r difference bet
-00000170: 7765 656e 2060 6064 6a61 6e67 6f2d 6e6f  ween ``django-no
-00000180: 7469 6669 6361 7469 6f6e 7360 6020 616e  tifications`` an
-00000190: 6420 6060 646a 616e 676f 2d61 6374 6976  d ``django-activ
-000001a0: 6974 792d 7374 7265 616d 6060 3a0a 0a2a  ity-stream``:..*
-000001b0: 2060 6064 6a61 6e67 6f2d 6e6f 7469 6669   ``django-notifi
-000001c0: 6361 7469 6f6e 7360 6020 6973 2066 6f72  cations`` is for
-000001d0: 2062 7569 6c64 696e 6720 736f 6d65 7468   building someth
-000001e0: 696e 6720 6c69 6b65 2047 6974 6875 6220  ing like Github 
-000001f0: 224e 6f74 6966 6963 6174 696f 6e73 220a  "Notifications".
-00000200: 2a20 5768 696c 6520 6060 646a 616e 676f  * While ``django
-00000210: 2d61 6374 6976 6974 792d 7374 7265 616d  -activity-stream
-00000220: 6060 2069 7320 666f 7220 6275 696c 6469  `` is for buildi
-00000230: 6e67 2047 6974 6875 6220 224e 6577 7320  ng Github "News 
-00000240: 4665 6564 220a 0a4e 6f74 6966 6963 6174  Feed"..Notificat
-00000250: 696f 6e73 2061 7265 2061 6374 7561 6c6c  ions are actuall
-00000260: 7920 6163 7469 6f6e 7320 6576 656e 7473  y actions events
-00000270: 2c20 7768 6963 6820 6172 6520 6361 7465  , which are cate
-00000280: 676f 7269 7a65 6420 6279 2066 6f75 7220  gorized by four 
-00000290: 6d61 696e 2063 6f6d 706f 6e65 6e74 732e  main components.
-000002a0: 0a0a 2a20 6060 4163 746f 7260 602e 2054  ..* ``Actor``. T
-000002b0: 6865 206f 626a 6563 7420 7468 6174 2070  he object that p
-000002c0: 6572 666f 726d 6564 2074 6865 2061 6374  erformed the act
-000002d0: 6976 6974 792e 0a2a 2060 6056 6572 6260  ivity..* ``Verb`
-000002e0: 602e 2054 6865 2076 6572 6220 7068 7261  `. The verb phra
-000002f0: 7365 2074 6861 7420 6964 656e 7469 6669  se that identifi
-00000300: 6573 2074 6865 2061 6374 696f 6e20 6f66  es the action of
-00000310: 2074 6865 2061 6374 6976 6974 792e 0a2a   the activity..*
-00000320: 2060 6041 6374 696f 6e20 4f62 6a65 6374   ``Action Object
-00000330: 6060 2e20 2a28 4f70 7469 6f6e 616c 292a  ``. *(Optional)*
-00000340: 2054 6865 206f 626a 6563 7420 6c69 6e6b   The object link
-00000350: 6564 2074 6f20 7468 6520 6163 7469 6f6e  ed to the action
-00000360: 2069 7473 656c 662e 0a2a 2060 6054 6172   itself..* ``Tar
-00000370: 6765 7460 602e 202a 284f 7074 696f 6e61  get``. *(Optiona
-00000380: 6c29 2a20 5468 6520 6f62 6a65 6374 2074  l)* The object t
-00000390: 6f20 7768 6963 6820 7468 6520 6163 7469  o which the acti
-000003a0: 7669 7479 2077 6173 2070 6572 666f 726d  vity was perform
-000003b0: 6564 2e0a 0a60 6041 6374 6f72 6060 2c20  ed...``Actor``, 
-000003c0: 6060 4163 7469 6f6e 204f 626a 6563 7460  ``Action Object`
-000003d0: 6020 616e 6420 6060 5461 7267 6574 6060  ` and ``Target``
-000003e0: 2061 7265 2060 6047 656e 6572 6963 466f   are ``GenericFo
-000003f0: 7265 6967 6e4b 6579 7360 6020 746f 2061  reignKeys`` to a
-00000400: 6e79 2061 7262 6974 7261 7279 2044 6a61  ny arbitrary Dja
-00000410: 6e67 6f20 6f62 6a65 6374 2e0a 416e 2061  ngo object..An a
-00000420: 6374 696f 6e20 6973 2061 2064 6573 6372  ction is a descr
-00000430: 6970 7469 6f6e 206f 6620 616e 2061 6374  iption of an act
-00000440: 696f 6e20 7468 6174 2077 6173 2070 6572  ion that was per
-00000450: 666f 726d 6564 2028 6060 5665 7262 6060  formed (``Verb``
-00000460: 2920 6174 2073 6f6d 6520 696e 7374 616e  ) at some instan
-00000470: 7420 696e 2074 696d 6520 6279 2073 6f6d  t in time by som
-00000480: 6520 6060 4163 746f 7260 6020 6f6e 2073  e ``Actor`` on s
-00000490: 6f6d 6520 6f70 7469 6f6e 616c 2060 6054  ome optional ``T
-000004a0: 6172 6765 7460 6020 7468 6174 2072 6573  arget`` that res
-000004b0: 756c 7473 2069 6e20 616e 2060 6041 6374  ults in an ``Act
-000004c0: 696f 6e20 4f62 6a65 6374 6060 2067 6574  ion Object`` get
-000004d0: 7469 6e67 2063 7265 6174 6564 2f75 7064  ting created/upd
-000004e0: 6174 6564 2f64 656c 6574 6564 2e0a 0a46  ated/deleted...F
-000004f0: 6f72 2065 7861 6d70 6c65 3a20 606a 7573  or example: `jus
-00000500: 7471 7569 636b 203c 6874 7470 733a 2f2f  tquick <https://
-00000510: 6769 7468 7562 2e63 6f6d 2f6a 7573 7471  github.com/justq
-00000520: 7569 636b 2f3e 605f 2060 6028 6163 746f  uick/>`_ ``(acto
-00000530: 7229 6060 202a 636c 6f73 6564 2a20 6060  r)`` *closed* ``
-00000540: 2876 6572 6229 6060 2060 6973 7375 6520  (verb)`` `issue 
-00000550: 3220 3c68 7474 7073 3a2f 2f67 6974 6875  2 <https://githu
-00000560: 622e 636f 6d2f 6a75 7374 7175 6963 6b2f  b.com/justquick/
-00000570: 646a 616e 676f 2d61 6374 6976 6974 792d  django-activity-
-00000580: 7374 7265 616d 2f69 7373 7565 732f 323e  stream/issues/2>
-00000590: 605f 2060 6028 6163 7469 6f6e 5f6f 626a  `_ ``(action_obj
-000005a0: 6563 7429 6060 206f 6e20 6061 6374 6976  ect)`` on `activ
-000005b0: 6974 792d 7374 7265 616d 203c 6874 7470  ity-stream <http
-000005c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000005d0: 7573 7471 7569 636b 2f64 6a61 6e67 6f2d  ustquick/django-
-000005e0: 6163 7469 7669 7479 2d73 7472 6561 6d2f  activity-stream/
-000005f0: 3e60 5f20 6060 2874 6172 6765 7429 6060  >`_ ``(target)``
-00000600: 2031 3220 686f 7572 7320 6167 6f0a 0a4e   12 hours ago..N
-00000610: 6f6d 656e 636c 6174 7572 6520 6f66 2074  omenclature of t
-00000620: 6869 7320 7370 6563 6966 6963 6174 696f  his specificatio
-00000630: 6e20 6973 2062 6173 6564 206f 6e20 7468  n is based on th
-00000640: 6520 4163 7469 7669 7479 2053 7472 6561  e Activity Strea
-00000650: 6d73 2053 7065 633a 2060 3c68 7474 703a  ms Spec: `<http:
-00000660: 2f2f 6163 7469 7669 7479 7374 7265 612e  //activitystrea.
-00000670: 6d73 2f73 7065 6373 2f61 746f 6d2f 312e  ms/specs/atom/1.
-00000680: 302f 3e60 5f0a 0a52 6571 7569 7265 6d65  0/>`_..Requireme
-00000690: 6e74 730a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  nts.============
-000006a0: 0a0a 2d20 5079 7468 6f6e 2033 2e35 2c20  ..- Python 3.5, 
-000006b0: 332e 362c 2033 2e37 2c20 332e 380a 2d20  3.6, 3.7, 3.8.- 
-000006c0: 446a 616e 676f 2032 2e32 2c20 332e 300a  Django 2.2, 3.0.
-000006d0: 0a49 6e73 7461 6c6c 6174 696f 6e0a 3d3d  .Installation.==
-000006e0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 496e 7374  ==========..Inst
-000006f0: 616c 6c61 7469 6f6e 2069 7320 6561 7379  allation is easy
-00000700: 2075 7369 6e67 2060 6070 6970 6060 2061   using ``pip`` a
-00000710: 6e64 2077 696c 6c20 696e 7374 616c 6c20  nd will install 
-00000720: 616c 6c20 7265 7175 6972 6564 206c 6962  all required lib
-00000730: 7261 7269 6573 2e0a 0a3a 3a0a 0a20 2020  raries...::..   
-00000740: 2024 2070 6970 2069 6e73 7461 6c6c 2064   $ pip install d
-00000750: 6a61 6e67 6f2d 6e6f 7469 6669 6361 7469  jango-notificati
-00000760: 6f6e 732d 6871 0a0a 6f72 2067 6574 2069  ons-hq..or get i
-00000770: 7420 6672 6f6d 2073 6f75 7263 650a 0a3a  t from source..:
-00000780: 3a0a 0a20 2020 2024 2067 6974 2063 6c6f  :..    $ git clo
-00000790: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
-000007a0: 622e 636f 6d2f 646a 616e 676f 2d6e 6f74  b.com/django-not
-000007b0: 6966 6963 6174 696f 6e73 2f64 6a61 6e67  ifications/djang
-000007c0: 6f2d 6e6f 7469 6669 6361 7469 6f6e 730a  o-notifications.
-000007d0: 2020 2020 2420 6364 2064 6a61 6e67 6f2d      $ cd django-
-000007e0: 6e6f 7469 6669 6361 7469 6f6e 730a 2020  notifications.  
-000007f0: 2020 2420 7079 7468 6f6e 2073 6574 7570    $ python setup
-00000800: 2e70 7920 7364 6973 740a 2020 2020 2420  .py sdist.    $ 
-00000810: 7069 7020 696e 7374 616c 6c20 6469 7374  pip install dist
-00000820: 2f64 6a61 6e67 6f2d 6e6f 7469 6669 6361  /django-notifica
-00000830: 7469 6f6e 732d 6871 2a0a 0a4e 6f74 6520  tions-hq*..Note 
-00000840: 7468 6174 2060 646a 616e 676f 2d6d 6f64  that `django-mod
-00000850: 656c 2d75 7469 6c73 203c 6874 7470 3a2f  el-utils <http:/
-00000860: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
-00000870: 2f70 7970 692f 646a 616e 676f 2d6d 6f64  /pypi/django-mod
-00000880: 656c 2d75 7469 6c73 3e60 5f20 7769 6c6c  el-utils>`_ will
-00000890: 2062 6520 696e 7374 616c 6c65 643a 2074   be installed: t
-000008a0: 6869 7320 6973 2072 6571 7569 7265 6420  his is required 
-000008b0: 666f 7220 7468 6520 7061 7373 2d74 6872  for the pass-thr
-000008c0: 6f75 6768 2051 7565 7279 5365 7420 6d61  ough QuerySet ma
-000008d0: 6e61 6765 722e 0a0a 5468 656e 2074 6f20  nager...Then to 
-000008e0: 6164 6420 7468 6520 446a 616e 676f 204e  add the Django N
-000008f0: 6f74 6966 6963 6174 696f 6e73 2074 6f20  otifications to 
-00000900: 796f 7572 2070 726f 6a65 6374 2061 6464  your project add
-00000910: 2074 6865 2061 7070 2060 606e 6f74 6966   the app ``notif
-00000920: 6963 6174 696f 6e73 6060 2074 6f20 796f  ications`` to yo
-00000930: 7572 2060 6049 4e53 5441 4c4c 4544 5f41  ur ``INSTALLED_A
-00000940: 5050 5360 6020 616e 6420 7572 6c63 6f6e  PPS`` and urlcon
-00000950: 662e 0a0a 5468 6520 6170 7020 7368 6f75  f...The app shou
-00000960: 6c64 2067 6f20 736f 6d65 7768 6572 6520  ld go somewhere 
-00000970: 6166 7465 7220 616c 6c20 7468 6520 6170  after all the ap
-00000980: 7073 2074 6861 7420 6172 6520 676f 696e  ps that are goin
-00000990: 6720 746f 2062 6520 6765 6e65 7261 7469  g to be generati
-000009a0: 6e67 206e 6f74 6966 6963 6174 696f 6e73  ng notifications
-000009b0: 206c 696b 6520 6060 646a 616e 676f 2e63   like ``django.c
-000009c0: 6f6e 7472 6962 2e61 7574 6860 600a 0a3a  ontrib.auth``..:
-000009d0: 3a0a 0a20 2020 2049 4e53 5441 4c4c 4544  :..    INSTALLED
-000009e0: 5f41 5050 5320 3d20 280a 2020 2020 2020  _APPS = (.      
-000009f0: 2020 2764 6a61 6e67 6f2e 636f 6e74 7269    'django.contri
-00000a00: 622e 6175 7468 272c 0a20 2020 2020 2020  b.auth',.       
-00000a10: 202e 2e2e 0a20 2020 2020 2020 2027 6e6f   ....        'no
-00000a20: 7469 6669 6361 7469 6f6e 7327 2c0a 2020  tifications',.  
-00000a30: 2020 2020 2020 2e2e 2e0a 2020 2020 290a        ....    ).
-00000a40: 0a41 6464 2074 6865 206e 6f74 6966 6963  .Add the notific
-00000a50: 6174 696f 6e73 2075 726c 7320 746f 2079  ations urls to y
-00000a60: 6f75 7220 7572 6c63 6f6e 663a 3a0a 0a20  our urlconf::.. 
-00000a70: 2020 2069 6d70 6f72 7420 6e6f 7469 6669     import notifi
-00000a80: 6361 7469 6f6e 732e 7572 6c73 0a0a 2020  cations.urls..  
-00000a90: 2020 7572 6c70 6174 7465 726e 7320 3d20    urlpatterns = 
-00000aa0: 5b0a 2020 2020 2020 2020 2e2e 2e0a 2020  [.        ....  
-00000ab0: 2020 2020 2020 7572 6c28 275e 696e 626f        url('^inbo
-00000ac0: 782f 6e6f 7469 6669 6361 7469 6f6e 732f  x/notifications/
-00000ad0: 272c 2069 6e63 6c75 6465 286e 6f74 6966  ', include(notif
-00000ae0: 6963 6174 696f 6e73 2e75 726c 732c 206e  ications.urls, n
-00000af0: 616d 6573 7061 6365 3d27 6e6f 7469 6669  amespace='notifi
-00000b00: 6361 7469 6f6e 7327 2929 2c0a 2020 2020  cations')),.    
-00000b10: 2020 2020 2e2e 2e0a 2020 2020 5d0a 0a54      ....    ]..T
-00000b20: 6865 206d 6574 686f 6420 6f66 2069 6e73  he method of ins
-00000b30: 7461 6c6c 696e 6720 7468 6573 6520 7572  talling these ur
-00000b40: 6c73 2c20 696d 706f 7274 696e 6720 7261  ls, importing ra
-00000b50: 7468 6572 2074 6861 6e20 7573 696e 6720  ther than using 
-00000b60: 6060 276e 6f74 6966 6963 6174 696f 6e73  ``'notifications
-00000b70: 2e75 726c 7327 6060 2c20 6973 2072 6571  .urls'``, is req
-00000b80: 7569 7265 6420 746f 2065 6e73 7572 6520  uired to ensure 
-00000b90: 7468 6174 2074 6865 2075 726c 7320 6172  that the urls ar
-00000ba0: 6520 696e 7374 616c 6c65 6420 696e 2074  e installed in t
-00000bb0: 6865 2060 606e 6f74 6966 6963 6174 696f  he ``notificatio
-00000bc0: 6e73 6060 206e 616d 6573 7061 6365 2e0a  ns`` namespace..
-00000bd0: 0a54 6f20 7275 6e20 7363 6865 6d61 206d  .To run schema m
-00000be0: 6967 7261 7469 6f6e 2c20 6578 6563 7574  igration, execut
-00000bf0: 6520 6060 7079 7468 6f6e 206d 616e 6167  e ``python manag
-00000c00: 652e 7079 206d 6967 7261 7465 206e 6f74  e.py migrate not
-00000c10: 6966 6963 6174 696f 6e73 6060 2e0a 0a47  ifications``...G
-00000c20: 656e 6572 6174 696e 6720 4e6f 7469 6669  enerating Notifi
-00000c30: 6361 7469 6f6e 730a 3d3d 3d3d 3d3d 3d3d  cations.========
-00000c40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000c50: 3d0a 0a47 656e 6572 6174 696e 6720 6e6f  =..Generating no
-00000c60: 7469 6669 6361 7469 6f6e 7320 6973 2070  tifications is p
-00000c70: 726f 6261 626c 7920 6265 7374 2064 6f6e  robably best don
-00000c80: 6520 696e 2061 2073 6570 6172 6174 6520  e in a separate 
-00000c90: 7369 676e 616c 2e0a 0a3a 3a0a 0a20 2020  signal...::..   
-00000ca0: 2066 726f 6d20 646a 616e 676f 2e64 622e   from django.db.
-00000cb0: 6d6f 6465 6c73 2e73 6967 6e61 6c73 2069  models.signals i
-00000cc0: 6d70 6f72 7420 706f 7374 5f73 6176 650a  mport post_save.
-00000cd0: 2020 2020 6672 6f6d 206e 6f74 6966 6963      from notific
-00000ce0: 6174 696f 6e73 2e73 6967 6e61 6c73 2069  ations.signals i
-00000cf0: 6d70 6f72 7420 6e6f 7469 6679 0a20 2020  mport notify.   
-00000d00: 2066 726f 6d20 6d79 6170 702e 6d6f 6465   from myapp.mode
-00000d10: 6c73 2069 6d70 6f72 7420 4d79 4d6f 6465  ls import MyMode
-00000d20: 6c0a 0a20 2020 2064 6566 206d 795f 6861  l..    def my_ha
-00000d30: 6e64 6c65 7228 7365 6e64 6572 2c20 696e  ndler(sender, in
-00000d40: 7374 616e 6365 2c20 6372 6561 7465 642c  stance, created,
-00000d50: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00000d60: 2020 2020 6e6f 7469 6679 2e73 656e 6428      notify.send(
-00000d70: 696e 7374 616e 6365 2c20 7665 7262 3d27  instance, verb='
-00000d80: 7761 7320 7361 7665 6427 290a 0a20 2020  was saved')..   
-00000d90: 2070 6f73 745f 7361 7665 2e63 6f6e 6e65   post_save.conne
-00000da0: 6374 286d 795f 6861 6e64 6c65 722c 2073  ct(my_handler, s
-00000db0: 656e 6465 723d 4d79 4d6f 6465 6c29 0a0a  ender=MyModel)..
-00000dc0: 546f 2067 656e 6572 6174 6520 616e 206e  To generate an n
-00000dd0: 6f74 6966 6963 6174 696f 6e20 616e 7977  otification anyw
-00000de0: 6865 7265 2069 6e20 796f 7572 2063 6f64  here in your cod
-00000df0: 652c 2073 696d 706c 7920 696d 706f 7274  e, simply import
-00000e00: 2074 6865 206e 6f74 6966 7920 7369 676e   the notify sign
-00000e10: 616c 2061 6e64 2073 656e 6420 6974 2077  al and send it w
-00000e20: 6974 6820 796f 7572 2061 6374 6f72 2c20  ith your actor, 
-00000e30: 7265 6369 7069 656e 742c 2061 6e64 2076  recipient, and v
-00000e40: 6572 622e 0a0a 3a3a 0a0a 2020 2020 6672  erb...::..    fr
-00000e50: 6f6d 206e 6f74 6966 6963 6174 696f 6e73  om notifications
-00000e60: 2e73 6967 6e61 6c73 2069 6d70 6f72 7420  .signals import 
-00000e70: 6e6f 7469 6679 0a0a 2020 2020 6e6f 7469  notify..    noti
-00000e80: 6679 2e73 656e 6428 7573 6572 2c20 7265  fy.send(user, re
-00000e90: 6369 7069 656e 743d 7573 6572 2c20 7665  cipient=user, ve
-00000ea0: 7262 3d27 796f 7520 7265 6163 6865 6420  rb='you reached 
-00000eb0: 6c65 7665 6c20 3130 2729 0a0a 5468 6520  level 10')..The 
-00000ec0: 636f 6d70 6c65 7465 2073 796e 7461 7820  complete syntax 
-00000ed0: 6973 2e0a 0a3a 3a0a 0a20 2020 206e 6f74  is...::..    not
-00000ee0: 6966 792e 7365 6e64 2861 6374 6f72 2c20  ify.send(actor, 
-00000ef0: 7265 6369 7069 656e 742c 2076 6572 622c  recipient, verb,
-00000f00: 2061 6374 696f 6e5f 6f62 6a65 6374 2c20   action_object, 
-00000f10: 7461 7267 6574 2c20 6c65 7665 6c2c 2064  target, level, d
-00000f20: 6573 6372 6970 7469 6f6e 2c20 7075 626c  escription, publ
-00000f30: 6963 2c20 7469 6d65 7374 616d 702c 202a  ic, timestamp, *
-00000f40: 2a6b 7761 7267 7329 0a0a 4172 6775 6d65  *kwargs)..Argume
-00000f50: 6e74 733a 0a20 2a20 2a2a 6163 746f 722a  nts:. * **actor*
-00000f60: 2a3a 2041 6e20 6f62 6a65 6374 206f 6620  *: An object of 
-00000f70: 616e 7920 7479 7065 2e20 2852 6571 7569  any type. (Requi
-00000f80: 7265 6429 204e 6f74 653a 2055 7365 202a  red) Note: Use *
-00000f90: 2a73 656e 6465 722a 2a20 696e 7374 6561  *sender** instea
-00000fa0: 6420 6f66 202a 2a61 6374 6f72 2a2a 2069  d of **actor** i
-00000fb0: 6620 796f 7520 696e 7465 6e64 2074 6f20  f you intend to 
-00000fc0: 7573 6520 6b65 7977 6f72 6420 6172 6775  use keyword argu
-00000fd0: 6d65 6e74 730a 202a 202a 2a72 6563 6970  ments. * **recip
-00000fe0: 6965 6e74 2a2a 3a20 4120 2a2a 4772 6f75  ient**: A **Grou
-00000ff0: 702a 2a20 6f72 2061 202a 2a55 7365 7220  p** or a **User 
-00001000: 5175 6572 7953 6574 2a2a 206f 7220 6120  QuerySet** or a 
-00001010: 6c69 7374 206f 6620 2a2a 5573 6572 2a2a  list of **User**
-00001020: 2e20 2852 6571 7569 7265 6429 0a20 2a20  . (Required). * 
-00001030: 2a2a 7665 7262 2a2a 3a20 416e 2073 7472  **verb**: An str
-00001040: 696e 672e 2028 5265 7175 6972 6564 290a  ing. (Required).
-00001050: 202a 202a 2a61 6374 696f 6e5f 6f62 6a65   * **action_obje
-00001060: 6374 2a2a 3a20 416e 206f 626a 6563 7420  ct**: An object 
-00001070: 6f66 2061 6e79 2074 7970 652e 2028 4f70  of any type. (Op
-00001080: 7469 6f6e 616c 290a 202a 202a 2a74 6172  tional). * **tar
-00001090: 6765 742a 2a3a 2041 6e20 6f62 6a65 6374  get**: An object
-000010a0: 206f 6620 616e 7920 7479 7065 2e20 284f   of any type. (O
-000010b0: 7074 696f 6e61 6c29 0a20 2a20 2a2a 6c65  ptional). * **le
-000010c0: 7665 6c2a 2a3a 204f 6e65 206f 6620 4e6f  vel**: One of No
-000010d0: 7469 6669 6361 7469 6f6e 2e4c 4556 454c  tification.LEVEL
-000010e0: 5320 2827 7375 6363 6573 7327 2c20 2769  S ('success', 'i
-000010f0: 6e66 6f27 2c20 2777 6172 6e69 6e67 272c  nfo', 'warning',
-00001100: 2027 6572 726f 7227 2920 2864 6566 6175   'error') (defau
-00001110: 6c74 3d69 6e66 6f29 2e20 284f 7074 696f  lt=info). (Optio
-00001120: 6e61 6c29 0a20 2a20 2a2a 6465 7363 7269  nal). * **descri
-00001130: 7074 696f 6e2a 2a3a 2041 6e20 7374 7269  ption**: An stri
-00001140: 6e67 2e20 284f 7074 696f 6e61 6c29 0a20  ng. (Optional). 
-00001150: 2a20 2a2a 7075 626c 6963 2a2a 3a20 416e  * **public**: An
-00001160: 2062 6f6f 6c65 616e 2028 6465 6661 756c   boolean (defaul
-00001170: 743d 5472 7565 292e 2028 4f70 7469 6f6e  t=True). (Option
-00001180: 616c 290a 202a 202a 2a74 696d 6573 7461  al). * **timesta
-00001190: 6d70 2a2a 3a20 416e 2074 7a69 6e66 6f20  mp**: An tzinfo 
-000011a0: 2864 6566 6175 6c74 3d74 696d 657a 6f6e  (default=timezon
-000011b0: 652e 6e6f 7728 2929 2e20 284f 7074 696f  e.now()). (Optio
-000011c0: 6e61 6c29 0a0a 4578 7472 6120 6461 7461  nal)..Extra data
-000011d0: 0a2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a59 6f75  .----------..You
-000011e0: 2063 616e 2061 7474 6163 6820 6172 6269   can attach arbi
-000011f0: 7472 6172 7920 6461 7461 2074 6f20 796f  trary data to yo
-00001200: 7572 206e 6f74 6966 6963 6174 696f 6e73  ur notifications
-00001210: 2062 7920 646f 696e 6720 7468 6520 666f   by doing the fo
-00001220: 6c6c 6f77 696e 673a 0a0a 2a20 4164 6420  llowing:..* Add 
-00001230: 746f 2079 6f75 7220 7365 7474 696e 6773  to your settings
-00001240: 2e70 793a 2060 6044 4a41 4e47 4f5f 4e4f  .py: ``DJANGO_NO
-00001250: 5449 4649 4341 5449 4f4e 535f 434f 4e46  TIFICATIONS_CONF
-00001260: 4947 203d 207b 2027 5553 455f 4a53 4f4e  IG = { 'USE_JSON
-00001270: 4649 454c 4427 3a20 5472 7565 7d60 600a  FIELD': True}``.
-00001280: 0a54 6865 6e2c 2061 6e79 2065 7874 7261  .Then, any extra
-00001290: 2061 7267 756d 656e 7473 2079 6f75 2070   arguments you p
-000012a0: 6173 7320 746f 2060 606e 6f74 6966 792e  ass to ``notify.
-000012b0: 7365 6e64 282e 2e2e 2960 6020 7769 6c6c  send(...)`` will
-000012c0: 2062 6520 6174 7461 6368 6564 2074 6f20   be attached to 
-000012d0: 7468 6520 6060 2e64 6174 6160 6020 6174  the ``.data`` at
-000012e0: 7472 6962 7574 6520 6f66 2074 6865 206e  tribute of the n
-000012f0: 6f74 6966 6963 6174 696f 6e20 6f62 6a65  otification obje
-00001300: 6374 2e0a 5468 6573 6520 7769 6c6c 2062  ct..These will b
-00001310: 6520 7365 7269 616c 6973 6564 2075 7369  e serialised usi
-00001320: 6e67 2074 6865 204a 534f 4e46 6965 6c64  ng the JSONField
-00001330: 2773 2073 6572 6961 6c69 7365 722c 2073  's serialiser, s
-00001340: 6f20 796f 7520 6d61 7920 6e65 6564 2074  o you may need t
-00001350: 6f20 7461 6b65 2074 6861 7420 696e 746f  o take that into
-00001360: 2061 6363 6f75 6e74 3a20 7573 696e 6720   account: using 
-00001370: 6f6e 6c79 206f 626a 6563 7473 2074 6861  only objects tha
-00001380: 7420 7769 6c6c 2062 6520 7365 7269 616c  t will be serial
-00001390: 6973 6564 2069 7320 6120 676f 6f64 2069  ised is a good i
-000013a0: 6465 612e 0a0a 536f 6674 2064 656c 6574  dea...Soft delet
-000013b0: 650a 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a42  e.-----------..B
-000013c0: 7920 6465 6661 756c 742c 2060 6064 656c  y default, ``del
-000013d0: 6574 652f 283f 503c 736c 7567 3e5c 642b  ete/(?P<slug>\d+
-000013e0: 292f 6060 2064 656c 6574 6573 2073 7065  )/`` deletes spe
-000013f0: 6369 6669 6564 206e 6f74 6966 6963 6174  cified notificat
-00001400: 696f 6e20 7265 636f 7264 2066 726f 6d20  ion record from 
-00001410: 4442 2e0a 596f 7520 6361 6e20 6368 616e  DB..You can chan
-00001420: 6765 2074 6869 7320 6265 6861 7669 6f75  ge this behaviou
-00001430: 7220 746f 2022 6d61 726b 2060 604e 6f74  r to "mark ``Not
-00001440: 6966 6963 6174 696f 6e2e 6465 6c65 7465  ification.delete
-00001450: 6460 6020 6669 656c 6420 6173 2060 6054  d`` field as ``T
-00001460: 7275 6560 6022 2062 793a 0a0a 2a20 4164  rue``" by:..* Ad
-00001470: 6420 746f 2079 6f75 7220 7365 7474 696e  d to your settin
-00001480: 6773 2e70 793a 2060 6044 4a41 4e47 4f5f  gs.py: ``DJANGO_
-00001490: 4e4f 5449 4649 4341 5449 4f4e 535f 434f  NOTIFICATIONS_CO
-000014a0: 4e46 4947 203d 207b 2027 534f 4654 5f44  NFIG = { 'SOFT_D
-000014b0: 454c 4554 4527 3a20 5472 7565 7d60 600a  ELETE': True}``.
-000014c0: 0a57 6974 6820 7468 6973 206f 7074 696f  .With this optio
-000014d0: 6e2c 2051 7565 7279 5365 7420 6d65 7468  n, QuerySet meth
-000014e0: 6f64 7320 6060 756e 7265 6164 6060 2061  ods ``unread`` a
-000014f0: 6e64 2060 6072 6561 6460 6020 636f 6e74  nd ``read`` cont
-00001500: 6169 6e20 6f6e 6520 6d6f 7265 2066 696c  ain one more fil
-00001510: 7465 723a 2060 6064 656c 6574 6564 3d46  ter: ``deleted=F
-00001520: 616c 7365 6060 2e0a 4d65 616e 7768 696c  alse``..Meanwhil
-00001530: 652c 2051 7565 7279 5365 7420 6d65 7468  e, QuerySet meth
-00001540: 6f64 7320 6060 6465 6c65 7465 6460 602c  ods ``deleted``,
-00001550: 2060 6061 6374 6976 6560 602c 2060 606d   ``active``, ``m
-00001560: 6172 6b5f 616c 6c5f 6173 5f64 656c 6574  ark_all_as_delet
-00001570: 6564 6060 2c20 6060 6d61 726b 5f61 6c6c  ed``, ``mark_all
-00001580: 5f61 735f 6163 7469 7665 6060 2061 7265  _as_active`` are
-00001590: 2074 7572 6e65 6420 6f6e 2e0a 5365 6520   turned on..See 
-000015a0: 6d6f 7265 2064 6574 6169 6c73 2069 6e20  more details in 
-000015b0: 5175 6572 7953 6574 206d 6574 686f 6473  QuerySet methods
-000015c0: 2073 6563 7469 6f6e 2e0a 0a41 5049 0a3d   section...API.=
-000015d0: 3d3d 3d0a 0a51 7565 7279 5365 7420 6d65  ===..QuerySet me
-000015e0: 7468 6f64 730a 2d2d 2d2d 2d2d 2d2d 2d2d  thods.----------
-000015f0: 2d2d 2d2d 2d2d 2d0a 0a55 7369 6e67 2060  -------..Using `
-00001600: 6064 6a61 6e67 6f2d 6d6f 6465 6c2d 7574  `django-model-ut
-00001610: 696c 7360 602c 2077 6520 6765 7420 7468  ils``, we get th
-00001620: 6520 6162 696c 6974 7920 746f 2061 6464  e ability to add
-00001630: 2071 7565 7279 7365 7420 6d65 7468 6f64   queryset method
-00001640: 7320 746f 206e 6f74 206f 6e6c 7920 7468  s to not only th
-00001650: 6520 6d61 6e61 6765 722c 2062 7574 2074  e manager, but t
-00001660: 6f20 616c 6c20 7175 6572 7973 6574 7320  o all querysets 
-00001670: 7468 6174 2077 696c 6c20 6265 2075 7365  that will be use
-00001680: 642c 2069 6e63 6c75 6469 6e67 2072 656c  d, including rel
-00001690: 6174 6564 206f 626a 6563 7473 2e20 5468  ated objects. Th
-000016a0: 6973 2065 6e61 626c 6573 2075 7320 746f  is enables us to
-000016b0: 2064 6f20 7468 696e 6773 206c 696b 653a   do things like:
-000016c0: 3a0a 0a20 204e 6f74 6966 6963 6174 696f  :..  Notificatio
-000016d0: 6e2e 6f62 6a65 6374 732e 756e 7265 6164  n.objects.unread
-000016e0: 2829 0a0a 7768 6963 6820 7265 7475 726e  ()..which return
-000016f0: 7320 616c 6c20 756e 7265 6164 206e 6f74  s all unread not
-00001700: 6966 6963 6174 696f 6e73 2e20 546f 2064  ifications. To d
-00001710: 6f20 7468 6973 2066 6f72 2061 2073 696e  o this for a sin
-00001720: 676c 6520 7573 6572 2c20 7765 2063 616e  gle user, we can
-00001730: 2064 6f3a 3a0a 0a20 2075 7365 7220 3d20   do::..  user = 
-00001740: 5573 6572 2e6f 626a 6563 7473 2e67 6574  User.objects.get
-00001750: 2870 6b3d 706b 290a 2020 7573 6572 2e6e  (pk=pk).  user.n
-00001760: 6f74 6966 6963 6174 696f 6e73 2e75 6e72  otifications.unr
-00001770: 6561 6428 290a 0a54 6865 7265 2061 7265  ead()..There are
-00001780: 2073 6f6d 6520 6f74 6865 7220 5175 6572   some other Quer
-00001790: 7953 6574 206d 6574 686f 6473 2c20 746f  ySet methods, to
-000017a0: 6f2e 0a0a 6060 7173 2e75 6e73 656e 7428  o...``qs.unsent(
-000017b0: 2960 600a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  )``.~~~~~~~~~~~~
-000017c0: 7e7e 7e0a 0a52 6574 7572 6e20 616c 6c20  ~~~..Return all 
-000017d0: 6f66 2074 6865 2075 6e73 656e 7420 6e6f  of the unsent no
-000017e0: 7469 6669 6361 7469 6f6e 732c 2066 696c  tifications, fil
-000017f0: 7465 7269 6e67 2074 6865 2063 7572 7265  tering the curre
-00001800: 6e74 2071 7565 7279 7365 742e 2028 656d  nt queryset. (em
-00001810: 6169 6c65 643d 4661 6c73 6529 0a0a 6060  ailed=False)..``
-00001820: 7173 2e73 656e 7428 2960 600a 7e7e 7e7e  qs.sent()``.~~~~
-00001830: 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a52 6574  ~~~~~~~~~~~..Ret
-00001840: 7572 6e20 616c 6c20 6f66 2074 6865 2073  urn all of the s
-00001850: 656e 7420 6e6f 7469 6669 6361 7469 6f6e  ent notification
-00001860: 732c 2066 696c 7465 7269 6e67 2074 6865  s, filtering the
-00001870: 2063 7572 7265 6e74 2071 7565 7279 7365   current queryse
-00001880: 742e 2028 656d 6169 6c65 643d 5472 7565  t. (emailed=True
-00001890: 290a 0a60 6071 732e 756e 7265 6164 2829  )..``qs.unread()
-000018a0: 6060 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ``.~~~~~~~~~~~~~
-000018b0: 7e7e 0a0a 5265 7475 726e 2061 6c6c 206f  ~~..Return all o
-000018c0: 6620 7468 6520 756e 7265 6164 206e 6f74  f the unread not
-000018d0: 6966 6963 6174 696f 6e73 2c20 6669 6c74  ifications, filt
-000018e0: 6572 696e 6720 7468 6520 6375 7272 656e  ering the curren
-000018f0: 7420 7175 6572 7973 6574 2e0a 5768 656e  t queryset..When
-00001900: 2060 6053 4f46 545f 4445 4c45 5445 3d54   ``SOFT_DELETE=T
-00001910: 7275 6560 602c 2074 6869 7320 6669 6c74  rue``, this filt
-00001920: 6572 2063 6f6e 7461 696e 7320 6060 6465  er contains ``de
-00001930: 6c65 7465 643d 4661 6c73 6560 602e 0a0a  leted=False``...
-00001940: 6060 7173 2e72 6561 6428 2960 600a 7e7e  ``qs.read()``.~~
-00001950: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a52  ~~~~~~~~~~~~~..R
-00001960: 6574 7572 6e20 616c 6c20 6f66 2074 6865  eturn all of the
-00001970: 2072 6561 6420 6e6f 7469 6669 6361 7469   read notificati
-00001980: 6f6e 732c 2066 696c 7465 7269 6e67 2074  ons, filtering t
-00001990: 6865 2063 7572 7265 6e74 2071 7565 7279  he current query
-000019a0: 7365 742e 0a57 6865 6e20 6060 534f 4654  set..When ``SOFT
-000019b0: 5f44 454c 4554 453d 5472 7565 6060 2c20  _DELETE=True``, 
-000019c0: 7468 6973 2066 696c 7465 7220 636f 6e74  this filter cont
-000019d0: 6169 6e73 2060 6064 656c 6574 6564 3d46  ains ``deleted=F
-000019e0: 616c 7365 6060 2e0a 0a0a 6060 7173 2e6d  alse``....``qs.m
-000019f0: 6172 6b5f 616c 6c5f 6173 5f72 6561 6428  ark_all_as_read(
-00001a00: 2960 6020 7c20 6060 7173 2e6d 6172 6b5f  )`` | ``qs.mark_
-00001a10: 616c 6c5f 6173 5f72 6561 6428 7265 6369  all_as_read(reci
-00001a20: 7069 656e 7429 6060 0a7e 7e7e 7e7e 7e7e  pient)``.~~~~~~~
-00001a30: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001a40: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001a50: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001a60: 7e7e 7e7e 7e7e 7e0a 0a4d 6172 6b20 616c  ~~~~~~~..Mark al
-00001a70: 6c20 6f66 2074 6865 2075 6e72 6561 6420  l of the unread 
-00001a80: 6e6f 7469 6669 6361 7469 6f6e 7320 696e  notifications in
-00001a90: 2074 6865 2071 7565 7279 7365 7420 286f   the queryset (o
-00001aa0: 7074 696f 6e61 6c6c 7920 616c 736f 2066  ptionally also f
-00001ab0: 696c 7465 7265 6420 6279 2060 6072 6563  iltered by ``rec
-00001ac0: 6970 6965 6e74 6060 2920 6173 2072 6561  ipient``) as rea
-00001ad0: 642e 0a0a 0a60 6071 732e 6d61 726b 5f61  d....``qs.mark_a
-00001ae0: 6c6c 5f61 735f 756e 7265 6164 2829 6060  ll_as_unread()``
-00001af0: 207c 2060 6071 732e 6d61 726b 5f61 6c6c   | ``qs.mark_all
-00001b00: 5f61 735f 756e 7265 6164 2872 6563 6970  _as_unread(recip
-00001b10: 6965 6e74 2960 600a 7e7e 7e7e 7e7e 7e7e  ient)``.~~~~~~~~
-00001b20: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001b30: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001b40: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001b50: 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 4d61 726b  ~~~~~~~~~~..Mark
-00001b60: 2061 6c6c 206f 6620 7468 6520 7265 6164   all of the read
-00001b70: 206e 6f74 6966 6963 6174 696f 6e73 2069   notifications i
-00001b80: 6e20 7468 6520 7175 6572 7973 6574 2028  n the queryset (
-00001b90: 6f70 7469 6f6e 616c 6c79 2061 6c73 6f20  optionally also 
-00001ba0: 6669 6c74 6572 6564 2062 7920 6060 7265  filtered by ``re
-00001bb0: 6369 7069 656e 7460 6029 2061 7320 756e  cipient``) as un
-00001bc0: 7265 6164 2e0a 0a60 6071 732e 6d61 726b  read...``qs.mark
-00001bd0: 5f61 735f 7365 6e74 2829 6060 207c 2060  _as_sent()`` | `
-00001be0: 6071 732e 6d61 726b 5f61 735f 7365 6e74  `qs.mark_as_sent
-00001bf0: 2872 6563 6970 6965 6e74 2960 600a 7e7e  (recipient)``.~~
-00001c00: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001c10: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001c20: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001c30: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 4d61  ~~~~~~~~~~~~..Ma
-00001c40: 726b 2061 6c6c 206f 6620 7468 6520 756e  rk all of the un
-00001c50: 7365 6e74 206e 6f74 6966 6963 6174 696f  sent notificatio
-00001c60: 6e73 2069 6e20 7468 6520 7175 6572 7973  ns in the querys
-00001c70: 6574 2028 6f70 7469 6f6e 616c 6c79 2061  et (optionally a
-00001c80: 6c73 6f20 6669 6c74 6572 6564 2062 7920  lso filtered by 
-00001c90: 6060 7265 6369 7069 656e 7460 6029 2061  ``recipient``) a
-00001ca0: 7320 7365 6e74 2e0a 0a0a 6060 7173 2e6d  s sent....``qs.m
-00001cb0: 6172 6b5f 6173 5f75 6e73 656e 7428 2960  ark_as_unsent()`
-00001cc0: 6020 7c20 6060 7173 2e6d 6172 6b5f 6173  ` | ``qs.mark_as
-00001cd0: 5f75 6e73 656e 7428 7265 6369 7069 656e  _unsent(recipien
-00001ce0: 7429 6060 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  t)``.~~~~~~~~~~~
-00001cf0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001d00: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001d10: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001d20: 7e7e 7e7e 7e7e 7e0a 0a4d 6172 6b20 616c  ~~~~~~~..Mark al
-00001d30: 6c20 6f66 2074 6865 2073 656e 7420 6e6f  l of the sent no
-00001d40: 7469 6669 6361 7469 6f6e 7320 696e 2074  tifications in t
-00001d50: 6865 2071 7565 7279 7365 7420 286f 7074  he queryset (opt
-00001d60: 696f 6e61 6c6c 7920 616c 736f 2066 696c  ionally also fil
-00001d70: 7465 7265 6420 6279 2060 6072 6563 6970  tered by ``recip
-00001d80: 6965 6e74 6060 2920 6173 2075 6e73 656e  ient``) as unsen
-00001d90: 742e 0a0a 6060 7173 2e64 656c 6574 6564  t...``qs.deleted
-00001da0: 2829 6060 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  ()``.~~~~~~~~~~~
-00001db0: 7e7e 7e7e 7e0a 0a52 6574 7572 6e20 616c  ~~~~~..Return al
-00001dc0: 6c20 6e6f 7469 6669 6361 7469 6f6e 7320  l notifications 
-00001dd0: 7468 6174 2068 6176 6520 6060 6465 6c65  that have ``dele
-00001de0: 7465 643d 5472 7565 6060 2c20 6669 6c74  ted=True``, filt
-00001df0: 6572 696e 6720 7468 6520 6375 7272 656e  ering the curren
-00001e00: 7420 7175 6572 7973 6574 2e0a 4d75 7374  t queryset..Must
-00001e10: 2062 6520 7573 6564 2077 6974 6820 6060   be used with ``
-00001e20: 534f 4654 5f44 454c 4554 453d 5472 7565  SOFT_DELETE=True
-00001e30: 6060 2e0a 0a60 6071 732e 6163 7469 7665  ``...``qs.active
-00001e40: 2829 6060 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  ()``.~~~~~~~~~~~
-00001e50: 7e7e 7e7e 0a0a 5265 7475 726e 2061 6c6c  ~~~~..Return all
-00001e60: 206e 6f74 6966 6963 6174 696f 6e73 2074   notifications t
-00001e70: 6861 7420 6861 7665 2060 6064 656c 6574  hat have ``delet
-00001e80: 6564 3d46 616c 7365 6060 2c20 6669 6c74  ed=False``, filt
-00001e90: 6572 696e 6720 7468 6520 6375 7272 656e  ering the curren
-00001ea0: 7420 7175 6572 7973 6574 2e0a 4d75 7374  t queryset..Must
-00001eb0: 2062 6520 7573 6564 2077 6974 6820 6060   be used with ``
-00001ec0: 4445 4c45 5445 3d54 7275 6560 602e 0a0a  DELETE=True``...
-00001ed0: 6060 7173 2e6d 6172 6b5f 616c 6c5f 6173  ``qs.mark_all_as
-00001ee0: 5f64 656c 6574 6564 2829 6060 207c 2060  _deleted()`` | `
-00001ef0: 6071 732e 6d61 726b 5f61 6c6c 5f61 735f  `qs.mark_all_as_
-00001f00: 6465 6c65 7465 6428 7265 6369 7069 656e  deleted(recipien
-00001f10: 7429 6060 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  t)``.~~~~~~~~~~~
-00001f20: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001f30: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001f40: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001f50: 7e7e 7e7e 7e7e 7e7e 7e0a 0a4d 6172 6b20  ~~~~~~~~~..Mark 
-00001f60: 616c 6c20 6e6f 7469 6669 6361 7469 6f6e  all notification
-00001f70: 7320 696e 2074 6865 2071 7565 7279 7365  s in the queryse
-00001f80: 7420 286f 7074 696f 6e61 6c6c 7920 616c  t (optionally al
-00001f90: 736f 2066 696c 7465 7265 6420 6279 2060  so filtered by `
-00001fa0: 6072 6563 6970 6965 6e74 6060 2920 6173  `recipient``) as
-00001fb0: 2060 6064 656c 6574 6564 3d54 7275 6560   ``deleted=True`
-00001fc0: 602e 0a4d 7573 7420 6265 2075 7365 6420  `..Must be used 
-00001fd0: 7769 7468 2060 6044 454c 4554 453d 5472  with ``DELETE=Tr
-00001fe0: 7565 6060 2e0a 0a60 6071 732e 6d61 726b  ue``...``qs.mark
-00001ff0: 5f61 6c6c 5f61 735f 6163 7469 7665 2829  _all_as_active()
-00002000: 6060 207c 2060 6071 732e 6d61 726b 5f61  `` | ``qs.mark_a
-00002010: 6c6c 5f61 735f 6163 7469 7665 2872 6563  ll_as_active(rec
-00002020: 6970 6965 6e74 2960 600a 7e7e 7e7e 7e7e  ipient)``.~~~~~~
-00002030: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00002040: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00002050: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00002060: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 4d61  ~~~~~~~~~~~~..Ma
-00002070: 726b 2061 6c6c 206e 6f74 6966 6963 6174  rk all notificat
-00002080: 696f 6e73 2069 6e20 7468 6520 7175 6572  ions in the quer
-00002090: 7973 6574 2028 6f70 7469 6f6e 616c 6c79  yset (optionally
-000020a0: 2061 6c73 6f20 6669 6c74 6572 6564 2062   also filtered b
-000020b0: 7920 6060 7265 6369 7069 656e 7460 6029  y ``recipient``)
-000020c0: 2061 7320 6060 6465 6c65 7465 643d 4661   as ``deleted=Fa
-000020d0: 6c73 6560 602e 0a4d 7573 7420 6265 2075  lse``..Must be u
-000020e0: 7365 6420 7769 7468 2060 6053 4f46 545f  sed with ``SOFT_
-000020f0: 4445 4c45 5445 3d54 7275 6560 602e 0a0a  DELETE=True``...
-00002100: 0a4d 6f64 656c 206d 6574 686f 6473 0a2d  .Model methods.-
-00002110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 6060  ------------..``
-00002120: 6f62 6a2e 7469 6d65 7369 6e63 6528 5b64  obj.timesince([d
-00002130: 6174 6574 696d 655d 2960 600a 7e7e 7e7e  atetime])``.~~~~
-00002140: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00002150: 7e7e 7e7e 7e7e 7e7e 7e0a 0a41 2077 7261  ~~~~~~~~~..A wra
-00002160: 7070 6572 2066 6f72 2044 6a61 6e67 6f27  pper for Django'
-00002170: 7320 6060 7469 6d65 7369 6e63 6560 6020  s ``timesince`` 
-00002180: 6675 6e63 7469 6f6e 2e0a 0a60 606f 626a  function...``obj
-00002190: 2e6d 6172 6b5f 6173 5f72 6561 6428 2960  .mark_as_read()`
-000021a0: 600a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  `.~~~~~~~~~~~~~~
-000021b0: 7e7e 7e7e 7e7e 7e7e 0a0a 4d61 726b 2074  ~~~~~~~~..Mark t
-000021c0: 6865 2063 7572 7265 6e74 206f 626a 6563  he current objec
-000021d0: 7420 6173 2072 6561 642e 0a0a 0a54 656d  t as read....Tem
-000021e0: 706c 6174 6520 7461 6773 0a2d 2d2d 2d2d  plate tags.-----
-000021f0: 2d2d 2d2d 2d2d 2d2d 0a0a 5075 7420 607b  --------..Put `{
-00002200: 2520 6c6f 6164 206e 6f74 6966 6963 6174  % load notificat
-00002210: 696f 6e73 5f74 6167 7320 257d 6020 696e  ions_tags %}` in
-00002220: 2074 6865 2074 656d 706c 6174 6520 6265   the template be
-00002230: 666f 7265 2079 6f75 2061 6374 7561 6c6c  fore you actuall
-00002240: 7920 7573 6520 6e6f 7469 6669 6361 7469  y use notificati
-00002250: 6f6e 2074 6167 732e 0a0a 0a60 606e 6f74  on tags....``not
-00002260: 6966 6963 6174 696f 6e73 5f75 6e72 6561  ifications_unrea
-00002270: 6460 600a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  d``.~~~~~~~~~~~~
-00002280: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 3a3a  ~~~~~~~~~~~~..::
-00002290: 0a0a 2020 2020 7b25 206e 6f74 6966 6963  ..    {% notific
-000022a0: 6174 696f 6e73 5f75 6e72 6561 6420 257d  ations_unread %}
-000022b0: 0a0a 4769 7665 2074 6865 206e 756d 6265  ..Give the numbe
-000022c0: 7220 6f66 2075 6e72 6561 6420 6e6f 7469  r of unread noti
-000022d0: 6669 6361 7469 6f6e 7320 666f 7220 6120  fications for a 
-000022e0: 7573 6572 2c20 6f72 206e 6f74 6869 6e67  user, or nothing
-000022f0: 2028 616e 2065 6d70 7479 2073 7472 696e   (an empty strin
-00002300: 6729 2066 6f72 2061 6e20 616e 6f6e 796d  g) for an anonym
-00002310: 6f75 7320 7573 6572 2e0a 0a53 746f 7269  ous user...Stori
-00002320: 6e67 2074 6865 2063 6f75 6e74 2069 6e20  ng the count in 
-00002330: 6120 7661 7269 6162 6c65 2066 6f72 2066  a variable for f
-00002340: 7572 7468 6572 2070 726f 6365 7373 696e  urther processin
-00002350: 6720 6973 2061 6476 6973 6564 2c20 7375  g is advised, su
-00002360: 6368 2061 733a 3a0a 0a20 2020 207b 2520  ch as::..    {% 
-00002370: 6e6f 7469 6669 6361 7469 6f6e 735f 756e  notifications_un
-00002380: 7265 6164 2061 7320 756e 7265 6164 5f63  read as unread_c
-00002390: 6f75 6e74 2025 7d0a 2020 2020 2e2e 2e0a  ount %}.    ....
-000023a0: 2020 2020 7b25 2069 6620 756e 7265 6164      {% if unread
-000023b0: 5f63 6f75 6e74 2025 7d0a 2020 2020 2020  _count %}.      
-000023c0: 2020 596f 7520 6861 7665 203c 7374 726f    You have <stro
-000023d0: 6e67 3e7b 7b20 756e 7265 6164 5f63 6f75  ng>{{ unread_cou
-000023e0: 6e74 207d 7d3c 2f73 7472 6f6e 673e 2075  nt }}</strong> u
-000023f0: 6e72 6561 6420 6e6f 7469 6669 6361 7469  nread notificati
-00002400: 6f6e 732e 0a20 2020 207b 2520 656e 6469  ons..    {% endi
-00002410: 6620 257d 0a0a 4c69 7665 2d75 7064 6174  f %}..Live-updat
-00002420: 6572 2041 5049 0a3d 3d3d 3d3d 3d3d 3d3d  er API.=========
-00002430: 3d3d 3d3d 3d3d 3d0a 0a54 6f20 656e 7375  =======..To ensu
-00002440: 7265 2075 7365 7273 2061 6c77 6179 7320  re users always 
-00002450: 6861 7665 2074 6865 206d 6f73 7420 7570  have the most up
-00002460: 2d74 6f2d 6461 7465 206e 6f74 6966 6963  -to-date notific
-00002470: 6174 696f 6e73 2c20 6064 6a61 6e67 6f2d  ations, `django-
-00002480: 6e6f 7469 6669 6361 7469 6f6e 7360 2069  notifications` i
-00002490: 6e63 6c75 6465 7320 6120 7369 6d70 6c65  ncludes a simple
-000024a0: 206a 6176 6173 6372 6970 7420 4150 490a   javascript API.
-000024b0: 666f 7220 7570 6461 7469 6e67 2073 7065  for updating spe
-000024c0: 6369 6669 6320 6669 656c 6473 2077 6974  cific fields wit
-000024d0: 6869 6e20 6120 646a 616e 676f 2074 656d  hin a django tem
-000024e0: 706c 6174 652e 0a0a 5468 6572 6520 6172  plate...There ar
-000024f0: 6520 7477 6f20 706f 7373 6962 6c65 2041  e two possible A
-00002500: 5049 2063 616c 6c73 2074 6861 7420 6361  PI calls that ca
-00002510: 6e20 6265 206d 6164 653a 0a0a 312e 2060  n be made:..1. `
-00002520: 6061 7069 2f75 6e72 6561 645f 636f 756e  `api/unread_coun
-00002530: 742f 6060 2074 6861 7420 7265 7475 726e  t/`` that return
-00002540: 7320 6120 6a61 7661 7363 7269 7074 206f  s a javascript o
-00002550: 626a 6563 7420 7769 7468 2031 206b 6579  bject with 1 key
-00002560: 3a20 6060 756e 7265 6164 5f63 6f75 6e74  : ``unread_count
-00002570: 6060 2065 673a 3a0a 0a20 2020 2020 2020  `` eg::..       
-00002580: 207b 2275 6e72 6561 645f 636f 756e 7422   {"unread_count"
-00002590: 3a31 7d0a 0a23 2e20 6060 6170 692f 756e  :1}..#. ``api/un
-000025a0: 7265 6164 5f6c 6973 742f 6060 2074 6861  read_list/`` tha
-000025b0: 7420 7265 7475 726e 7320 6120 6a61 7661  t returns a java
-000025c0: 7363 7269 7074 206f 626a 6563 7420 7769  script object wi
-000025d0: 7468 2032 206b 6579 733a 2060 756e 7265  th 2 keys: `unre
-000025e0: 6164 5f63 6f75 6e74 6020 616e 6420 6075  ad_count` and `u
-000025f0: 6e72 6561 645f 6c69 7374 6020 6567 3a3a  nread_list` eg::
-00002600: 0a0a 2020 2020 2020 2020 7b0a 2020 2020  ..        {.    
-00002610: 2020 2020 2022 756e 7265 6164 5f63 6f75       "unread_cou
-00002620: 6e74 223a 312c 0a20 2020 2020 2020 2020  nt":1,.         
-00002630: 2275 6e72 6561 645f 6c69 7374 223a 5b2d  "unread_list":[-
-00002640: 2d6c 6973 7420 6f66 206a 736f 6e20 7265  -list of json re
-00002650: 7072 6573 656e 7461 7469 6f6e 7320 6f66  presentations of
-00002660: 206e 6f74 6966 6963 6174 696f 6e73 2d2d   notifications--
-00002670: 5d0a 2020 2020 2020 2020 7d0a 0a20 2020  ].        }..   
-00002680: 5265 7072 6573 656e 7461 7469 6f6e 7320  Representations 
-00002690: 6f66 206e 6f74 6966 6963 6174 696f 6e73  of notifications
-000026a0: 2061 7265 2062 6173 6564 206f 6e20 7468   are based on th
-000026b0: 6520 646a 616e 676f 206d 6574 686f 643a  e django method:
-000026c0: 2060 606d 6f64 656c 5f74 6f5f 6469 6374   ``model_to_dict
-000026d0: 6060 0a0a 2020 2051 7565 7279 2073 7472  ``..   Query str
-000026e0: 696e 6720 6172 6775 6d65 6e74 733a 0a0a  ing arguments:..
-000026f0: 2020 202d 202a 2a6d 6178 2a2a 202d 206d     - **max** - m
-00002700: 6178 696d 756d 206c 656e 6774 6820 6f66  aximum length of
-00002710: 2075 6e72 6561 6420 6c69 7374 2e0a 2020   unread list..  
-00002720: 202d 202a 2a6d 6172 6b5f 6173 5f72 6561   - **mark_as_rea
-00002730: 642a 2a20 2d20 6d61 726b 206e 6f74 6966  d** - mark notif
-00002740: 6963 6174 696f 6e20 696e 206c 6973 7420  ication in list 
-00002750: 6173 2072 6561 642e 0a0a 2020 2046 6f72  as read...   For
-00002760: 2065 7861 6d70 6c65 2c20 6765 7420 6060   example, get ``
-00002770: 6170 692f 756e 7265 6164 5f6c 6973 742f  api/unread_list/
-00002780: 3f6d 6178 3d33 266d 6172 6b5f 6173 5f72  ?max=3&mark_as_r
-00002790: 6561 643d 7472 7565 6060 2072 6574 7572  ead=true`` retur
-000027a0: 6e73 2033 206e 6f74 6966 6963 6174 696f  ns 3 notificatio
-000027b0: 6e73 2061 6e64 206d 6172 6b20 7468 656d  ns and mark them
-000027c0: 2072 6561 6420 2872 656d 6f76 6520 6672   read (remove fr
-000027d0: 6f6d 206c 6973 7420 6f6e 206e 6578 7420  om list on next 
-000027e0: 7265 7175 6573 7429 2e0a 0a0a 486f 7720  request)....How 
-000027f0: 746f 2075 7365 3a0a 2d2d 2d2d 2d2d 2d2d  to use:.--------
-00002800: 2d2d 2d0a 0a31 2e20 5075 7420 6060 7b25  ---..1. Put ``{%
-00002810: 206c 6f61 6420 6e6f 7469 6669 6361 7469   load notificati
-00002820: 6f6e 735f 7461 6773 2025 7d60 6020 696e  ons_tags %}`` in
-00002830: 2074 6865 2074 656d 706c 6174 6520 6265   the template be
-00002840: 666f 7265 2079 6f75 2061 6374 7561 6c6c  fore you actuall
-00002850: 7920 7573 6520 6e6f 7469 6669 6361 7469  y use notificati
-00002860: 6f6e 2074 6167 732e 0a32 2e20 496e 2074  on tags..2. In t
-00002870: 6865 2061 7265 6120 7768 6572 6520 796f  he area where yo
-00002880: 7520 6172 6520 6c6f 6164 696e 6720 6a61  u are loading ja
-00002890: 7661 7363 7269 7074 2072 6573 6f75 7263  vascript resourc
-000028a0: 6573 2061 6464 2074 6865 2066 6f6c 6c6f  es add the follo
-000028b0: 7769 6e67 2074 6167 7320 696e 2074 6865  wing tags in the
-000028c0: 206f 7264 6572 2062 656c 6f77 3a3a 0a0a   order below::..
-000028d0: 2020 2020 2020 203c 7363 7269 7074 2073         <script s
-000028e0: 7263 3d22 7b25 2073 7461 7469 6320 276e  rc="{% static 'n
-000028f0: 6f74 6966 6963 6174 696f 6e73 2f6e 6f74  otifications/not
-00002900: 6966 792e 6a73 2720 257d 2220 7479 7065  ify.js' %}" type
-00002910: 3d22 7465 7874 2f6a 6176 6173 6372 6970  ="text/javascrip
-00002920: 7422 3e3c 2f73 6372 6970 743e 0a20 2020  t"></script>.   
-00002930: 2020 2020 7b25 2072 6567 6973 7465 725f      {% register_
-00002940: 6e6f 7469 6679 5f63 616c 6c62 6163 6b73  notify_callbacks
-00002950: 2063 616c 6c62 6163 6b73 3d27 6669 6c6c   callbacks='fill
-00002960: 5f6e 6f74 6966 6963 6174 696f 6e5f 6c69  _notification_li
-00002970: 7374 2c66 696c 6c5f 6e6f 7469 6669 6361  st,fill_notifica
-00002980: 7469 6f6e 5f62 6164 6765 2720 257d 0a0a  tion_badge' %}..
-00002990: 2020 2060 6072 6567 6973 7465 725f 6e6f     ``register_no
-000029a0: 7469 6679 5f63 616c 6c62 6163 6b73 6060  tify_callbacks``
-000029b0: 2074 616b 6573 2074 6865 2066 6f6c 6c6f   takes the follo
-000029c0: 7769 6e67 2061 7267 756d 656e 7473 3a0a  wing arguments:.
-000029d0: 0a20 2020 312e 2060 6062 6164 6765 5f63  .   1. ``badge_c
-000029e0: 6c61 7373 6060 2028 6465 6661 756c 7420  lass`` (default 
-000029f0: 6060 6c69 7665 5f6e 6f74 6966 795f 6261  ``live_notify_ba
-00002a00: 6467 6560 6029 202d 2054 6865 2069 6465  dge``) - The ide
-00002a10: 6e74 6966 6965 7220 6063 6c61 7373 6020  ntifier `class` 
-00002a20: 6f66 2074 6865 2065 6c65 6d65 6e74 2074  of the element t
-00002a30: 6f20 7368 6f77 2074 6865 2075 6e72 6561  o show the unrea
-00002a40: 6420 636f 756e 742c 2074 6861 7420 7769  d count, that wi
-00002a50: 6c6c 2062 6520 7065 7269 6f64 6963 616c  ll be periodical
-00002a60: 6c79 2075 7064 6174 6564 2e0a 2020 2023  ly updated..   #
-00002a70: 2e20 6060 6d65 6e75 5f63 6c61 7373 6060  . ``menu_class``
-00002a80: 2028 6465 6661 756c 7420 6060 6c69 7665   (default ``live
-00002a90: 5f6e 6f74 6966 795f 6c69 7374 6060 2920  _notify_list``) 
-00002aa0: 2d20 5468 6520 6964 656e 7469 6669 6572  - The identifier
-00002ab0: 2060 636c 6173 7360 206f 6620 7468 6520   `class` of the 
-00002ac0: 656c 656d 656e 7420 746f 2069 6e73 6572  element to inser
-00002ad0: 7420 6120 6c69 7374 206f 6620 756e 7265  t a list of unre
-00002ae0: 6164 2069 7465 6d73 2c20 7468 6174 2077  ad items, that w
-00002af0: 696c 6c20 6265 2070 6572 696f 6469 6361  ill be periodica
-00002b00: 6c6c 7920 7570 6461 7465 642e 0a20 2020  lly updated..   
-00002b10: 232e 2060 6072 6566 7265 7368 5f70 6572  #. ``refresh_per
-00002b20: 696f 6460 6020 2864 6566 6175 6c74 2060  iod`` (default `
-00002b30: 6031 3560 6029 202d 2048 6f77 206f 6674  `15``) - How oft
-00002b40: 656e 2074 6f20 6665 7463 6820 756e 7265  en to fetch unre
-00002b50: 6164 2069 7465 6d73 2066 726f 6d20 7468  ad items from th
-00002b60: 6520 7365 7276 6572 2028 696e 7465 6765  e server (intege
-00002b70: 7220 696e 2073 6563 6f6e 6473 292e 0a20  r in seconds).. 
-00002b80: 2020 232e 2060 6066 6574 6368 6060 2028    #. ``fetch`` (
-00002b90: 6465 6661 756c 7420 6060 3560 6029 202d  default ``5``) -
-00002ba0: 2048 6f77 206d 616e 7920 6e6f 7469 6669   How many notifi
-00002bb0: 6361 7469 6f6e 7320 746f 2066 6574 6368  cations to fetch
-00002bc0: 2065 6163 6820 7469 6d65 2e0a 2020 2023   each time..   #
-00002bd0: 2e20 6060 6361 6c6c 6261 636b 7360 6020  . ``callbacks`` 
-00002be0: 2864 6566 6175 6c74 2060 603c 656d 7074  (default ``<empt
-00002bf0: 7920 7374 7269 6e67 3e60 6029 202d 2041  y string>``) - A
-00002c00: 2063 6f6d 6d61 2d73 6570 6172 6174 6564   comma-separated
-00002c10: 206c 6973 7420 6f66 206a 6176 6173 6372   list of javascr
-00002c20: 6970 7420 6675 6e63 7469 6f6e 7320 746f  ipt functions to
-00002c30: 2063 616c 6c20 6561 6368 2070 6572 696f   call each perio
-00002c40: 642e 0a20 2020 232e 2060 6061 7069 5f6e  d..   #. ``api_n
-00002c50: 616d 6560 6020 2864 6566 6175 6c74 2060  ame`` (default `
-00002c60: 606c 6973 7460 6029 202d 2054 6865 206e  `list``) - The n
-00002c70: 616d 6520 6f66 2074 6865 2041 5049 2074  ame of the API t
-00002c80: 6f20 6361 6c6c 2028 7468 6973 2063 616e  o call (this can
-00002c90: 2062 6520 6569 7468 6572 2060 606c 6973   be either ``lis
-00002ca0: 7460 6020 6f72 2060 6063 6f75 6e74 6060  t`` or ``count``
-00002cb0: 292e 0a0a 332e 2054 6f20 696e 7365 7274  )...3. To insert
-00002cc0: 2061 206c 6976 652d 7570 6461 7469 6e67   a live-updating
-00002cd0: 2075 6e72 6561 6420 636f 756e 742c 2075   unread count, u
-00002ce0: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
-00002cf0: 2074 656d 706c 6174 653a 3a0a 0a20 2020   template::..   
-00002d00: 2020 2020 7b25 206c 6976 655f 6e6f 7469      {% live_noti
-00002d10: 6679 5f62 6164 6765 2025 7d0a 0a20 2020  fy_badge %}..   
-00002d20: 6060 6c69 7665 5f6e 6f74 6966 795f 6261  ``live_notify_ba
-00002d30: 6467 6560 6020 7461 6b65 7320 7468 6520  dge`` takes the 
-00002d40: 666f 6c6c 6f77 696e 6720 6172 6775 6d65  following argume
-00002d50: 6e74 733a 0a0a 2020 2031 2e20 6060 6261  nts:..   1. ``ba
-00002d60: 6467 655f 636c 6173 7360 6020 2864 6566  dge_class`` (def
-00002d70: 6175 6c74 2060 606c 6976 655f 6e6f 7469  ault ``live_noti
-00002d80: 6679 5f62 6164 6765 6060 2920 2d20 5468  fy_badge``) - Th
-00002d90: 6520 6964 656e 7469 6669 6572 2060 6063  e identifier ``c
-00002da0: 6c61 7373 6060 2066 6f72 2074 6865 2060  lass`` for the `
-00002db0: 603c 7370 616e 3e60 6020 656c 656d 656e  `<span>`` elemen
-00002dc0: 7420 7468 6174 2077 696c 6c20 6265 2063  t that will be c
-00002dd0: 7265 6174 6564 2074 6f20 7368 6f77 2074  reated to show t
-00002de0: 6865 2075 6e72 6561 6420 636f 756e 742e  he unread count.
-00002df0: 0a0a 342e 2054 6f20 696e 7365 7274 2061  ..4. To insert a
-00002e00: 206c 6976 652d 7570 6461 7469 6e67 2075   live-updating u
-00002e10: 6e72 6561 6420 6c69 7374 2c20 7573 6520  nread list, use 
-00002e20: 7468 6520 666f 6c6c 6f77 696e 6720 7465  the following te
-00002e30: 6d70 6c61 7465 3a3a 0a0a 2020 2020 2020  mplate::..      
-00002e40: 207b 2520 6c69 7665 5f6e 6f74 6966 795f   {% live_notify_
-00002e50: 6c69 7374 2025 7d0a 0a20 2020 6060 6c69  list %}..   ``li
-00002e60: 7665 5f6e 6f74 6966 795f 6c69 7374 6060  ve_notify_list``
-00002e70: 2074 616b 6573 2074 6865 2066 6f6c 6c6f   takes the follo
-00002e80: 7769 6e67 2061 7267 756d 656e 7473 3a0a  wing arguments:.
-00002e90: 0a20 2020 312e 2060 606c 6973 745f 636c  .   1. ``list_cl
-00002ea0: 6173 7360 6020 2864 6566 6175 6c74 2060  ass`` (default `
-00002eb0: 606c 6976 655f 6e6f 7469 6679 5f6c 6973  `live_notify_lis
-00002ec0: 7460 6029 202d 2054 6865 2069 6465 6e74  t``) - The ident
-00002ed0: 6966 6965 7220 6060 636c 6173 7360 6020  ifier ``class`` 
-00002ee0: 666f 7220 7468 6520 6060 3c75 6c3e 6060  for the ``<ul>``
-00002ef0: 2065 6c65 6d65 6e74 2074 6861 7420 7769   element that wi
-00002f00: 6c6c 2062 6520 6372 6561 7465 6420 746f  ll be created to
-00002f10: 2069 6e73 6572 7420 7468 6520 6c69 7374   insert the list
-00002f20: 206f 6620 6e6f 7469 6669 6361 7469 6f6e   of notification
-00002f30: 7320 696e 746f 2e0a 0a55 7369 6e67 2074  s into...Using t
-00002f40: 6865 206c 6976 652d 7570 6461 7465 7220  he live-updater 
-00002f50: 7769 7468 2062 6f6f 7473 7472 6170 0a2d  with bootstrap.-
-00002f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002f80: 2d2d 2d2d 0a0a 5468 6520 4c69 7665 2d75  ----..The Live-u
-00002f90: 7064 6174 6572 2063 616e 2062 6520 696e  pdater can be in
-00002fa0: 636f 7270 6f72 6174 6564 2069 6e74 6f20  corporated into 
-00002fb0: 626f 6f74 7374 7261 7020 7769 7468 206d  bootstrap with m
-00002fc0: 696e 696d 616c 2063 6f64 652e 0a0a 546f  inimal code...To
-00002fd0: 2063 7265 6174 6520 6120 6c69 7665 2d75   create a live-u
-00002fe0: 7064 6174 696e 6720 626f 6f74 7374 7261  pdating bootstra
-00002ff0: 7020 6261 6467 6520 636f 6e74 6169 6e69  p badge containi
-00003000: 6e67 2074 6865 2075 6e72 6561 6420 636f  ng the unread co
-00003010: 756e 742c 2073 696d 706c 7920 7573 6520  unt, simply use 
-00003020: 7468 6520 7465 6d70 6c61 7465 2074 6167  the template tag
-00003030: 3a3a 0a0a 2020 2020 7b25 206c 6976 655f  ::..    {% live_
-00003040: 6e6f 7469 6679 5f62 6164 6765 2062 6164  notify_badge bad
-00003050: 6765 5f63 6c61 7373 3d22 6261 6467 6522  ge_class="badge"
-00003060: 2025 7d0a 0a54 6f20 6372 6561 7465 2061   %}..To create a
-00003070: 206c 6976 652d 7570 6461 7469 6e67 2062   live-updating b
-00003080: 6f6f 7473 7472 6170 2064 726f 7064 6f77  ootstrap dropdow
-00003090: 6e20 6d65 6e75 2063 6f6e 7461 696e 696e  n menu containin
-000030a0: 6720 6120 7365 6c65 6374 696f 6e20 6f66  g a selection of
-000030b0: 2072 6563 656e 7420 756e 7265 6164 206e   recent unread n
-000030c0: 6f74 6966 6963 6174 696f 6e73 2c20 7369  otifications, si
-000030d0: 6d70 6c79 2075 7365 2074 6865 2074 656d  mply use the tem
-000030e0: 706c 6174 6520 7461 673a 3a0a 0a20 2020  plate tag::..   
-000030f0: 207b 2520 6c69 7665 5f6e 6f74 6966 795f   {% live_notify_
-00003100: 6c69 7374 206c 6973 745f 636c 6173 733d  list list_class=
-00003110: 2264 726f 7064 6f77 6e2d 6d65 6e75 2220  "dropdown-menu" 
-00003120: 257d 0a0a 4375 7374 6f6d 6973 696e 6720  %}..Customising 
-00003130: 7468 6520 6469 7370 6c61 7920 6f66 206e  the display of n
-00003140: 6f74 6966 6963 6174 696f 6e73 2075 7369  otifications usi
-00003150: 6e67 206a 6176 6173 6372 6970 7420 6361  ng javascript ca
-00003160: 6c6c 6261 636b 730a 2d2d 2d2d 2d2d 2d2d  llbacks.--------
-00003170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000031a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a57 6869  -----------..Whi
-000031b0: 6c65 2074 6865 206c 6976 6520 6e6f 7469  le the live noti
-000031c0: 6669 6572 2066 6f72 2075 6e72 6561 6420  fier for unread 
-000031d0: 636f 756e 7473 2073 686f 756c 6420 7375  counts should su
-000031e0: 6974 206d 6f73 7420 7573 6520 6361 7365  it most use case
-000031f0: 732c 2075 7365 7273 206d 6179 2077 6973  s, users may wis
-00003200: 6820 746f 2061 6c74 6572 2068 6f77 0a75  h to alter how.u
-00003210: 6e72 6561 6420 6e6f 7469 6669 6361 7469  nread notificati
-00003220: 6f6e 7320 6172 6520 7368 6f77 6e2e 0a0a  ons are shown...
-00003230: 5468 6520 6060 6361 6c6c 6261 636b 7360  The ``callbacks`
-00003240: 6020 6172 6775 6d65 6e74 206f 6620 7468  ` argument of th
-00003250: 6520 6060 7265 6769 7374 6572 5f6e 6f74  e ``register_not
-00003260: 6966 795f 6361 6c6c 6261 636b 7360 6020  ify_callbacks`` 
-00003270: 6469 6374 6174 6573 2077 6869 6368 206a  dictates which j
-00003280: 6176 6173 6372 6970 7420 6675 6e63 7469  avascript functi
-00003290: 6f6e 7320 6172 6520 6361 6c6c 6564 2077  ons are called w
-000032a0: 6865 6e0a 7468 6520 756e 7265 6164 2061  hen.the unread a
-000032b0: 7069 2063 616c 6c20 6973 206d 6164 652e  pi call is made.
-000032c0: 0a0a 546f 2061 6464 2061 2063 7573 746f  ..To add a custo
-000032d0: 6d20 6a61 7661 7363 7269 7074 2063 616c  m javascript cal
-000032e0: 6c62 6163 6b2c 2073 696d 706c 7920 6164  lback, simply ad
-000032f0: 6420 7468 6973 2074 6f20 7468 6520 6c69  d this to the li
-00003300: 7374 2c20 6c69 6b65 2073 6f3a 3a0a 0a20  st, like so::.. 
-00003310: 2020 2020 2020 7b25 2072 6567 6973 7465        {% registe
-00003320: 725f 6e6f 7469 6679 5f63 616c 6c62 6163  r_notify_callbac
-00003330: 6b73 2063 616c 6c62 6163 6b73 3d27 6669  ks callbacks='fi
-00003340: 6c6c 5f6e 6f74 6966 6963 6174 696f 6e5f  ll_notification_
-00003350: 6261 6467 652c 6d79 5f73 7065 6369 616c  badge,my_special
-00003360: 5f6e 6f74 6966 6963 6174 696f 6e5f 6361  _notification_ca
-00003370: 6c6c 6261 636b 2720 257d 0a0a 5468 6520  llback' %}..The 
-00003380: 6162 6f76 6520 776f 756c 6420 6361 7573  above would caus
-00003390: 6520 7468 6520 6361 6c6c 6261 636b 2074  e the callback t
-000033a0: 6f20 7570 6461 7465 2074 6865 2075 6e72  o update the unr
-000033b0: 6561 6420 636f 756e 7420 6261 6467 652c  ead count badge,
-000033c0: 2061 6e64 2077 6f75 6c64 2063 616c 6c20   and would call 
-000033d0: 7468 6520 6375 7374 6f6d 2066 756e 6374  the custom funct
-000033e0: 696f 6e20 606d 795f 7370 6563 6961 6c5f  ion `my_special_
-000033f0: 6e6f 7469 6669 6361 7469 6f6e 5f63 616c  notification_cal
-00003400: 6c62 6163 6b60 2e0a 416c 6c20 6361 6c6c  lback`..All call
-00003410: 6261 636b 2066 756e 6374 696f 6e73 2061  back functions a
-00003420: 7265 2070 6173 7365 6420 6120 7369 6e67  re passed a sing
-00003430: 6c65 2061 7267 756d 656e 7420 6279 2063  le argument by c
-00003440: 6f6e 7665 6e74 696f 6e20 6361 6c6c 6564  onvention called
-00003450: 2060 6461 7461 602c 2077 6869 6368 2063   `data`, which c
-00003460: 6f6e 7461 696e 7320 7468 6520 656e 7469  ontains the enti
-00003470: 7265 2072 6573 756c 7420 6672 6f6d 2074  re result from t
-00003480: 6865 2041 5049 2e0a 0a46 6f72 2065 7861  he API...For exa
-00003490: 6d70 6c65 2c20 7468 6520 6265 6c6f 7720  mple, the below 
-000034a0: 6675 6e63 7469 6f6e 2077 6f75 6c64 2067  function would g
-000034b0: 6574 2074 6865 2072 6563 656e 7420 6c69  et the recent li
-000034c0: 7374 206f 6620 756e 7265 6164 206d 6573  st of unread mes
-000034d0: 7361 6765 7320 616e 6420 6c6f 6720 7468  sages and log th
-000034e0: 656d 2074 6f20 7468 6520 636f 6e73 6f6c  em to the consol
-000034f0: 653a 3a0a 0a20 2020 2066 756e 6374 696f  e::..    functio
-00003500: 6e20 6d79 5f73 7065 6369 616c 5f6e 6f74  n my_special_not
-00003510: 6966 6963 6174 696f 6e5f 6361 6c6c 6261  ification_callba
-00003520: 636b 2864 6174 6129 207b 0a20 2020 2020  ck(data) {.     
-00003530: 2020 2066 6f72 2028 7661 7220 693d 303b     for (var i=0;
-00003540: 2069 203c 2064 6174 612e 756e 7265 6164   i < data.unread
-00003550: 5f6c 6973 742e 6c65 6e67 7468 3b20 692b  _list.length; i+
-00003560: 2b29 207b 0a20 2020 2020 2020 2020 2020  +) {.           
-00003570: 206d 7367 203d 2064 6174 612e 756e 7265   msg = data.unre
-00003580: 6164 5f6c 6973 745b 695d 3b0a 2020 2020  ad_list[i];.    
-00003590: 2020 2020 2020 2020 636f 6e73 6f6c 652e          console.
-000035a0: 6c6f 6728 6d73 6729 3b0a 2020 2020 2020  log(msg);.      
-000035b0: 2020 7d0a 2020 2020 7d0a 0a54 6573 7469    }.    }..Testi
-000035c0: 6e67 2074 6865 206c 6976 652d 7570 6461  ng the live-upda
-000035d0: 7465 720a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ter.------------
-000035e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 312e  ------------..1.
-000035f0: 2043 6c6f 6e65 2074 6865 2072 6570 6f0a   Clone the repo.
-00003600: 322e 2052 756e 2060 2e2f 6d61 6e61 6765  2. Run `./manage
-00003610: 2e70 7920 7275 6e73 6572 7665 7260 0a33  .py runserver`.3
-00003620: 2e20 4272 6f77 7365 2074 6f20 6079 6f75  . Browse to `you
-00003630: 7273 6572 7665 7269 702f 7465 7374 2f60  rserverip/test/`
-00003640: 0a34 2e20 436c 6963 6b20 274d 616b 6520  .4. Click 'Make 
-00003650: 6120 6e6f 7469 6669 6361 7469 6f6e 2720  a notification' 
-00003660: 616e 6420 6120 6e65 7720 6e6f 7469 6669  and a new notifi
-00003670: 6361 7469 6f6e 2073 686f 756c 6420 6170  cation should ap
-00003680: 7065 6172 2069 6e20 7468 6520 6c69 7374  pear in the list
-00003690: 2069 6e20 352d 3130 2073 6563 6f6e 6473   in 5-10 seconds
-000036a0: 2e0a 0a53 6572 6961 6c69 7a69 6e67 2074  ...Serializing t
-000036b0: 6865 2064 6a61 6e67 6f2d 6e6f 7469 6669  he django-notifi
-000036c0: 6361 7469 6f6e 7320 4d6f 6465 6c0a 3d3d  cations Model.==
-000036d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000036e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000036f0: 3d3d 3d3d 3d3d 3d3d 0a0a 5365 6520 6865  ========..See he
-00003700: 7265 202d 2068 7474 703a 2f2f 7777 772e  re - http://www.
-00003710: 646a 616e 676f 2d72 6573 742d 6672 616d  django-rest-fram
-00003720: 6577 6f72 6b2e 6f72 672f 6170 692d 6775  ework.org/api-gu
-00003730: 6964 652f 7265 6c61 7469 6f6e 732f 2367  ide/relations/#g
-00003740: 656e 6572 6963 2d72 656c 6174 696f 6e73  eneric-relations
-00003750: 6869 7073 0a0a 496e 2074 6869 7320 6578  hips..In this ex
-00003760: 616d 706c 6520 7468 6520 7461 7267 6574  ample the target
-00003770: 206f 626a 6563 7420 6361 6e20 6265 206f   object can be o
-00003780: 6620 7479 7065 2046 6f6f 206f 7220 4261  f type Foo or Ba
-00003790: 7220 616e 6420 7468 6520 6170 7072 6f70  r and the approp
-000037a0: 7269 6174 6520 7365 7269 616c 697a 6572  riate serializer
-000037b0: 2077 696c 6c20 6265 2075 7365 642e 0a0a   will be used...
-000037c0: 3a3a 0a0a 2020 2020 636c 6173 7320 4765  ::..    class Ge
-000037d0: 6e65 7269 634e 6f74 6966 6963 6174 696f  nericNotificatio
-000037e0: 6e52 656c 6174 6564 4669 656c 6428 7365  nRelatedField(se
-000037f0: 7269 616c 697a 6572 732e 5265 6c61 7465  rializers.Relate
-00003800: 6446 6965 6c64 293a 0a0a 2020 2020 2020  dField):..      
-00003810: 2020 6465 6620 746f 5f72 6570 7265 7365    def to_represe
-00003820: 6e74 6174 696f 6e28 7365 6c66 2c20 7661  ntation(self, va
-00003830: 6c75 6529 3a0a 2020 2020 2020 2020 2020  lue):.          
-00003840: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00003850: 7661 6c75 652c 2046 6f6f 293a 0a20 2020  value, Foo):.   
-00003860: 2020 2020 2020 2020 2020 2020 2073 6572               ser
-00003870: 6961 6c69 7a65 7220 3d20 466f 6f53 6572  ializer = FooSer
-00003880: 6961 6c69 7a65 7228 7661 6c75 6529 0a20  ializer(value). 
-00003890: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-000038a0: 696e 7374 616e 6365 2876 616c 7565 2c20  instance(value, 
-000038b0: 4261 7229 3a0a 2020 2020 2020 2020 2020  Bar):.          
-000038c0: 2020 2020 2020 7365 7269 616c 697a 6572        serializer
-000038d0: 203d 2042 6172 5365 7269 616c 697a 6572   = BarSerializer
-000038e0: 2876 616c 7565 290a 0a20 2020 2020 2020  (value)..       
-000038f0: 2020 2020 2072 6574 7572 6e20 7365 7269       return seri
-00003900: 616c 697a 6572 2e64 6174 610a 0a0a 2020  alizer.data...  
-00003910: 2020 636c 6173 7320 4e6f 7469 6669 6361    class Notifica
-00003920: 7469 6f6e 5365 7269 616c 697a 6572 2873  tionSerializer(s
-00003930: 6572 6961 6c69 7a65 7273 2e53 6572 6961  erializers.Seria
-00003940: 6c69 7a65 7229 3a0a 2020 2020 2020 2020  lizer):.        
-00003950: 7265 6369 7069 656e 7420 3d20 5075 626c  recipient = Publ
-00003960: 6963 5573 6572 5365 7269 616c 697a 6572  icUserSerializer
-00003970: 2855 7365 722c 2072 6561 645f 6f6e 6c79  (User, read_only
-00003980: 3d54 7275 6529 0a20 2020 2020 2020 2075  =True).        u
-00003990: 6e72 6561 6420 3d20 7365 7269 616c 697a  nread = serializ
-000039a0: 6572 732e 426f 6f6c 6561 6e46 6965 6c64  ers.BooleanField
-000039b0: 2872 6561 645f 6f6e 6c79 3d54 7275 6529  (read_only=True)
-000039c0: 0a20 2020 2020 2020 2074 6172 6765 7420  .        target 
-000039d0: 3d20 4765 6e65 7269 634e 6f74 6966 6963  = GenericNotific
-000039e0: 6174 696f 6e52 656c 6174 6564 4669 656c  ationRelatedFiel
-000039f0: 6428 7265 6164 5f6f 6e6c 793d 5472 7565  d(read_only=True
-00003a00: 290a 0a54 6861 6e6b 7320 746f 2040 4461  )..Thanks to @Da
-00003a10: 5779 0a0a 6060 4162 7374 7261 6374 4e6f  Wy..``AbstractNo
-00003a20: 7469 6669 6361 7469 6f6e 6060 206d 6f64  tification`` mod
-00003a30: 656c 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  el.-------------
-00003a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003a50: 2d0a 0a49 6e20 6361 7365 2079 6f75 206e  -..In case you n
-00003a60: 6565 6420 746f 2063 7573 746f 6d69 7a65  eed to customize
-00003a70: 2074 6865 206e 6f74 6966 6963 6174 696f   the notificatio
-00003a80: 6e20 6d6f 6465 6c20 696e 206f 7264 6572  n model in order
-00003a90: 2074 6f20 6164 6420 6669 656c 6420 6f72   to add field or
-00003aa0: 0a63 7573 746f 6d69 7365 6420 6665 6174  .customised feat
-00003ab0: 7572 6573 2074 6861 7420 6465 7065 6e64  ures that depend
-00003ac0: 206f 6e20 796f 7572 2061 7070 6c69 6361   on your applica
-00003ad0: 7469 6f6e 2c20 796f 7520 6361 6e20 696e  tion, you can in
-00003ae0: 6865 7269 7420 616e 6420 6578 7465 6e64  herit and extend
-00003af0: 0a74 6865 2060 6041 6273 7472 6163 744e  .the ``AbstractN
-00003b00: 6f74 6966 6963 6174 696f 6e60 6020 6d6f  otification`` mo
-00003b10: 6465 6c2c 2065 7861 6d70 6c65 3a0a 0a2e  del, example:...
-00003b20: 2e20 2063 6f64 652d 626c 6f63 6b3a 3a20  .  code-block:: 
-00003b30: 7079 7468 6f6e 0a0a 2020 2020 2349 6e20  python..    #In 
-00003b40: 796f 7572 5f61 7070 2f6d 6f64 656c 732e  your_app/models.
-00003b50: 7079 0a0a 2020 2020 6672 6f6d 2064 6a61  py..    from dja
-00003b60: 6e67 6f2e 6462 2069 6d70 6f72 7420 6d6f  ngo.db import mo
-00003b70: 6465 6c73 0a20 2020 2066 726f 6d20 6e6f  dels.    from no
-00003b80: 7469 6669 6361 7469 6f6e 732e 6261 7365  tifications.base
-00003b90: 2e6d 6f64 656c 7320 696d 706f 7274 2041  .models import A
-00003ba0: 6273 7472 6163 744e 6f74 6966 6963 6174  bstractNotificat
-00003bb0: 696f 6e0a 0a0a 2020 2020 636c 6173 7320  ion...    class 
-00003bc0: 4e6f 7469 6669 6361 7469 6f6e 2841 6273  Notification(Abs
-00003bd0: 7472 6163 744e 6f74 6966 6963 6174 696f  tractNotificatio
-00003be0: 6e29 3a0a 2020 2020 2020 2020 2320 6375  n):.        # cu
-00003bf0: 7374 6f6d 2066 6965 6c64 2065 7861 6d70  stom field examp
-00003c00: 6c65 0a20 2020 2020 2020 2063 6174 6567  le.        categ
-00003c10: 6f72 7920 3d20 6d6f 6465 6c73 2e46 6f72  ory = models.For
-00003c20: 6569 676e 4b65 7928 276d 7961 7070 2e43  eignKey('myapp.C
-00003c30: 6174 6567 6f72 7927 2c0a 2020 2020 2020  ategory',.      
-00003c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c50: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00003c60: 6e5f 6465 6c65 7465 3d6d 6f64 656c 732e  n_delete=models.
-00003c70: 4341 5343 4144 4529 0a0a 2020 2020 2020  CASCADE)..      
-00003c80: 2020 636c 6173 7320 4d65 7461 2841 6273    class Meta(Abs
-00003c90: 7472 6163 744e 6f74 6966 6963 6174 696f  tractNotificatio
-00003ca0: 6e2e 4d65 7461 293a 0a20 2020 2020 2020  n.Meta):.       
-00003cb0: 2020 2020 2061 6273 7472 6163 7420 3d20       abstract = 
-00003cc0: 4661 6c73 650a 0a59 6f75 2077 696c 6c20  False..You will 
-00003cd0: 7265 7175 6972 6520 746f 2064 6566 696e  require to defin
-00003ce0: 6520 6060 4e4f 5449 4649 4341 5449 4f4e  e ``NOTIFICATION
-00003cf0: 535f 4e4f 5449 4649 4341 5449 4f4e 5f4d  S_NOTIFICATION_M
-00003d00: 4f44 454c 6060 2073 6574 7469 6e67 2069  ODEL`` setting i
-00003d10: 6e20 6073 6574 7469 6e67 2e70 7960 2061  n `setting.py` a
-00003d20: 7320 666f 6c6c 6f77 733a 0a0a 2e2e 2020  s follows:....  
-00003d30: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
-00003d40: 686f 6e0a 0a20 2020 2023 2049 6e20 796f  hon..    # In yo
-00003d50: 7572 5f70 726f 6a65 6374 2f73 6574 7469  ur_project/setti
-00003d60: 6e67 732e 7079 0a0a 2020 2020 4e4f 5449  ngs.py..    NOTI
-00003d70: 4649 4341 5449 4f4e 535f 4e4f 5449 4649  FICATIONS_NOTIFI
-00003d80: 4341 5449 4f4e 5f4d 4f44 454c 203d 2027  CATION_MODEL = '
-00003d90: 796f 7572 5f61 7070 2e4e 6f74 6966 6963  your_app.Notific
-00003da0: 6174 696f 6e27 0a0a 4e6f 7465 730a 3d3d  ation'..Notes.==
-00003db0: 3d3d 3d0a 0a45 6d61 696c 204e 6f74 6966  ===..Email Notif
-00003dc0: 6963 6174 696f 6e0a 2d2d 2d2d 2d2d 2d2d  ication.--------
-00003dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 5365 6e64  ----------..Send
-00003de0: 696e 6720 656d 6169 6c20 746f 2075 7365  ing email to use
-00003df0: 7273 2068 6173 206e 6f74 2062 6565 6e20  rs has not been 
-00003e00: 696e 7465 6772 6174 6564 2069 6e74 6f20  integrated into 
-00003e10: 7468 6973 206c 6962 7261 7279 2e20 536f  this library. So
-00003e20: 2066 6f72 206e 6f77 2079 6f75 206e 6565   for now you nee
-00003e30: 6420 746f 2069 6d70 6c65 6d65 6e74 2069  d to implement i
-00003e40: 7420 6966 206e 6565 6465 642e 2054 6865  t if needed. The
-00003e50: 7265 2069 7320 6120 7265 7365 7276 6564  re is a reserved
-00003e60: 2066 6965 6c64 2060 4e6f 7469 6669 6361   field `Notifica
-00003e70: 7469 6f6e 2e65 6d61 696c 6564 6020 746f  tion.emailed` to
-00003e80: 206d 616b 6520 6974 2065 6173 6965 722e   make it easier.
-00003e90: 0a0a 5361 6d70 6c65 2041 7070 0a2d 2d2d  ..Sample App.---
-00003ea0: 2d2d 2d2d 2d2d 2d0a 0a41 2073 616d 706c  -------..A sampl
-00003eb0: 6520 6170 7020 6861 7320 6265 656e 2069  e app has been i
-00003ec0: 6d70 6c65 6d65 6e74 6564 2069 6e20 6060  mplemented in ``
-00003ed0: 6e6f 7469 6669 6361 7469 6f6e 732f 7465  notifications/te
-00003ee0: 7374 732f 7361 6d70 6c65 5f6e 6f74 6966  sts/sample_notif
-00003ef0: 6963 6174 696f 6e73 6060 2074 6861 7420  ications`` that 
-00003f00: 6578 7465 6e64 7320 6060 646a 616e 676f  extends ``django
-00003f10: 2d6e 6f74 6966 6963 6174 696f 6e73 6060  -notifications``
-00003f20: 2077 6974 6820 7468 6520 736f 6c65 2070   with the sole p
-00003f30: 7572 706f 7365 206f 6620 7465 7374 696e  urpose of testin
-00003f40: 6720 6974 7320 6578 7465 6e73 6962 696c  g its extensibil
-00003f50: 6974 792e 0a59 6f75 2063 616e 2072 756e  ity..You can run
-00003f60: 2074 6865 2053 414d 504c 4520 4150 5020   the SAMPLE APP 
-00003f70: 6279 2073 6574 7469 6e67 2074 6865 2065  by setting the e
-00003f80: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00003f90: 626c 6520 6060 5341 4d50 4c45 5f41 5050  ble ``SAMPLE_APP
-00003fa0: 6060 2061 7320 666f 6c6c 6f77 730a 0a2e  `` as follows...
-00003fb0: 2e20 2063 6f64 652d 626c 6f63 6b3a 3a20  .  code-block:: 
-00003fc0: 7368 656c 6c0a 0a20 2020 2065 7870 6f72  shell..    expor
-00003fd0: 7420 5341 4d50 4c45 5f41 5050 3d31 0a20  t SAMPLE_APP=1. 
-00003fe0: 2020 2023 2052 756e 2074 6865 2044 6a61     # Run the Dja
-00003ff0: 6e67 6f20 6465 7665 6c6f 706d 656e 7420  ngo development 
-00004000: 7365 7276 6572 2077 6974 6820 7361 6d70  server with samp
-00004010: 6c65 5f6e 6f74 6966 6963 6174 696f 6e73  le_notifications
-00004020: 2061 7070 2069 6e73 7461 6c6c 6564 0a20   app installed. 
-00004030: 2020 2070 7974 686f 6e20 6d61 6e61 6765     python manage
-00004040: 2e70 7920 7275 6e73 6572 7665 720a 2020  .py runserver.  
-00004050: 2020 2320 556e 7365 7420 5341 4d50 4c45    # Unset SAMPLE
-00004060: 5f41 5050 2074 6f20 7265 6d6f 7665 2073  _APP to remove s
-00004070: 616d 706c 655f 6e6f 7469 6669 6361 7469  ample_notificati
-00004080: 6f6e 7320 6170 7020 6672 6f6d 206c 6973  ons app from lis
-00004090: 7420 6f66 2049 4e53 5441 4c4c 4544 5f41  t of INSTALLED_A
-000040a0: 5050 530a 2020 2020 756e 7365 7420 5341  PPS.    unset SA
-000040b0: 4d50 4c45 5f41 5050 0a0a 0a60 6064 6a61  MPLE_APP...``dja
-000040c0: 6e67 6f2d 6e6f 7469 6669 6361 7469 6f6e  ngo-notification
-000040d0: 7360 6020 5465 616d 0a3d 3d3d 3d3d 3d3d  s`` Team.=======
-000040e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000040f0: 3d3d 3d3d 3d3d 3d0a 0a43 6f72 6520 636f  =======..Core co
-00004100: 6e74 7269 6275 746f 7273 2028 696e 2061  ntributors (in a
-00004110: 6c70 6861 6265 7469 6361 6c20 6f72 6465  lphabetical orde
-00004120: 7229 3a0a 0a2d 2060 416c 7661 726f 204c  r):..- `Alvaro L
-00004130: 656f 6e65 6c20 3c68 7474 7073 3a2f 2f67  eonel <https://g
-00004140: 6974 6875 622e 636f 6d2f 416c 7661 726f  ithub.com/Alvaro
-00004150: 4c51 7565 6972 6f7a 3e60 5f0a 2d20 6046  LQueiroz>`_.- `F
-00004160: 6564 6572 6963 6f20 4361 706f 616e 6f20  ederico Capoano 
-00004170: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00004180: 636f 6d2f 6e65 6d65 7369 7364 6573 6967  com/nemesisdesig
-00004190: 6e3e 605f 0a2d 2060 5361 6d75 656c 2053  n>`_.- `Samuel S
-000041a0: 7065 6e63 6572 203c 6874 7470 733a 2f2f  pencer <https://
-000041b0: 6769 7468 7562 2e63 6f6d 2f4c 6567 6f53  github.com/LegoS
-000041c0: 746f 726d 7472 6f6f 7072 3e60 5f0a 2d20  tormtroopr>`_.- 
-000041d0: 6059 616e 6720 5975 626f 203c 6874 7470  `Yang Yubo <http
-000041e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f79  s://github.com/y
-000041f0: 616e 6779 7562 6f3e 605f 0a2d 2060 5a68  angyubo>`_.- `Zh
-00004200: 6f6e 6779 7561 6e20 5a68 616e 6720 3c68  ongyuan Zhang <h
-00004210: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004220: 6d2f 7a68 616e 672d 7a3e 605f 0a0a 2e2e  m/zhang-z>`_....
-00004230: 207c 6275 696c 642d 7374 6174 7573 7c20   |build-status| 
-00004240: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
-00004250: 7472 6176 6973 2d63 692e 6f72 672f 646a  travis-ci.org/dj
-00004260: 616e 676f 2d6e 6f74 6966 6963 6174 696f  ango-notificatio
-00004270: 6e73 2f64 6a61 6e67 6f2d 6e6f 7469 6669  ns/django-notifi
-00004280: 6361 7469 6f6e 732e 7376 670a 2020 2020  cations.svg.    
-00004290: 3a74 6172 6765 743a 2068 7474 7073 3a2f  :target: https:/
-000042a0: 2f74 7261 7669 732d 6369 2e6f 7267 2f64  /travis-ci.org/d
-000042b0: 6a61 6e67 6f2d 6e6f 7469 6669 6361 7469  jango-notificati
-000042c0: 6f6e 732f 646a 616e 676f 2d6e 6f74 6966  ons/django-notif
-000042d0: 6963 6174 696f 6e73 0a0a 2e2e 207c 636f  ications.... |co
-000042e0: 7665 7261 6c6c 737c 2069 6d61 6765 3a3a  veralls| image::
-000042f0: 2068 7474 7073 3a2f 2f63 6f76 6572 616c   https://coveral
-00004300: 6c73 2e69 6f2f 7265 706f 732f 646a 616e  ls.io/repos/djan
-00004310: 676f 2d6e 6f74 6966 6963 6174 696f 6e73  go-notifications
-00004320: 2f64 6a61 6e67 6f2d 6e6f 7469 6669 6361  /django-notifica
-00004330: 7469 6f6e 732f 6261 6467 652e 706e 673f  tions/badge.png?
-00004340: 6272 616e 6368 3d6d 6173 7465 720a 2020  branch=master.  
-00004350: 2020 3a61 6c74 3a20 436f 6465 2063 6f76    :alt: Code cov
-00004360: 6572 6167 6520 6f6e 2063 6f76 6572 616c  erage on coveral
-00004370: 6c73 0a20 2020 203a 7363 616c 653a 2031  ls.    :scale: 1
-00004380: 3030 250a 2020 2020 3a74 6172 6765 743a  00%.    :target:
-00004390: 2068 7474 7073 3a2f 2f63 6f76 6572 616c   https://coveral
-000043a0: 6c73 2e69 6f2f 722f 646a 616e 676f 2d6e  ls.io/r/django-n
-000043b0: 6f74 6966 6963 6174 696f 6e73 2f64 6a61  otifications/dja
-000043c0: 6e67 6f2d 6e6f 7469 6669 6361 7469 6f6e  ngo-notification
-000043d0: 733f 6272 616e 6368 3d6d 6173 7465 720a  s?branch=master.
-000043e0: 0a43 6f6e 7472 6962 7574 650a 3d3d 3d3d  .Contribute.====
-000043f0: 3d3d 3d3d 3d3d 0a0a 5765 2061 7265 206c  ======..We are l
-00004400: 6f6f 6b69 6e67 2066 6f72 2063 6f6e 7472  ooking for contr
-00004410: 6962 7574 6f72 732c 2066 6f72 2061 6e79  ibutors, for any
-00004420: 6f6e 6520 7768 6f27 6420 6c69 6b65 2074  one who'd like t
-00004430: 6f20 636f 6e74 7269 6275 7465 2061 6e64  o contribute and
-00004440: 2077 696c 6c69 6e67 2074 6f20 7075 7420   willing to put 
-00004450: 7469 6d65 2061 6e64 2065 6e65 7267 7920  time and energy 
-00004460: 6f6e 2074 6869 7320 7072 6f6a 6563 742c  on this project,
-00004470: 2070 6c65 6173 6520 636f 6e74 6163 7420   please contact 
-00004480: 6059 616e 6720 5975 626f 203c 6874 7470  `Yang Yubo <http
-00004490: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f79  s://github.com/y
-000044a0: 616e 6779 7562 6f3e 605f 2e0a            angyubo>`_..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
+00000020: 676f 2d6e 6f74 6966 6963 6174 696f 6e73  go-notifications
+00000030: 2d68 710a 5665 7273 696f 6e3a 2031 2e38  -hq.Version: 1.8
+00000040: 2e30 0a53 756d 6d61 7279 3a20 4769 7448  .0.Summary: GitH
+00000050: 7562 206e 6f74 6966 6963 6174 696f 6e73  ub notifications
+00000060: 2061 6c69 6b65 2061 7070 2066 6f72 2044   alike app for D
+00000070: 6a61 6e67 6f2e 0a48 6f6d 652d 7061 6765  jango..Home-page
+00000080: 3a20 6874 7470 3a2f 2f67 6974 6875 622e  : http://github.
+00000090: 636f 6d2f 646a 616e 676f 2d6e 6f74 6966  com/django-notif
+000000a0: 6963 6174 696f 6e73 2f64 6a61 6e67 6f2d  ications/django-
+000000b0: 6e6f 7469 6669 6361 7469 6f6e 730a 4175  notifications.Au
+000000c0: 7468 6f72 3a20 646a 616e 676f 2d6e 6f74  thor: django-not
+000000d0: 6966 6963 6174 696f 6e73 2074 6561 6d0a  ifications team.
+000000e0: 4175 7468 6f72 2d65 6d61 696c 3a20 7961  Author-email: ya
+000000f0: 6e67 4079 616e 6779 7562 6f2e 636f 6d0a  ng@yangyubo.com.
+00000100: 4c69 6365 6e73 653a 204d 4954 0a4b 6579  License: MIT.Key
+00000110: 776f 7264 733a 2064 6a61 6e67 6f20 6e6f  words: django no
+00000120: 7469 6669 6361 7469 6f6e 7320 6769 7468  tifications gith
+00000130: 7562 2061 6374 696f 6e20 6576 656e 7420  ub action event 
+00000140: 7374 7265 616d 0a43 6c61 7373 6966 6965  stream.Classifie
+00000150: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
+00000160: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
+00000170: 6475 6374 696f 6e2f 5374 6162 6c65 0a43  duction/Stable.C
+00000180: 6c61 7373 6966 6965 723a 2045 6e76 6972  lassifier: Envir
+00000190: 6f6e 6d65 6e74 203a 3a20 5765 6220 456e  onment :: Web En
+000001a0: 7669 726f 6e6d 656e 740a 436c 6173 7369  vironment.Classi
+000001b0: 6669 6572 3a20 4672 616d 6577 6f72 6b20  fier: Framework 
+000001c0: 3a3a 2044 6a61 6e67 6f0a 436c 6173 7369  :: Django.Classi
+000001d0: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
+000001e0: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
+000001f0: 6f70 6572 730a 436c 6173 7369 6669 6572  opers.Classifier
+00000200: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
+00000210: 2041 7070 726f 7665 6420 3a3a 2042 5344   Approved :: BSD
+00000220: 204c 6963 656e 7365 0a43 6c61 7373 6966   License.Classif
+00000230: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
+00000240: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+00000250: 7065 6e64 656e 740a 436c 6173 7369 6669  pendent.Classifi
+00000260: 6572 3a20 4672 616d 6577 6f72 6b20 3a3a  er: Framework ::
+00000270: 2044 6a61 6e67 6f0a 436c 6173 7369 6669   Django.Classifi
+00000280: 6572 3a20 4672 616d 6577 6f72 6b20 3a3a  er: Framework ::
+00000290: 2044 6a61 6e67 6f20 3a3a 2033 2e32 0a43   Django :: 3.2.C
+000002a0: 6c61 7373 6966 6965 723a 2046 7261 6d65  lassifier: Frame
+000002b0: 776f 726b 203a 3a20 446a 616e 676f 203a  work :: Django :
+000002c0: 3a20 342e 300a 436c 6173 7369 6669 6572  : 4.0.Classifier
+000002d0: 3a20 4672 616d 6577 6f72 6b20 3a3a 2044  : Framework :: D
+000002e0: 6a61 6e67 6f20 3a3a 2034 2e31 0a43 6c61  jango :: 4.1.Cla
+000002f0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000300: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000310: 2050 7974 686f 6e0a 436c 6173 7369 6669   Python.Classifi
+00000320: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000330: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000340: 6f6e 203a 3a20 330a 436c 6173 7369 6669  on :: 3.Classifi
+00000350: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000360: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000370: 6f6e 203a 3a20 332e 370a 436c 6173 7369  on :: 3.7.Classi
+00000380: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000390: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000003a0: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
+000003b0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000003c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000003d0: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
+000003e0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000003f0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000400: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000410: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000420: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000430: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000440: 2e31 310a 436c 6173 7369 6669 6572 3a20  .11.Classifier: 
+00000450: 546f 7069 6320 3a3a 2055 7469 6c69 7469  Topic :: Utiliti
+00000460: 6573 0a44 6573 6372 6970 7469 6f6e 2d43  es.Description-C
+00000470: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+00000480: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
+00000490: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
+000004a0: 2e74 7874 0a4c 6963 656e 7365 2d46 696c  .txt.License-Fil
+000004b0: 653a 2041 5554 484f 5253 2e74 7874 0a0a  e: AUTHORS.txt..
+000004c0: 2320 6064 6a61 6e67 6f2d 6e6f 7469 6669  # `django-notifi
+000004d0: 6361 7469 6f6e 7360 2044 6f63 756d 656e  cations` Documen
+000004e0: 7461 7469 6f6e 0a0a 5b21 5b62 7569 6c64  tation..[![build
+000004f0: 2d73 7461 7475 735d 2868 7474 7073 3a2f  -status](https:/
+00000500: 2f74 7261 7669 732d 6369 2e6f 7267 2f64  /travis-ci.org/d
+00000510: 6a61 6e67 6f2d 6e6f 7469 6669 6361 7469  jango-notificati
+00000520: 6f6e 732f 646a 616e 676f 2d6e 6f74 6966  ons/django-notif
+00000530: 6963 6174 696f 6e73 2e73 7667 295d 2868  ications.svg)](h
+00000540: 7474 7073 3a2f 2f74 7261 7669 732d 6369  ttps://travis-ci
+00000550: 2e6f 7267 2f64 6a61 6e67 6f2d 6e6f 7469  .org/django-noti
+00000560: 6669 6361 7469 6f6e 732f 646a 616e 676f  fications/django
+00000570: 2d6e 6f74 6966 6963 6174 696f 6e73 290a  -notifications).
+00000580: 5b21 5b43 6f76 6572 6167 6520 5374 6174  [![Coverage Stat
+00000590: 7573 5d28 6874 7470 733a 2f2f 636f 7665  us](https://cove
+000005a0: 7261 6c6c 732e 696f 2f72 6570 6f73 2f67  ralls.io/repos/g
+000005b0: 6974 6875 622f 646a 616e 676f 2d6e 6f74  ithub/django-not
+000005c0: 6966 6963 6174 696f 6e73 2f64 6a61 6e67  ifications/djang
+000005d0: 6f2d 6e6f 7469 6669 6361 7469 6f6e 732f  o-notifications/
+000005e0: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
+000005f0: 3d6d 6173 7465 7229 5d28 6874 7470 733a  =master)](https:
+00000600: 2f2f 636f 7665 7261 6c6c 732e 696f 2f67  //coveralls.io/g
+00000610: 6974 6875 622f 646a 616e 676f 2d6e 6f74  ithub/django-not
+00000620: 6966 6963 6174 696f 6e73 2f64 6a61 6e67  ifications/djang
+00000630: 6f2d 6e6f 7469 6669 6361 7469 6f6e 733f  o-notifications?
+00000640: 6272 616e 6368 3d6d 6173 7465 7229 0a0a  branch=master)..
+00000650: 0a5b 646a 616e 676f 2d6e 6f74 6966 6963  .[django-notific
+00000660: 6174 696f 6e73 5d28 6874 7470 733a 2f2f  ations](https://
+00000670: 6769 7468 7562 2e63 6f6d 2f64 6a61 6e67  github.com/djang
+00000680: 6f2d 6e6f 7469 6669 6361 7469 6f6e 732f  o-notifications/
+00000690: 646a 616e 676f 2d6e 6f74 6966 6963 6174  django-notificat
+000006a0: 696f 6e73 2920 6973 2061 2047 6974 4875  ions) is a GitHu
+000006b0: 6220 6e6f 7469 6669 6361 7469 6f6e 2061  b notification a
+000006c0: 6c69 6b65 2061 7070 2066 6f72 2044 6a61  like app for Dja
+000006d0: 6e67 6f2c 2069 7420 7761 7320 6465 7269  ngo, it was deri
+000006e0: 7665 6420 6672 6f6d 205b 646a 616e 676f  ved from [django
+000006f0: 2d61 6374 6976 6974 792d 7374 7265 616d  -activity-stream
+00000700: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000710: 2e63 6f6d 2f6a 7573 7471 7569 636b 2f64  .com/justquick/d
+00000720: 6a61 6e67 6f2d 6163 7469 7669 7479 2d73  jango-activity-s
+00000730: 7472 6561 6d29 0a0a 5468 6520 6d61 6a6f  tream)..The majo
+00000740: 7220 6469 6666 6572 656e 6365 2062 6574  r difference bet
+00000750: 7765 656e 2060 646a 616e 676f 2d6e 6f74  ween `django-not
+00000760: 6966 6963 6174 696f 6e73 6020 616e 6420  ifications` and 
+00000770: 6064 6a61 6e67 6f2d 6163 7469 7669 7479  `django-activity
+00000780: 2d73 7472 6561 6d60 3a0a 0a2d 2060 646a  -stream`:..- `dj
+00000790: 616e 676f 2d6e 6f74 6966 6963 6174 696f  ango-notificatio
+000007a0: 6e73 6020 6973 2066 6f72 2062 7569 6c64  ns` is for build
+000007b0: 696e 6720 736f 6d65 7468 696e 6720 6c69  ing something li
+000007c0: 6b65 2047 6974 6875 6220 224e 6f74 6966  ke Github "Notif
+000007d0: 6963 6174 696f 6e73 220a 2d20 5768 696c  ications".- Whil
+000007e0: 6520 6064 6a61 6e67 6f2d 6163 7469 7669  e `django-activi
+000007f0: 7479 2d73 7472 6561 6d60 2069 7320 666f  ty-stream` is fo
+00000800: 7220 6275 696c 6469 6e67 2047 6974 6875  r building Githu
+00000810: 6220 224e 6577 7320 4665 6564 220a 0a4e  b "News Feed"..N
+00000820: 6f74 6966 6963 6174 696f 6e73 2061 7265  otifications are
+00000830: 2061 6374 7561 6c6c 7920 6163 7469 6f6e   actually action
+00000840: 7320 6576 656e 7473 2c20 7768 6963 6820  s events, which 
+00000850: 6172 6520 6361 7465 676f 7269 7a65 6420  are categorized 
+00000860: 6279 2066 6f75 7220 6d61 696e 2063 6f6d  by four main com
+00000870: 706f 6e65 6e74 732e 0a0a 2d20 2020 6041  ponents...-   `A
+00000880: 6374 6f72 602e 2054 6865 206f 626a 6563  ctor`. The objec
+00000890: 7420 7468 6174 2070 6572 666f 726d 6564  t that performed
+000008a0: 2074 6865 2061 6374 6976 6974 792e 0a2d   the activity..-
+000008b0: 2020 2060 5665 7262 602e 2054 6865 2076     `Verb`. The v
+000008c0: 6572 6220 7068 7261 7365 2074 6861 7420  erb phrase that 
+000008d0: 6964 656e 7469 6669 6573 2074 6865 2061  identifies the a
+000008e0: 6374 696f 6e20 6f66 2074 6865 2061 6374  ction of the act
+000008f0: 6976 6974 792e 0a2d 2020 2060 4163 7469  ivity..-   `Acti
+00000900: 6f6e 204f 626a 6563 7460 2e20 2a28 4f70  on Object`. *(Op
+00000910: 7469 6f6e 616c 292a 2054 6865 206f 626a  tional)* The obj
+00000920: 6563 7420 6c69 6e6b 6564 2074 6f20 7468  ect linked to th
+00000930: 6520 6163 7469 6f6e 0a20 2020 2069 7473  e action.    its
+00000940: 656c 662e 0a2d 2020 2060 5461 7267 6574  elf..-   `Target
+00000950: 602e 202a 284f 7074 696f 6e61 6c29 2a20  `. *(Optional)* 
+00000960: 5468 6520 6f62 6a65 6374 2074 6f20 7768  The object to wh
+00000970: 6963 6820 7468 6520 6163 7469 7669 7479  ich the activity
+00000980: 2077 6173 0a20 2020 2070 6572 666f 726d   was.    perform
+00000990: 6564 2e0a 0a60 4163 746f 7260 2c20 6041  ed...`Actor`, `A
+000009a0: 6374 696f 6e20 4f62 6a65 6374 6020 616e  ction Object` an
+000009b0: 6420 6054 6172 6765 7460 2061 7265 2060  d `Target` are `
+000009c0: 4765 6e65 7269 6346 6f72 6569 676e 4b65  GenericForeignKe
+000009d0: 7973 6020 746f 2061 6e79 0a61 7262 6974  ys` to any.arbit
+000009e0: 7261 7279 2044 6a61 6e67 6f20 6f62 6a65  rary Django obje
+000009f0: 6374 2e20 416e 2061 6374 696f 6e20 6973  ct. An action is
+00000a00: 2061 2064 6573 6372 6970 7469 6f6e 206f   a description o
+00000a10: 6620 616e 2061 6374 696f 6e20 7468 6174  f an action that
+00000a20: 0a77 6173 2070 6572 666f 726d 6564 2028  .was performed (
+00000a30: 6056 6572 6260 2920 6174 2073 6f6d 6520  `Verb`) at some 
+00000a40: 696e 7374 616e 7420 696e 2074 696d 6520  instant in time 
+00000a50: 6279 2073 6f6d 6520 6041 6374 6f72 6020  by some `Actor` 
+00000a60: 6f6e 2073 6f6d 650a 6f70 7469 6f6e 616c  on some.optional
+00000a70: 2060 5461 7267 6574 6020 7468 6174 2072   `Target` that r
+00000a80: 6573 756c 7473 2069 6e20 616e 2060 4163  esults in an `Ac
+00000a90: 7469 6f6e 204f 626a 6563 7460 2067 6574  tion Object` get
+00000aa0: 7469 6e67 0a63 7265 6174 6564 2f75 7064  ting.created/upd
+00000ab0: 6174 6564 2f64 656c 6574 6564 2e0a 0a46  ated/deleted...F
+00000ac0: 6f72 2065 7861 6d70 6c65 3a20 5b6a 7573  or example: [jus
+00000ad0: 7471 7569 636b 5d28 6874 7470 733a 2f2f  tquick](https://
+00000ae0: 6769 7468 7562 2e63 6f6d 2f6a 7573 7471  github.com/justq
+00000af0: 7569 636b 2f29 2060 2861 6374 6f72 2960  uick/) `(actor)`
+00000b00: 0a2a 636c 6f73 6564 2a20 6028 7665 7262  .*closed* `(verb
+00000b10: 2960 205b 6973 7375 650a 325d 2868 7474  )` [issue.2](htt
+00000b20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000b30: 6a75 7374 7175 6963 6b2f 646a 616e 676f  justquick/django
+00000b40: 2d61 6374 6976 6974 792d 7374 7265 616d  -activity-stream
+00000b50: 2f69 7373 7565 732f 3229 0a60 2861 6374  /issues/2).`(act
+00000b60: 696f 6e5f 6f62 6a65 6374 2960 206f 6e0a  ion_object)` on.
+00000b70: 5b61 6374 6976 6974 792d 7374 7265 616d  [activity-stream
+00000b80: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000b90: 2e63 6f6d 2f6a 7573 7471 7569 636b 2f64  .com/justquick/d
+00000ba0: 6a61 6e67 6f2d 6163 7469 7669 7479 2d73  jango-activity-s
+00000bb0: 7472 6561 6d2f 290a 6028 7461 7267 6574  tream/).`(target
+00000bc0: 2960 2031 3220 686f 7572 7320 6167 6f0a  )` 12 hours ago.
+00000bd0: 0a4e 6f6d 656e 636c 6174 7572 6520 6f66  .Nomenclature of
+00000be0: 2074 6869 7320 7370 6563 6966 6963 6174   this specificat
+00000bf0: 696f 6e20 6973 2062 6173 6564 206f 6e20  ion is based on 
+00000c00: 7468 6520 4163 7469 7669 7479 2053 7472  the Activity Str
+00000c10: 6561 6d73 0a53 7065 633a 203c 6874 7470  eams.Spec: <http
+00000c20: 3a2f 2f61 6374 6976 6974 7973 7472 6561  ://activitystrea
+00000c30: 2e6d 732f 7370 6563 732f 6174 6f6d 2f31  .ms/specs/atom/1
+00000c40: 2e30 2f3e 0a0a 2323 2052 6571 7569 7265  .0/>..## Require
+00000c50: 6d65 6e74 730a 0a2d 2020 2050 7974 686f  ments..-   Pytho
+00000c60: 6e20 332e 372c 2033 2e38 2c20 332e 392c  n 3.7, 3.8, 3.9,
+00000c70: 2033 2e31 302c 2033 2e31 310a 2d20 2020   3.10, 3.11.-   
+00000c80: 446a 616e 676f 2033 2e32 2c20 342e 302c  Django 3.2, 4.0,
+00000c90: 2034 2e31 0a0a 2323 2049 6e73 7461 6c6c   4.1..## Install
+00000ca0: 6174 696f 6e0a 0a49 6e73 7461 6c6c 6174  ation..Installat
+00000cb0: 696f 6e20 6973 2065 6173 7920 7573 696e  ion is easy usin
+00000cc0: 6720 6070 6970 6020 616e 6420 7769 6c6c  g `pip` and will
+00000cd0: 2069 6e73 7461 6c6c 2061 6c6c 2072 6571   install all req
+00000ce0: 7569 7265 640a 6c69 6272 6172 6965 732e  uired.libraries.
+00000cf0: 0a60 6060 6261 7368 0a24 2070 6970 2069  .```bash.$ pip i
+00000d00: 6e73 7461 6c6c 2064 6a61 6e67 6f2d 6e6f  nstall django-no
+00000d10: 7469 6669 6361 7469 6f6e 732d 6871 0a60  tifications-hq.`
+00000d20: 6060 0a6f 7220 6765 7420 6974 2066 726f  ``.or get it fro
+00000d30: 6d20 736f 7572 6365 0a0a 6060 6062 6173  m source..```bas
+00000d40: 680a 2420 6769 7420 636c 6f6e 6520 6874  h.$ git clone ht
+00000d50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000d60: 2f64 6a61 6e67 6f2d 6e6f 7469 6669 6361  /django-notifica
+00000d70: 7469 6f6e 732f 646a 616e 676f 2d6e 6f74  tions/django-not
+00000d80: 6966 6963 6174 696f 6e73 0a24 2063 6420  ifications.$ cd 
+00000d90: 646a 616e 676f 2d6e 6f74 6966 6963 6174  django-notificat
+00000da0: 696f 6e73 0a24 2070 7974 686f 6e20 7365  ions.$ python se
+00000db0: 7475 702e 7079 2073 6469 7374 0a24 2070  tup.py sdist.$ p
+00000dc0: 6970 2069 6e73 7461 6c6c 2064 6973 742f  ip install dist/
+00000dd0: 646a 616e 676f 2d6e 6f74 6966 6963 6174  django-notificat
+00000de0: 696f 6e73 2d68 712a 0a60 6060 0a0a 4e6f  ions-hq*.```..No
+00000df0: 7465 2074 6861 7420 5b64 6a61 6e67 6f2d  te that [django-
+00000e00: 6d6f 6465 6c2d 7574 696c 735d 2868 7474  model-utils](htt
+00000e10: 703a 2f2f 7079 7069 2e70 7974 686f 6e2e  p://pypi.python.
+00000e20: 6f72 672f 7079 7069 2f64 6a61 6e67 6f2d  org/pypi/django-
+00000e30: 6d6f 6465 6c2d 7574 696c 7329 0a77 696c  model-utils).wil
+00000e40: 6c20 6265 2069 6e73 7461 6c6c 6564 3a20  l be installed: 
+00000e50: 7468 6973 2069 7320 7265 7175 6972 6564  this is required
+00000e60: 2066 6f72 2074 6865 2070 6173 732d 7468   for the pass-th
+00000e70: 726f 7567 6820 5175 6572 7953 6574 206d  rough QuerySet m
+00000e80: 616e 6167 6572 2e0a 0a54 6865 6e20 746f  anager...Then to
+00000e90: 2061 6464 2074 6865 2044 6a61 6e67 6f20   add the Django 
+00000ea0: 4e6f 7469 6669 6361 7469 6f6e 7320 746f  Notifications to
+00000eb0: 2079 6f75 7220 7072 6f6a 6563 7420 6164   your project ad
+00000ec0: 6420 7468 6520 6170 700a 606e 6f74 6966  d the app.`notif
+00000ed0: 6963 6174 696f 6e73 6020 746f 2079 6f75  ications` to you
+00000ee0: 7220 6049 4e53 5441 4c4c 4544 5f41 5050  r `INSTALLED_APP
+00000ef0: 5360 2061 6e64 2075 726c 636f 6e66 2e0a  S` and urlconf..
+00000f00: 0a54 6865 2061 7070 2073 686f 756c 6420  .The app should 
+00000f10: 676f 2073 6f6d 6577 6865 7265 2061 6674  go somewhere aft
+00000f20: 6572 2061 6c6c 2074 6865 2061 7070 7320  er all the apps 
+00000f30: 7468 6174 2061 7265 2067 6f69 6e67 2074  that are going t
+00000f40: 6f20 6265 0a67 656e 6572 6174 696e 6720  o be.generating 
+00000f50: 6e6f 7469 6669 6361 7469 6f6e 7320 6c69  notifications li
+00000f60: 6b65 2060 646a 616e 676f 2e63 6f6e 7472  ke `django.contr
+00000f70: 6962 2e61 7574 6860 0a0a 6060 6070 7974  ib.auth`..```pyt
+00000f80: 686f 6e0a 494e 5354 414c 4c45 445f 4150  hon.INSTALLED_AP
+00000f90: 5053 203d 2028 0a20 2020 2027 646a 616e  PS = (.    'djan
+00000fa0: 676f 2e63 6f6e 7472 6962 2e61 7574 6827  go.contrib.auth'
+00000fb0: 2c0a 2020 2020 2e2e 2e0a 2020 2020 276e  ,.    ....    'n
+00000fc0: 6f74 6966 6963 6174 696f 6e73 272c 0a20  otifications',. 
+00000fd0: 2020 202e 2e2e 0a29 0a60 6060 0a0a 4164     ....).```..Ad
+00000fe0: 6420 7468 6520 6e6f 7469 6669 6361 7469  d the notificati
+00000ff0: 6f6e 7320 7572 6c73 2074 6f20 796f 7572  ons urls to your
+00001000: 2075 726c 636f 6e66 3a0a 0a60 6060 7079   urlconf:..```py
+00001010: 7468 6f6e 0a69 6d70 6f72 7420 6e6f 7469  thon.import noti
+00001020: 6669 6361 7469 6f6e 732e 7572 6c73 0a0a  fications.urls..
+00001030: 7572 6c70 6174 7465 726e 7320 3d20 5b0a  urlpatterns = [.
+00001040: 2020 2020 2e2e 2e0a 2020 2020 7572 6c28      ....    url(
+00001050: 275e 696e 626f 782f 6e6f 7469 6669 6361  '^inbox/notifica
+00001060: 7469 6f6e 732f 272c 2069 6e63 6c75 6465  tions/', include
+00001070: 286e 6f74 6966 6963 6174 696f 6e73 2e75  (notifications.u
+00001080: 726c 732c 206e 616d 6573 7061 6365 3d27  rls, namespace='
+00001090: 6e6f 7469 6669 6361 7469 6f6e 7327 2929  notifications'))
+000010a0: 2c0a 2020 2020 2e2e 2e0a 5d0a 6060 600a  ,.    ....].```.
+000010b0: 0a54 6865 206d 6574 686f 6420 6f66 2069  .The method of i
+000010c0: 6e73 7461 6c6c 696e 6720 7468 6573 6520  nstalling these 
+000010d0: 7572 6c73 2c20 696d 706f 7274 696e 6720  urls, importing 
+000010e0: 7261 7468 6572 2074 6861 6e20 7573 696e  rather than usin
+000010f0: 670a 6027 6e6f 7469 6669 6361 7469 6f6e  g.`'notification
+00001100: 732e 7572 6c73 2760 2c20 6973 2072 6571  s.urls'`, is req
+00001110: 7569 7265 6420 746f 2065 6e73 7572 6520  uired to ensure 
+00001120: 7468 6174 2074 6865 2075 726c 7320 6172  that the urls ar
+00001130: 650a 696e 7374 616c 6c65 6420 696e 2074  e.installed in t
+00001140: 6865 2060 6e6f 7469 6669 6361 7469 6f6e  he `notification
+00001150: 7360 206e 616d 6573 7061 6365 2e0a 0a54  s` namespace...T
+00001160: 6f20 7275 6e20 7363 6865 6d61 206d 6967  o run schema mig
+00001170: 7261 7469 6f6e 2c20 6578 6563 7574 650a  ration, execute.
+00001180: 6070 7974 686f 6e20 6d61 6e61 6765 2e70  `python manage.p
+00001190: 7920 6d69 6772 6174 6520 6e6f 7469 6669  y migrate notifi
+000011a0: 6361 7469 6f6e 7360 2e0a 0a23 2320 4765  cations`...## Ge
+000011b0: 6e65 7261 7469 6e67 204e 6f74 6966 6963  nerating Notific
+000011c0: 6174 696f 6e73 0a0a 4765 6e65 7261 7469  ations..Generati
+000011d0: 6e67 206e 6f74 6966 6963 6174 696f 6e73  ng notifications
+000011e0: 2069 7320 7072 6f62 6162 6c79 2062 6573   is probably bes
+000011f0: 7420 646f 6e65 2069 6e20 6120 7365 7061  t done in a sepa
+00001200: 7261 7465 2073 6967 6e61 6c2e 0a0a 6060  rate signal...``
+00001210: 6070 7974 686f 6e0a 6672 6f6d 2064 6a61  `python.from dja
+00001220: 6e67 6f2e 6462 2e6d 6f64 656c 732e 7369  ngo.db.models.si
+00001230: 676e 616c 7320 696d 706f 7274 2070 6f73  gnals import pos
+00001240: 745f 7361 7665 0a66 726f 6d20 6e6f 7469  t_save.from noti
+00001250: 6669 6361 7469 6f6e 732e 7369 676e 616c  fications.signal
+00001260: 7320 696d 706f 7274 206e 6f74 6966 790a  s import notify.
+00001270: 6672 6f6d 206d 7961 7070 2e6d 6f64 656c  from myapp.model
+00001280: 7320 696d 706f 7274 204d 794d 6f64 656c  s import MyModel
+00001290: 0a0a 6465 6620 6d79 5f68 616e 646c 6572  ..def my_handler
+000012a0: 2873 656e 6465 722c 2069 6e73 7461 6e63  (sender, instanc
+000012b0: 652c 2063 7265 6174 6564 2c20 2a2a 6b77  e, created, **kw
+000012c0: 6172 6773 293a 0a20 2020 206e 6f74 6966  args):.    notif
+000012d0: 792e 7365 6e64 2869 6e73 7461 6e63 652c  y.send(instance,
+000012e0: 2076 6572 623d 2777 6173 2073 6176 6564   verb='was saved
+000012f0: 2729 0a0a 706f 7374 5f73 6176 652e 636f  ')..post_save.co
+00001300: 6e6e 6563 7428 6d79 5f68 616e 646c 6572  nnect(my_handler
+00001310: 2c20 7365 6e64 6572 3d4d 794d 6f64 656c  , sender=MyModel
+00001320: 290a 6060 600a 546f 2067 656e 6572 6174  ).```.To generat
+00001330: 6520 616e 206e 6f74 6966 6963 6174 696f  e an notificatio
+00001340: 6e20 616e 7977 6865 7265 2069 6e20 796f  n anywhere in yo
+00001350: 7572 2063 6f64 652c 2073 696d 706c 7920  ur code, simply 
+00001360: 696d 706f 7274 2074 6865 0a6e 6f74 6966  import the.notif
+00001370: 7920 7369 676e 616c 2061 6e64 2073 656e  y signal and sen
+00001380: 6420 6974 2077 6974 6820 796f 7572 2061  d it with your a
+00001390: 6374 6f72 2c20 7265 6369 7069 656e 742c  ctor, recipient,
+000013a0: 2061 6e64 2076 6572 622e 0a0a 6060 6070   and verb...```p
+000013b0: 7974 686f 6e0a 6672 6f6d 206e 6f74 6966  ython.from notif
+000013c0: 6963 6174 696f 6e73 2e73 6967 6e61 6c73  ications.signals
+000013d0: 2069 6d70 6f72 7420 6e6f 7469 6679 0a0a   import notify..
+000013e0: 6e6f 7469 6679 2e73 656e 6428 7573 6572  notify.send(user
+000013f0: 2c20 7265 6369 7069 656e 743d 7573 6572  , recipient=user
+00001400: 2c20 7665 7262 3d27 796f 7520 7265 6163  , verb='you reac
+00001410: 6865 6420 6c65 7665 6c20 3130 2729 0a60  hed level 10').`
+00001420: 6060 0a0a 5468 6520 636f 6d70 6c65 7465  ``..The complete
+00001430: 2073 796e 7461 7820 6973 2e0a 0a60 6060   syntax is...```
+00001440: 7079 7468 6f6e 0a6e 6f74 6966 792e 7365  python.notify.se
+00001450: 6e64 2861 6374 6f72 2c20 7265 6369 7069  nd(actor, recipi
+00001460: 656e 742c 2076 6572 622c 2061 6374 696f  ent, verb, actio
+00001470: 6e5f 6f62 6a65 6374 2c20 7461 7267 6574  n_object, target
+00001480: 2c20 6c65 7665 6c2c 2064 6573 6372 6970  , level, descrip
+00001490: 7469 6f6e 2c20 7075 626c 6963 2c20 7469  tion, public, ti
+000014a0: 6d65 7374 616d 702c 202a 2a6b 7761 7267  mestamp, **kwarg
+000014b0: 7329 0a60 6060 0a0a 4172 6775 6d65 6e74  s).```..Argument
+000014c0: 733a 0a0a 2d20 2020 2a2a 6163 746f 722a  s:..-   **actor*
+000014d0: 2a3a 2041 6e20 6f62 6a65 6374 206f 6620  *: An object of 
+000014e0: 616e 7920 7479 7065 2e20 2852 6571 7569  any type. (Requi
+000014f0: 7265 6429 204e 6f74 653a 2055 7365 0a20  red) Note: Use. 
+00001500: 2020 202a 2a73 656e 6465 722a 2a20 696e     **sender** in
+00001510: 7374 6561 6420 6f66 202a 2a61 6374 6f72  stead of **actor
+00001520: 2a2a 2069 6620 796f 7520 696e 7465 6e64  ** if you intend
+00001530: 2074 6f20 7573 6520 6b65 7977 6f72 640a   to use keyword.
+00001540: 2020 2020 6172 6775 6d65 6e74 730a 2d20      arguments.- 
+00001550: 2020 2a2a 7265 6369 7069 656e 742a 2a3a    **recipient**:
+00001560: 2041 202a 2a47 726f 7570 2a2a 206f 7220   A **Group** or 
+00001570: 6120 2a2a 5573 6572 2051 7565 7279 5365  a **User QuerySe
+00001580: 742a 2a20 6f72 2061 206c 6973 7420 6f66  t** or a list of
+00001590: 0a20 2020 202a 2a55 7365 722a 2a2e 2028  .    **User**. (
+000015a0: 5265 7175 6972 6564 290a 2d20 2020 2a2a  Required).-   **
+000015b0: 7665 7262 2a2a 3a20 416e 2073 7472 696e  verb**: An strin
+000015c0: 672e 2028 5265 7175 6972 6564 290a 2d20  g. (Required).- 
+000015d0: 2020 2a2a 6163 7469 6f6e 5c5f 6f62 6a65    **action\_obje
+000015e0: 6374 2a2a 3a20 416e 206f 626a 6563 7420  ct**: An object 
+000015f0: 6f66 2061 6e79 2074 7970 652e 2028 4f70  of any type. (Op
+00001600: 7469 6f6e 616c 290a 2d20 2020 2a2a 7461  tional).-   **ta
+00001610: 7267 6574 2a2a 3a20 416e 206f 626a 6563  rget**: An objec
+00001620: 7420 6f66 2061 6e79 2074 7970 652e 2028  t of any type. (
+00001630: 4f70 7469 6f6e 616c 290a 2d20 2020 2a2a  Optional).-   **
+00001640: 6c65 7665 6c2a 2a3a 204f 6e65 206f 6620  level**: One of 
+00001650: 4e6f 7469 6669 6361 7469 6f6e 2e4c 4556  Notification.LEV
+00001660: 454c 5320 285c 2773 7563 6365 7373 5c27  ELS (\'success\'
+00001670: 2c20 5c27 696e 666f 5c27 2c0a 2020 2020  , \'info\',.    
+00001680: 5c27 7761 726e 696e 675c 272c 205c 2765  \'warning\', \'e
+00001690: 7272 6f72 5c27 2920 2864 6566 6175 6c74  rror\') (default
+000016a0: 3d69 6e66 6f29 2e20 284f 7074 696f 6e61  =info). (Optiona
+000016b0: 6c29 0a2d 2020 202a 2a64 6573 6372 6970  l).-   **descrip
+000016c0: 7469 6f6e 2a2a 3a20 416e 2073 7472 696e  tion**: An strin
+000016d0: 672e 2028 4f70 7469 6f6e 616c 290a 2d20  g. (Optional).- 
+000016e0: 2020 2a2a 7075 626c 6963 2a2a 3a20 416e    **public**: An
+000016f0: 2062 6f6f 6c65 616e 2028 6465 6661 756c   boolean (defaul
+00001700: 743d 5472 7565 292e 2028 4f70 7469 6f6e  t=True). (Option
+00001710: 616c 290a 2d20 2020 2a2a 7469 6d65 7374  al).-   **timest
+00001720: 616d 702a 2a3a 2041 6e20 747a 696e 666f  amp**: An tzinfo
+00001730: 2028 6465 6661 756c 743d 7469 6d65 7a6f   (default=timezo
+00001740: 6e65 2e6e 6f77 2829 292e 2028 4f70 7469  ne.now()). (Opti
+00001750: 6f6e 616c 290a 0a23 2323 2045 7874 7261  onal)..### Extra
+00001760: 2064 6174 610a 0a59 6f75 2063 616e 2061   data..You can a
+00001770: 7474 6163 6820 6172 6269 7472 6172 7920  ttach arbitrary 
+00001780: 6461 7461 2074 6f20 796f 7572 206e 6f74  data to your not
+00001790: 6966 6963 6174 696f 6e73 2062 7920 646f  ifications by do
+000017a0: 696e 6720 7468 650a 666f 6c6c 6f77 696e  ing the.followin
+000017b0: 673a 0a0a 2d20 2020 4164 6420 746f 2079  g:..-   Add to y
+000017c0: 6f75 7220 7365 7474 696e 6773 2e70 793a  our settings.py:
+000017d0: 0a20 2020 2060 444a 414e 474f 5f4e 4f54  .    `DJANGO_NOT
+000017e0: 4946 4943 4154 494f 4e53 5f43 4f4e 4649  IFICATIONS_CONFI
+000017f0: 4720 3d20 7b20 2755 5345 5f4a 534f 4e46  G = { 'USE_JSONF
+00001800: 4945 4c44 273a 2054 7275 657d 600a 0a54  IELD': True}`..T
+00001810: 6865 6e2c 2061 6e79 2065 7874 7261 2061  hen, any extra a
+00001820: 7267 756d 656e 7473 2079 6f75 2070 6173  rguments you pas
+00001830: 7320 746f 2060 6e6f 7469 6679 2e73 656e  s to `notify.sen
+00001840: 6428 2e2e 2e29 6020 7769 6c6c 2062 650a  d(...)` will be.
+00001850: 6174 7461 6368 6564 2074 6f20 7468 6520  attached to the 
+00001860: 602e 6461 7461 6020 6174 7472 6962 7574  `.data` attribut
+00001870: 6520 6f66 2074 6865 206e 6f74 6966 6963  e of the notific
+00001880: 6174 696f 6e20 6f62 6a65 6374 2e20 5468  ation object. Th
+00001890: 6573 6520 7769 6c6c 0a62 6520 7365 7269  ese will.be seri
+000018a0: 616c 6973 6564 2075 7369 6e67 2074 6865  alised using the
+000018b0: 204a 534f 4e46 6965 6c64 5c27 7320 7365   JSONField\'s se
+000018c0: 7269 616c 6973 6572 2c20 736f 2079 6f75  rialiser, so you
+000018d0: 206d 6179 206e 6565 6420 746f 2074 616b   may need to tak
+000018e0: 650a 7468 6174 2069 6e74 6f20 6163 636f  e.that into acco
+000018f0: 756e 743a 2075 7369 6e67 206f 6e6c 7920  unt: using only 
+00001900: 6f62 6a65 6374 7320 7468 6174 2077 696c  objects that wil
+00001910: 6c20 6265 2073 6572 6961 6c69 7365 6420  l be serialised 
+00001920: 6973 2061 2067 6f6f 640a 6964 6561 2e0a  is a good.idea..
+00001930: 0a23 2323 2053 6f66 7420 6465 6c65 7465  .### Soft delete
+00001940: 0a0a 4279 2064 6566 6175 6c74 2c20 6064  ..By default, `d
+00001950: 656c 6574 652f 283f 503c 736c 7567 3e5c  elete/(?P<slug>\
+00001960: 642b 292f 6020 6465 6c65 7465 7320 7370  d+)/` deletes sp
+00001970: 6563 6966 6965 6420 6e6f 7469 6669 6361  ecified notifica
+00001980: 7469 6f6e 0a72 6563 6f72 6420 6672 6f6d  tion.record from
+00001990: 2044 422e 2059 6f75 2063 616e 2063 6861   DB. You can cha
+000019a0: 6e67 6520 7468 6973 2062 6568 6176 696f  nge this behavio
+000019b0: 7572 2074 6f20 5c22 6d61 726b 0a60 4e6f  ur to \"mark.`No
+000019c0: 7469 6669 6361 7469 6f6e 2e64 656c 6574  tification.delet
+000019d0: 6564 6020 6669 656c 6420 6173 2060 5472  ed` field as `Tr
+000019e0: 7565 605c 2220 6279 3a0a 0a2d 2020 2041  ue`\" by:..-   A
+000019f0: 6464 2074 6f20 796f 7572 2073 6574 7469  dd to your setti
+00001a00: 6e67 732e 7079 3a0a 2020 2020 6044 4a41  ngs.py:.    `DJA
+00001a10: 4e47 4f5f 4e4f 5449 4649 4341 5449 4f4e  NGO_NOTIFICATION
+00001a20: 535f 434f 4e46 4947 203d 207b 2027 534f  S_CONFIG = { 'SO
+00001a30: 4654 5f44 454c 4554 4527 3a20 5472 7565  FT_DELETE': True
+00001a40: 7d60 0a0a 5769 7468 2074 6869 7320 6f70  }`..With this op
+00001a50: 7469 6f6e 2c20 5175 6572 7953 6574 206d  tion, QuerySet m
+00001a60: 6574 686f 6473 2060 756e 7265 6164 6020  ethods `unread` 
+00001a70: 616e 6420 6072 6561 6460 2063 6f6e 7461  and `read` conta
+00001a80: 696e 206f 6e65 206d 6f72 650a 6669 6c74  in one more.filt
+00001a90: 6572 3a20 6064 656c 6574 6564 3d46 616c  er: `deleted=Fal
+00001aa0: 7365 602e 204d 6561 6e77 6869 6c65 2c20  se`. Meanwhile, 
+00001ab0: 5175 6572 7953 6574 206d 6574 686f 6473  QuerySet methods
+00001ac0: 2060 6465 6c65 7465 6460 2c0a 6061 6374   `deleted`,.`act
+00001ad0: 6976 6560 2c20 606d 6172 6b5f 616c 6c5f  ive`, `mark_all_
+00001ae0: 6173 5f64 656c 6574 6564 602c 2060 6d61  as_deleted`, `ma
+00001af0: 726b 5f61 6c6c 5f61 735f 6163 7469 7665  rk_all_as_active
+00001b00: 6020 6172 6520 7475 726e 6564 206f 6e2e  ` are turned on.
+00001b10: 2053 6565 0a6d 6f72 6520 6465 7461 696c   See.more detail
+00001b20: 7320 696e 2051 7565 7279 5365 7420 6d65  s in QuerySet me
+00001b30: 7468 6f64 7320 7365 6374 696f 6e2e 0a0a  thods section...
+00001b40: 2323 2041 5049 0a0a 2323 2320 5175 6572  ## API..### Quer
+00001b50: 7953 6574 206d 6574 686f 6473 0a0a 5573  ySet methods..Us
+00001b60: 696e 6720 6064 6a61 6e67 6f2d 6d6f 6465  ing `django-mode
+00001b70: 6c2d 7574 696c 7360 2c20 7765 2067 6574  l-utils`, we get
+00001b80: 2074 6865 2061 6269 6c69 7479 2074 6f20   the ability to 
+00001b90: 6164 6420 7175 6572 7973 6574 206d 6574  add queryset met
+00001ba0: 686f 6473 0a74 6f20 6e6f 7420 6f6e 6c79  hods.to not only
+00001bb0: 2074 6865 206d 616e 6167 6572 2c20 6275   the manager, bu
+00001bc0: 7420 746f 2061 6c6c 2071 7565 7279 7365  t to all queryse
+00001bd0: 7473 2074 6861 7420 7769 6c6c 2062 6520  ts that will be 
+00001be0: 7573 6564 2c0a 696e 636c 7564 696e 6720  used,.including 
+00001bf0: 7265 6c61 7465 6420 6f62 6a65 6374 732e  related objects.
+00001c00: 2054 6869 7320 656e 6162 6c65 7320 7573   This enables us
+00001c10: 2074 6f20 646f 2074 6869 6e67 7320 6c69   to do things li
+00001c20: 6b65 3a0a 0a60 6060 7079 7468 6f6e 0a20  ke:..```python. 
+00001c30: 2020 204e 6f74 6966 6963 6174 696f 6e2e     Notification.
+00001c40: 6f62 6a65 6374 732e 756e 7265 6164 2829  objects.unread()
+00001c50: 0a60 6060 0a0a 7768 6963 6820 7265 7475  .```..which retu
+00001c60: 726e 7320 616c 6c20 756e 7265 6164 206e  rns all unread n
+00001c70: 6f74 6966 6963 6174 696f 6e73 2e20 546f  otifications. To
+00001c80: 2064 6f20 7468 6973 2066 6f72 2061 2073   do this for a s
+00001c90: 696e 676c 6520 7573 6572 2c20 7765 0a63  ingle user, we.c
+00001ca0: 616e 2064 6f3a 0a0a 6060 6070 7974 686f  an do:..```pytho
+00001cb0: 6e0a 2020 2020 7573 6572 203d 2055 7365  n.    user = Use
+00001cc0: 722e 6f62 6a65 6374 732e 6765 7428 706b  r.objects.get(pk
+00001cd0: 3d70 6b29 0a20 2020 2075 7365 722e 6e6f  =pk).    user.no
+00001ce0: 7469 6669 6361 7469 6f6e 732e 756e 7265  tifications.unre
+00001cf0: 6164 2829 0a60 6060 0a0a 5468 6572 6520  ad().```..There 
+00001d00: 6172 6520 736f 6d65 206f 7468 6572 2051  are some other Q
+00001d10: 7565 7279 5365 7420 6d65 7468 6f64 732c  uerySet methods,
+00001d20: 2074 6f6f 2e0a 0a23 2323 2320 6071 732e   too...#### `qs.
+00001d30: 756e 7365 6e74 2829 600a 0a52 6574 7572  unsent()`..Retur
+00001d40: 6e20 616c 6c20 6f66 2074 6865 2075 6e73  n all of the uns
+00001d50: 656e 7420 6e6f 7469 6669 6361 7469 6f6e  ent notification
+00001d60: 732c 2066 696c 7465 7269 6e67 2074 6865  s, filtering the
+00001d70: 2063 7572 7265 6e74 2071 7565 7279 7365   current queryse
+00001d80: 742e 0a28 656d 6169 6c65 643d 4661 6c73  t..(emailed=Fals
+00001d90: 6529 0a0a 2323 2323 2060 7173 2e73 656e  e)..#### `qs.sen
+00001da0: 7428 2960 0a0a 5265 7475 726e 2061 6c6c  t()`..Return all
+00001db0: 206f 6620 7468 6520 7365 6e74 206e 6f74   of the sent not
+00001dc0: 6966 6963 6174 696f 6e73 2c20 6669 6c74  ifications, filt
+00001dd0: 6572 696e 6720 7468 6520 6375 7272 656e  ering the curren
+00001de0: 7420 7175 6572 7973 6574 2e0a 2865 6d61  t queryset..(ema
+00001df0: 696c 6564 3d54 7275 6529 0a0a 2323 2323  iled=True)..####
+00001e00: 2060 7173 2e75 6e72 6561 6428 2960 0a0a   `qs.unread()`..
+00001e10: 5265 7475 726e 2061 6c6c 206f 6620 7468  Return all of th
+00001e20: 6520 756e 7265 6164 206e 6f74 6966 6963  e unread notific
+00001e30: 6174 696f 6e73 2c20 6669 6c74 6572 696e  ations, filterin
+00001e40: 6720 7468 6520 6375 7272 656e 7420 7175  g the current qu
+00001e50: 6572 7973 6574 2e0a 5768 656e 2060 534f  eryset..When `SO
+00001e60: 4654 5f44 454c 4554 453d 5472 7565 602c  FT_DELETE=True`,
+00001e70: 2074 6869 7320 6669 6c74 6572 2063 6f6e   this filter con
+00001e80: 7461 696e 7320 6064 656c 6574 6564 3d46  tains `deleted=F
+00001e90: 616c 7365 602e 0a0a 2323 2323 2060 7173  alse`...#### `qs
+00001ea0: 2e72 6561 6428 2960 0a0a 5265 7475 726e  .read()`..Return
+00001eb0: 2061 6c6c 206f 6620 7468 6520 7265 6164   all of the read
+00001ec0: 206e 6f74 6966 6963 6174 696f 6e73 2c20   notifications, 
+00001ed0: 6669 6c74 6572 696e 6720 7468 6520 6375  filtering the cu
+00001ee0: 7272 656e 7420 7175 6572 7973 6574 2e0a  rrent queryset..
+00001ef0: 5768 656e 2060 534f 4654 5f44 454c 4554  When `SOFT_DELET
+00001f00: 453d 5472 7565 602c 2074 6869 7320 6669  E=True`, this fi
+00001f10: 6c74 6572 2063 6f6e 7461 696e 7320 6064  lter contains `d
+00001f20: 656c 6574 6564 3d46 616c 7365 602e 0a0a  eleted=False`...
+00001f30: 2323 2323 2060 7173 2e6d 6172 6b5f 616c  #### `qs.mark_al
+00001f40: 6c5f 6173 5f72 6561 6428 2960 205c 7c20  l_as_read()` \| 
+00001f50: 6071 732e 6d61 726b 5f61 6c6c 5f61 735f  `qs.mark_all_as_
+00001f60: 7265 6164 2872 6563 6970 6965 6e74 2960  read(recipient)`
+00001f70: 0a0a 4d61 726b 2061 6c6c 206f 6620 7468  ..Mark all of th
+00001f80: 6520 756e 7265 6164 206e 6f74 6966 6963  e unread notific
+00001f90: 6174 696f 6e73 2069 6e20 7468 6520 7175  ations in the qu
+00001fa0: 6572 7973 6574 2028 6f70 7469 6f6e 616c  eryset (optional
+00001fb0: 6c79 2061 6c73 6f0a 6669 6c74 6572 6564  ly also.filtered
+00001fc0: 2062 7920 6072 6563 6970 6965 6e74 6029   by `recipient`)
+00001fd0: 2061 7320 7265 6164 2e0a 0a23 2323 2320   as read...#### 
+00001fe0: 6071 732e 6d61 726b 5f61 6c6c 5f61 735f  `qs.mark_all_as_
+00001ff0: 756e 7265 6164 2829 6020 5c7c 2060 7173  unread()` \| `qs
+00002000: 2e6d 6172 6b5f 616c 6c5f 6173 5f75 6e72  .mark_all_as_unr
+00002010: 6561 6428 7265 6369 7069 656e 7429 600a  ead(recipient)`.
+00002020: 0a4d 6172 6b20 616c 6c20 6f66 2074 6865  .Mark all of the
+00002030: 2072 6561 6420 6e6f 7469 6669 6361 7469   read notificati
+00002040: 6f6e 7320 696e 2074 6865 2071 7565 7279  ons in the query
+00002050: 7365 7420 286f 7074 696f 6e61 6c6c 7920  set (optionally 
+00002060: 616c 736f 0a66 696c 7465 7265 6420 6279  also.filtered by
+00002070: 2060 7265 6369 7069 656e 7460 2920 6173   `recipient`) as
+00002080: 2075 6e72 6561 642e 0a0a 2323 2323 2060   unread...#### `
+00002090: 7173 2e6d 6172 6b5f 6173 5f73 656e 7428  qs.mark_as_sent(
+000020a0: 2960 205c 7c20 6071 732e 6d61 726b 5f61  )` \| `qs.mark_a
+000020b0: 735f 7365 6e74 2872 6563 6970 6965 6e74  s_sent(recipient
+000020c0: 2960 0a0a 4d61 726b 2061 6c6c 206f 6620  )`..Mark all of 
+000020d0: 7468 6520 756e 7365 6e74 206e 6f74 6966  the unsent notif
+000020e0: 6963 6174 696f 6e73 2069 6e20 7468 6520  ications in the 
+000020f0: 7175 6572 7973 6574 2028 6f70 7469 6f6e  queryset (option
+00002100: 616c 6c79 2061 6c73 6f0a 6669 6c74 6572  ally also.filter
+00002110: 6564 2062 7920 6072 6563 6970 6965 6e74  ed by `recipient
+00002120: 6029 2061 7320 7365 6e74 2e0a 0a23 2323  `) as sent...###
+00002130: 2320 6071 732e 6d61 726b 5f61 735f 756e  # `qs.mark_as_un
+00002140: 7365 6e74 2829 6020 5c7c 2060 7173 2e6d  sent()` \| `qs.m
+00002150: 6172 6b5f 6173 5f75 6e73 656e 7428 7265  ark_as_unsent(re
+00002160: 6369 7069 656e 7429 600a 0a4d 6172 6b20  cipient)`..Mark 
+00002170: 616c 6c20 6f66 2074 6865 2073 656e 7420  all of the sent 
+00002180: 6e6f 7469 6669 6361 7469 6f6e 7320 696e  notifications in
+00002190: 2074 6865 2071 7565 7279 7365 7420 286f   the queryset (o
+000021a0: 7074 696f 6e61 6c6c 7920 616c 736f 0a66  ptionally also.f
+000021b0: 696c 7465 7265 6420 6279 2060 7265 6369  iltered by `reci
+000021c0: 7069 656e 7460 2920 6173 2075 6e73 656e  pient`) as unsen
+000021d0: 742e 0a0a 2323 2323 2060 7173 2e64 656c  t...#### `qs.del
+000021e0: 6574 6564 2829 600a 0a52 6574 7572 6e20  eted()`..Return 
+000021f0: 616c 6c20 6e6f 7469 6669 6361 7469 6f6e  all notification
+00002200: 7320 7468 6174 2068 6176 6520 6064 656c  s that have `del
+00002210: 6574 6564 3d54 7275 6560 2c20 6669 6c74  eted=True`, filt
+00002220: 6572 696e 6720 7468 6520 6375 7272 656e  ering the curren
+00002230: 740a 7175 6572 7973 6574 2e20 4d75 7374  t.queryset. Must
+00002240: 2062 6520 7573 6564 2077 6974 6820 6053   be used with `S
+00002250: 4f46 545f 4445 4c45 5445 3d54 7275 6560  OFT_DELETE=True`
+00002260: 2e0a 0a23 2323 2320 6071 732e 6163 7469  ...#### `qs.acti
+00002270: 7665 2829 600a 0a52 6574 7572 6e20 616c  ve()`..Return al
+00002280: 6c20 6e6f 7469 6669 6361 7469 6f6e 7320  l notifications 
+00002290: 7468 6174 2068 6176 6520 6064 656c 6574  that have `delet
+000022a0: 6564 3d46 616c 7365 602c 2066 696c 7465  ed=False`, filte
+000022b0: 7269 6e67 2074 6865 0a63 7572 7265 6e74  ring the.current
+000022c0: 2071 7565 7279 7365 742e 204d 7573 7420   queryset. Must 
+000022d0: 6265 2075 7365 6420 7769 7468 2060 4445  be used with `DE
+000022e0: 4c45 5445 3d54 7275 6560 2e0a 0a23 2323  LETE=True`...###
+000022f0: 2320 6071 732e 6d61 726b 5f61 6c6c 5f61  # `qs.mark_all_a
+00002300: 735f 6465 6c65 7465 6428 2960 205c 7c20  s_deleted()` \| 
+00002310: 6071 732e 6d61 726b 5f61 6c6c 5f61 735f  `qs.mark_all_as_
+00002320: 6465 6c65 7465 6428 7265 6369 7069 656e  deleted(recipien
+00002330: 7429 600a 0a4d 6172 6b20 616c 6c20 6e6f  t)`..Mark all no
+00002340: 7469 6669 6361 7469 6f6e 7320 696e 2074  tifications in t
+00002350: 6865 2071 7565 7279 7365 7420 286f 7074  he queryset (opt
+00002360: 696f 6e61 6c6c 7920 616c 736f 2066 696c  ionally also fil
+00002370: 7465 7265 6420 6279 0a60 7265 6369 7069  tered by.`recipi
+00002380: 656e 7460 2920 6173 2060 6465 6c65 7465  ent`) as `delete
+00002390: 643d 5472 7565 602e 204d 7573 7420 6265  d=True`. Must be
+000023a0: 2075 7365 6420 7769 7468 2060 4445 4c45   used with `DELE
+000023b0: 5445 3d54 7275 6560 2e0a 0a23 2323 2320  TE=True`...#### 
+000023c0: 6071 732e 6d61 726b 5f61 6c6c 5f61 735f  `qs.mark_all_as_
+000023d0: 6163 7469 7665 2829 6020 5c7c 2060 7173  active()` \| `qs
+000023e0: 2e6d 6172 6b5f 616c 6c5f 6173 5f61 6374  .mark_all_as_act
+000023f0: 6976 6528 7265 6369 7069 656e 7429 600a  ive(recipient)`.
+00002400: 0a4d 6172 6b20 616c 6c20 6e6f 7469 6669  .Mark all notifi
+00002410: 6361 7469 6f6e 7320 696e 2074 6865 2071  cations in the q
+00002420: 7565 7279 7365 7420 286f 7074 696f 6e61  ueryset (optiona
+00002430: 6c6c 7920 616c 736f 2066 696c 7465 7265  lly also filtere
+00002440: 6420 6279 0a60 7265 6369 7069 656e 7460  d by.`recipient`
+00002450: 2920 6173 2060 6465 6c65 7465 643d 4661  ) as `deleted=Fa
+00002460: 6c73 6560 2e20 4d75 7374 2062 6520 7573  lse`. Must be us
+00002470: 6564 2077 6974 6820 6053 4f46 545f 4445  ed with `SOFT_DE
+00002480: 4c45 5445 3d54 7275 6560 2e0a 0a23 2323  LETE=True`...###
+00002490: 204d 6f64 656c 206d 6574 686f 6473 0a0a   Model methods..
+000024a0: 2323 2323 2060 6f62 6a2e 7469 6d65 7369  #### `obj.timesi
+000024b0: 6e63 6528 5b64 6174 6574 696d 655d 2960  nce([datetime])`
+000024c0: 0a0a 4120 7772 6170 7065 7220 666f 7220  ..A wrapper for 
+000024d0: 446a 616e 676f 5c27 7320 6074 696d 6573  Django\'s `times
+000024e0: 696e 6365 6020 6675 6e63 7469 6f6e 2e0a  ince` function..
+000024f0: 0a23 2323 2320 606f 626a 2e6d 6172 6b5f  .#### `obj.mark_
+00002500: 6173 5f72 6561 6428 2960 0a0a 4d61 726b  as_read()`..Mark
+00002510: 2074 6865 2063 7572 7265 6e74 206f 626a   the current obj
+00002520: 6563 7420 6173 2072 6561 642e 0a0a 2323  ect as read...##
+00002530: 2320 5465 6d70 6c61 7465 2074 6167 730a  # Template tags.
+00002540: 0a50 7574 2060 7b25 206c 6f61 6420 6e6f  .Put `{% load no
+00002550: 7469 6669 6361 7469 6f6e 735c 5f74 6167  tifications\_tag
+00002560: 7320 257d 6020 696e 2074 6865 2074 656d  s %}` in the tem
+00002570: 706c 6174 6520 6265 666f 7265 0a79 6f75  plate before.you
+00002580: 2061 6374 7561 6c6c 7920 7573 6520 6e6f   actually use no
+00002590: 7469 6669 6361 7469 6f6e 2074 6167 732e  tification tags.
+000025a0: 0a0a 2323 2320 606e 6f74 6966 6963 6174  ..### `notificat
+000025b0: 696f 6e73 5f75 6e72 6561 6460 0a0a 6060  ions_unread`..``
+000025c0: 6070 7974 686f 6e0a 2020 2020 7b25 206e  `python.    {% n
+000025d0: 6f74 6966 6963 6174 696f 6e73 5f75 6e72  otifications_unr
+000025e0: 6561 6420 257d 0a60 6060 0a0a 4769 7665  ead %}.```..Give
+000025f0: 2074 6865 206e 756d 6265 7220 6f66 2075   the number of u
+00002600: 6e72 6561 6420 6e6f 7469 6669 6361 7469  nread notificati
+00002610: 6f6e 7320 666f 7220 6120 7573 6572 2c20  ons for a user, 
+00002620: 6f72 206e 6f74 6869 6e67 2028 616e 2065  or nothing (an e
+00002630: 6d70 7479 0a73 7472 696e 6729 2066 6f72  mpty.string) for
+00002640: 2061 6e20 616e 6f6e 796d 6f75 7320 7573   an anonymous us
+00002650: 6572 2e0a 0a53 746f 7269 6e67 2074 6865  er...Storing the
+00002660: 2063 6f75 6e74 2069 6e20 6120 7661 7269   count in a vari
+00002670: 6162 6c65 2066 6f72 2066 7572 7468 6572  able for further
+00002680: 2070 726f 6365 7373 696e 6720 6973 2061   processing is a
+00002690: 6476 6973 6564 2c20 7375 6368 0a61 733a  dvised, such.as:
+000026a0: 0a0a 6060 6070 7974 686f 6e0a 2020 2020  ..```python.    
+000026b0: 7b25 206e 6f74 6966 6963 6174 696f 6e73  {% notifications
+000026c0: 5f75 6e72 6561 6420 6173 2075 6e72 6561  _unread as unrea
+000026d0: 645f 636f 756e 7420 257d 0a20 2020 202e  d_count %}.    .
+000026e0: 2e2e 0a20 2020 207b 2520 6966 2075 6e72  ...    {% if unr
+000026f0: 6561 645f 636f 756e 7420 257d 0a20 2020  ead_count %}.   
+00002700: 2020 2020 2059 6f75 2068 6176 6520 3c73       You have <s
+00002710: 7472 6f6e 673e 7b7b 2075 6e72 6561 645f  trong>{{ unread_
+00002720: 636f 756e 7420 7d7d 3c2f 7374 726f 6e67  count }}</strong
+00002730: 3e20 756e 7265 6164 206e 6f74 6966 6963  > unread notific
+00002740: 6174 696f 6e73 2e0a 2020 2020 7b25 2065  ations..    {% e
+00002750: 6e64 6966 2025 7d0a 6060 600a 0a23 2320  ndif %}.```..## 
+00002760: 4c69 7665 2d75 7064 6174 6572 2041 5049  Live-updater API
+00002770: 0a0a 546f 2065 6e73 7572 6520 7573 6572  ..To ensure user
+00002780: 7320 616c 7761 7973 2068 6176 6520 7468  s always have th
+00002790: 6520 6d6f 7374 2075 702d 746f 2d64 6174  e most up-to-dat
+000027a0: 6520 6e6f 7469 6669 6361 7469 6f6e 732c  e notifications,
+000027b0: 0a60 646a 616e 676f 2d6e 6f74 6966 6963  .`django-notific
+000027c0: 6174 696f 6e73 6020 696e 636c 7564 6573  ations` includes
+000027d0: 2061 2073 696d 706c 6520 6a61 7661 7363   a simple javasc
+000027e0: 7269 7074 2041 5049 2066 6f72 0a75 7064  ript API for.upd
+000027f0: 6174 696e 6720 7370 6563 6966 6963 2066  ating specific f
+00002800: 6965 6c64 7320 7769 7468 696e 2061 2064  ields within a d
+00002810: 6a61 6e67 6f20 7465 6d70 6c61 7465 2e0a  jango template..
+00002820: 0a54 6865 7265 2061 7265 2074 776f 2070  .There are two p
+00002830: 6f73 7369 626c 6520 4150 4920 6361 6c6c  ossible API call
+00002840: 7320 7468 6174 2063 616e 2062 6520 6d61  s that can be ma
+00002850: 6465 3a0a 0a31 2e20 2060 6170 692f 756e  de:..1.  `api/un
+00002860: 7265 6164 5f63 6f75 6e74 2f60 2074 6861  read_count/` tha
+00002870: 7420 7265 7475 726e 7320 6120 6a61 7661  t returns a java
+00002880: 7363 7269 7074 206f 626a 6563 7420 7769  script object wi
+00002890: 7468 2031 206b 6579 3a0a 2020 2020 6075  th 1 key:.    `u
+000028a0: 6e72 6561 645f 636f 756e 7460 2065 673a  nread_count` eg:
+000028b0: 0a0a 2020 2020 2020 2020 7b22 756e 7265  ..        {"unre
+000028c0: 6164 5f63 6f75 6e74 223a 317d 0a0a 322e  ad_count":1}..2.
+000028d0: 2020 6061 7069 2f75 6e72 6561 645f 6c69    `api/unread_li
+000028e0: 7374 2f60 2074 6861 7420 7265 7475 726e  st/` that return
+000028f0: 7320 6120 6a61 7661 7363 7269 7074 206f  s a javascript o
+00002900: 626a 6563 7420 7769 7468 2032 206b 6579  bject with 2 key
+00002910: 733a 0a20 2020 2060 756e 7265 6164 5f63  s:.    `unread_c
+00002920: 6f75 6e74 6020 616e 6420 6075 6e72 6561  ount` and `unrea
+00002930: 645f 6c69 7374 6020 6567 3a0a 0a20 2020  d_list` eg:..   
+00002940: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00002950: 2275 6e72 6561 645f 636f 756e 7422 3a31  "unread_count":1
+00002960: 2c0a 2020 2020 2020 2020 2022 756e 7265  ,.         "unre
+00002970: 6164 5f6c 6973 7422 3a5b 2d2d 6c69 7374  ad_list":[--list
+00002980: 206f 6620 6a73 6f6e 2072 6570 7265 7365   of json represe
+00002990: 6e74 6174 696f 6e73 206f 6620 6e6f 7469  ntations of noti
+000029a0: 6669 6361 7469 6f6e 732d 2d5d 0a20 2020  fications--].   
+000029b0: 2020 2020 207d 0a0a 2020 2020 5265 7072       }..    Repr
+000029c0: 6573 656e 7461 7469 6f6e 7320 6f66 206e  esentations of n
+000029d0: 6f74 6966 6963 6174 696f 6e73 2061 7265  otifications are
+000029e0: 2062 6173 6564 206f 6e20 7468 6520 646a   based on the dj
+000029f0: 616e 676f 206d 6574 686f 643a 0a20 2020  ango method:.   
+00002a00: 2060 6d6f 6465 6c5f 746f 5f64 6963 7460   `model_to_dict`
+00002a10: 0a0a 2020 2020 5175 6572 7920 7374 7269  ..    Query stri
+00002a20: 6e67 2061 7267 756d 656e 7473 3a0a 0a20  ng arguments:.. 
+00002a30: 2020 202d 2020 202a 2a6d 6178 2a2a 202d     -   **max** -
+00002a40: 206d 6178 696d 756d 206c 656e 6774 6820   maximum length 
+00002a50: 6f66 2075 6e72 6561 6420 6c69 7374 2e0a  of unread list..
+00002a60: 2020 2020 2d20 2020 2a2a 6d61 726b 5c5f      -   **mark\_
+00002a70: 6173 5c5f 7265 6164 2a2a 202d 206d 6172  as\_read** - mar
+00002a80: 6b20 6e6f 7469 6669 6361 7469 6f6e 2069  k notification i
+00002a90: 6e20 6c69 7374 2061 7320 7265 6164 2e0a  n list as read..
+00002aa0: 0a20 2020 2046 6f72 2065 7861 6d70 6c65  .    For example
+00002ab0: 2c20 6765 7420 6061 7069 2f75 6e72 6561  , get `api/unrea
+00002ac0: 645f 6c69 7374 2f3f 6d61 783d 3326 6d61  d_list/?max=3&ma
+00002ad0: 726b 5f61 735f 7265 6164 3d74 7275 6560  rk_as_read=true`
+00002ae0: 2072 6574 7572 6e73 0a20 2020 2033 206e   returns.    3 n
+00002af0: 6f74 6966 6963 6174 696f 6e73 2061 6e64  otifications and
+00002b00: 206d 6172 6b20 7468 656d 2072 6561 6420   mark them read 
+00002b10: 2872 656d 6f76 6520 6672 6f6d 206c 6973  (remove from lis
+00002b20: 7420 6f6e 206e 6578 740a 2020 2020 7265  t on next.    re
+00002b30: 7175 6573 7429 2e0a 0a23 2323 2048 6f77  quest)...### How
+00002b40: 2074 6f20 7573 653a 0a0a 312e 2020 5075   to use:..1.  Pu
+00002b50: 7420 607b 2520 6c6f 6164 206e 6f74 6966  t `{% load notif
+00002b60: 6963 6174 696f 6e73 5f74 6167 7320 257d  ications_tags %}
+00002b70: 6020 696e 2074 6865 2074 656d 706c 6174  ` in the templat
+00002b80: 6520 6265 666f 7265 2079 6f75 0a20 2020  e before you.   
+00002b90: 2061 6374 7561 6c6c 7920 7573 6520 6e6f   actually use no
+00002ba0: 7469 6669 6361 7469 6f6e 2074 6167 732e  tification tags.
+00002bb0: 0a0a 322e 2020 496e 2074 6865 2061 7265  ..2.  In the are
+00002bc0: 6120 7768 6572 6520 796f 7520 6172 6520  a where you are 
+00002bd0: 6c6f 6164 696e 6720 6a61 7661 7363 7269  loading javascri
+00002be0: 7074 2072 6573 6f75 7263 6573 2061 6464  pt resources add
+00002bf0: 2074 6865 0a20 2020 2066 6f6c 6c6f 7769   the.    followi
+00002c00: 6e67 2074 6167 7320 696e 2074 6865 206f  ng tags in the o
+00002c10: 7264 6572 2062 656c 6f77 3a0a 0a20 2020  rder below:..   
+00002c20: 2020 2020 203c 7363 7269 7074 2073 7263       <script src
+00002c30: 3d22 7b25 2073 7461 7469 6320 276e 6f74  ="{% static 'not
+00002c40: 6966 6963 6174 696f 6e73 2f6e 6f74 6966  ifications/notif
+00002c50: 792e 6a73 2720 257d 2220 7479 7065 3d22  y.js' %}" type="
+00002c60: 7465 7874 2f6a 6176 6173 6372 6970 7422  text/javascript"
+00002c70: 3e3c 2f73 6372 6970 743e 0a20 2020 2020  ></script>.     
+00002c80: 2020 207b 2520 7265 6769 7374 6572 5f6e     {% register_n
+00002c90: 6f74 6966 795f 6361 6c6c 6261 636b 7320  otify_callbacks 
+00002ca0: 6361 6c6c 6261 636b 733d 2766 696c 6c5f  callbacks='fill_
+00002cb0: 6e6f 7469 6669 6361 7469 6f6e 5f6c 6973  notification_lis
+00002cc0: 742c 6669 6c6c 5f6e 6f74 6966 6963 6174  t,fill_notificat
+00002cd0: 696f 6e5f 6261 6467 6527 2025 7d0a 0a20  ion_badge' %}.. 
+00002ce0: 2020 2060 7265 6769 7374 6572 5f6e 6f74     `register_not
+00002cf0: 6966 795f 6361 6c6c 6261 636b 7360 2074  ify_callbacks` t
+00002d00: 616b 6573 2074 6865 2066 6f6c 6c6f 7769  akes the followi
+00002d10: 6e67 2061 7267 756d 656e 7473 3a0a 0a20  ng arguments:.. 
+00002d20: 2020 2031 2e20 2060 6261 6467 655f 636c     1.  `badge_cl
+00002d30: 6173 7360 2028 6465 6661 756c 7420 606c  ass` (default `l
+00002d40: 6976 655f 6e6f 7469 6679 5f62 6164 6765  ive_notify_badge
+00002d50: 6029 202d 2054 6865 2069 6465 6e74 6966  `) - The identif
+00002d60: 6965 720a 2020 2020 2020 2020 6063 6c61  ier.        `cla
+00002d70: 7373 6020 6f66 2074 6865 2065 6c65 6d65  ss` of the eleme
+00002d80: 6e74 2074 6f20 7368 6f77 2074 6865 2075  nt to show the u
+00002d90: 6e72 6561 6420 636f 756e 742c 0a20 2020  nread count,.   
+00002da0: 2020 2020 2074 6861 7420 7769 6c6c 2062       that will b
+00002db0: 6520 7065 7269 6f64 6963 616c 6c79 2075  e periodically u
+00002dc0: 7064 6174 6564 2e0a 2020 2020 322e 2020  pdated..    2.  
+00002dd0: 606d 656e 755f 636c 6173 7360 2028 6465  `menu_class` (de
+00002de0: 6661 756c 7420 606c 6976 655f 6e6f 7469  fault `live_noti
+00002df0: 6679 5f6c 6973 7460 2920 2d20 5468 6520  fy_list`) - The 
+00002e00: 6964 656e 7469 6669 6572 0a20 2020 2020  identifier.     
+00002e10: 2020 2060 636c 6173 7360 206f 6620 7468     `class` of th
+00002e20: 6520 656c 656d 656e 7420 746f 2069 6e73  e element to ins
+00002e30: 6572 7420 6120 6c69 7374 206f 6620 756e  ert a list of un
+00002e40: 7265 6164 0a20 2020 2020 2020 2069 7465  read.        ite
+00002e50: 6d73 2c20 7468 6174 2077 696c 6c20 6265  ms, that will be
+00002e60: 2070 6572 696f 6469 6361 6c6c 7920 7570   periodically up
+00002e70: 6461 7465 642e 0a20 2020 2033 2e20 2060  dated..    3.  `
+00002e80: 7265 6672 6573 685f 7065 7269 6f64 6020  refresh_period` 
+00002e90: 2864 6566 6175 6c74 2060 3135 6029 202d  (default `15`) -
+00002ea0: 2048 6f77 206f 6674 656e 2074 6f20 6665   How often to fe
+00002eb0: 7463 6820 756e 7265 6164 0a20 2020 2020  tch unread.     
+00002ec0: 2020 2069 7465 6d73 2066 726f 6d20 7468     items from th
+00002ed0: 6520 7365 7276 6572 2028 696e 7465 6765  e server (intege
+00002ee0: 7220 696e 2073 6563 6f6e 6473 292e 0a20  r in seconds).. 
+00002ef0: 2020 2034 2e20 2060 6665 7463 6860 2028     4.  `fetch` (
+00002f00: 6465 6661 756c 7420 6035 6029 202d 2048  default `5`) - H
+00002f10: 6f77 206d 616e 7920 6e6f 7469 6669 6361  ow many notifica
+00002f20: 7469 6f6e 7320 746f 2066 6574 6368 2065  tions to fetch e
+00002f30: 6163 680a 2020 2020 2020 2020 7469 6d65  ach.        time
+00002f40: 2e0a 2020 2020 352e 2020 6063 616c 6c62  ..    5.  `callb
+00002f50: 6163 6b73 6020 2864 6566 6175 6c74 2060  acks` (default `
+00002f60: 3c65 6d70 7479 2073 7472 696e 673e 6029  <empty string>`)
+00002f70: 202d 2041 2063 6f6d 6d61 2d73 6570 6172   - A comma-separ
+00002f80: 6174 6564 206c 6973 740a 2020 2020 2020  ated list.      
+00002f90: 2020 6f66 206a 6176 6173 6372 6970 7420    of javascript 
+00002fa0: 6675 6e63 7469 6f6e 7320 746f 2063 616c  functions to cal
+00002fb0: 6c20 6561 6368 2070 6572 696f 642e 0a20  l each period.. 
+00002fc0: 2020 2036 2e20 2060 6170 695f 6e61 6d65     6.  `api_name
+00002fd0: 6020 2864 6566 6175 6c74 2060 6c69 7374  ` (default `list
+00002fe0: 6029 202d 2054 6865 206e 616d 6520 6f66  `) - The name of
+00002ff0: 2074 6865 2041 5049 2074 6f20 6361 6c6c   the API to call
+00003000: 2028 7468 6973 0a20 2020 2020 2020 2063   (this.        c
+00003010: 616e 2062 6520 6569 7468 6572 2060 6c69  an be either `li
+00003020: 7374 6020 6f72 2060 636f 756e 7460 292e  st` or `count`).
+00003030: 0a20 2020 2037 2e20 6060 6d61 726b 5f61  .    7. ``mark_a
+00003040: 735f 7265 6164 6060 2028 6465 6661 756c  s_read`` (defaul
+00003050: 7420 6060 4661 6c73 6560 6029 202d 204d  t ``False``) - M
+00003060: 6172 6b73 206e 6f74 6966 6963 6174 696f  arks notificatio
+00003070: 6e73 2061 7320 7265 6164 2077 6865 6e20  ns as read when 
+00003080: 6665 7463 6865 642e 0a0a 332e 2020 546f  fetched...3.  To
+00003090: 2069 6e73 6572 7420 6120 6c69 7665 2d75   insert a live-u
+000030a0: 7064 6174 696e 6720 756e 7265 6164 2063  pdating unread c
+000030b0: 6f75 6e74 2c20 7573 6520 7468 6520 666f  ount, use the fo
+000030c0: 6c6c 6f77 696e 6720 7465 6d70 6c61 7465  llowing template
+000030d0: 3a0a 0a20 2020 2020 2020 207b 2520 6c69  :..        {% li
+000030e0: 7665 5f6e 6f74 6966 795f 6261 6467 6520  ve_notify_badge 
+000030f0: 257d 0a0a 2020 2020 606c 6976 655f 6e6f  %}..    `live_no
+00003100: 7469 6679 5f62 6164 6765 6020 7461 6b65  tify_badge` take
+00003110: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
+00003120: 6172 6775 6d65 6e74 733a 0a0a 2020 2020  arguments:..    
+00003130: 2d20 2060 6261 6467 655f 636c 6173 7360  -  `badge_class`
+00003140: 2028 6465 6661 756c 7420 606c 6976 655f   (default `live_
+00003150: 6e6f 7469 6679 5f62 6164 6765 6029 202d  notify_badge`) -
+00003160: 2054 6865 2069 6465 6e74 6966 6965 720a   The identifier.
+00003170: 2020 2020 2020 2020 6063 6c61 7373 6020          `class` 
+00003180: 666f 7220 7468 6520 603c 7370 616e 3e60  for the `<span>`
+00003190: 2065 6c65 6d65 6e74 2074 6861 7420 7769   element that wi
+000031a0: 6c6c 2062 6520 6372 6561 7465 6420 746f  ll be created to
+000031b0: 2073 686f 770a 2020 2020 2020 2020 7468   show.        th
+000031c0: 6520 756e 7265 6164 2063 6f75 6e74 2e0a  e unread count..
+000031d0: 0a34 2e20 2054 6f20 696e 7365 7274 2061  .4.  To insert a
+000031e0: 206c 6976 652d 7570 6461 7469 6e67 2075   live-updating u
+000031f0: 6e72 6561 6420 6c69 7374 2c20 7573 6520  nread list, use 
+00003200: 7468 6520 666f 6c6c 6f77 696e 6720 7465  the following te
+00003210: 6d70 6c61 7465 3a0a 0a20 2020 2020 2020  mplate:..       
+00003220: 207b 2520 6c69 7665 5f6e 6f74 6966 795f   {% live_notify_
+00003230: 6c69 7374 2025 7d0a 0a20 2020 2060 6c69  list %}..    `li
+00003240: 7665 5f6e 6f74 6966 795f 6c69 7374 6020  ve_notify_list` 
+00003250: 7461 6b65 7320 7468 6520 666f 6c6c 6f77  takes the follow
+00003260: 696e 6720 6172 6775 6d65 6e74 733a 0a0a  ing arguments:..
+00003270: 2020 2020 2d20 2060 6c69 7374 5f63 6c61      -  `list_cla
+00003280: 7373 6020 2864 6566 6175 6c74 2060 6c69  ss` (default `li
+00003290: 7665 5f6e 6f74 6966 795f 6c69 7374 6029  ve_notify_list`)
+000032a0: 202d 2054 6865 2069 6465 6e74 6966 6965   - The identifie
+000032b0: 720a 2020 2020 2020 2020 6063 6c61 7373  r.        `class
+000032c0: 6020 666f 7220 7468 6520 603c 756c 3e60  ` for the `<ul>`
+000032d0: 2065 6c65 6d65 6e74 2074 6861 7420 7769   element that wi
+000032e0: 6c6c 2062 6520 6372 6561 7465 6420 746f  ll be created to
+000032f0: 2069 6e73 6572 740a 2020 2020 2020 2020   insert.        
+00003300: 7468 6520 6c69 7374 206f 6620 6e6f 7469  the list of noti
+00003310: 6669 6361 7469 6f6e 7320 696e 746f 2e0a  fications into..
+00003320: 0a23 2323 2055 7369 6e67 2074 6865 206c  .### Using the l
+00003330: 6976 652d 7570 6461 7465 7220 7769 7468  ive-updater with
+00003340: 2062 6f6f 7473 7472 6170 0a0a 5468 6520   bootstrap..The 
+00003350: 4c69 7665 2d75 7064 6174 6572 2063 616e  Live-updater can
+00003360: 2062 6520 696e 636f 7270 6f72 6174 6564   be incorporated
+00003370: 2069 6e74 6f20 626f 6f74 7374 7261 7020   into bootstrap 
+00003380: 7769 7468 206d 696e 696d 616c 2063 6f64  with minimal cod
+00003390: 652e 0a0a 546f 2063 7265 6174 6520 6120  e...To create a 
+000033a0: 6c69 7665 2d75 7064 6174 696e 6720 626f  live-updating bo
+000033b0: 6f74 7374 7261 7020 6261 6467 6520 636f  otstrap badge co
+000033c0: 6e74 6169 6e69 6e67 2074 6865 2075 6e72  ntaining the unr
+000033d0: 6561 6420 636f 756e 742c 0a73 696d 706c  ead count,.simpl
+000033e0: 7920 7573 6520 7468 6520 7465 6d70 6c61  y use the templa
+000033f0: 7465 2074 6167 3a0a 0a20 2020 207b 2520  te tag:..    {% 
+00003400: 6c69 7665 5f6e 6f74 6966 795f 6261 6467  live_notify_badg
+00003410: 6520 6261 6467 655f 636c 6173 733d 2262  e badge_class="b
+00003420: 6164 6765 2220 257d 0a0a 546f 2063 7265  adge" %}..To cre
+00003430: 6174 6520 6120 6c69 7665 2d75 7064 6174  ate a live-updat
+00003440: 696e 6720 626f 6f74 7374 7261 7020 6472  ing bootstrap dr
+00003450: 6f70 646f 776e 206d 656e 7520 636f 6e74  opdown menu cont
+00003460: 6169 6e69 6e67 2061 2073 656c 6563 7469  aining a selecti
+00003470: 6f6e 0a6f 6620 7265 6365 6e74 2075 6e72  on.of recent unr
+00003480: 6561 6420 6e6f 7469 6669 6361 7469 6f6e  ead notification
+00003490: 732c 2073 696d 706c 7920 7573 6520 7468  s, simply use th
+000034a0: 6520 7465 6d70 6c61 7465 2074 6167 3a0a  e template tag:.
+000034b0: 0a20 2020 207b 2520 6c69 7665 5f6e 6f74  .    {% live_not
+000034c0: 6966 795f 6c69 7374 206c 6973 745f 636c  ify_list list_cl
+000034d0: 6173 733d 2264 726f 7064 6f77 6e2d 6d65  ass="dropdown-me
+000034e0: 6e75 2220 257d 0a0a 2323 2320 4375 7374  nu" %}..### Cust
+000034f0: 6f6d 6973 696e 6720 7468 6520 6469 7370  omising the disp
+00003500: 6c61 7920 6f66 206e 6f74 6966 6963 6174  lay of notificat
+00003510: 696f 6e73 2075 7369 6e67 206a 6176 6173  ions using javas
+00003520: 6372 6970 7420 6361 6c6c 6261 636b 730a  cript callbacks.
+00003530: 0a57 6869 6c65 2074 6865 206c 6976 6520  .While the live 
+00003540: 6e6f 7469 6669 6572 2066 6f72 2075 6e72  notifier for unr
+00003550: 6561 6420 636f 756e 7473 2073 686f 756c  ead counts shoul
+00003560: 6420 7375 6974 206d 6f73 7420 7573 6520  d suit most use 
+00003570: 6361 7365 732c 0a75 7365 7273 206d 6179  cases,.users may
+00003580: 2077 6973 6820 746f 2061 6c74 6572 2068   wish to alter h
+00003590: 6f77 2075 6e72 6561 6420 6e6f 7469 6669  ow unread notifi
+000035a0: 6361 7469 6f6e 7320 6172 6520 7368 6f77  cations are show
+000035b0: 6e2e 0a0a 5468 6520 6063 616c 6c62 6163  n...The `callbac
+000035c0: 6b73 6020 6172 6775 6d65 6e74 206f 6620  ks` argument of 
+000035d0: 7468 6520 6072 6567 6973 7465 725f 6e6f  the `register_no
+000035e0: 7469 6679 5f63 616c 6c62 6163 6b73 6020  tify_callbacks` 
+000035f0: 6469 6374 6174 6573 0a77 6869 6368 206a  dictates.which j
+00003600: 6176 6173 6372 6970 7420 6675 6e63 7469  avascript functi
+00003610: 6f6e 7320 6172 6520 6361 6c6c 6564 2077  ons are called w
+00003620: 6865 6e20 7468 6520 756e 7265 6164 2061  hen the unread a
+00003630: 7069 2063 616c 6c20 6973 206d 6164 652e  pi call is made.
+00003640: 0a0a 546f 2061 6464 2061 2063 7573 746f  ..To add a custo
+00003650: 6d20 6a61 7661 7363 7269 7074 2063 616c  m javascript cal
+00003660: 6c62 6163 6b2c 2073 696d 706c 7920 6164  lback, simply ad
+00003670: 6420 7468 6973 2074 6f20 7468 6520 6c69  d this to the li
+00003680: 7374 2c20 6c69 6b65 0a73 6f3a 0a0a 2020  st, like.so:..  
+00003690: 2020 7b25 2072 6567 6973 7465 725f 6e6f    {% register_no
+000036a0: 7469 6679 5f63 616c 6c62 6163 6b73 2063  tify_callbacks c
+000036b0: 616c 6c62 6163 6b73 3d27 6669 6c6c 5f6e  allbacks='fill_n
+000036c0: 6f74 6966 6963 6174 696f 6e5f 6261 6467  otification_badg
+000036d0: 652c 6d79 5f73 7065 6369 616c 5f6e 6f74  e,my_special_not
+000036e0: 6966 6963 6174 696f 6e5f 6361 6c6c 6261  ification_callba
+000036f0: 636b 2720 257d 0a0a 5468 6520 6162 6f76  ck' %}..The abov
+00003700: 6520 776f 756c 6420 6361 7573 6520 7468  e would cause th
+00003710: 6520 6361 6c6c 6261 636b 2074 6f20 7570  e callback to up
+00003720: 6461 7465 2074 6865 2075 6e72 6561 6420  date the unread 
+00003730: 636f 756e 7420 6261 6467 652c 2061 6e64  count badge, and
+00003740: 0a77 6f75 6c64 2063 616c 6c20 7468 6520  .would call the 
+00003750: 6375 7374 6f6d 2066 756e 6374 696f 6e0a  custom function.
+00003760: 606d 795f 7370 6563 6961 6c5f 6e6f 7469  `my_special_noti
+00003770: 6669 6361 7469 6f6e 5f63 616c 6c62 6163  fication_callbac
+00003780: 6b60 2e20 416c 6c20 6361 6c6c 6261 636b  k`. All callback
+00003790: 0a66 756e 6374 696f 6e73 2061 7265 2070  .functions are p
+000037a0: 6173 7365 6420 6120 7369 6e67 6c65 2061  assed a single a
+000037b0: 7267 756d 656e 7420 6279 2063 6f6e 7665  rgument by conve
+000037c0: 6e74 696f 6e20 6361 6c6c 6564 0a60 6461  ntion called.`da
+000037d0: 7461 602c 2077 6869 6368 2063 6f6e 7461  ta`, which conta
+000037e0: 696e 7320 7468 6520 656e 7469 7265 2072  ins the entire r
+000037f0: 6573 756c 7420 6672 6f6d 2074 6865 2041  esult from the A
+00003800: 5049 2e0a 0a46 6f72 2065 7861 6d70 6c65  PI...For example
+00003810: 2c20 7468 6520 6265 6c6f 7720 6675 6e63  , the below func
+00003820: 7469 6f6e 2077 6f75 6c64 2067 6574 2074  tion would get t
+00003830: 6865 2072 6563 656e 7420 6c69 7374 206f  he recent list o
+00003840: 6620 756e 7265 6164 0a6d 6573 7361 6765  f unread.message
+00003850: 7320 616e 6420 6c6f 6720 7468 656d 2074  s and log them t
+00003860: 6f20 7468 6520 636f 6e73 6f6c 653a 0a0a  o the console:..
+00003870: 6060 606a 6176 6173 6372 6970 740a 6675  ```javascript.fu
+00003880: 6e63 7469 6f6e 206d 795f 7370 6563 6961  nction my_specia
+00003890: 6c5f 6e6f 7469 6669 6361 7469 6f6e 5f63  l_notification_c
+000038a0: 616c 6c62 6163 6b28 6461 7461 2920 7b0a  allback(data) {.
+000038b0: 2020 2020 666f 7220 2876 6172 2069 3d30      for (var i=0
+000038c0: 3b20 6920 3c20 6461 7461 2e75 6e72 6561  ; i < data.unrea
+000038d0: 645f 6c69 7374 2e6c 656e 6774 683b 2069  d_list.length; i
+000038e0: 2b2b 2920 7b0a 2020 2020 2020 2020 6d73  ++) {.        ms
+000038f0: 6720 3d20 6461 7461 2e75 6e72 6561 645f  g = data.unread_
+00003900: 6c69 7374 5b69 5d3b 0a20 2020 2020 2020  list[i];.       
+00003910: 2063 6f6e 736f 6c65 2e6c 6f67 286d 7367   console.log(msg
+00003920: 293b 0a20 2020 207d 0a7d 0a60 6060 0a0a  );.    }.}.```..
+00003930: 2323 2320 5465 7374 696e 6720 7468 6520  ### Testing the 
+00003940: 6c69 7665 2d75 7064 6174 6572 0a0a 312e  live-updater..1.
+00003950: 2020 436c 6f6e 6520 7468 6520 7265 706f    Clone the repo
+00003960: 0a32 2e20 2052 756e 2060 2e2f 6d61 6e61  .2.  Run `./mana
+00003970: 6765 2e70 7920 7275 6e73 6572 7665 7260  ge.py runserver`
+00003980: 0a33 2e20 2042 726f 7773 6520 746f 2060  .3.  Browse to `
+00003990: 796f 7572 7365 7276 6572 6970 2f74 6573  yourserverip/tes
+000039a0: 742f 600a 342e 2020 436c 6963 6b20 5c27  t/`.4.  Click \'
+000039b0: 4d61 6b65 2061 206e 6f74 6966 6963 6174  Make a notificat
+000039c0: 696f 6e5c 2720 616e 6420 6120 6e65 7720  ion\' and a new 
+000039d0: 6e6f 7469 6669 6361 7469 6f6e 2073 686f  notification sho
+000039e0: 756c 6420 6170 7065 6172 0a20 2020 2069  uld appear.    i
+000039f0: 6e20 7468 6520 6c69 7374 2069 6e20 352d  n the list in 5-
+00003a00: 3130 2073 6563 6f6e 6473 2e0a 0a23 2320  10 seconds...## 
+00003a10: 5365 7269 616c 697a 696e 6720 7468 6520  Serializing the 
+00003a20: 646a 616e 676f 2d6e 6f74 6966 6963 6174  django-notificat
+00003a30: 696f 6e73 204d 6f64 656c 0a0a 5365 6520  ions Model..See 
+00003a40: 6865 7265 202d 203c 6874 7470 3a2f 2f77  here - <http://w
+00003a50: 7777 2e64 6a61 6e67 6f2d 7265 7374 2d66  ww.django-rest-f
+00003a60: 7261 6d65 776f 726b 2e6f 7267 2f61 7069  ramework.org/api
+00003a70: 2d67 7569 6465 2f72 656c 6174 696f 6e73  -guide/relations
+00003a80: 2f23 6765 6e65 7269 632d 7265 6c61 7469  /#generic-relati
+00003a90: 6f6e 7368 6970 733e 0a0a 496e 2074 6869  onships>..In thi
+00003aa0: 7320 6578 616d 706c 6520 7468 6520 7461  s example the ta
+00003ab0: 7267 6574 206f 626a 6563 7420 6361 6e20  rget object can 
+00003ac0: 6265 206f 6620 7479 7065 2046 6f6f 206f  be of type Foo o
+00003ad0: 7220 4261 7220 616e 6420 7468 650a 6170  r Bar and the.ap
+00003ae0: 7072 6f70 7269 6174 6520 7365 7269 616c  propriate serial
+00003af0: 697a 6572 2077 696c 6c20 6265 2075 7365  izer will be use
+00003b00: 642e 0a0a 6060 6070 7974 686f 6e0a 636c  d...```python.cl
+00003b10: 6173 7320 4765 6e65 7269 634e 6f74 6966  ass GenericNotif
+00003b20: 6963 6174 696f 6e52 656c 6174 6564 4669  icationRelatedFi
+00003b30: 656c 6428 7365 7269 616c 697a 6572 732e  eld(serializers.
+00003b40: 5265 6c61 7465 6446 6965 6c64 293a 0a0a  RelatedField):..
+00003b50: 2020 2020 6465 6620 746f 5f72 6570 7265      def to_repre
+00003b60: 7365 6e74 6174 696f 6e28 7365 6c66 2c20  sentation(self, 
+00003b70: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
+00003b80: 6966 2069 7369 6e73 7461 6e63 6528 7661  if isinstance(va
+00003b90: 6c75 652c 2046 6f6f 293a 0a20 2020 2020  lue, Foo):.     
+00003ba0: 2020 2020 2020 2073 6572 6961 6c69 7a65         serialize
+00003bb0: 7220 3d20 466f 6f53 6572 6961 6c69 7a65  r = FooSerialize
+00003bc0: 7228 7661 6c75 6529 0a20 2020 2020 2020  r(value).       
+00003bd0: 2069 6620 6973 696e 7374 616e 6365 2876   if isinstance(v
+00003be0: 616c 7565 2c20 4261 7229 3a0a 2020 2020  alue, Bar):.    
+00003bf0: 2020 2020 2020 2020 7365 7269 616c 697a          serializ
+00003c00: 6572 203d 2042 6172 5365 7269 616c 697a  er = BarSerializ
+00003c10: 6572 2876 616c 7565 290a 0a20 2020 2020  er(value)..     
+00003c20: 2020 2072 6574 7572 6e20 7365 7269 616c     return serial
+00003c30: 697a 6572 2e64 6174 610a 0a0a 636c 6173  izer.data...clas
+00003c40: 7320 4e6f 7469 6669 6361 7469 6f6e 5365  s NotificationSe
+00003c50: 7269 616c 697a 6572 2873 6572 6961 6c69  rializer(seriali
+00003c60: 7a65 7273 2e53 6572 6961 6c69 7a65 7229  zers.Serializer)
+00003c70: 3a0a 2020 2020 7265 6369 7069 656e 7420  :.    recipient 
+00003c80: 3d20 5075 626c 6963 5573 6572 5365 7269  = PublicUserSeri
+00003c90: 616c 697a 6572 2855 7365 722c 2072 6561  alizer(User, rea
+00003ca0: 645f 6f6e 6c79 3d54 7275 6529 0a20 2020  d_only=True).   
+00003cb0: 2075 6e72 6561 6420 3d20 7365 7269 616c   unread = serial
+00003cc0: 697a 6572 732e 426f 6f6c 6561 6e46 6965  izers.BooleanFie
+00003cd0: 6c64 2872 6561 645f 6f6e 6c79 3d54 7275  ld(read_only=Tru
+00003ce0: 6529 0a20 2020 2074 6172 6765 7420 3d20  e).    target = 
+00003cf0: 4765 6e65 7269 634e 6f74 6966 6963 6174  GenericNotificat
+00003d00: 696f 6e52 656c 6174 6564 4669 656c 6428  ionRelatedField(
+00003d10: 7265 6164 5f6f 6e6c 793d 5472 7565 290a  read_only=True).
+00003d20: 6060 600a 0a54 6861 6e6b 7320 746f 2040  ```..Thanks to @
+00003d30: 4461 5779 0a0a 2323 2320 6041 6273 7472  DaWy..### `Abstr
+00003d40: 6163 744e 6f74 6966 6963 6174 696f 6e60  actNotification`
+00003d50: 206d 6f64 656c 0a0a 496e 2063 6173 6520   model..In case 
+00003d60: 796f 7520 6e65 6564 2074 6f20 6375 7374  you need to cust
+00003d70: 6f6d 697a 6520 7468 6520 6e6f 7469 6669  omize the notifi
+00003d80: 6361 7469 6f6e 206d 6f64 656c 2069 6e20  cation model in 
+00003d90: 6f72 6465 7220 746f 2061 6464 0a66 6965  order to add.fie
+00003da0: 6c64 206f 7220 6375 7374 6f6d 6973 6564  ld or customised
+00003db0: 2066 6561 7475 7265 7320 7468 6174 2064   features that d
+00003dc0: 6570 656e 6420 6f6e 2079 6f75 7220 6170  epend on your ap
+00003dd0: 706c 6963 6174 696f 6e2c 2079 6f75 2063  plication, you c
+00003de0: 616e 0a69 6e68 6572 6974 2061 6e64 2065  an.inherit and e
+00003df0: 7874 656e 6420 7468 6520 6041 6273 7472  xtend the `Abstr
+00003e00: 6163 744e 6f74 6966 6963 6174 696f 6e60  actNotification`
+00003e10: 206d 6f64 656c 2c20 6578 616d 706c 653a   model, example:
+00003e20: 0a0a 6060 6070 7974 686f 6e0a 2349 6e20  ..```python.#In 
+00003e30: 796f 7572 5f61 7070 2f6d 6f64 656c 732e  your_app/models.
+00003e40: 7079 0a0a 6672 6f6d 2064 6a61 6e67 6f2e  py..from django.
+00003e50: 6462 2069 6d70 6f72 7420 6d6f 6465 6c73  db import models
+00003e60: 0a66 726f 6d20 6e6f 7469 6669 6361 7469  .from notificati
+00003e70: 6f6e 732e 6261 7365 2e6d 6f64 656c 7320  ons.base.models 
+00003e80: 696d 706f 7274 2041 6273 7472 6163 744e  import AbstractN
+00003e90: 6f74 6966 6963 6174 696f 6e0a 0a0a 636c  otification...cl
+00003ea0: 6173 7320 4e6f 7469 6669 6361 7469 6f6e  ass Notification
+00003eb0: 2841 6273 7472 6163 744e 6f74 6966 6963  (AbstractNotific
+00003ec0: 6174 696f 6e29 3a0a 2020 2020 2320 6375  ation):.    # cu
+00003ed0: 7374 6f6d 2066 6965 6c64 2065 7861 6d70  stom field examp
+00003ee0: 6c65 0a20 2020 2063 6174 6567 6f72 7920  le.    category 
+00003ef0: 3d20 6d6f 6465 6c73 2e46 6f72 6569 676e  = models.Foreign
+00003f00: 4b65 7928 276d 7961 7070 2e43 6174 6567  Key('myapp.Categ
+00003f10: 6f72 7927 2c0a 2020 2020 2020 2020 2020  ory',.          
+00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f30: 2020 2020 2020 206f 6e5f 6465 6c65 7465         on_delete
+00003f40: 3d6d 6f64 656c 732e 4341 5343 4144 4529  =models.CASCADE)
+00003f50: 0a0a 2020 2020 636c 6173 7320 4d65 7461  ..    class Meta
+00003f60: 2841 6273 7472 6163 744e 6f74 6966 6963  (AbstractNotific
+00003f70: 6174 696f 6e2e 4d65 7461 293a 0a20 2020  ation.Meta):.   
+00003f80: 2020 2020 2061 6273 7472 6163 7420 3d20       abstract = 
+00003f90: 4661 6c73 650a 6060 600a 0a59 6f75 2077  False.```..You w
+00003fa0: 696c 6c20 7265 7175 6972 6520 746f 2064  ill require to d
+00003fb0: 6566 696e 6520 604e 4f54 4946 4943 4154  efine `NOTIFICAT
+00003fc0: 494f 4e53 5f4e 4f54 4946 4943 4154 494f  IONS_NOTIFICATIO
+00003fd0: 4e5f 4d4f 4445 4c60 2073 6574 7469 6e67  N_MODEL` setting
+00003fe0: 2069 6e0a 6073 6574 7469 6e67 2e70 7960   in.`setting.py`
+00003ff0: 2061 7320 666f 6c6c 6f77 733a 0a0a 6060   as follows:..``
+00004000: 6070 7974 686f 6e0a 2320 496e 2079 6f75  `python.# In you
+00004010: 725f 7072 6f6a 6563 742f 7365 7474 696e  r_project/settin
+00004020: 6773 2e70 790a 0a4e 4f54 4946 4943 4154  gs.py..NOTIFICAT
+00004030: 494f 4e53 5f4e 4f54 4946 4943 4154 494f  IONS_NOTIFICATIO
+00004040: 4e5f 4d4f 4445 4c20 3d20 2779 6f75 725f  N_MODEL = 'your_
+00004050: 6170 702e 4e6f 7469 6669 6361 7469 6f6e  app.Notification
+00004060: 270a 6060 600a 0a23 2320 4e6f 7465 730a  '.```..## Notes.
+00004070: 0a23 2323 2045 6d61 696c 204e 6f74 6966  .### Email Notif
+00004080: 6963 6174 696f 6e0a 0a53 656e 6469 6e67  ication..Sending
+00004090: 2065 6d61 696c 2074 6f20 7573 6572 7320   email to users 
+000040a0: 6861 7320 6e6f 7420 6265 656e 2069 6e74  has not been int
+000040b0: 6567 7261 7465 6420 696e 746f 2074 6869  egrated into thi
+000040c0: 7320 6c69 6272 6172 792e 2053 6f20 666f  s library. So fo
+000040d0: 720a 6e6f 7720 796f 7520 6e65 6564 2074  r.now you need t
+000040e0: 6f20 696d 706c 656d 656e 7420 6974 2069  o implement it i
+000040f0: 6620 6e65 6564 6564 2e20 5468 6572 6520  f needed. There 
+00004100: 6973 2061 2072 6573 6572 7665 6420 6669  is a reserved fi
+00004110: 656c 640a 604e 6f74 6966 6963 6174 696f  eld.`Notificatio
+00004120: 6e2e 656d 6169 6c65 6460 2074 6f20 6d61  n.emailed` to ma
+00004130: 6b65 2069 7420 6561 7369 6572 2e0a 0a23  ke it easier...#
+00004140: 2323 2053 616d 706c 6520 4170 700a 0a41  ## Sample App..A
+00004150: 2073 616d 706c 6520 6170 7020 6861 7320   sample app has 
+00004160: 6265 656e 2069 6d70 6c65 6d65 6e74 6564  been implemented
+00004170: 2069 6e0a 606e 6f74 6966 6963 6174 696f   in.`notificatio
+00004180: 6e73 2f74 6573 7473 2f73 616d 706c 655f  ns/tests/sample_
+00004190: 6e6f 7469 6669 6361 7469 6f6e 7360 2074  notifications` t
+000041a0: 6861 7420 6578 7465 6e64 730a 6064 6a61  hat extends.`dja
+000041b0: 6e67 6f2d 6e6f 7469 6669 6361 7469 6f6e  ngo-notification
+000041c0: 7360 2077 6974 6820 7468 6520 736f 6c65  s` with the sole
+000041d0: 2070 7572 706f 7365 206f 6620 7465 7374   purpose of test
+000041e0: 696e 6720 6974 730a 6578 7465 6e73 6962  ing its.extensib
+000041f0: 696c 6974 792e 2059 6f75 2063 616e 2072  ility. You can r
+00004200: 756e 2074 6865 2053 414d 504c 4520 4150  un the SAMPLE AP
+00004210: 5020 6279 2073 6574 7469 6e67 2074 6865  P by setting the
+00004220: 2065 6e76 6972 6f6e 6d65 6e74 0a76 6172   environment.var
+00004230: 6961 626c 6520 6053 414d 504c 455f 4150  iable `SAMPLE_AP
+00004240: 5060 2061 7320 666f 6c6c 6f77 730a 0a60  P` as follows..`
+00004250: 6060 6261 7368 0a65 7870 6f72 7420 5341  ``bash.export SA
+00004260: 4d50 4c45 5f41 5050 3d31 0a23 2052 756e  MPLE_APP=1.# Run
+00004270: 2074 6865 2044 6a61 6e67 6f20 6465 7665   the Django deve
+00004280: 6c6f 706d 656e 7420 7365 7276 6572 2077  lopment server w
+00004290: 6974 6820 7361 6d70 6c65 5f6e 6f74 6966  ith sample_notif
+000042a0: 6963 6174 696f 6e73 2061 7070 2069 6e73  ications app ins
+000042b0: 7461 6c6c 6564 0a70 7974 686f 6e20 6d61  talled.python ma
+000042c0: 6e61 6765 2e70 7920 7275 6e73 6572 7665  nage.py runserve
+000042d0: 720a 2320 556e 7365 7420 5341 4d50 4c45  r.# Unset SAMPLE
+000042e0: 5f41 5050 2074 6f20 7265 6d6f 7665 2073  _APP to remove s
+000042f0: 616d 706c 655f 6e6f 7469 6669 6361 7469  ample_notificati
+00004300: 6f6e 7320 6170 7020 6672 6f6d 206c 6973  ons app from lis
+00004310: 7420 6f66 2049 4e53 5441 4c4c 4544 5f41  t of INSTALLED_A
+00004320: 5050 530a 756e 7365 7420 5341 4d50 4c45  PPS.unset SAMPLE
+00004330: 5f41 5050 0a60 6060 0a0a 2323 2060 646a  _APP.```..## `dj
+00004340: 616e 676f 2d6e 6f74 6966 6963 6174 696f  ango-notificatio
+00004350: 6e73 6020 5465 616d 0a0a 436f 7265 2063  ns` Team..Core c
+00004360: 6f6e 7472 6962 7574 6f72 7320 2869 6e20  ontributors (in 
+00004370: 616c 7068 6162 6574 6963 616c 206f 7264  alphabetical ord
+00004380: 6572 293a 0a0a 2d20 2020 5b41 6c76 6172  er):..-   [Alvar
+00004390: 6f20 4c65 6f6e 656c 5d28 6874 7470 733a  o Leonel](https:
+000043a0: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6c76  //github.com/Alv
+000043b0: 6172 6f4c 5175 6569 726f 7a29 0a2d 2020  aroLQueiroz).-  
+000043c0: 205b 4665 6465 7269 636f 2043 6170 6f61   [Federico Capoa
+000043d0: 6e6f 5d28 6874 7470 733a 2f2f 6769 7468  no](https://gith
+000043e0: 7562 2e63 6f6d 2f6e 656d 6573 6973 6465  ub.com/nemesisde
+000043f0: 7369 676e 290a 2d20 2020 5b53 616d 7565  sign).-   [Samue
+00004400: 6c20 5370 656e 6365 725d 2868 7474 7073  l Spencer](https
+00004410: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c65  ://github.com/Le
+00004420: 676f 5374 6f72 6d74 726f 6f70 7229 0a2d  goStormtroopr).-
+00004430: 2020 205b 5961 6e67 2059 7562 6f5d 2868     [Yang Yubo](h
+00004440: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00004450: 6d2f 7961 6e67 7975 626f 290a 2d20 2020  m/yangyubo).-   
+00004460: 5b59 5043 7275 6d62 6c65 5d28 6874 7470  [YPCrumble](http
+00004470: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f59  s://github.com/Y
+00004480: 5043 7275 6d62 6c65 290a 2d20 2020 5b5a  PCrumble).-   [Z
+00004490: 686f 6e67 7975 616e 205a 6861 6e67 5d28  hongyuan Zhang](
+000044a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000044b0: 6f6d 2f7a 6861 6e67 2d7a 290a 0a23 2320  om/zhang-z)..## 
+000044c0: 436f 6e74 7269 6275 7465 0a0a 5765 2061  Contribute..We a
+000044d0: 7265 206c 6f6f 6b69 6e67 2066 6f72 2063  re looking for c
+000044e0: 6f6e 7472 6962 7574 6f72 732c 2066 6f72  ontributors, for
+000044f0: 2061 6e79 6f6e 6520 7768 6f5c 2764 206c   anyone who\'d l
+00004500: 696b 6520 746f 2063 6f6e 7472 6962 7574  ike to contribut
+00004510: 650a 616e 6420 7769 6c6c 696e 6720 746f  e.and willing to
+00004520: 2070 7574 2074 696d 6520 616e 6420 656e   put time and en
+00004530: 6572 6779 206f 6e20 7468 6973 2070 726f  ergy on this pro
+00004540: 6a65 6374 2c20 706c 6561 7365 2063 6f6e  ject, please con
+00004550: 7461 6374 205b 5961 6e67 0a59 7562 6f5d  tact [Yang.Yubo]
+00004560: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00004570: 636f 6d2f 7961 6e67 7975 626f 292e 0a    com/yangyubo)..
```

### Comparing `django-notifications-hq-1.7.0/django_notifications_hq.egg-info/SOURCES.txt` & `django-notifications-hq-1.8.0/django_notifications_hq.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 AUTHORS.txt
-CHANGELOG.rst
+CHANGELOG.md
 LICENSE.txt
 MANIFEST.in
-README.rst
+README.md
 setup.cfg
 setup.py
 django_notifications_hq.egg-info/PKG-INFO
 django_notifications_hq.egg-info/SOURCES.txt
 django_notifications_hq.egg-info/dependency_links.txt
 django_notifications_hq.egg-info/requires.txt
 django_notifications_hq.egg-info/top_level.txt
 notifications/__init__.py
 notifications/admin.py
 notifications/apps.py
+notifications/helpers.py
 notifications/models.py
 notifications/settings.py
 notifications/signals.py
 notifications/urls.py
 notifications/utils.py
 notifications/views.py
 notifications/base/__init__.py
 notifications/base/admin.py
 notifications/base/models.py
+notifications/locale/ru/LC_MESSAGES/django.po
 notifications/migrations/0001_initial.py
 notifications/migrations/0002_auto_20150224_1134.py
 notifications/migrations/0003_notification_data.py
 notifications/migrations/0004_auto_20150826_1508.py
 notifications/migrations/0005_auto_20160504_1520.py
 notifications/migrations/0006_indexes.py
 notifications/migrations/0007_add_timestamp_index.py
 notifications/migrations/0008_index_together_recipient_unread.py
 notifications/migrations/__init__.py
-notifications/static/notifications/notify.js
 notifications/templates/notifications/list.html
 notifications/templates/notifications/notice.html
 notifications/templates/notifications/test_tags.html
 notifications/templatetags/__init__.py
 notifications/templatetags/notifications_tags.py
 notifications/tests/__init__.py
 notifications/tests/settings.py
```

### Comparing `django-notifications-hq-1.7.0/notifications/base/models.py` & `django-notifications-hq-1.8.0/notifications/base/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,27 +7,35 @@
 from django.conf import settings
 from django.contrib.auth.models import Group
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ImproperlyConfigured
 from django.db import models
 from django.db.models.query import QuerySet
 from django.utils import timezone
+from django.utils.translation import gettext_lazy as _
+from django.utils.html import format_html
+
 from jsonfield.fields import JSONField
 from model_utils import Choices
-
 from notifications import settings as notifications_settings
 from notifications.signals import notify
 from notifications.utils import id2slug
 from swapper import load_model
 
 if StrictVersion(get_version()) >= StrictVersion('1.8.0'):
     from django.contrib.contenttypes.fields import GenericForeignKey  # noqa
 else:
     from django.contrib.contenttypes.generic import GenericForeignKey  # noqa
 
+try:
+    # Django >= 1.7
+    from django.urls import reverse, NoReverseMatch
+except ImportError:
+    # Django <= 1.6
+    from django.core.urlresolvers import reverse, NoReverseMatch  # pylint: disable=no-name-in-module,import-error
 
 EXTRA_DATA = notifications_settings.get_config()['USE_JSONFIELD']
 
 
 def is_soft_delete():
     return notifications_settings.get_config()['SOFT_DELETE']
 
@@ -163,76 +171,95 @@
 
     HTML Representation::
 
         <a href="http://oebfare.com/">brosner</a> commented on <a href="http://github.com/pinax/pinax">pinax/pinax</a> 2 hours ago # noqa
 
     """
     LEVELS = Choices('success', 'info', 'warning', 'error')
-    level = models.CharField(choices=LEVELS, default=LEVELS.info, max_length=20)
+    level = models.CharField(_('level'), choices=LEVELS, default=LEVELS.info, max_length=20)
 
     recipient = models.ForeignKey(
         settings.AUTH_USER_MODEL,
-        blank=False,
+        on_delete=models.CASCADE,
         related_name='notifications',
-        on_delete=models.CASCADE
+        verbose_name=_('recipient'),
+        blank=False,
     )
-    unread = models.BooleanField(default=True, blank=False, db_index=True)
+    unread = models.BooleanField(_('unread'), default=True, blank=False, db_index=True)
 
-    actor_content_type = models.ForeignKey(ContentType, related_name='notify_actor', on_delete=models.CASCADE)
-    actor_object_id = models.CharField(max_length=255)
+    actor_content_type = models.ForeignKey(
+        ContentType,
+        on_delete=models.CASCADE,
+        related_name='notify_actor',
+        verbose_name=_('actor content type')
+    )
+    actor_object_id = models.CharField(_('actor object id'), max_length=255)
     actor = GenericForeignKey('actor_content_type', 'actor_object_id')
+    actor.short_description = _('actor')
 
-    verb = models.CharField(max_length=255)
-    description = models.TextField(blank=True, null=True)
+    verb = models.CharField(_('verb'), max_length=255)
+    description = models.TextField(_('description'), blank=True, null=True)
 
     target_content_type = models.ForeignKey(
         ContentType,
+        on_delete=models.CASCADE,
         related_name='notify_target',
+        verbose_name=_('target content type'),
         blank=True,
-        null=True,
-        on_delete=models.CASCADE
+        null=True
     )
-    target_object_id = models.CharField(max_length=255, blank=True, null=True)
+    target_object_id = models.CharField(_('target object id'), max_length=255, blank=True, null=True)
     target = GenericForeignKey('target_content_type', 'target_object_id')
+    target.short_description = _('target')
 
-    action_object_content_type = models.ForeignKey(ContentType, blank=True, null=True,
-                                                   related_name='notify_action_object', on_delete=models.CASCADE)
-    action_object_object_id = models.CharField(max_length=255, blank=True, null=True)
+    action_object_content_type = models.ForeignKey(
+        ContentType,
+        on_delete=models.CASCADE,
+        related_name='notify_action_object',
+        verbose_name=_('action object content type'),
+        blank=True,
+        null=True
+    )
+    action_object_object_id = models.CharField(_('action object object id'), max_length=255, blank=True, null=True)
     action_object = GenericForeignKey('action_object_content_type', 'action_object_object_id')
+    action_object.short_description = _('action object')
 
-    timestamp = models.DateTimeField(default=timezone.now, db_index=True)
+    timestamp = models.DateTimeField(_('timestamp'), default=timezone.now, db_index=True)
 
-    public = models.BooleanField(default=True, db_index=True)
-    deleted = models.BooleanField(default=False, db_index=True)
-    emailed = models.BooleanField(default=False, db_index=True)
+    public = models.BooleanField(_('public'), default=True, db_index=True)
+    deleted = models.BooleanField(_('deleted'), default=False, db_index=True)
+    emailed = models.BooleanField(_('emailed'), default=False, db_index=True)
+
+    data = JSONField(_('data'), blank=True, null=True)
 
-    data = JSONField(blank=True, null=True)
     objects = NotificationQuerySet.as_manager()
 
     class Meta:
         abstract = True
         ordering = ('-timestamp',)
         # speed up notifications count query
         index_together = ('recipient', 'unread')
+        verbose_name = _('Notification')
+        verbose_name_plural = _('Notifications')
 
     def __str__(self):
         ctx = {
             'actor': self.actor,
             'verb': self.verb,
             'action_object': self.action_object,
             'target': self.target,
             'timesince': self.timesince()
         }
         if self.target:
             if self.action_object:
-                return u'%(actor)s %(verb)s %(action_object)s on %(target)s %(timesince)s ago' % ctx
-            return u'%(actor)s %(verb)s %(target)s %(timesince)s ago' % ctx
+                return _('%(actor)s %(verb)s %(action_object)s on %(target)s %(timesince)s ago') % ctx
+            return _('%(actor)s %(verb)s %(target)s %(timesince)s ago') % ctx
         if self.action_object:
-            return u'%(actor)s %(verb)s %(action_object)s %(timesince)s ago' % ctx
-        return u'%(actor)s %(verb)s %(timesince)s ago' % ctx
+            return _('%(actor)s %(verb)s %(action_object)s %(timesince)s ago') % ctx
+        return _('%(actor)s %(verb)s %(timesince)s ago') % ctx
 
     def timesince(self, now=None):
         """
         Shortcut for the ``django.utils.timesince.timesince`` function of the
         current timestamp.
         """
         from django.utils.timesince import timesince as timesince_
@@ -248,14 +275,41 @@
             self.save()
 
     def mark_as_unread(self):
         if not self.unread:
             self.unread = True
             self.save()
 
+    def actor_object_url(self):
+        try:
+            url = reverse("admin:{0}_{1}_change".format(self.actor_content_type.app_label,
+                                                        self.actor_content_type.model),
+                          args=(self.actor_object_id,))
+            return format_html("<a href='{url}'>{id}</a>", url=url, id=self.actor_object_id)
+        except NoReverseMatch:
+            return self.actor_object_id
+
+    def action_object_url(self):
+        try:
+            url = reverse("admin:{0}_{1}_change".format(self.action_object_content_type.app_label,
+                                                        self.action_content_type.model),
+                          args=(self.action_object_id,))
+            return format_html("<a href='{url}'>{id}</a>", url=url, id=self.action_object_object_id)
+        except NoReverseMatch:
+            return self.action_object_object_id
+
+    def target_object_url(self):
+        try:
+            url = reverse("admin:{0}_{1}_change".format(self.target_content_type.app_label,
+                                                        self.target_content_type.model),
+                          args=(self.target_object_id,))
+            return format_html("<a href='{url}'>{id}</a>", url=url, id=self.target_object_id)
+        except NoReverseMatch:
+            return self.target_object_id
+
 
 def notify_handler(verb, **kwargs):
     """
     Handler function to create Notification instance upon action signal call.
     """
     # Pull the options out of kwargs
     kwargs.pop('signal', None)
@@ -266,45 +320,51 @@
         for opt in ('target', 'action_object')
     ]
     public = bool(kwargs.pop('public', True))
     description = kwargs.pop('description', None)
     timestamp = kwargs.pop('timestamp', timezone.now())
     Notification = load_model('notifications', 'Notification')
     level = kwargs.pop('level', Notification.LEVELS.info)
+    actor_for_concrete_model = kwargs.pop('actor_for_concrete_model', True)
 
     # Check if User or Group
     if isinstance(recipient, Group):
         recipients = recipient.user_set.all()
     elif isinstance(recipient, (QuerySet, list)):
         recipients = recipient
     else:
         recipients = [recipient]
 
     new_notifications = []
 
     for recipient in recipients:
         newnotify = Notification(
             recipient=recipient,
-            actor_content_type=ContentType.objects.get_for_model(actor),
+            actor_content_type=ContentType.objects.get_for_model(actor, for_concrete_model=actor_for_concrete_model),
             actor_object_id=actor.pk,
             verb=str(verb),
             public=public,
             description=description,
             timestamp=timestamp,
             level=level,
         )
 
         # Set optional objects
         for obj, opt in optional_objs:
             if obj is not None:
+                for_concrete_model = kwargs.pop(f'{opt}_for_concrete_model', True)
                 setattr(newnotify, '%s_object_id' % opt, obj.pk)
                 setattr(newnotify, '%s_content_type' % opt,
-                        ContentType.objects.get_for_model(obj))
+                        ContentType.objects.get_for_model(obj, for_concrete_model=for_concrete_model))
 
         if kwargs and EXTRA_DATA:
+            # set kwargs as model column if available
+            for key in list(kwargs.keys()):
+                if hasattr(newnotify, key):
+                    setattr(newnotify, key, kwargs.pop(key))
             newnotify.data = kwargs
 
         newnotify.save()
         new_notifications.append(newnotify)
 
     return new_notifications
```

### Comparing `django-notifications-hq-1.7.0/notifications/migrations/0001_initial.py` & `django-notifications-hq-1.8.0/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.7.0/notifications/migrations/0002_auto_20150224_1134.py` & `django-notifications-hq-1.8.0/notifications/migrations/0002_auto_20150224_1134.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.7.0/notifications/migrations/0005_auto_20160504_1520.py` & `django-notifications-hq-1.8.0/notifications/migrations/0005_auto_20160504_1520.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.7.0/notifications/migrations/0006_indexes.py` & `django-notifications-hq-1.8.0/notifications/migrations/0006_indexes.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.7.0/notifications/templates/notifications/notice.html` & `django-notifications-hq-1.8.0/notifications/templates/notifications/notice.html`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.7.0/notifications/tests/sample_notifications/migrations/0001_initial.py` & `django-notifications-hq-1.8.0/notifications/tests/sample_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.7.0/notifications/tests/sample_notifications/tests.py` & `django-notifications-hq-1.8.0/notifications/tests/sample_notifications/tests.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import os
 from unittest import skipUnless
 
+from django.contrib.auth.models import User
 import swapper
+
+from notifications.signals import notify
 from notifications.tests.tests import AdminTest as BaseAdminTest
 from notifications.tests.tests import NotificationTest as BaseNotificationTest
 
 Notification = swapper.load_model('notifications', 'Notification')
 
 
 @skipUnless(os.environ.get('SAMPLE_APP', False), 'Running tests on standard django-notifications models')
@@ -16,7 +19,28 @@
         super().setUpClass()
         BaseAdminTest.app_name = 'sample_notifications'
 
 
 @skipUnless(os.environ.get('SAMPLE_APP', False), 'Running tests on standard django-notifications models')
 class NotificationTest(BaseNotificationTest):
     pass
+
+
+class TestExtraDataCustomAccessor(NotificationTest):
+    def setUp(self):
+        self.from_user = User.objects.create_user(username="from_extra", password="pwd", email="example@example.com")
+        self.to_user = User.objects.create_user(username="to_extra", password="pwd", email="example@example.com")
+        notify.send(
+            self.from_user,
+            recipient=self.to_user,
+            verb='commented',
+            action_object=self.from_user,
+            url="/learn/ask-a-pro/q/test-question-9/299/",
+            other_content="Hello my 'world'",
+            details="test detail"
+        )
+
+    def test_extra_data(self):
+        notification = Notification.objects.get(details="test detail")
+        assert notification, "Expected a notification retrieved by custom extra data accessor"
+        assert notification.details == "test detail", "Custom accessor should return set value"
+        assert "details" not in notification.data, "Custom accessor should not be in json data"
```

### Comparing `django-notifications-hq-1.7.0/notifications/tests/settings.py` & `django-notifications-hq-1.8.0/notifications/tests/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,7 +73,9 @@
 USE_TZ = True
 
 if os.environ.get('SAMPLE_APP', False):
     INSTALLED_APPS.remove('notifications')
     INSTALLED_APPS.append('notifications.tests.sample_notifications')
     NOTIFICATIONS_NOTIFICATION_MODEL = 'sample_notifications.Notification'
     TEMPLATES[0]['DIRS'] += [os.path.join(BASE_DIR, '../templates')]
+
+ALLOWED_HOSTS = []
```

### Comparing `django-notifications-hq-1.7.0/notifications/tests/tests.py` & `django-notifications-hq-1.8.0/notifications/tests/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import pytz
 
 from django.conf import settings
 from django.contrib.auth.models import Group, User
 from django.core.exceptions import ImproperlyConfigured
 from django.db import connection
 from django.template import Context, Template
-from django.test import RequestFactory, TestCase
+from django.test import Client, RequestFactory, TestCase
 from django.test.utils import CaptureQueriesContext
 from django.utils import timezone
 from django.utils.timezone import localtime, utc
 from notifications.base.models import notify_handler
 from notifications.signals import notify
 from notifications.utils import id2slug
 from swapper import load_model
@@ -35,15 +35,21 @@
 try:
     # Django >= 1.7
     from django.urls import reverse
 except ImportError:
     # Django <= 1.6
     from django.core.urlresolvers import reverse  # pylint: disable=no-name-in-module,import-error
 
-
+MALICIOUS_NEXT_URLS = [
+    "http://bla.com",
+    "http://www.bla.com",
+    "https://bla.com",
+    "https://www.bla.com",
+    "ftp://www.bla.com/file.exe",
+]
 
 class NotificationTest(TestCase):
     ''' Django notifications automated tests '''
     @override_settings(USE_TZ=True)
     @override_settings(TIME_ZONE='Asia/Shanghai')
     def test_use_timezone(self):
         from_user = User.objects.create(username="from", password="pwd", email="example@example.com")
@@ -64,14 +70,27 @@
         from_user = User.objects.create(username="from2", password="pwd", email="example@example.com")
         to_user = User.objects.create(username="to2", password="pwd", email="example@example.com")
         notify.send(from_user, recipient=to_user, verb='commented', action_object=from_user)
         notification = Notification.objects.get(recipient=to_user)
         delta = timezone.now() - notification.timestamp
         self.assertTrue(delta.seconds < 60)
 
+    def test_humanize_naturalday_timestamp(self):
+        from_user = User.objects.create(username="from2", password="pwd", email="example@example.com")
+        to_user = User.objects.create(username="to2", password="pwd", email="example@example.com")
+        notify.send(from_user, recipient=to_user, verb='commented', action_object=from_user)
+        notification = Notification.objects.get(recipient=to_user)
+        self.assertEqual(notification.naturalday(), 'today')
+
+    def test_humanize_naturaltime_timestamp(self):
+        from_user = User.objects.create(username="from2", password="pwd", email="example@example.com")
+        to_user = User.objects.create(username="to2", password="pwd", email="example@example.com")
+        notify.send(from_user, recipient=to_user, verb='commented', action_object=from_user)
+        notification = Notification.objects.get(recipient=to_user)
+        self.assertEqual(notification.naturaltime(), 'now')
 
 class NotificationManagersTest(TestCase):
     ''' Django notifications Manager automated tests '''
     def setUp(self):
         self.message_count = 10
         self.other_user = User.objects.create(username="other1", password="pwd", email="example@example.com")
 
@@ -246,14 +265,25 @@
 
         slug = id2slug(self.to_user.notifications.first().id)
         response = self.client.get(reverse('notifications:mark_as_unread', args=[slug]), {
             "next": reverse('notifications:unread') + query_parameters,
         })
         self.assertRedirects(response, reverse('notifications:unread') + query_parameters)
 
+    @override_settings(ALLOWED_HOSTS=["www.notifications.com"])
+    def test_malicious_next_pages(self):
+        self.client.force_login(self.to_user)
+        query_parameters = '?var1=hello&var2=world'
+
+        for next_url in MALICIOUS_NEXT_URLS:
+            response = self.client.get(reverse('notifications:mark_all_as_read'),data={
+                "next": next_url  + query_parameters,
+            })
+            self.assertRedirects(response, reverse('notifications:unread'))
+
     def test_delete_messages_pages(self):
         self.login('to', 'pwd')
 
         slug = id2slug(self.to_user.notifications.first().id)
         response = self.client.get(reverse('notifications:delete', args=[slug]))
         self.assertRedirects(response, reverse('notifications:all'))
 
@@ -432,15 +462,15 @@
 
         self.login('to', 'pwd')
         factory = RequestFactory()
 
         request = factory.get('/notification/live_updater')
         request.user = self.to_user
 
-        render(request, 'notifications/test_tags.html', {'request': request})
+        render(request, 'notifications/test_tags.html', {'request': request, 'nonce': 'nonce-T5esDNXMnDe5lKMQ6ZzTUw=='})
 
         # TODO: Add more tests to check what is being output.
 
     def test_anon_user_gets_nothing(self):
         response = self.client.post(reverse('notifications:live_unread_notification_count'))
         self.assertEqual(response.status_code, 200)
         data = json.loads(response.content.decode('utf-8'))
```

### Comparing `django-notifications-hq-1.7.0/notifications/tests/urls.py` & `django-notifications-hq-1.8.0/notifications/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.7.0/notifications/tests/views.py` & `django-notifications-hq-1.8.0/notifications/tests/views.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.7.0/notifications/urls.py` & `django-notifications-hq-1.8.0/notifications/urls.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.7.0/notifications/views.py` & `django-notifications-hq-1.8.0/notifications/views.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 # -*- coding: utf-8 -*-
 ''' Django Notifications example views '''
 from distutils.version import \
     StrictVersion  # pylint: disable=no-name-in-module,import-error
 
 from django import get_version
+from django.conf import settings
 from django.contrib.auth.decorators import login_required
-from django.forms import model_to_dict
 from django.shortcuts import get_object_or_404, redirect
 from django.utils.decorators import method_decorator
+from django.utils.encoding import iri_to_uri
+from django.utils.http import url_has_allowed_host_and_scheme
 from django.views.decorators.cache import never_cache
 from django.views.generic import ListView
-from notifications import settings
-from notifications.settings import get_config
-from notifications.utils import id2slug, slug2id
 from swapper import load_model
 
+from notifications import settings as notification_settings
+from notifications.helpers import get_notification_list
+from notifications.utils import slug2id
+
 Notification = load_model('notifications', 'Notification')
 
 if StrictVersion(get_version()) >= StrictVersion('1.7.0'):
     from django.http import JsonResponse  # noqa
 else:
     # Django 1.6 doesn't have a proper JsonResponse
     import json
+
     from django.http import HttpResponse  # noqa
 
     def date_handler(obj):
         return obj.isoformat() if hasattr(obj, 'isoformat') else obj
 
     def JsonResponse(data):  # noqa
         return HttpResponse(
             json.dumps(data, default=date_handler),
             content_type="application/json")
 
 
 class NotificationViewList(ListView):
     template_name = 'notifications/list.html'
     context_object_name = 'notifications'
-    paginate_by = settings.get_config()['PAGINATE_BY']
+    paginate_by = notification_settings.get_config()['PAGINATE_BY']
 
     @method_decorator(login_required)
     def dispatch(self, request, *args, **kwargs):
         return super(NotificationViewList, self).dispatch(
             request, *args, **kwargs)
 
 
 class AllNotificationsList(NotificationViewList):
     """
     Index page for authenticated user
     """
 
     def get_queryset(self):
-        if settings.get_config()['SOFT_DELETE']:
+        if notification_settings.get_config()['SOFT_DELETE']:
             qset = self.request.user.notifications.active()
         else:
             qset = self.request.user.notifications.all()
         return qset
 
 
 class UnreadNotificationsList(NotificationViewList):
@@ -65,68 +69,68 @@
 
 @login_required
 def mark_all_as_read(request):
     request.user.notifications.mark_all_as_read()
 
     _next = request.GET.get('next')
 
-    if _next:
-        return redirect(_next)
+    if _next and url_has_allowed_host_and_scheme(_next, settings.ALLOWED_HOSTS):
+        return redirect(iri_to_uri(_next))
     return redirect('notifications:unread')
 
 
 @login_required
 def mark_as_read(request, slug=None):
     notification_id = slug2id(slug)
 
     notification = get_object_or_404(
         Notification, recipient=request.user, id=notification_id)
     notification.mark_as_read()
 
     _next = request.GET.get('next')
 
-    if _next:
-        return redirect(_next)
+    if _next and url_has_allowed_host_and_scheme(_next, settings.ALLOWED_HOSTS):
+        return redirect(iri_to_uri(_next))
 
     return redirect('notifications:unread')
 
 
 @login_required
 def mark_as_unread(request, slug=None):
     notification_id = slug2id(slug)
 
     notification = get_object_or_404(
         Notification, recipient=request.user, id=notification_id)
     notification.mark_as_unread()
 
     _next = request.GET.get('next')
 
-    if _next:
-        return redirect(_next)
+    if _next and url_has_allowed_host_and_scheme(_next, settings.ALLOWED_HOSTS):
+        return redirect(iri_to_uri(_next))
 
     return redirect('notifications:unread')
 
 
 @login_required
 def delete(request, slug=None):
     notification_id = slug2id(slug)
 
     notification = get_object_or_404(
         Notification, recipient=request.user, id=notification_id)
 
-    if settings.get_config()['SOFT_DELETE']:
+    if notification_settings.get_config()['SOFT_DELETE']:
         notification.deleted = True
         notification.save()
     else:
         notification.delete()
 
     _next = request.GET.get('next')
 
-    if _next:
-        return redirect(_next)
+    if _next and url_has_allowed_host_and_scheme(_next, settings.ALLOWED_HOSTS):
+        return redirect(iri_to_uri(_next))
 
     return redirect('notifications:all')
 
 
 @never_cache
 def live_unread_notification_count(request):
     try:
@@ -156,40 +160,16 @@
     if not user_is_authenticated:
         data = {
             'unread_count': 0,
             'unread_list': []
         }
         return JsonResponse(data)
 
-    default_num_to_fetch = get_config()['NUM_TO_FETCH']
-    try:
-        # If they don't specify, make it 5.
-        num_to_fetch = request.GET.get('max', default_num_to_fetch)
-        num_to_fetch = int(num_to_fetch)
-        if not (1 <= num_to_fetch <= 100):
-            num_to_fetch = default_num_to_fetch
-    except ValueError:  # If casting to an int fails.
-        num_to_fetch = default_num_to_fetch
-
-    unread_list = []
-
-    for notification in request.user.notifications.unread()[0:num_to_fetch]:
-        struct = model_to_dict(notification)
-        struct['slug'] = id2slug(notification.id)
-        if notification.actor:
-            struct['actor'] = str(notification.actor)
-        if notification.target:
-            struct['target'] = str(notification.target)
-        if notification.action_object:
-            struct['action_object'] = str(notification.action_object)
-        if notification.data:
-            struct['data'] = notification.data
-        unread_list.append(struct)
-        if request.GET.get('mark_as_read'):
-            notification.mark_as_read()
+    unread_list = get_notification_list(request, 'unread')
+
     data = {
         'unread_count': request.user.notifications.unread().count(),
         'unread_list': unread_list
     }
     return JsonResponse(data)
 
 
@@ -204,40 +184,16 @@
     if not user_is_authenticated:
         data = {
             'all_count': 0,
             'all_list': []
         }
         return JsonResponse(data)
 
-    default_num_to_fetch = get_config()['NUM_TO_FETCH']
-    try:
-        # If they don't specify, make it 5.
-        num_to_fetch = request.GET.get('max', default_num_to_fetch)
-        num_to_fetch = int(num_to_fetch)
-        if not (1 <= num_to_fetch <= 100):
-            num_to_fetch = default_num_to_fetch
-    except ValueError:  # If casting to an int fails.
-        num_to_fetch = default_num_to_fetch
-
-    all_list = []
-
-    for notification in request.user.notifications.all()[0:num_to_fetch]:
-        struct = model_to_dict(notification)
-        struct['slug'] = id2slug(notification.id)
-        if notification.actor:
-            struct['actor'] = str(notification.actor)
-        if notification.target:
-            struct['target'] = str(notification.target)
-        if notification.action_object:
-            struct['action_object'] = str(notification.action_object)
-        if notification.data:
-            struct['data'] = notification.data
-        all_list.append(struct)
-        if request.GET.get('mark_as_read'):
-            notification.mark_as_read()
+    all_list = get_notification_list(request)
+
     data = {
         'all_count': request.user.notifications.count(),
         'all_list': all_list
     }
     return JsonResponse(data)
```

### Comparing `django-notifications-hq-1.7.0/setup.py` & `django-notifications-hq-1.8.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,56 +17,57 @@
         f.read().decode('utf-8')).group(1)))
 
 
 setup(
     name='django-notifications-hq',
     version=version,
     description='GitHub notifications alike app for Django.',
-    long_description=open('README.rst').read(),
+    long_description=open('README.md').read(),
+    long_description_content_type="text/markdown",
     author='django-notifications team',
     author_email='yang@yangyubo.com',
     url='http://github.com/django-notifications/django-notifications',
     install_requires=[
-        'django>=2.2',
+        'django>=3.2',
         'django-model-utils>=3.1.0',
         'jsonfield>=2.1.0',
         'pytz',
         'swapper'
     ],
     test_requires=[
-        'django>=2.2',
+        'django>=3.2',
         'django-model-utils>=3.1.0',
         'jsonfield>=2.1.0',
         'pytz'
     ],
     packages=[
         'notifications',
         'notifications.base',
         'notifications.templatetags',
         'notifications.migrations',
     ],
-    package_data={
-        'notifications': ['templates/notifications/*.html', 'static/notifications/*.js']
-    },
+    include_package_data=True,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Utilities'
     ],
     keywords='django notifications github action event stream',
     license='MIT',
 )
```

