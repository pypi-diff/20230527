# Comparing `tmp/klu-0.1.4.tar.gz` & `tmp/klu-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klu-0.1.4.tar", max compression
+gzip compressed data, was "klu-0.1.5.tar", max compression
```

## Comparing `klu-0.1.4.tar` & `klu-0.1.5.tar`

### file list

```diff
@@ -1,82 +1,84 @@
--rw-r--r--   0        0        0     1070 2023-04-02 23:20:08.165888 klu-0.1.4/LICENSE
--rw-r--r--   0        0        0     2901 2023-05-17 21:55:04.290201 klu-0.1.4/README.md
--rw-r--r--   0        0        0      156 2023-05-07 13:13:15.007463 klu-0.1.4/klu/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/action/__init__.py
--rw-r--r--   0        0        0    12135 2023-05-25 10:19:42.438116 klu-0.1.4/klu/action/client.py
--rw-r--r--   0        0        0      272 2023-05-23 00:00:29.822238 klu-0.1.4/klu/action/constants.py
--rw-r--r--   0        0        0      542 2023-05-01 22:54:25.386914 klu-0.1.4/klu/action/errors.py
--rw-r--r--   0        0        0     1700 2023-05-24 12:53:09.893852 klu-0.1.4/klu/action/models.py
--rw-r--r--   0        0        0        0 2023-04-16 12:33:25.776741 klu-0.1.4/klu/api/__init__.py
--rw-r--r--   0        0        0     3516 2023-05-24 00:48:31.834759 klu-0.1.4/klu/api/client.py
--rw-r--r--   0        0        0      199 2023-05-16 02:22:01.505533 klu-0.1.4/klu/api/config.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648620 klu-0.1.4/klu/application/__init__.py
--rw-r--r--   0        0        0     7677 2023-05-22 23:57:57.911029 klu-0.1.4/klu/application/client.py
--rw-r--r--   0        0        0      259 2023-05-22 23:48:54.892441 klu-0.1.4/klu/application/constants.py
--rw-r--r--   0        0        0      325 2023-05-18 00:09:26.025264 klu-0.1.4/klu/application/errors.py
--rw-r--r--   0        0        0     1303 2023-05-16 01:32:56.622223 klu-0.1.4/klu/application/models.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/client/__init__.py
--rw-r--r--   0        0        0      714 2023-05-16 00:56:56.414877 klu-0.1.4/klu/client/klu.py
--rw-r--r--   0        0        0        0 2023-04-17 20:44:45.994154 klu-0.1.4/klu/common/__init__.py
--rw-r--r--   0        0        0     3103 2023-05-17 23:44:49.628180 klu-0.1.4/klu/common/client.py
--rw-r--r--   0        0        0     2967 2023-05-18 00:09:26.039775 klu-0.1.4/klu/common/errors.py
--rw-r--r--   0        0        0     2268 2023-05-07 22:15:35.049953 klu-0.1.4/klu/common/models.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/data/__init__.py
--rw-r--r--   0        0        0     2240 2023-05-17 21:42:29.875608 klu-0.1.4/klu/data/client.py
--rw-r--r--   0        0        0       24 2023-04-20 00:36:52.119366 klu-0.1.4/klu/data/constants.py
--rw-r--r--   0        0        0      281 2023-05-18 00:09:26.054468 klu-0.1.4/klu/data/errors.py
--rw-r--r--   0        0        0     2537 2023-05-16 00:57:12.476673 klu-0.1.4/klu/data/models.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/data_index/__init__.py
--rw-r--r--   0        0        0     8445 2023-05-22 18:49:52.214610 klu-0.1.4/klu/data_index/client.py
--rw-r--r--   0        0        0      289 2023-05-15 02:29:51.422572 klu-0.1.4/klu/data_index/constants.py
--rw-r--r--   0        0        0      316 2023-05-18 00:09:26.046973 klu-0.1.4/klu/data_index/errors.py
--rw-r--r--   0        0        0     3263 2023-05-21 21:41:28.245219 klu-0.1.4/klu/data_index/models.py
--rw-r--r--   0        0        0       19 2023-04-02 23:20:08.167789 klu-0.1.4/klu/klu.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/model/__init__.py
--rw-r--r--   0        0        0     3450 2023-05-22 18:50:10.373905 klu-0.1.4/klu/model/client.py
--rw-r--r--   0        0        0       27 2023-04-22 00:45:10.009144 klu-0.1.4/klu/model/constants.py
--rw-r--r--   0        0        0      454 2023-05-18 00:09:26.016842 klu-0.1.4/klu/model/errors.py
--rw-r--r--   0        0        0     1193 2023-05-17 00:20:41.308393 klu-0.1.4/klu/model/models.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/session/__init__.py
--rw-r--r--   0        0        0     1412 2023-05-16 01:10:51.006332 klu-0.1.4/klu/session/client.py
--rw-r--r--   0        0        0       31 2023-05-15 22:59:54.895982 klu-0.1.4/klu/session/constants.py
--rw-r--r--   0        0        0     1094 2023-05-16 00:57:12.477952 klu-0.1.4/klu/session/models.py
--rw-r--r--   0        0        0      111 2023-05-11 23:52:15.155255 klu-0.1.4/klu/utils/dict_helpers.py
--rw-r--r--   0        0        0      719 2023-05-01 22:31:07.149352 klu-0.1.4/klu/utils/file_upload.py
--rw-r--r--   0        0        0     2308 2023-05-22 23:37:24.956177 klu-0.1.4/klu/utils/paginator.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/workspace/__init__.py
--rw-r--r--   0        0        0     7968 2023-05-23 00:00:29.836509 klu-0.1.4/klu/workspace/client.py
--rw-r--r--   0        0        0      321 2023-05-22 23:57:57.890361 klu-0.1.4/klu/workspace/constants.py
--rw-r--r--   0        0        0      244 2023-05-18 00:09:26.033318 klu-0.1.4/klu/workspace/errors.py
--rw-r--r--   0        0        0      815 2023-05-15 22:31:50.548346 klu-0.1.4/klu/workspace/models.py
--rw-r--r--   0        0        0     2797 2023-05-25 10:18:27.765075 klu-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       33 2023-04-02 23:20:08.169124 klu-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      103 2023-05-15 22:17:30.645200 klu-0.1.4/tests/integration/__init__.py
--rw-r--r--   0        0        0      128 2023-05-21 22:12:08.785805 klu-0.1.4/tests/integration/conftest.py
--rw-r--r--   0        0        0      252 2023-05-24 21:54:58.783798 klu-0.1.4/tests/integration/constants.py
--rw-r--r--   0        0        0        0 2023-05-17 01:53:20.259063 klu-0.1.4/tests/integration/files/__init__.py
--rw-r--r--   0        0        0   108574 2021-08-07 16:43:25.870000 klu-0.1.4/tests/integration/files/test-file-upload.pdf
--rw-r--r--   0        0        0     4782 2023-05-24 23:20:44.781905 klu-0.1.4/tests/integration/test_actions.py
--rw-r--r--   0        0        0     3749 2023-05-22 23:33:40.123465 klu-0.1.4/tests/integration/test_applications.py
--rw-r--r--   0        0        0     1148 2023-05-17 01:34:42.355919 klu-0.1.4/tests/integration/test_data.py
--rw-r--r--   0        0        0     2864 2023-05-21 21:55:43.590354 klu-0.1.4/tests/integration/test_data_index.py
--rw-r--r--   0        0        0      958 2023-05-17 01:35:15.023120 klu-0.1.4/tests/integration/test_models.py
--rw-r--r--   0        0        0     2263 2023-05-17 01:35:19.655390 klu-0.1.4/tests/integration/test_workspaces.py
--rw-r--r--   0        0        0     1435 2023-05-24 12:44:20.921698 klu-0.1.4/tests/integration/utils/actions.py
--rw-r--r--   0        0        0      752 2023-05-17 01:19:00.668605 klu-0.1.4/tests/integration/utils/applications.py
--rw-r--r--   0        0        0       68 2023-05-15 22:17:30.698602 klu-0.1.4/tests/integration/utils/common.py
--rw-r--r--   0        0        0     1555 2023-05-17 01:27:25.631403 klu-0.1.4/tests/integration/utils/data.py
--rw-r--r--   0        0        0      816 2023-05-17 01:27:25.638985 klu-0.1.4/tests/integration/utils/data_index.py
--rw-r--r--   0        0        0      830 2023-05-24 23:19:18.771498 klu-0.1.4/tests/integration/utils/models.py
--rw-r--r--   0        0        0      842 2023-05-17 01:19:00.583265 klu-0.1.4/tests/integration/utils/sessions.py
--rw-r--r--   0        0        0      658 2023-05-17 01:19:00.519346 klu-0.1.4/tests/integration/utils/workspace.py
--rw-r--r--   0        0        0        0 2023-05-08 13:03:00.679856 klu-0.1.4/tests/unit/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/tests/unit/action/__init__.py
--rw-r--r--   0        0        0     1692 2023-05-23 00:20:51.639436 klu-0.1.4/tests/unit/action/test_client.py
--rw-r--r--   0        0        0     1156 2023-05-15 21:48:29.904995 klu-0.1.4/tests/unit/action/utils.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/tests/unit/application/__init__.py
--rw-r--r--   0        0        0     1433 2023-05-23 00:20:51.607538 klu-0.1.4/tests/unit/application/test_client.py
--rw-r--r--   0        0        0     1170 2023-05-16 00:57:16.848585 klu-0.1.4/tests/unit/application/utils.py
--rw-r--r--   0        0        0      156 2023-05-21 22:55:55.517974 klu-0.1.4/tests/unit/conftest.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0      768 2023-05-01 22:56:20.546102 klu-0.1.4/tests/unit/utils/mock.py
--rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 klu-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-02 23:20:08.165888 klu-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2957 2023-05-26 00:37:42.513833 klu-0.1.5/README.md
+-rw-r--r--   0        0        0      150 2023-05-27 14:30:24.721088 klu-0.1.5/klu/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/action/__init__.py
+-rw-r--r--   0        0        0    11171 2023-05-26 00:17:00.539207 klu-0.1.5/klu/action/client.py
+-rw-r--r--   0        0        0      280 2023-05-27 13:56:44.465656 klu-0.1.5/klu/action/constants.py
+-rw-r--r--   0        0        0      542 2023-05-01 22:54:25.386914 klu-0.1.5/klu/action/errors.py
+-rw-r--r--   0        0        0     1700 2023-05-24 12:53:09.893852 klu-0.1.5/klu/action/models.py
+-rw-r--r--   0        0        0        0 2023-04-16 12:33:25.776741 klu-0.1.5/klu/api/__init__.py
+-rw-r--r--   0        0        0     3039 2023-05-25 23:34:25.415214 klu-0.1.5/klu/api/client.py
+-rw-r--r--   0        0        0      199 2023-05-27 14:00:15.080309 klu-0.1.5/klu/api/config.py
+-rw-r--r--   0        0        0      118 2023-05-25 23:21:28.634469 klu-0.1.5/klu/api/constants.py
+-rw-r--r--   0        0        0     1429 2023-05-26 00:23:42.481009 klu-0.1.5/klu/api/sse_client.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648620 klu-0.1.5/klu/application/__init__.py
+-rw-r--r--   0        0        0     7677 2023-05-22 23:57:57.911029 klu-0.1.5/klu/application/client.py
+-rw-r--r--   0        0        0      259 2023-05-27 13:56:44.512450 klu-0.1.5/klu/application/constants.py
+-rw-r--r--   0        0        0      325 2023-05-18 00:09:26.025264 klu-0.1.5/klu/application/errors.py
+-rw-r--r--   0        0        0     1303 2023-05-16 01:32:56.622223 klu-0.1.5/klu/application/models.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/client/__init__.py
+-rw-r--r--   0        0        0      794 2023-05-26 00:09:53.956182 klu-0.1.5/klu/client/klu.py
+-rw-r--r--   0        0        0        0 2023-04-17 20:44:45.994154 klu-0.1.5/klu/common/__init__.py
+-rw-r--r--   0        0        0     3146 2023-05-27 13:10:59.677590 klu-0.1.5/klu/common/client.py
+-rw-r--r--   0        0        0     2967 2023-05-18 00:09:26.039775 klu-0.1.5/klu/common/errors.py
+-rw-r--r--   0        0        0     2268 2023-05-07 22:15:35.049953 klu-0.1.5/klu/common/models.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/data/__init__.py
+-rw-r--r--   0        0        0     2240 2023-05-17 21:42:29.875608 klu-0.1.5/klu/data/client.py
+-rw-r--r--   0        0        0       25 2023-05-27 12:58:54.884230 klu-0.1.5/klu/data/constants.py
+-rw-r--r--   0        0        0      281 2023-05-18 00:09:26.054468 klu-0.1.5/klu/data/errors.py
+-rw-r--r--   0        0        0     2537 2023-05-16 00:57:12.476673 klu-0.1.5/klu/data/models.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/data_index/__init__.py
+-rw-r--r--   0        0        0     8445 2023-05-22 18:49:52.214610 klu-0.1.5/klu/data_index/client.py
+-rw-r--r--   0        0        0      287 2023-05-27 13:56:44.504025 klu-0.1.5/klu/data_index/constants.py
+-rw-r--r--   0        0        0      316 2023-05-18 00:09:26.046973 klu-0.1.5/klu/data_index/errors.py
+-rw-r--r--   0        0        0     3263 2023-05-21 21:41:28.245219 klu-0.1.5/klu/data_index/models.py
+-rw-r--r--   0        0        0       19 2023-04-02 23:20:08.167789 klu-0.1.5/klu/klu.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/model/__init__.py
+-rw-r--r--   0        0        0     3450 2023-05-22 18:50:10.373905 klu-0.1.5/klu/model/client.py
+-rw-r--r--   0        0        0       28 2023-05-27 12:58:54.475873 klu-0.1.5/klu/model/constants.py
+-rw-r--r--   0        0        0      454 2023-05-18 00:09:26.016842 klu-0.1.5/klu/model/errors.py
+-rw-r--r--   0        0        0     1193 2023-05-17 00:20:41.308393 klu-0.1.5/klu/model/models.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/session/__init__.py
+-rw-r--r--   0        0        0     1412 2023-05-16 01:10:51.006332 klu-0.1.5/klu/session/client.py
+-rw-r--r--   0        0        0       32 2023-05-27 12:58:54.666310 klu-0.1.5/klu/session/constants.py
+-rw-r--r--   0        0        0     1094 2023-05-16 00:57:12.477952 klu-0.1.5/klu/session/models.py
+-rw-r--r--   0        0        0      111 2023-05-11 23:52:15.155255 klu-0.1.5/klu/utils/dict_helpers.py
+-rw-r--r--   0        0        0      719 2023-05-01 22:31:07.149352 klu-0.1.5/klu/utils/file_upload.py
+-rw-r--r--   0        0        0     2308 2023-05-22 23:37:24.956177 klu-0.1.5/klu/utils/paginator.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/workspace/__init__.py
+-rw-r--r--   0        0        0     7968 2023-05-23 00:00:29.836509 klu-0.1.5/klu/workspace/client.py
+-rw-r--r--   0        0        0      321 2023-05-27 13:56:44.493674 klu-0.1.5/klu/workspace/constants.py
+-rw-r--r--   0        0        0      244 2023-05-18 00:09:26.033318 klu-0.1.5/klu/workspace/errors.py
+-rw-r--r--   0        0        0      815 2023-05-15 22:31:50.548346 klu-0.1.5/klu/workspace/models.py
+-rw-r--r--   0        0        0     2820 2023-05-27 14:30:24.732873 klu-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-04-02 23:20:08.169124 klu-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-15 22:17:30.645200 klu-0.1.5/tests/integration/__init__.py
+-rw-r--r--   0        0        0      128 2023-05-26 00:17:59.829216 klu-0.1.5/tests/integration/conftest.py
+-rw-r--r--   0        0        0      252 2023-05-27 14:00:25.824775 klu-0.1.5/tests/integration/constants.py
+-rw-r--r--   0        0        0        0 2023-05-17 01:53:20.259063 klu-0.1.5/tests/integration/files/__init__.py
+-rw-r--r--   0        0        0   108574 2021-08-07 16:43:25.870000 klu-0.1.5/tests/integration/files/test-file-upload.pdf
+-rw-r--r--   0        0        0     4826 2023-05-27 14:02:35.049808 klu-0.1.5/tests/integration/test_actions.py
+-rw-r--r--   0        0        0     3749 2023-05-27 14:01:15.447974 klu-0.1.5/tests/integration/test_applications.py
+-rw-r--r--   0        0        0     1148 2023-05-17 01:34:42.355919 klu-0.1.5/tests/integration/test_data.py
+-rw-r--r--   0        0        0     2864 2023-05-21 21:55:43.590354 klu-0.1.5/tests/integration/test_data_index.py
+-rw-r--r--   0        0        0      958 2023-05-17 01:35:15.023120 klu-0.1.5/tests/integration/test_models.py
+-rw-r--r--   0        0        0     2212 2023-05-27 14:01:44.839869 klu-0.1.5/tests/integration/test_workspaces.py
+-rw-r--r--   0        0        0     1435 2023-05-24 12:44:20.921698 klu-0.1.5/tests/integration/utils/actions.py
+-rw-r--r--   0        0        0      752 2023-05-17 01:19:00.668605 klu-0.1.5/tests/integration/utils/applications.py
+-rw-r--r--   0        0        0       68 2023-05-15 22:17:30.698602 klu-0.1.5/tests/integration/utils/common.py
+-rw-r--r--   0        0        0     1555 2023-05-17 01:27:25.631403 klu-0.1.5/tests/integration/utils/data.py
+-rw-r--r--   0        0        0      816 2023-05-17 01:27:25.638985 klu-0.1.5/tests/integration/utils/data_index.py
+-rw-r--r--   0        0        0      830 2023-05-24 23:19:18.771498 klu-0.1.5/tests/integration/utils/models.py
+-rw-r--r--   0        0        0      842 2023-05-17 01:19:00.583265 klu-0.1.5/tests/integration/utils/sessions.py
+-rw-r--r--   0        0        0      658 2023-05-17 01:19:00.519346 klu-0.1.5/tests/integration/utils/workspace.py
+-rw-r--r--   0        0        0        0 2023-05-08 13:03:00.679856 klu-0.1.5/tests/unit/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/tests/unit/action/__init__.py
+-rw-r--r--   0        0        0     1692 2023-05-23 00:20:51.639436 klu-0.1.5/tests/unit/action/test_client.py
+-rw-r--r--   0        0        0     1156 2023-05-15 21:48:29.904995 klu-0.1.5/tests/unit/action/utils.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/tests/unit/application/__init__.py
+-rw-r--r--   0        0        0     1433 2023-05-23 00:20:51.607538 klu-0.1.5/tests/unit/application/test_client.py
+-rw-r--r--   0        0        0     1170 2023-05-16 00:57:16.848585 klu-0.1.5/tests/unit/application/utils.py
+-rw-r--r--   0        0        0      156 2023-05-21 22:55:55.517974 klu-0.1.5/tests/unit/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0      768 2023-05-01 22:56:20.546102 klu-0.1.5/tests/unit/utils/mock.py
+-rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 klu-0.1.5/PKG-INFO
```

### Comparing `klu-0.1.4/LICENSE` & `klu-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/README.md` & `klu-0.1.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -29,56 +29,63 @@
 ```
 
 ## Getting Started
 
 To use the Klu.AI Python SDK, you must first obtain an API key from the Klu.AI website. Once you have your API key, you can create a `KluClient` object:
 
 ```python
