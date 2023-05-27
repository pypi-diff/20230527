# Comparing `tmp/django-wm-4.0.2.tar.gz` & `tmp/django-wm-4.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-wm-4.0.2.tar", last modified: Sat May 27 15:10:08 2023, max compression
+gzip compressed data, was "django-wm-4.1.0.dev0.tar", last modified: Tue May  9 17:16:22 2023, max compression
```

## Comparing `django-wm-4.0.2.tar` & `django-wm-4.1.0.dev0.tar`

### file list

```diff
@@ -1,128 +1,133 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.166755 django-wm-4.0.2/
--rwxrw-r-x   0 michael   (1000) michael   (1000)    35149 2022-01-27 11:41:47.000000 django-wm-4.0.2/LICENSE
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2921 2023-05-27 15:10:08.166893 django-wm-4.0.2/PKG-INFO
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2085 2022-11-25 16:03:29.000000 django-wm-4.0.2/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.104666 django-wm-4.0.2/django_wm.egg-info/
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2921 2023-05-27 15:10:08.000000 django-wm-4.0.2/django_wm.egg-info/PKG-INFO
--rwxrw-r-x   0 michael   (1000) michael   (1000)     3724 2023-05-27 15:10:08.000000 django-wm-4.0.2/django_wm.egg-info/SOURCES.txt
--rwxrw-r-x   0 michael   (1000) michael   (1000)        1 2023-05-27 15:10:08.000000 django-wm-4.0.2/django_wm.egg-info/dependency_links.txt
--rwxrw-r-x   0 michael   (1000) michael   (1000)      137 2023-05-27 15:10:08.000000 django-wm-4.0.2/django_wm.egg-info/requires.txt
--rwxrw-r-x   0 michael   (1000) michael   (1000)        9 2023-05-27 15:10:08.000000 django-wm-4.0.2/django_wm.egg-info/top_level.txt
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.110494 django-wm-4.0.2/mentions/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       73 2023-05-27 12:17:59.000000 django-wm-4.0.2/mentions/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     4963 2023-05-27 14:50:00.000000 django-wm-4.0.2/mentions/admin.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)       91 2022-11-16 17:49:32.000000 django-wm-4.0.2/mentions/apps.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      583 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/config.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      288 2023-05-26 11:12:16.000000 django-wm-4.0.2/mentions/contract.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2222 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/exceptions.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.111625 django-wm-4.0.2/mentions/forms/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       52 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/forms/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      224 2023-05-07 14:24:34.000000 django-wm-4.0.2/mentions/forms/submit_webmention.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.114688 django-wm-4.0.2/mentions/helpers/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       50 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/helpers/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1819 2022-12-22 15:35:08.000000 django-wm-4.0.2/mentions/helpers/resolution.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.115387 django-wm-4.0.2/mentions/helpers/thirdparty/
--rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/helpers/thirdparty/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.119670 django-wm-4.0.2/mentions/helpers/thirdparty/wagtail/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      160 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/helpers/thirdparty/wagtail/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2096 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/helpers/thirdparty/wagtail/proxy.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     3484 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/helpers/thirdparty/wagtail/resolution.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     6964 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/helpers/thirdparty/wagtail/urls.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      635 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/helpers/thirdparty/wagtail/util.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      849 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/helpers/types.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     5883 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/helpers/urls.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      788 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/helpers/util.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.120290 django-wm-4.0.2/mentions/management/
--rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-02-05 17:15:41.000000 django-wm-4.0.2/mentions/management/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.123368 django-wm-4.0.2/mentions/management/commands/
--rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-02-05 17:15:41.000000 django-wm-4.0.2/mentions/management/commands/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1030 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/management/commands/mentions_pending.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2124 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/management/commands/mentions_reverify.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      143 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/management/commands/pending_mentions.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      296 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/microformats.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.124531 django-wm-4.0.2/mentions/middleware/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       65 2022-10-26 15:53:11.000000 django-wm-4.0.2/mentions/middleware/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      739 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/middleware/webmention_head_middleware.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.133043 django-wm-4.0.2/mentions/migrations/
--rwxrw-r-x   0 michael   (1000) michael   (1000)     8690 2022-02-03 11:01:16.000000 django-wm-4.0.2/mentions/migrations/0001_initial.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1626 2022-10-27 12:03:01.000000 django-wm-4.0.2/mentions/migrations/0002_pendingincomingwebmention_pendingoutgoingcontent.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      664 2022-03-26 13:17:25.000000 django-wm-4.0.2/mentions/migrations/0003_alter_simplemention_published_and_more.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1349 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/migrations/0004_simplemention_post_type_webmention_post_type_and_more.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     3250 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/migrations/0005_rebuild_pending_models_with_constraints.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2853 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/migrations/0006_add_retryablemixin_pendingincomingwebmention_outgoingwebmentionstatus.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1076 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/migrations/0007_dashboardpermissionproxy.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      361 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/migrations/0008_alter_webmention_options.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      471 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/migrations/0009_alter_outgoingwebmentionstatus_options.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      781 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/migrations/0010_alter_hcard_avatar_alter_hcard_name.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      539 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/migrations/0011_alter_pendingoutgoingcontent_text.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)    16916 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/migrations/0012_alter_hcard_options_and_more.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-01-27 11:41:47.000000 django-wm-4.0.2/mentions/migrations/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.137174 django-wm-4.0.2/mentions/models/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      271 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/models/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      291 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/models/base.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2993 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/models/hcard.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.140153 django-wm-4.0.2/mentions/models/mixins/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      137 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/models/mixins/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     4541 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/models/mixins/mentionable.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     3372 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/models/mixins/quotable.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2879 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/models/mixins/retryable.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2522 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/models/outgoing_status.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2169 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/models/pending.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.141877 django-wm-4.0.2/mentions/models/proxy/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       50 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/models/proxy/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      386 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/models/proxy/permissions.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      649 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/models/simple_mention.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1677 2023-05-26 11:12:16.000000 django-wm-4.0.2/mentions/models/webmention.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     6958 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/options.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      956 2023-05-26 11:12:16.000000 django-wm-4.0.2/mentions/permissions.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     5026 2023-05-26 11:12:16.000000 django-wm-4.0.2/mentions/resolution.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.143823 django-wm-4.0.2/mentions/tasks/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      178 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/tasks/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1333 2022-10-12 15:23:17.000000 django-wm-4.0.2/mentions/tasks/celeryproxy.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.148317 django-wm-4.0.2/mentions/tasks/incoming/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       49 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/tasks/incoming/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1138 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/tasks/incoming/local.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.150466 django-wm-4.0.2/mentions/tasks/incoming/parsing/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       90 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/tasks/incoming/parsing/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     3496 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/tasks/incoming/parsing/hcard.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      981 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/tasks/incoming/parsing/post_type.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     4288 2023-05-07 14:23:52.000000 django-wm-4.0.2/mentions/tasks/incoming/process.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     3023 2023-05-07 14:24:22.000000 django-wm-4.0.2/mentions/tasks/incoming/remote.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2557 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/tasks/incoming/reverify.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      848 2023-05-07 13:24:39.000000 django-wm-4.0.2/mentions/tasks/incoming/status.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.153100 django-wm-4.0.2/mentions/tasks/outgoing/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      125 2022-10-06 19:42:52.000000 django-wm-4.0.2/mentions/tasks/outgoing/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2483 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/tasks/outgoing/local.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.154632 django-wm-4.0.2/mentions/tasks/outgoing/parsing/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      159 2022-10-06 19:42:52.000000 django-wm-4.0.2/mentions/tasks/outgoing/parsing/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1893 2022-10-06 19:42:52.000000 django-wm-4.0.2/mentions/tasks/outgoing/parsing/webmention_endpoint.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2351 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/tasks/outgoing/process.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     5224 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/tasks/outgoing/remote.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     5707 2023-05-07 14:24:27.000000 django-wm-4.0.2/mentions/tasks/scheduling.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.097992 django-wm-4.0.2/mentions/templates/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.156847 django-wm-4.0.2/mentions/templates/mentions/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      261 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/templates/mentions/webmention-accepted.html
--rwxrw-r-x   0 michael   (1000) michael   (1000)     8130 2023-05-26 11:13:40.000000 django-wm-4.0.2/mentions/templates/mentions/webmention-dashboard.html
--rwxrw-r-x   0 michael   (1000) michael   (1000)      585 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/templates/mentions/webmention-submit-manual.html
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.159153 django-wm-4.0.2/mentions/templatetags/
--rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-02-03 11:01:16.000000 django-wm-4.0.2/mentions/templatetags/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1766 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/templatetags/webmention_dashboard.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      332 2022-09-29 19:47:26.000000 django-wm-4.0.2/mentions/templatetags/webmention_endpoint.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1317 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/templatetags/webmentions.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      942 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/urls.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.161439 django-wm-4.0.2/mentions/util/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      166 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/util/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      547 2022-10-06 19:42:52.000000 django-wm-4.0.2/mentions/util/html.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      559 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/util/requests.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      934 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/util/url.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 15:10:08.166229 django-wm-4.0.2/mentions/views/
--rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/views/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      409 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/views/contract.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1338 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/views/dashboard.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2355 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/views/retrieve.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1810 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/views/serialize.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1804 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/views/submit.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      486 2022-11-25 16:03:29.000000 django-wm-4.0.2/mentions/views/view_names.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      112 2022-09-29 19:47:26.000000 django-wm-4.0.2/pyproject.toml
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1104 2023-05-27 15:10:08.167530 django-wm-4.0.2/setup.cfg
--rwxrw-r-x   0 michael   (1000) michael   (1000)       69 2022-09-29 19:47:26.000000 django-wm-4.0.2/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.496719 django-wm-4.1.0.dev0/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)    35149 2022-01-27 11:41:47.000000 django-wm-4.1.0.dev0/LICENSE
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2926 2023-05-09 17:16:22.496848 django-wm-4.1.0.dev0/PKG-INFO
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2085 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.415917 django-wm-4.1.0.dev0/django_wm.egg-info/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2926 2023-05-09 17:16:22.000000 django-wm-4.1.0.dev0/django_wm.egg-info/PKG-INFO
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     3884 2023-05-09 17:16:22.000000 django-wm-4.1.0.dev0/django_wm.egg-info/SOURCES.txt
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        1 2023-05-09 17:16:22.000000 django-wm-4.1.0.dev0/django_wm.egg-info/dependency_links.txt
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      137 2023-05-09 17:16:22.000000 django-wm-4.1.0.dev0/django_wm.egg-info/requires.txt
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        9 2023-05-09 17:16:22.000000 django-wm-4.1.0.dev0/django_wm.egg-info/top_level.txt
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.423068 django-wm-4.1.0.dev0/mentions/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       78 2023-05-08 10:58:46.000000 django-wm-4.1.0.dev0/mentions/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     4091 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/admin.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       91 2022-11-16 17:49:32.000000 django-wm-4.1.0.dev0/mentions/apps.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      583 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/config.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      295 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/context_processors.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      365 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/contract.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2222 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/exceptions.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.425026 django-wm-4.1.0.dev0/mentions/forms/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       52 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/forms/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      224 2023-05-07 14:24:34.000000 django-wm-4.1.0.dev0/mentions/forms/submit_webmention.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.431152 django-wm-4.1.0.dev0/mentions/helpers/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       50 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/helpers/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1819 2022-12-22 15:35:08.000000 django-wm-4.1.0.dev0/mentions/helpers/resolution.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.432066 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.436609 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      160 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2096 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/proxy.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     3484 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/resolution.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     6964 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/urls.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      635 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/util.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      849 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/types.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     5883 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/urls.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      788 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/util.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.437240 django-wm-4.1.0.dev0/mentions/management/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-02-05 17:15:41.000000 django-wm-4.1.0.dev0/mentions/management/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.440226 django-wm-4.1.0.dev0/mentions/management/commands/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-02-05 17:15:41.000000 django-wm-4.1.0.dev0/mentions/management/commands/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1030 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/management/commands/mentions_pending.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2124 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/management/commands/mentions_reverify.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      143 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/management/commands/pending_mentions.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      296 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/microformats.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.441361 django-wm-4.1.0.dev0/mentions/middleware/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       65 2022-10-26 15:53:11.000000 django-wm-4.1.0.dev0/mentions/middleware/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      739 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/middleware/webmention_head_middleware.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.455308 django-wm-4.1.0.dev0/mentions/migrations/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     8690 2022-02-03 11:01:16.000000 django-wm-4.1.0.dev0/mentions/migrations/0001_initial.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1626 2022-10-27 12:03:01.000000 django-wm-4.1.0.dev0/mentions/migrations/0002_pendingincomingwebmention_pendingoutgoingcontent.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      664 2022-03-26 13:17:25.000000 django-wm-4.1.0.dev0/mentions/migrations/0003_alter_simplemention_published_and_more.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1349 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0004_simplemention_post_type_webmention_post_type_and_more.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     3250 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0005_rebuild_pending_models_with_constraints.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2853 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0006_add_retryablemixin_pendingincomingwebmention_outgoingwebmentionstatus.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1076 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0007_dashboardpermissionproxy.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      361 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0008_alter_webmention_options.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      471 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0009_alter_outgoingwebmentionstatus_options.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      781 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0010_alter_hcard_avatar_alter_hcard_name.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      539 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/migrations/0011_alter_pendingoutgoingcontent_text.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)    16916 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/migrations/0012_alter_hcard_options_and_more.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      430 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0013_webmention_has_been_read.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-01-27 11:41:47.000000 django-wm-4.1.0.dev0/mentions/migrations/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.461822 django-wm-4.1.0.dev0/mentions/models/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      271 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/models/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      291 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/models/base.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2993 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/models/hcard.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.463030 django-wm-4.1.0.dev0/mentions/models/managers/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/models/managers/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      984 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/models/managers/webmention.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.466191 django-wm-4.1.0.dev0/mentions/models/mixins/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      137 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/models/mixins/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     4541 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/models/mixins/mentionable.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     3372 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/models/mixins/quotable.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2879 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/models/mixins/retryable.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2522 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/models/outgoing_status.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2169 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/models/pending.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.467615 django-wm-4.1.0.dev0/mentions/models/proxy/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       50 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/models/proxy/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      386 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/models/proxy/permissions.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      649 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/models/simple_mention.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1880 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/models/webmention.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     6958 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/options.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1178 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/permissions.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     5118 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/resolution.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.469782 django-wm-4.1.0.dev0/mentions/tasks/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      178 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/tasks/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1333 2022-10-12 15:23:17.000000 django-wm-4.1.0.dev0/mentions/tasks/celeryproxy.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.475664 django-wm-4.1.0.dev0/mentions/tasks/incoming/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       49 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1138 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/local.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.478332 django-wm-4.1.0.dev0/mentions/tasks/incoming/parsing/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       90 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/parsing/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     3496 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/parsing/hcard.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      981 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/parsing/post_type.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     4288 2023-05-07 14:23:52.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/process.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     3023 2023-05-07 14:24:22.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/remote.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2557 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/reverify.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      848 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/status.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.481712 django-wm-4.1.0.dev0/mentions/tasks/outgoing/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      125 2022-10-06 19:42:52.000000 django-wm-4.1.0.dev0/mentions/tasks/outgoing/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2483 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/tasks/outgoing/local.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.483137 django-wm-4.1.0.dev0/mentions/tasks/outgoing/parsing/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      159 2022-10-06 19:42:52.000000 django-wm-4.1.0.dev0/mentions/tasks/outgoing/parsing/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1893 2022-10-06 19:42:52.000000 django-wm-4.1.0.dev0/mentions/tasks/outgoing/parsing/webmention_endpoint.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2351 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/tasks/outgoing/process.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     5224 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/tasks/outgoing/remote.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     5707 2023-05-07 14:24:27.000000 django-wm-4.1.0.dev0/mentions/tasks/scheduling.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.410485 django-wm-4.1.0.dev0/mentions/templates/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.485443 django-wm-4.1.0.dev0/mentions/templates/mentions/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      261 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/templates/mentions/webmention-accepted.html
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     8130 2023-05-09 16:46:35.000000 django-wm-4.1.0.dev0/mentions/templates/mentions/webmention-dashboard.html
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      585 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/templates/mentions/webmention-submit-manual.html
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.488167 django-wm-4.1.0.dev0/mentions/templatetags/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-02-03 11:01:16.000000 django-wm-4.1.0.dev0/mentions/templatetags/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1766 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/templatetags/webmention_dashboard.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      332 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/templatetags/webmention_endpoint.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1317 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/templatetags/webmentions.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      942 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/urls.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.490590 django-wm-4.1.0.dev0/mentions/util/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      166 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/util/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      547 2022-10-06 19:42:52.000000 django-wm-4.1.0.dev0/mentions/util/html.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      559 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/util/requests.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      934 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/util/url.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.496248 django-wm-4.1.0.dev0/mentions/views/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      409 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/contract.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1338 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/dashboard.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2355 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/retrieve.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1810 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/serialize.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1804 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/submit.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      486 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/view_names.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      112 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/pyproject.toml
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1104 2023-05-09 17:16:22.497443 django-wm-4.1.0.dev0/setup.cfg
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       69 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/setup.py
```

### Comparing `django-wm-4.0.2/LICENSE` & `django-wm-4.1.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/PKG-INFO` & `django-wm-4.1.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-wm
-Version: 4.0.2
+Version: 4.1.0.dev0
 Summary: Webmention support for Django.
 Home-page: https://beatonma.org/webmentions_tester/
 Author: Michael Beaton
 Author-email: michael@beatonma.org
 License: GPLv3
 Project-URL: Source, https://github.com/beatonma/django-wm
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-wm Version: 4.0.2 Summary: Webmention
+Metadata-Version: 2.1 Name: django-wm Version: 4.1.0.dev0 Summary: Webmention
 support for Django. Home-page: https://beatonma.org/webmentions_tester/ Author:
 Michael Beaton Author-email: michael@beatonma.org License: GPLv3 Project-URL:
 Source, https://github.com/beatonma/django-wm Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `django-wm-4.0.2/README.md` & `django-wm-4.1.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/django_wm.egg-info/PKG-INFO` & `django-wm-4.1.0.dev0/django_wm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-wm