-from klu.client.klu import KluClient
+from klu import KluClient
 
-api_key = "YOUR_API_KEY"
-client = KluClient(api_key)
+client = KluClient("YOUR_API_KEY")
 ```
 
 Once you have a `KluClient` object, you can access the different models available in the Klu API:
 
 ```python
-from klu.client.klu import KluClient
+from klu import KluClient
 
-api_key = "YOUR_API_KEY"
-client = KluClient(api_key)
+client = KluClient("YOUR_API_KEY")
+
+models = await client.models.get("model_guid")
 
-models = client.models.get_models()
-data = client.data.get_action_data("action_guid")
-application = client.applications.get("application_guid")
-action = client.actions.run_action_prompt("action_id", "prompt")
-workspace = client.workspace.get_workspace_apps("workspace_guid")
-data_index = client.data_index.process_data_index("data_index_id", "splitter")
 ```
 
+There is also a separate function to stream action prompt
+
 Each of these objects provides methods for interacting with the corresponding model in the Klu API. For example, to list all applications in your workspace, you can use:
 
 ```python
-from klu.client.klu import KluClient
+from klu import KluClient
 
-api_key = "YOUR_API_KEY"
-client = KluClient(api_key)
+client = KluClient("YOUR_API_KEY")
 applications = client.applications.list()
 ```
 
 In a similar manner, in order to get a list of data points for an action, you can do the following
 
 ```python
-from klu.client.klu import KluClient
+from klu import KluClient
 
-api_key = "YOUR_API_KEY"
-client = KluClient(api_key)
+client = KluClient("YOUR_API_KEY")
 data = client.data.get_action_data("action_id")
 ```
 
+There is a special client that allows to stream action prompts.
+The streaming url can be received from the action creation response.
+
+```python
+from klu import KluClient
+
+client = KluClient("YOUR_API_KEY")
+
+prompt_response = await client.actions.run_action_prompt("action_guid", "prompt", streaming=True)
+async for message in client.sse_client.get_streaming_data(prompt_response.streaming_url):
+    print(message)
+```
+
 ## Development
 For more detailed developer information, please refer to the [Developer's README](README.dev.md).
 
 ## Documentation
 
 For more detailed information on how to use the Klu.AI Python SDK, please refer to the [API documentation](https://docs.klu.ai/).
```

### Comparing `klu-0.1.4/klu/action/client.py` & `klu-0.1.5/klu/action/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import aiohttp
+
 from typing import Optional, List
 
-import aiohttp
 from aiohttp import ClientResponseError
 from aiohttp.web_exceptions import HTTPNotFound
 
 from klu.common.errors import (
     UnknownKluError,
     UnknownKluAPIError,
     InvalidUpdateParamsError,
@@ -214,55 +215,32 @@
                 if e.status == 400:
                     raise InvalidActionPromptData(e.message)
 
                 raise UnknownKluAPIError(e.status, e.message)
             except Exception:
                 raise UnknownKluError()
 
-    # async def get_action_streaming_data(self, streaming_url: str) -> AsyncIterator[str]:
-    #     """
-    #     Get a streams of messages from an SQS queue for a specific channel.
-    #
-    #     Args:
-    #         streaming_url (str): The url you received from run_action_prompt with streaming param set to True.
-    #
-    #     Returns:
-    #         An asynchronous generator, which can be used to read chunks of data from the streaming url. Usage example:
-    #
-    #         async for chunk in get_streaming_data():
-    #             # Process the chunk of data here
-    #             print(chunk)
-    #     """
-    #     async with aiohttp.ClientSession() as session:
-    #         client = self._get_api_client(session)
-    #
-    #         async for data in client.get_streaming_data(streaming_url):
-    #             if data == "No messages to stream":
-    #                 client.get_streaming_data(streaming_url).aclose()
-    #
-    #             yield data
-
-    async def get_action_data(self, id: str) -> List[Data]:
+    async def get_action_data(self, guid: str) -> List[Data]:
         """
         Retrieves data information for an action.
 
         Args:
-            id (str): Guid of an action to fetch data for.
+            guid (str): Guid of an action to fetch data for.
 
         Returns: An array of actions found by provided app id.
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
 
             try:
-                response = await client.get(ACTION_DATA_ENDPOINT.format(id=id))
+                response = await client.get(ACTION_DATA_ENDPOINT.format(id=guid))
                 return [Data._from_engine_format(data) for data in response]
             except (HTTPNotFound, ClientResponseError) as e:
                 if e.status == 404:
-                    raise ActionNotFoundError(id)
+                    raise ActionNotFoundError(guid)
 
                 raise UnknownKluAPIError(e.status, e.message)
             except Exception:
                 raise UnknownKluError()
 
     async def list(self) -> List[Action]:
         """
```

### Comparing `klu-0.1.4/klu/action/errors.py` & `klu-0.1.5/klu/action/errors.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/action/models.py` & `klu-0.1.5/klu/action/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/api/client.py` & `klu-0.1.5/klu/api/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from functools import wraps
-
 import aiohttp
 
-from typing import List, Union, Optional, AsyncIterator
+from functools import wraps
+from typing import List, Union, Optional
 
 from aiohttp import ClientResponseError
 from aiohttp.web_exceptions import HTTPNotFound
 
-from klu.api.config import get_api_url
 from klu.common.errors import (
     UnknownKluError,
     InvalidDataSent,
     UnauthorizedError,
     BadRequestAPIError,
     UnknownKluAPIError,
     InvalidApiMethodUsedError,
 )
+from klu.api.config import get_api_url
 
 
 def _handle_http_exception(func):
     @wraps(func)
     async def wrapper(*args, **kwargs):
         try:
             return await func(*args, **kwargs)
@@ -85,20 +84,7 @@
 
     @_handle_http_exception
     async def delete(self, path: str) -> dict:
         url = f"{self.api_url}{path}"
         async with self.session.delete(url, headers=self.headers) as response:
             response.raise_for_status()
             return await response.json()
-
-    async def get_streaming_data(self, url: str) -> AsyncIterator[str]:
-        try:
-            async with self.session.get(url) as response:
-                response.raise_for_status()
-
-                async for data in response.content.iter_any():
-                    yield data.decode("utf-8")
-
-        except ClientResponseError as e:
-            raise UnknownKluAPIError(e.status, e.message)
-        except Exception:
-            raise UnknownKluError()
```

### Comparing `klu-0.1.4/klu/application/client.py` & `klu-0.1.5/klu/application/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/application/models.py` & `klu-0.1.5/klu/application/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/client/klu.py` & `klu-0.1.5/klu/client/klu.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from klu.data.client import DataClient
+from klu.api.sse_client import SSEClient
 from klu.model.client import ModelsClient
 from klu.action.client import ActionsClient
 from klu.session.client import SessionClient
 from klu.workspace.client import WorkspaceClient
 from klu.data_index.client import DataIndexClient
 from klu.application.client import ApplicationsClient
 
 
 class KluClient:
     def __init__(self, api_key: str):
+        self.sse_client = SSEClient()
+
         self.data = DataClient(api_key)
         self.models = ModelsClient(api_key)
         self.actions = ActionsClient(api_key)
         self.sessions = SessionClient(api_key)
         self.workspace = WorkspaceClient(api_key)
         self.data_index = DataIndexClient(api_key)
         self.applications = ApplicationsClient(api_key)
```

### Comparing `klu-0.1.4/klu/common/client.py` & `klu-0.1.5/klu/common/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,26 @@
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
                 response = await client.post(url or self._base_path, kwargs)
                 return self._model._from_engine_format(response)
             except (HTTPNotFound, ClientResponseError) as e:
                 if e.status == 404:
-                    raise InstanceRelationshipNotFoundError(self._model.__name__, e.message)
+                    raise InstanceRelationshipNotFoundError(
+                        self._model.__name__, e.message
+                    )
 
                 raise e
 
     @abstractmethod
     async def get(self, id: KluId) -> T:
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
-                response = await client.get(f"{self._base_path}/{id}")
+                response = await client.get(f"{self._base_path}{id}")
                 return self._model._from_engine_format(response)
             except (HTTPNotFound, ClientResponseError) as e:
                 if e.status == 404:
                     raise InstanceNotFoundError(self._model.__name__, id)
 
                 raise e
 
@@ -60,27 +62,27 @@
         id = kwargs.pop("id", None)
         if not id:
             raise IdNotProvidedError()
 
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
-                response = await client.put(f"{self._base_path}/{id}", kwargs)
+                response = await client.put(f"{self._base_path}{id}", kwargs)
                 return self._model._from_engine_format(response)
             except (HTTPNotFound, ClientResponseError) as e:
                 if e.status == 404:
                     raise InstanceNotFoundError(self._model.__name__, id)
 
                 raise e
 
     @abstractmethod
     async def delete(self, id: KluId) -> T:
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
-                response = await client.delete(f"{self._base_path}/{id}")
+                response = await client.delete(f"{self._base_path}{id}")
                 return self._model._from_engine_format(response)
             except (HTTPNotFound, ClientResponseError) as e:
                 if e.status == 404:
                     raise InstanceNotFoundError(self._model.__name__, id)
 
                 raise e
```

### Comparing `klu-0.1.4/klu/common/errors.py` & `klu-0.1.5/klu/common/errors.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/common/models.py` & `klu-0.1.5/klu/common/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/data/client.py` & `klu-0.1.5/klu/data/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/data/models.py` & `klu-0.1.5/klu/data/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/data_index/client.py` & `klu-0.1.5/klu/data_index/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/data_index/models.py` & `klu-0.1.5/klu/data_index/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/model/client.py` & `klu-0.1.5/klu/model/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/model/models.py` & `klu-0.1.5/klu/model/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/session/client.py` & `klu-0.1.5/klu/session/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/session/models.py` & `klu-0.1.5/klu/session/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/utils/file_upload.py` & `klu-0.1.5/klu/utils/file_upload.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/utils/paginator.py` & `klu-0.1.5/klu/utils/paginator.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/workspace/client.py` & `klu-0.1.5/klu/workspace/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/klu/workspace/models.py` & `klu-0.1.5/klu/workspace/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/pyproject.toml` & `klu-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool]
 [tool.poetry]
 name = "klu"