-Version: 4.0.2
+Version: 4.1.0.dev0
 Summary: Webmention support for Django.
 Home-page: https://beatonma.org/webmentions_tester/
 Author: Michael Beaton
 Author-email: michael@beatonma.org
 License: GPLv3
 Project-URL: Source, https://github.com/beatonma/django-wm
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-wm Version: 4.0.2 Summary: Webmention
+Metadata-Version: 2.1 Name: django-wm Version: 4.1.0.dev0 Summary: Webmention
 support for Django. Home-page: https://beatonma.org/webmentions_tester/ Author:
 Michael Beaton Author-email: michael@beatonma.org License: GPLv3 Project-URL:
 Source, https://github.com/beatonma/django-wm Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `django-wm-4.0.2/django_wm.egg-info/SOURCES.txt` & `django-wm-4.1.0.dev0/django_wm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 django_wm.egg-info/dependency_links.txt
 django_wm.egg-info/requires.txt
 django_wm.egg-info/top_level.txt
 mentions/__init__.py
 mentions/admin.py
 mentions/apps.py
 mentions/config.py
+mentions/context_processors.py
 mentions/contract.py
 mentions/exceptions.py
 mentions/microformats.py
 mentions/options.py
 mentions/permissions.py
 mentions/resolution.py
 mentions/urls.py