-version = "0.1.4"
+version = "0.1.5"
 homepage = "https://github.com/ssabev/klu"
 description = "SDK for building AI Enabled apps."
-authors = ["Stefan Sabev <stefan@launchpad.pm>"]
+authors = ["Stefan Sabev <stefan@klu.ai>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
@@ -22,14 +22,15 @@
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.6.2,<4.0"
 aiohttp = "3.8.4"
 aiofiles = "23.1.0"
+aiohttp-sse-client = "0.2.1"
 
 black  = { version = "^21.5b2", optional = true}
 isort  = { version = "^5.8.0", optional = true}
 flake8  = { version = "^3.9.2", optional = true}
 flake8-docstrings = { version = "^1.6.0", optional = true }
 mypy = {version = "^0.900", optional = true}
 pytest  = { version = "^6.2.4", optional = true}
```

### Comparing `klu-0.1.4/tests/integration/files/test-file-upload.pdf` & `klu-0.1.5/tests/integration/files/test-file-upload.pdf`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/integration/test_actions.py` & `klu-0.1.5/tests/integration/test_actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import math
 import pytest
 
 # import asyncio
+#
+# from klu.api.sse_client import SSEClient
 
 from tests.integration import client
 from tests.integration.utils.data import create_data
 from tests.integration.utils.models import ModelSingleton
 from tests.integration.utils.applications import AppSingleton
 from tests.integration.utils.actions import create_action, ActionSingleton
 
@@ -22,19 +24,20 @@
 #         "What are the risks of Artificial general intelligence?",
 #         streaming=True,
 #     )
 #     action_streaming_url = action_prompt_result.streaming_url
 #     assert action_streaming_url is not None
 #
 #     await asyncio.sleep(5)
-#     data = None
-#     async for data in client.actions.get_action_streaming_data(action_streaming_url):
-#         assert data is not None
+#     tokens = []
+#     async for token in SSEClient.get_streaming_data(action_streaming_url):
+#         tokens.append(token)
 #
-#     assert data == "No messages to stream"
+#     print("".join(tokens))
+#     assert len(tokens) > 0
 
 
 @pytest.mark.asyncio
 async def test_run_action_prompt():
     action = await action_singleton.get_default_action()
     action_prompt_result = await client.actions.run_action_prompt(
         action.guid, "test", "test", False
```

### Comparing `klu-0.1.4/tests/integration/test_applications.py` & `klu-0.1.5/tests/integration/test_applications.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/integration/test_data.py` & `klu-0.1.5/tests/integration/test_data.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/integration/test_data_index.py` & `klu-0.1.5/tests/integration/test_data_index.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/integration/test_models.py` & `klu-0.1.5/tests/integration/test_models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/integration/test_workspaces.py` & `klu-0.1.5/tests/integration/test_workspaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import pytest
 
 from klu.client.klu import KluClient
 
 from tests.integration.constants import API_KEY
-from tests.integration.utils.applications import create_application
-from tests.integration.utils.workspace import create_workspace, get_unique_test_ws_name, WorkspaceSingleton
+from tests.integration.utils.workspace import (
+    create_workspace,
+    WorkspaceSingleton,
+    get_unique_test_ws_name,
+)
 
 client = KluClient(API_KEY)
 workspace_singleton = WorkspaceSingleton()
 
 
 # TODO requires creation of an api_key for new workspace because app workspace is retrieved based on the api_key provided
 # @pytest.mark.asyncio
```

### Comparing `klu-0.1.4/tests/integration/utils/actions.py` & `klu-0.1.5/tests/integration/utils/actions.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/integration/utils/applications.py` & `klu-0.1.5/tests/integration/utils/applications.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/integration/utils/data.py` & `klu-0.1.5/tests/integration/utils/data.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/integration/utils/data_index.py` & `klu-0.1.5/tests/integration/utils/data_index.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/integration/utils/models.py` & `klu-0.1.5/tests/integration/utils/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/integration/utils/sessions.py` & `klu-0.1.5/tests/integration/utils/sessions.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/integration/utils/workspace.py` & `klu-0.1.5/tests/integration/utils/workspace.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/unit/action/test_client.py` & `klu-0.1.5/tests/unit/action/test_client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/unit/action/utils.py` & `klu-0.1.5/tests/unit/action/utils.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/unit/application/test_client.py` & `klu-0.1.5/tests/unit/application/test_client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/unit/application/utils.py` & `klu-0.1.5/tests/unit/application/utils.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/tests/unit/utils/mock.py` & `klu-0.1.5/tests/unit/utils/mock.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.4/PKG-INFO` & `klu-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: klu
-Version: 0.1.4
+Version: 0.1.5
 Summary: SDK for building AI Enabled apps.
 Home-page: https://github.com/ssabev/klu
 License: MIT
 Author: Stefan Sabev
-Author-email: stefan@launchpad.pm
+Author-email: stefan@klu.ai
 Requires-Python: >=3.6.2,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: aiofiles (==23.1.0)
 Requires-Dist: aiohttp (==3.8.4)
+Requires-Dist: aiohttp-sse-client (==0.2.1)
 Requires-Dist: black (>=21.5b2,<22.0) ; extra == "test"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
 Requires-Dist: flake8 (>=3.9.2,<4.0.0) ; extra == "test"
 Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
 Requires-Dist: isort (>=5.8.0,<6.0.0) ; extra == "test"
 Requires-Dist: mkdocs (>=1.1.2,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-autorefs (>=0.2.1,<0.3.0) ; extra == "doc"
@@ -75,56 +76,63 @@
 ```
 
 ## Getting Started
 
 To use the Klu.AI Python SDK, you must first obtain an API key from the Klu.AI website. Once you have your API key, you can create a `KluClient` object:
 
 ```python
-from klu.client.klu import KluClient
+from klu import KluClient
 
-api_key = "YOUR_API_KEY"
-client = KluClient(api_key)
+client = KluClient("YOUR_API_KEY")
 ```
 
 Once you have a `KluClient` object, you can access the different models available in the Klu API:
 
 ```python
-from klu.client.klu import KluClient
+from klu import KluClient
 
-api_key = "YOUR_API_KEY"
-client = KluClient(api_key)
+client = KluClient("YOUR_API_KEY")
+
+models = await client.models.get("model_guid")
 
-models = client.models.get_models()
-data = client.data.get_action_data("action_guid")
-application = client.applications.get("application_guid")
-action = client.actions.run_action_prompt("action_id", "prompt")
-workspace = client.workspace.get_workspace_apps("workspace_guid")
-data_index = client.data_index.process_data_index("data_index_id", "splitter")
 ```
 
+There is also a separate function to stream action prompt
+
 Each of these objects provides methods for interacting with the corresponding model in the Klu API. For example, to list all applications in your workspace, you can use:
 
 ```python
-from klu.client.klu import KluClient
+from klu import KluClient
 
-api_key = "YOUR_API_KEY"
-client = KluClient(api_key)
+client = KluClient("YOUR_API_KEY")
 applications = client.applications.list()
 ```
 
 In a similar manner, in order to get a list of data points for an action, you can do the following
 
 ```python
-from klu.client.klu import KluClient
+from klu import KluClient
 
-api_key = "YOUR_API_KEY"
-client = KluClient(api_key)
+client = KluClient("YOUR_API_KEY")
 data = client.data.get_action_data("action_id")
 ```
 
+There is a special client that allows to stream action prompts.
+The streaming url can be received from the action creation response.
+
+```python
+from klu import KluClient
+
+client = KluClient("YOUR_API_KEY")
+
+prompt_response = await client.actions.run_action_prompt("action_guid", "prompt", streaming=True)
+async for message in client.sse_client.get_streaming_data(prompt_response.streaming_url):
+    print(message)
+```
+
 ## Development
 For more detailed developer information, please refer to the [Developer's README](README.dev.md).
 
 ## Documentation
 
 For more detailed information on how to use the Klu.AI Python SDK, please refer to the [API documentation](https://docs.klu.ai/).
```