@@ -47,22 +48,25 @@
 mentions/migrations/0006_add_retryablemixin_pendingincomingwebmention_outgoingwebmentionstatus.py
 mentions/migrations/0007_dashboardpermissionproxy.py
 mentions/migrations/0008_alter_webmention_options.py
 mentions/migrations/0009_alter_outgoingwebmentionstatus_options.py
 mentions/migrations/0010_alter_hcard_avatar_alter_hcard_name.py
 mentions/migrations/0011_alter_pendingoutgoingcontent_text.py
 mentions/migrations/0012_alter_hcard_options_and_more.py
+mentions/migrations/0013_webmention_has_been_read.py
 mentions/migrations/__init__.py
 mentions/models/__init__.py
 mentions/models/base.py
 mentions/models/hcard.py
 mentions/models/outgoing_status.py
 mentions/models/pending.py
 mentions/models/simple_mention.py
 mentions/models/webmention.py
+mentions/models/managers/__init__.py
+mentions/models/managers/webmention.py
 mentions/models/mixins/__init__.py
 mentions/models/mixins/mentionable.py
 mentions/models/mixins/quotable.py
 mentions/models/mixins/retryable.py
 mentions/models/proxy/__init__.py
 mentions/models/proxy/permissions.py
 mentions/tasks/__init__.py
```

### Comparing `django-wm-4.0.2/mentions/admin.py` & `django-wm-4.1.0.dev0/mentions/admin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,221 +1,179 @@
 from django import forms
 from django.contrib import admin
-from django.utils.html import format_html
-from django.utils.translation import gettext_lazy as _
 
 from mentions.models import (
     HCard,
     OutgoingWebmentionStatus,
     PendingIncomingWebmention,
     PendingOutgoingContent,
     SimpleMention,
     Webmention,
 )
+from mentions.models.managers.webmention import WebmentionQuerySet
 
 RETRYABLEMIXIN_FIELDS = [
     "is_awaiting_retry",
     "last_retry_attempt",
     "retry_attempt_count",
 ]
 
 
 @admin.action(permissions=["change"])
-def approve_webmention(modeladmin, request, queryset):
-    queryset.update(approved=True)
+def mark_webmention_approved(modeladmin, request, queryset: WebmentionQuerySet):
+    queryset.mark_as_approved()
 
 
 @admin.action(permissions=["change"])
-def disapprove_webmention(modeladmin, request, queryset):
-    queryset.update(approved=False)
+def mark_webmention_unapproved(modeladmin, request, queryset: WebmentionQuerySet):
+    queryset.mark_as_unapproved()
 
 
-class BaseAdmin(admin.ModelAdmin):
-    save_on_top = True
-
-
-class ClickableUrlMixin:
-    def clickable_source_url(self, obj):
-        return clickable_link(obj.source_url)
-
-    clickable_source_url.short_description = _("source URL")
+@admin.action(permissions=["change"])
+def mark_webmention_read(modeladmin, request, queryset: WebmentionQuerySet):
+    queryset.mark_as_read()
 
-    def clickable_target_url(self, obj):
-        return clickable_link(obj.target_url)
 
-    clickable_target_url.short_description = _("target URL")
+@admin.action(permissions=["change"])
+def mark_webmention_unread(modeladmin, request, queryset: WebmentionQuerySet):
+    queryset.mark_as_unread()
 
 
-class TextAreaForm(forms.ModelForm):
-    class Meta:
-        widgets = {
-            "quote": forms.Textarea(attrs={"rows": 3}),
-            "notes": forms.Textarea(attrs={"rows": 3}),
-        }
+class BaseAdmin(admin.ModelAdmin):
+    save_on_top = True
 
 
 @admin.register(SimpleMention)
 class QuotableAdmin(BaseAdmin):
-    form = TextAreaForm
-    date_hierarchy = "published"
     list_display = [
         "source_url",
         "target_url",
-        "get_hcard_name",
-        "published",
+        "hcard",
     ]
-    list_filter = [
-        "post_type",
+    search_fields = [
+        "source_url",
+        "target_url",
+        "hcard",
     ]
     readonly_fields = [
         "target_object",
         "published",
     ]
-    search_fields = [
-        "quote",
-        "source_url",
-        "target_url",
-        "hcard__name",
-        "hcard__homepage",
-    ]
+    date_hierarchy = "published"
 
-    def get_hcard_name(self, obj):
-        if obj.hcard:
-            return obj.hcard.name
 
-    get_hcard_name.short_description = _("h-card name")
+class WebmentionModelForm(forms.ModelForm):
+    class Meta:
+        model = Webmention
+        widgets = {
+            "quote": forms.Textarea(attrs={"rows": 3}),
+            "notes": forms.Textarea(attrs={"rows": 3}),
+        }
+        fields = "__all__"
 
 
 @admin.register(Webmention)
-class WebmentionAdmin(ClickableUrlMixin, QuotableAdmin):
-    form = TextAreaForm
+class WebmentionAdmin(QuotableAdmin):
+    form = WebmentionModelForm
+    readonly_fields = QuotableAdmin.readonly_fields + [
+        "content_type",
+        "object_id",
+    ]
     actions = [
-        approve_webmention,
-        disapprove_webmention,
+        mark_webmention_approved,
+        mark_webmention_unapproved,
+        mark_webmention_read,
+        mark_webmention_unread,
     ]
     list_display = [
         "source_url",
         "target_url",
-        "get_hcard_name",
+        "has_been_read",
+        "published",
         "validated",
         "approved",
-        "published",
         "target_object",
     ]
-    list_filter = ["validated", "approved"] + QuotableAdmin.list_filter
     fieldsets = (
         (
             "Remote source",
             {
                 "fields": (
-                    "clickable_source_url",
+                    "source_url",
                     "sent_by",
                     "hcard",
                     "quote",
                     "post_type",
                 ),
             },
         ),
         (
             "Local target",
             {
                 "fields": (
-                    "clickable_target_url",
+                    "target_url",
                     "content_type",
                     "object_id",
                     "target_object",
                 ),
             },
         ),
         (
             "Metadata",
             {
                 "fields": (
                     "published",
+                    "has_been_read",
                     "approved",
                     "validated",
                     "notes",
                 ),
             },
         ),
     )
-    readonly_fields = QuotableAdmin.readonly_fields + [
-        "content_type",
-        "object_id",
-        "clickable_source_url",
-        "clickable_target_url",
-        "sent_by",
-    ]
 
 
 @admin.register(OutgoingWebmentionStatus)
-class OutgoingWebmentionStatusAdmin(ClickableUrlMixin, BaseAdmin):
-    date_hierarchy = "created_at"
-    list_display = [
-        "source_url",
-        "target_url",
-        "successful",
+class OutgoingWebmentionStatusAdmin(BaseAdmin):
+    readonly_fields = [
         "created_at",
-    ]
-    list_filter = [
-        "successful",
-        "is_awaiting_retry",
-    ]
-    search_fields = [
         "source_url",
         "target_url",
-    ]
-    exclude = [
-        "source_url",
-        "target_url",
-    ]
-    readonly_fields = [
-        "created_at",
-        "clickable_source_url",
-        "clickable_target_url",
         "target_webmention_endpoint",
         "status_message",
         "response_code",
         "successful",
         *RETRYABLEMIXIN_FIELDS,
     ]
+    list_display = [
+        "source_url",
+        "target_url",
+        "successful",
+        "created_at",
+    ]
+    date_hierarchy = "created_at"
 
 
 @admin.register(HCard)
 class HCardAdmin(BaseAdmin):
     list_display = ["name", "homepage"]
     search_fields = ["name", "homepage"]
 
 
 @admin.register(PendingIncomingWebmention)
 class PendingIncomingAdmin(BaseAdmin):
-    list_filter = [
-        "is_awaiting_retry",
-    ]
     readonly_fields = [
         "created_at",
         "source_url",
         "target_url",
         "sent_by",
         *RETRYABLEMIXIN_FIELDS,
     ]
-    search_fields = [
-        "source_url",
-        "target_url",
-    ]
 
 
 @admin.register(PendingOutgoingContent)
 class PendingOutgoingAdmin(BaseAdmin):
     readonly_fields = [
         "created_at",
         "absolute_url",
         "text",
     ]
-    search_fields = [
-        "absolute_url",
-        "text",
-    ]
-
-
-def clickable_link(url: str) -> str:
-    return format_html(f"<a href={url}>{url}</a>")
```

### Comparing `django-wm-4.0.2/mentions/config.py` & `django-wm-4.1.0.dev0/mentions/config.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/exceptions.py` & `django-wm-4.1.0.dev0/mentions/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/helpers/resolution.py` & `django-wm-4.1.0.dev0/mentions/helpers/resolution.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/helpers/thirdparty/wagtail/proxy.py` & `django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/proxy.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/helpers/thirdparty/wagtail/resolution.py` & `django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/resolution.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/helpers/thirdparty/wagtail/urls.py` & `django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/urls.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/helpers/thirdparty/wagtail/util.py` & `django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/util.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/helpers/types.py` & `django-wm-4.1.0.dev0/mentions/helpers/types.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/helpers/urls.py` & `django-wm-4.1.0.dev0/mentions/helpers/urls.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/helpers/util.py` & `django-wm-4.1.0.dev0/mentions/helpers/util.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/management/commands/mentions_pending.py` & `django-wm-4.1.0.dev0/mentions/management/commands/mentions_pending.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/management/commands/mentions_reverify.py` & `django-wm-4.1.0.dev0/mentions/management/commands/mentions_reverify.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/middleware/webmention_head_middleware.py` & `django-wm-4.1.0.dev0/mentions/middleware/webmention_head_middleware.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/migrations/0001_initial.py` & `django-wm-4.1.0.dev0/mentions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/migrations/0002_pendingincomingwebmention_pendingoutgoingcontent.py` & `django-wm-4.1.0.dev0/mentions/migrations/0002_pendingincomingwebmention_pendingoutgoingcontent.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/migrations/0003_alter_simplemention_published_and_more.py` & `django-wm-4.1.0.dev0/mentions/migrations/0003_alter_simplemention_published_and_more.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/migrations/0004_simplemention_post_type_webmention_post_type_and_more.py` & `django-wm-4.1.0.dev0/mentions/migrations/0004_simplemention_post_type_webmention_post_type_and_more.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/migrations/0005_rebuild_pending_models_with_constraints.py` & `django-wm-4.1.0.dev0/mentions/migrations/0005_rebuild_pending_models_with_constraints.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/migrations/0006_add_retryablemixin_pendingincomingwebmention_outgoingwebmentionstatus.py` & `django-wm-4.1.0.dev0/mentions/migrations/0006_add_retryablemixin_pendingincomingwebmention_outgoingwebmentionstatus.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/migrations/0007_dashboardpermissionproxy.py` & `django-wm-4.1.0.dev0/mentions/migrations/0007_dashboardpermissionproxy.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/migrations/0010_alter_hcard_avatar_alter_hcard_name.py` & `django-wm-4.1.0.dev0/mentions/migrations/0010_alter_hcard_avatar_alter_hcard_name.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/migrations/0011_alter_pendingoutgoingcontent_text.py` & `django-wm-4.1.0.dev0/mentions/migrations/0011_alter_pendingoutgoingcontent_text.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/migrations/0012_alter_hcard_options_and_more.py` & `django-wm-4.1.0.dev0/mentions/migrations/0012_alter_hcard_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/models/hcard.py` & `django-wm-4.1.0.dev0/mentions/models/hcard.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/models/mixins/mentionable.py` & `django-wm-4.1.0.dev0/mentions/models/mixins/mentionable.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/models/mixins/quotable.py` & `django-wm-4.1.0.dev0/mentions/models/mixins/quotable.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/models/mixins/retryable.py` & `django-wm-4.1.0.dev0/mentions/models/mixins/retryable.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/models/outgoing_status.py` & `django-wm-4.1.0.dev0/mentions/models/outgoing_status.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/models/pending.py` & `django-wm-4.1.0.dev0/mentions/models/pending.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/models/simple_mention.py` & `django-wm-4.1.0.dev0/mentions/models/simple_mention.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/models/webmention.py` & `django-wm-4.1.0.dev0/mentions/models/webmention.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from mentions import options
 from mentions.models.base import MentionsBaseModel
+from mentions.models.managers.webmention import WebmentionQuerySet
 from mentions.models.mixins import QuotableMixin
 
 __all__ = [
     "Webmention",
 ]
 
 
 def _approve_default():
     return options.auto_approve()
 
 
 class Webmention(QuotableMixin, MentionsBaseModel):
     """An incoming webmention that is received by your server."""
 
+    objects = WebmentionQuerySet.as_manager()
+
     sent_by = models.URLField(
         _("sent by"),
         blank=True,
         help_text=_("Source address of the HTTP request that sent this webmention."),
     )
 
     approved = models.BooleanField(
@@ -32,14 +35,18 @@
         _("validated"),
         default=False,
         help_text=_(
             "True if both source and target have been validated, "
             "confirmed to exist, and source really does link to target."
         ),
     )
+    has_been_read = models.BooleanField(
+        _("Read"),
+        default=False,
+    )
 
     notes = models.CharField(
         _("notes"),
         max_length=1024,
         blank=True,
         help_text=_(
             "A description of any errors encountered when building this Webmention."
```

### Comparing `django-wm-4.0.2/mentions/options.py` & `django-wm-4.1.0.dev0/mentions/options.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/permissions.py` & `django-wm-4.1.0.dev0/mentions/permissions.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from django.contrib.auth.models import Permission
 from django.utils.translation import gettext_lazy as _
 
 from mentions.apps import MentionsConfig
 
 __all__ = [
+    "can_change_webmention",
     "can_view_dashboard",
 ]
 
 
 @dataclass
 class MentionsPermission:
     codename: str
@@ -35,7 +36,13 @@
         return self.fqn()
 
 
 can_view_dashboard = MentionsPermission(
     "view_webmention_dashboard",
     _("Can view the webmention dashboard/status page."),
 )
+
+
+# The following permissions are created automatically by Django.
+can_change_webmention = MentionsPermission(
+    "change_webmention", _("Default 'change' permission for Webmention model.")
+)
```

### Comparing `django-wm-4.0.2/mentions/resolution.py` & `django-wm-4.1.0.dev0/mentions/resolution.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,39 +131,41 @@
     except ObjectDoesNotExist:
         raise TargetDoesNotExist(
             f"Cannot find instance of model `{model_class}` with kwargs=`{urlpattern_kwargs}`"
         )
 
 
 def get_mentions_for_url(url: str) -> List[QuotableMixin]:
+    if "://" not in url:
+        url = config.build_url(url)
+
     try:
         obj = get_model_for_url(url)
         return obj.get_mentions()
 
     except NoModelForUrlPath:
         pass
 
-    if "://" not in url:
-        url = config.build_url(url)
-
     return get_public_mentions(target_url=url)
 
 
 def get_mentions_for_view(request: HttpRequest) -> List[QuotableMixin]:
     return get_mentions_for_url(request.build_absolute_uri())
 
 
 def get_mentions_for_object(obj: MentionableMixin) -> List[QuotableMixin]:
     ctype = ContentType.objects.get_for_model(obj.__class__)
 
     return get_public_mentions(content_type=ctype, object_id=obj.id)
 
 
-def get_public_mentions(**filter) -> List[QuotableMixin]:
-    webmentions = Webmention.objects.filter(
-        **filter,
-        approved=True,
-        validated=True,
+def get_public_mentions(**filter_kwargs) -> List[QuotableMixin]:
+    webmentions = Webmention.objects.filter_public().filter(**filter_kwargs)
+    simple_mentions = SimpleMention.objects.filter(**filter_kwargs)
+
+    return list(
+        sorted(
+            list(webmentions) + list(simple_mentions),
+            key=lambda x: x.created_at,
+            reverse=True,
+        )
     )
-    simple_mentions = SimpleMention.objects.filter(**filter)
-
-    return list(webmentions) + list(simple_mentions)
```

### Comparing `django-wm-4.0.2/mentions/tasks/celeryproxy.py` & `django-wm-4.1.0.dev0/mentions/tasks/celeryproxy.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/tasks/incoming/local.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/local.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/tasks/incoming/parsing/hcard.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/parsing/hcard.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/tasks/incoming/parsing/post_type.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/parsing/post_type.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/tasks/incoming/process.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/process.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/tasks/incoming/remote.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/remote.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/tasks/incoming/reverify.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/reverify.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/tasks/incoming/status.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/status.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/tasks/outgoing/local.py` & `django-wm-4.1.0.dev0/mentions/tasks/outgoing/local.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/tasks/outgoing/parsing/webmention_endpoint.py` & `django-wm-4.1.0.dev0/mentions/tasks/outgoing/parsing/webmention_endpoint.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/tasks/outgoing/process.py` & `django-wm-4.1.0.dev0/mentions/tasks/outgoing/process.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/tasks/outgoing/remote.py` & `django-wm-4.1.0.dev0/mentions/tasks/outgoing/remote.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/tasks/scheduling.py` & `django-wm-4.1.0.dev0/mentions/tasks/scheduling.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/templates/mentions/webmention-dashboard.html` & `django-wm-4.1.0.dev0/mentions/templates/mentions/webmention-dashboard.html`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/templates/mentions/webmention-submit-manual.html` & `django-wm-4.1.0.dev0/mentions/templates/mentions/webmention-submit-manual.html`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/templatetags/webmention_dashboard.py` & `django-wm-4.1.0.dev0/mentions/templatetags/webmention_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/templatetags/webmentions.py` & `django-wm-4.1.0.dev0/mentions/templatetags/webmentions.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/urls.py` & `django-wm-4.1.0.dev0/mentions/urls.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/util/html.py` & `django-wm-4.1.0.dev0/mentions/util/html.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/util/requests.py` & `django-wm-4.1.0.dev0/mentions/util/requests.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/util/url.py` & `django-wm-4.1.0.dev0/mentions/util/url.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/views/dashboard.py` & `django-wm-4.1.0.dev0/mentions/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/views/retrieve.py` & `django-wm-4.1.0.dev0/mentions/views/retrieve.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/views/serialize.py` & `django-wm-4.1.0.dev0/mentions/views/serialize.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/mentions/views/submit.py` & `django-wm-4.1.0.dev0/mentions/views/submit.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.2/setup.cfg` & `django-wm-4.1.0.dev0/setup.cfg`

 * *Files identical despite different names*

