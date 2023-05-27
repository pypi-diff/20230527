# Comparing `tmp/IntuneCD-1.4.6b1.tar.gz` & `tmp/IntuneCD-1.4.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IntuneCD-1.4.6b1.tar", last modified: Mon May 22 06:52:59 2023, max compression
+gzip compressed data, was "IntuneCD-1.4.7b1.tar", last modified: Sat May 27 12:22:39 2023, max compression
```

## Comparing `IntuneCD-1.4.6b1.tar` & `IntuneCD-1.4.7b1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.992976 IntuneCD-1.4.6b1/
--rw-r--r--   0 tobias     (501) staff       (20)     1059 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/LICENSE
--rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-05-22 06:52:59.993116 IntuneCD-1.4.6b1/PKG-INFO
--rw-r--r--   0 tobias     (501) staff       (20)     2697 2023-01-24 09:42:37.000000 IntuneCD-1.4.6b1/README.md
--rw-r--r--   0 tobias     (501) staff       (20)      103 2022-05-03 19:33:01.000000 IntuneCD-1.4.6b1/pyproject.toml
--rw-r--r--   0 tobias     (501) staff       (20)      999 2023-05-22 06:52:59.993592 IntuneCD-1.4.6b1/setup.cfg
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.958227 IntuneCD-1.4.6b1/src/
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.987295 IntuneCD-1.4.6b1/src/IntuneCD/
--rw-r--r--   0 tobias     (501) staff       (20)        0 2022-05-03 19:33:01.000000 IntuneCD-1.4.6b1/src/IntuneCD/__init__.py
--rw-r--r--   0 tobias     (501) staff       (20)     2344 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/archive.py
--rw-r--r--   0 tobias     (501) staff       (20)     3938 2023-03-20 07:54:18.000000 IntuneCD-1.4.6b1/src/IntuneCD/assignment_report.py
--rw-r--r--   0 tobias     (501) staff       (20)     2241 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_AppProtection.py
--rw-r--r--   0 tobias     (501) staff       (20)     1327 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_apns.py
--rw-r--r--   0 tobias     (501) staff       (20)     3001 2023-05-22 06:37:51.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_appConfiguration.py
--rw-r--r--   0 tobias     (501) staff       (20)     1865 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_appleEnrollmentProfile.py
--rw-r--r--   0 tobias     (501) staff       (20)     4651 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_applications.py
--rw-r--r--   0 tobias     (501) staff       (20)     1370 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_assignmentFilters.py
--rw-r--r--   0 tobias     (501) staff       (20)     1090 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_autopilotDevices.py
--rw-r--r--   0 tobias     (501) staff       (20)     2473 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_compliance.py
--rw-r--r--   0 tobias     (501) staff       (20)     1454 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_compliancePartner.py
--rw-r--r--   0 tobias     (501) staff       (20)     1655 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_conditionalAccess.py
--rw-r--r--   0 tobias     (501) staff       (20)     2386 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_configurationPolicies.py
--rw-r--r--   0 tobias     (501) staff       (20)     2718 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_customAttributeShellScript.py
--rw-r--r--   0 tobias     (501) staff       (20)     1245 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_deviceManagementSettings.py
--rw-r--r--   0 tobias     (501) staff       (20)     2359 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_enrollmentConfigurations.py
--rw-r--r--   0 tobias     (501) staff       (20)     2926 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_enrollmentStatusPage.py
--rw-r--r--   0 tobias     (501) staff       (20)     2508 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_groupPolicyConfiguration.py
--rw-r--r--   0 tobias     (501) staff       (20)     1378 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_managedGPlay.py
--rw-r--r--   0 tobias     (501) staff       (20)     2467 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_managementIntents.py
--rw-r--r--   0 tobias     (501) staff       (20)     1445 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_managementPartner.py
--rw-r--r--   0 tobias     (501) staff       (20)     1754 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_notificationTemplate.py
--rw-r--r--   0 tobias     (501) staff       (20)     2710 2023-05-16 06:42:29.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_powershellScripts.py
--rw-r--r--   0 tobias     (501) staff       (20)     3289 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_proactiveRemediation.py
--rw-r--r--   0 tobias     (501) staff       (20)     4962 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_profiles.py
--rw-r--r--   0 tobias     (501) staff       (20)     1486 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_remoteAssistancePartner.py
--rw-r--r--   0 tobias     (501) staff       (20)     2589 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_shellScripts.py
--rw-r--r--   0 tobias     (501) staff       (20)     1312 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_vppTokens.py
--rw-r--r--   0 tobias     (501) staff       (20)     1961 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_windowsEnrollmentProfile.py
--rw-r--r--   0 tobias     (501) staff       (20)      548 2022-08-09 15:09:09.000000 IntuneCD-1.4.6b1/src/IntuneCD/check_file.py
--rw-r--r--   0 tobias     (501) staff       (20)      515 2022-08-09 15:09:09.000000 IntuneCD-1.4.6b1/src/IntuneCD/clean_filename.py
--rw-r--r--   0 tobias     (501) staff       (20)     1933 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/diff_summary.py
--rw-r--r--   0 tobias     (501) staff       (20)    15819 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/documentation_functions.py
--rw-r--r--   0 tobias     (501) staff       (20)     3701 2023-03-08 08:59:36.000000 IntuneCD-1.4.6b1/src/IntuneCD/get_accesstoken.py
--rw-r--r--   0 tobias     (501) staff       (20)     3198 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/get_authparams.py
--rw-r--r--   0 tobias     (501) staff       (20)    10342 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/graph_batch.py
--rw-r--r--   0 tobias     (501) staff       (20)     7753 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/graph_request.py
--rw-r--r--   0 tobias     (501) staff       (20)      622 2022-08-09 15:09:09.000000 IntuneCD-1.4.6b1/src/IntuneCD/load_file.py
--rw-r--r--   0 tobias     (501) staff       (20)      987 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/remove_keys.py
--rw-r--r--   0 tobias     (501) staff       (20)    12362 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/run_backup.py
--rw-r--r--   0 tobias     (501) staff       (20)    12356 2023-03-20 12:09:40.000000 IntuneCD-1.4.6b1/src/IntuneCD/run_documentation.py
--rw-r--r--   0 tobias     (501) staff       (20)    11471 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/run_update.py
--rw-r--r--   0 tobias     (501) staff       (20)      934 2023-03-06 07:57:06.000000 IntuneCD-1.4.6b1/src/IntuneCD/save_output.py
--rw-r--r--   0 tobias     (501) staff       (20)     7900 2023-05-22 06:40:42.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_appConfiguration.py
--rw-r--r--   0 tobias     (501) staff       (20)     7963 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_appProtection.py
--rw-r--r--   0 tobias     (501) staff       (20)     3524 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_appleEnrollmentProfile.py
--rw-r--r--   0 tobias     (501) staff       (20)     7443 2023-03-06 09:55:38.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_assignment.py
--rw-r--r--   0 tobias     (501) staff       (20)     3741 2023-04-25 08:44:13.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_assignmentFilter.py
--rw-r--r--   0 tobias     (501) staff       (20)     9372 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_compliance.py
--rw-r--r--   0 tobias     (501) staff       (20)     7193 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_conditionalAccess.py
--rw-r--r--   0 tobias     (501) staff       (20)     7703 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_configurationPolicies.py
--rw-r--r--   0 tobias     (501) staff       (20)     8929 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_customAttributeShellScript.py
--rw-r--r--   0 tobias     (501) staff       (20)     2630 2023-03-20 12:09:40.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_deviceManagementSettings.py
--rw-r--r--   0 tobias     (501) staff       (20)    11648 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_enrollmentConfigurations.py
--rw-r--r--   0 tobias     (501) staff       (20)     8715 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_enrollmentStatusPage.py
--rw-r--r--   0 tobias     (501) staff       (20)      749 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_frontend.py
--rw-r--r--   0 tobias     (501) staff       (20)    24286 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_groupPolicyConfiguration.py
--rw-r--r--   0 tobias     (501) staff       (20)     9069 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_managementIntents.py
--rw-r--r--   0 tobias     (501) staff       (20)     8066 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_notificationTemplate.py
--rw-r--r--   0 tobias     (501) staff       (20)     8428 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_powershellScripts.py
--rw-r--r--   0 tobias     (501) staff       (20)    10612 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_proactiveRemediation.py
--rw-r--r--   0 tobias     (501) staff       (20)    16118 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_profiles.py
--rw-r--r--   0 tobias     (501) staff       (20)     8385 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_shellScripts.py
--rw-r--r--   0 tobias     (501) staff       (20)     7197 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_windowsEnrollmentProfile.py
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.988462 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/
--rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/PKG-INFO
--rw-r--r--   0 tobias     (501) staff       (20)     3153 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/SOURCES.txt
--rw-r--r--   0 tobias     (501) staff       (20)        1 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/dependency_links.txt
--rw-r--r--   0 tobias     (501) staff       (20)      179 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/entry_points.txt
--rw-r--r--   0 tobias     (501) staff       (20)      102 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/requires.txt
--rw-r--r--   0 tobias     (501) staff       (20)        9 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/top_level.txt
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.992787 IntuneCD-1.4.6b1/tests/
--rw-r--r--   0 tobias     (501) staff       (20)     2042 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/tests/test_archive.py
--rw-r--r--   0 tobias     (501) staff       (20)     2005 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_check_file.py
--rw-r--r--   0 tobias     (501) staff       (20)      848 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_clean_filename.py
--rw-r--r--   0 tobias     (501) staff       (20)     2096 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_diff_summary.py
--rw-r--r--   0 tobias     (501) staff       (20)     7233 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/tests/test_documentation_functions.py
--rw-r--r--   0 tobias     (501) staff       (20)      953 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_get_added_removed.py
--rw-r--r--   0 tobias     (501) staff       (20)     9753 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_get_authparams.py
--rw-r--r--   0 tobias     (501) staff       (20)    12241 2023-03-08 09:16:49.000000 IntuneCD-1.4.6b1/tests/test_graph_batch.py
--rw-r--r--   0 tobias     (501) staff       (20)    17428 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/tests/test_graph_request.py
--rw-r--r--   0 tobias     (501) staff       (20)     2980 2023-03-08 10:43:23.000000 IntuneCD-1.4.6b1/tests/test_group_report.py
--rw-r--r--   0 tobias     (501) staff       (20)     1279 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_load_file.py
--rw-r--r--   0 tobias     (501) staff       (20)     1622 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_match.py
--rw-r--r--   0 tobias     (501) staff       (20)      559 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_remove_keys.py
--rw-r--r--   0 tobias     (501) staff       (20)     1888 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_save_output.py
--rw-r--r--   0 tobias     (501) staff       (20)     2292 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_update_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:38.995552 IntuneCD-1.4.7b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/src/IntuneCD/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/assignment_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_AppProtection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_apns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_appConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_appleEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_assignmentFilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_autopilotDevices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_compliancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_conditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_configurationPolicies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_customAttributeShellScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_deviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_enrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_enrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_groupPolicyConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_managedGPlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_managementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_managementPartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_notificationTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_powershellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_proactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_remoteAssistancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_shellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_vppTokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_windowsEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/check_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/clean_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/diff_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/get_accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/get_authparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/graph_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/load_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/remove_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/run_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/run_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/run_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/save_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_appConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_appProtection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_appleEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_assignmentFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_conditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_configurationPolicies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_customAttributeShellScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_deviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_enrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_enrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_groupPolicyConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_managementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_notificationTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_powershellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_proactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16118 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_shellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_windowsEnrollmentProfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_check_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_clean_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_diff_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_get_added_removed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_get_authparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_graph_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17428 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_group_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_load_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_remove_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_save_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_update_frontend.py
```

### Comparing `IntuneCD-1.4.6b1/LICENSE` & `IntuneCD-1.4.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/PKG-INFO` & `IntuneCD-1.4.7b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.6b1
+Version: 1.4.7b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.6b1/README.md` & `IntuneCD-1.4.7b1/README.md`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/setup.cfg` & `IntuneCD-1.4.7b1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = IntuneCD
-version = 1.4.6.beta1
+version = 1.4.7.beta1
 author = Tobias Almén
 author_email = almenscorner@outlook.com
 description = Tool to backup and update configurations in Intune
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/almenscorner/IntuneCD
 project_urls =
```

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/archive.py` & `IntuneCD-1.4.7b1/src/IntuneCD/archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/assignment_report.py` & `IntuneCD-1.4.7b1/src/IntuneCD/assignment_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_AppProtection.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_AppProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_apns.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_apns.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_appConfiguration.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_appConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_appleEnrollmentProfile.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_applications.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_applications.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_assignmentFilters.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_assignmentFilters.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_autopilotDevices.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_autopilotDevices.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_compliance.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_compliancePartner.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_compliancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_conditionalAccess.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_conditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_configurationPolicies.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_configurationPolicies.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_customAttributeShellScript.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_customAttributeShellScript.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_deviceManagementSettings.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_enrollmentConfigurations.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_enrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_enrollmentStatusPage.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_enrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_groupPolicyConfiguration.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_groupPolicyConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_managedGPlay.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_managedGPlay.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_managementIntents.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_managementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_managementPartner.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_managementPartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_notificationTemplate.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_notificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_powershellScripts.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_powershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_proactiveRemediation.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_proactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_profiles.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_profiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_remoteAssistancePartner.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_remoteAssistancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_shellScripts.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_shellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_vppTokens.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_vppTokens.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/backup_windowsEnrollmentProfile.py` & `IntuneCD-1.4.7b1/src/IntuneCD/backup_windowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/check_file.py` & `IntuneCD-1.4.7b1/src/IntuneCD/check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/clean_filename.py` & `IntuneCD-1.4.7b1/src/IntuneCD/clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/diff_summary.py` & `IntuneCD-1.4.7b1/src/IntuneCD/diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/documentation_functions.py` & `IntuneCD-1.4.7b1/src/IntuneCD/documentation_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python3
 
 """
 This module contains all functions for the documentation.
 """
 
+import binascii
 import yaml
 import json
 import os
 import glob
 import re
 import platform
+import base64
 
 from pytablewriter import MarkdownTableWriter
 
 
 def md_file(outpath):
     """
     This function creates the markdown file.
@@ -120,25 +122,53 @@
     remove_chars = '#@}{]["'
     for char in remove_chars:
         string = string.replace(char, "")
 
     return string
 
 
-def clean_list(data):
+def is_base64(s):
+    try:
+        # Attempt to decode the string
+        if type(s) is str:
+            s = s.encode("utf-8")
+            base64.b64decode(s)
+            return True
+    except binascii.Error:
+        # If decoding fails, it's not base64 encoded
+        return False
+
+
+def decode_base64(data):
+    """
+    This function decodes the data if it is base64 encoded.
+    :param data: The data to be decoded
+    :return: The decoded data
+    """
+
+    try:
+        return base64.b64decode(data).decode("utf-8")
+    except Exception:
+        return data
+
+
+def clean_list(data, decode):
     """
     This function returns a list with strings to be used in a table.
     :param data: The data to be cleaned
     :return: The list of strings
     """
 
     def list_to_string(l) -> str:
         string = ""
         for i in l:
             if isinstance(i, (str, int, bool)):
+                if decode:
+                    if is_base64(i):
+                        i = decode_base64(i)
                 string += f"<li> {i} </li>"
             elif isinstance(i, dict):
                 string += dict_to_string(i)
             else:
                 string += i
 
         return string
@@ -158,21 +188,33 @@
                     elif isinstance(v, dict):
                         for k2, v2 in v.items():
                             if isinstance(v2, list):
                                 string += f"**{k2}:** <ul>"
                                 string += list_to_string(v2)
                                 string += "</ul>"
                             elif isinstance(v2, (str, bool, int)):
+                                if decode:
+                                    if is_base64(v2):
+                                        v2 = decode_base64(v2)
                                 string += f"**{k2}:** {v2}</br>"
                             else:
+                                if decode:
+                                    if is_base64(v2):
+                                        v2 = decode_base64(v2)
                                 string += f"**{k2}:** {v2}</br>"
                     else:
+                        if decode:
+                            if is_base64(v):
+                                v = decode_base64(v)
                         string += f"**{k}:** {v}</br>"
                 string += "</ul>"
             else:
+                if decode:
+                    if is_base64(val):
+                        val = decode_base64(val)
                 string += f"**{key}:** {val}<br/>"
 
         string += "<br/>"
 
         return string
 
     def dict_to_table(d) -> str:
@@ -189,33 +231,45 @@
                         string += list_to_string(v)
                         string += "</ul>"
                     elif isinstance(v, dict):
                         string += f"**{k}** <ul>"
                         string += dict_to_string(v)
                         string += "</ul>"
                     else:
+                        if decode:
+                            if is_base64(v):
+                                v = decode_base64(v)
                         string += f"**{k}:** {v}</br>"
             else:
+                if decode:
+                    if is_base64(val):
+                        val = decode_base64(val)
                 string += f"**{key}:** {val}</br>"
 
         return string
 
     def list_string(l) -> str:
         string = ""
         for i in l:
             if isinstance(i, (str, int, bool)):
+                if decode:
+                    if is_base64(i):
+                        i = decode_base64(i)
                 string += f"{i}<br/>"
             if isinstance(i, list):
                 string += list_to_string(i)
             if isinstance(i, dict):
                 string += dict_to_string(i)
 
         return string
 
     def string(s) -> str:
+        if decode:
+            if is_base64(s):
+                s = decode_base64(s)
         if len(s) > 200:
             string = f"<details><summary>Click to expand...</summary>{item}</details>"
         else:
             string = item
 
         return string
 
@@ -232,15 +286,15 @@
             values.append(item)
         else:
             values.append(item)
 
     return values
 
 
-def document_configs(configpath, outpath, header, max_length, split, cleanup):
+def document_configs(configpath, outpath, header, max_length, split, cleanup, decode):
     """
     This function documents the configuration.
 
     :param configpath: The path to where the backup files are saved
     :param outpath: The path to save the Markdown document to
     :param header: Header of the configuration being documented
     :param max_length: The maximum length of the configuration to write to the Markdown document
@@ -279,15 +333,15 @@
                 if "description" in repo_data:
                     if repo_data["description"] is not None:
                         description = repo_data["description"]
                         repo_data.pop("description")
 
                 # Write configuration Markdown table
                 config_table_list = []
-                for key, value in zip(repo_data.keys(), clean_list(repo_data.values())):
+                for key, value in zip(repo_data.keys(), clean_list(repo_data.values(), decode)):
                     if cleanup:
                         if not value and type(value) is not bool:
                             continue
 
                     if key == "@odata.type":
                         key = "Odata type"
 
@@ -296,14 +350,18 @@
                         key = re.findall("[A-Z][^A-Z]*", key)
                         key = " ".join(key)
 
                     if max_length:
                         if value and isinstance(value, str) and len(value) > max_length:
                             value = "Value too long to display"
 
+                    if decode:
+                        if is_base64(value):
+                            value = decode_base64(value)
+
                     config_table_list.append([key, value])
 
                 config_table = write_table(config_table_list)
 
                 # Write data to file
                 with open(outpath, "a") as md:
                     if "displayName" in repo_data:
@@ -311,15 +369,15 @@
                     if "name" in repo_data:
                         md.write("## " + repo_data["name"] + "\n")
                     if description:
                         md.write(f"Description: {escape_markdown(description)} \n")
                     if assignments_table:
                         md.write("### Assignments \n")
                         md.write(str(assignments_table) + "\n")
-                    md.write('### Configuration \n')
+                    md.write("### Configuration \n")
                     md.write(str(config_table) + "\n")
 
 
 def document_management_intents(configpath, outpath, header, split):
     """
     This function documents the management intents.
 
@@ -386,15 +444,15 @@
                 if "description" in repo_data:
                     if repo_data["description"] is not None:
                         description = repo_data["description"]
                         repo_data.pop("description")
 
                 intent_table_list = []
 
-                for key, value in zip(repo_data.keys(), clean_list(repo_data.values())):
+                for key, value in zip(repo_data.keys(), clean_list(repo_data.values(), decode=False)):
                     key = key[0].upper() + key[1:]
                     key = re.findall("[A-Z][^A-Z]*", key)
                     key = " ".join(key)
 
                     if value and isinstance(value, str):
                         if len(value.split(",")) > 1:
                             vals = []
@@ -417,15 +475,15 @@
                     if "name" in repo_data:
                         md.write("## " + repo_data["name"] + "\n")
                     if description:
                         md.write(f"Description: {escape_markdown(description)} \n")
                     if assignments_table:
                         md.write("### Assignments \n")
                         md.write(str(assignments_table) + "\n")
-                    md.write('### Configuration \n')
+                    md.write("### Configuration \n")
                     md.write(str(config_table) + "\n")
 
 
 def get_md_files(configpath):
     """
     This function gets the Markdown files in the configpath directory.
     :return: List of Markdown files
```

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/get_accesstoken.py` & `IntuneCD-1.4.7b1/src/IntuneCD/get_accesstoken.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/get_authparams.py` & `IntuneCD-1.4.7b1/src/IntuneCD/get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/graph_batch.py` & `IntuneCD-1.4.7b1/src/IntuneCD/graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/graph_request.py` & `IntuneCD-1.4.7b1/src/IntuneCD/graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/load_file.py` & `IntuneCD-1.4.7b1/src/IntuneCD/load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/remove_keys.py` & `IntuneCD-1.4.7b1/src/IntuneCD/remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/run_backup.py` & `IntuneCD-1.4.7b1/src/IntuneCD/run_backup.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/run_documentation.py` & `IntuneCD-1.4.7b1/src/IntuneCD/run_documentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,17 +32,15 @@
     get_md_files,
 )
 
 REPO_DIR = os.environ.get("REPO_DIR")
 
 
 def start():
-    parser = argparse.ArgumentParser(
-        description="Create markdown document from backup files"
-    )
+    parser = argparse.ArgumentParser(description="Create markdown document from backup files")
     parser.add_argument(
         "-p",
         "--path",
         help="Path to where the backup is saved, default is REPO_DIR",
         default=REPO_DIR,
     )
     parser.add_argument(
@@ -80,304 +78,331 @@
     )
     parser.add_argument(
         "-c",
         "--cleanup",
         help="If set, will remove all table rows with an empty value",
         action="store_true",
     )
+    parser.add_argument(
+        "-d",
+        "--decode",
+        help="If set, will decode all base64 encoded values",
+        action="store_true",
+    )
 
     args = parser.parse_args()
 
-    def run_documentation(
-        configpath, outpath, tenantname, jsondata, maxlength, split, cleanup
-    ):
+    def run_documentation(configpath, outpath, tenantname, jsondata, maxlength, split, cleanup, decode):
         now = datetime.now()
         current_date = now.strftime("%d/%m/%Y %H:%M:%S")
 
         if not split:
             md_file(outpath)
 
         # Document App Configuration
         document_configs(
             f"{configpath}/App Configuration",
             outpath,
             "App Configuration",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document App Protection
         document_configs(
             f"{configpath}/App Protection",
             outpath,
             "App Protection",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Apple Push Notification
         document_configs(
             f"{configpath}/Apple Push Notification",
             outpath,
             "Apple Push Notification",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Apple VPP Tokens
         document_configs(
             f"{configpath}/Apple VPP Tokens",
             outpath,
             "Apple VPP Tokens",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document iOS Applications
         document_configs(
             f"{configpath}/Applications/iOS",
             outpath,
             "iOS Applications",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document macOS Applications
         document_configs(
             f"{configpath}/Applications/macOS",
             outpath,
             "macOS Applications",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Android Applications
         document_configs(
             f"{configpath}/Applications/Android",
             outpath,
             "Android Applications",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Windows Applications
         document_configs(
             f"{configpath}/Applications/Windows",
             outpath,
             "Windows Applications",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Web Apps
         document_configs(
             f"{configpath}/Applications/Web App",
             outpath,
             "Web Applications",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Office Suite apps
         document_configs(
             f"{configpath}/Applications/Office Suite",
             outpath,
             "Office Suite Applications",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document compliance
         document_configs(
             f"{configpath}/Compliance Policies/Policies",
             outpath,
             "Compliance Policies",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Message Templates
         document_configs(
             f"{configpath}/Compliance Policies/Message Templates",
             outpath,
             "Message Templates",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Conditional Access
         document_configs(
             f"{configpath}/Conditional Access",
             outpath,
             "Conditional Access",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document profiles
         document_configs(
             f"{configpath}/Device Configurations",
             outpath,
             "Configuration Profiles",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Device Management Settings
         document_configs(
             f"{configpath}/Device Management Settings",
             outpath,
             "Device Management Settings",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Group Policy Configurations
         document_configs(
             f"{configpath}/Group Policy Configurations",
             outpath,
             "Group Policy Configurations",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Apple Enrollment Profiles
         document_configs(
             f"{configpath}/Enrollment Profiles/Apple",
             outpath,
             "Apple Enrollment Profiles",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Windows Enrollment Profiles
         document_configs(
             f"{configpath}/Enrollment Profiles/Windows",
             outpath,
             "Windows Enrollment Profiles",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Enrollment Status Page profiles
         document_configs(
             f"{configpath}/Enrollment Profiles/Windows/ESP",
             outpath,
             "Enrollment Status Page",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Enrollment Configurations
         document_configs(
             f"{configpath}/Enrollment Configurations",
             outpath,
             "Enrollment Configurations",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document filters
-        document_configs(
-            f"{configpath}/Filters", outpath, "Filters", maxlength, split, cleanup
-        )
+        document_configs(f"{configpath}/Filters", outpath, "Filters", maxlength, split, cleanup, decode)
 
         # Managed Google Play
         document_configs(
             f"{configpath}/Managed Google Play",
             outpath,
             "Managed Google Play",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Intents
-        document_management_intents(
-            f"{configpath}/Management Intents/", outpath, "Management Intents", split
-        )
+        document_management_intents(f"{configpath}/Management Intents/", outpath, "Management Intents", split)
 
         # Document Partner Connections
         document_configs(
             f"{configpath}/Partner Connections/",
             outpath,
             "Partner Connections",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Proactive Remediations
         document_configs(
             f"{configpath}/Proactive Remediations",
             outpath,
             "Proactive Remediations",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Shell Scripts
         document_configs(
             f"{configpath}/Scripts/Shell",
             outpath,
             "Shell Scripts",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Custom Attributes
         document_configs(
             f"{configpath}/Custom Attributes",
             outpath,
             "Custom Attributes",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Powershell Scripts
         document_configs(
             f"{configpath}/Scripts/Powershell",
             outpath,
             "Powershell Scripts",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         # Document Settings Catalog
         document_configs(
             f"{configpath}/Settings Catalog",
             outpath,
             "Settings Catalog",
             maxlength,
             split,
             cleanup,
+            decode,
         )
 
         if jsondata:
             json_dict = json.loads(jsondata)
             if "title" in json_dict:
                 title = json_dict["title"]
             else:
@@ -420,17 +445,15 @@
                             "](",
                             str(file).replace(" ", "%20"),
                             ") \n\n",
                         ]
                     )
 
         else:
-            document = markdown_toclify(
-                input_file=outpath, back_to_top=True, exclude_h=[3]
-            )
+            document = markdown_toclify(input_file=outpath, back_to_top=True, exclude_h=[3])
             with open(outpath, "w") as doc:
                 l1 = f"# {title} \n\n"
                 l2 = f"{intro} \n\n"
                 l3 = f"{tenant} \n\n"
                 l4 = f"{updated} {current_date} \n\n"
                 doc.writelines([l1, l2, l3, l4, document])
 
@@ -438,12 +461,13 @@
         args.path,
         args.outpath,
         args.tenantname,
         args.jsondata,
         args.maxlength,
         args.split,
         args.cleanup,
+        args.decode,
     )
 
 
 if __name__ == "__main__":
     start()
```

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/run_update.py` & `IntuneCD-1.4.7b1/src/IntuneCD/run_update.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/save_output.py` & `IntuneCD-1.4.7b1/src/IntuneCD/save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_appConfiguration.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_appConfiguration.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,24 +122,30 @@
                                 token,
                             )
 
                 # If App Configuration does not exist, create it and assign
                 else:
                     print("-" * 90)
                     print("App Configuration not found, creating: " + repo_data["displayName"])
+
+                    if repo_data.get("payloadJson"):
+                        repo_data["payloadJson"] = base64.b64encode(
+                            json.dumps(repo_data["payloadJson"]).encode("utf-8")
+                        ).decode("utf-8")
+
                     app_ids = {}
                     # If backup contains targeted apps, search for the app
                     if repo_data["targetedMobileApps"]:
                         q_param = {
                             "$filter": "(isof("
                             + "'"
                             + str(repo_data["targetedMobileApps"]["type"]).replace("#", "")
                             + "'"
                             + "))",
-                            "$search": repo_data["targetedMobileApps"]["appName"],
+                            "$search": f'"{repo_data["targetedMobileApps"]["appName"]}"',
                         }
                         app_request = makeapirequest(APP_ENDPOINT, token, q_param)
                         if app_request["value"]:
                             app_ids = app_request["value"][0]["id"]
                     # If the app could be found and matches type and name in
                     # backup, continue to create
                     if app_ids and report is False:
```

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_appProtection.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_appProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_appleEnrollmentProfile.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_assignment.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_assignment.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_assignmentFilter.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_assignmentFilter.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_compliance.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_conditionalAccess.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_conditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_configurationPolicies.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_configurationPolicies.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_customAttributeShellScript.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_customAttributeShellScript.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_deviceManagementSettings.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_enrollmentConfigurations.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_enrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_enrollmentStatusPage.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_enrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_frontend.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_frontend.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_groupPolicyConfiguration.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_groupPolicyConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_managementIntents.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_managementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_notificationTemplate.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_notificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_powershellScripts.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_powershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_proactiveRemediation.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_proactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_profiles.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_profiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_shellScripts.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_shellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD/update_windowsEnrollmentProfile.py` & `IntuneCD-1.4.7b1/src/IntuneCD/update_windowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD.egg-info/PKG-INFO` & `IntuneCD-1.4.7b1/src/IntuneCD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.6b1
+Version: 1.4.7b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.6b1/src/IntuneCD.egg-info/SOURCES.txt` & `IntuneCD-1.4.7b1/src/IntuneCD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_archive.py` & `IntuneCD-1.4.7b1/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_check_file.py` & `IntuneCD-1.4.7b1/tests/test_check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_clean_filename.py` & `IntuneCD-1.4.7b1/tests/test_clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_diff_summary.py` & `IntuneCD-1.4.7b1/tests/test_diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_documentation_functions.py` & `IntuneCD-1.4.7b1/tests/test_documentation_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,45 +83,51 @@
 
         self.assertEqual(escape_markdown(self.string), "\\\\`\\*\\_\\{\\}\\[\\]\\(\\)\\#\\+\\-\\.\\!Hello World")
 
     def test_clean_list_list(self):
         """The list should be returned."""
         self.list = [{"teamIdentifier": "test", "bundleId": "test"}]
         self.expected_list = ["**teamIdentifier:** test</br>**bundleId:** test</br>"]
-        self.result = clean_list(self.list)
+        self.result = clean_list(self.list, decode=True)
 
         self.assertEqual(self.result, self.expected_list)
 
     def test_clean_list_dict(self):
         """The list should be returned."""
         self.dict = {"appName": "test", "type": "#microsoft.graph.iosVppApp"}
         self.expected_list = ["appName", "type"]
-        self.result = clean_list(self.dict)
+        self.result = clean_list(self.dict, decode=True)
 
         self.assertEqual(self.result, self.expected_list)
 
     def test_clean_list_string(self):
         """The list should be returned."""
         self.string = ["test"]
         self.expected_list = ["test"]
-        self.result = clean_list(self.string)
+        self.result = clean_list(self.string, decode=True)
 
         self.assertEqual(self.result, self.expected_list)
 
     def test_document_configs(self):
         """The list should be returned."""
         self.directory.write(
             "config/test_file_name.json",
             '{"@odata.type":"test","test":"test","name":"test","description":"test","testvals":"1,2","testbool":false,"testlist":["test"],"testlistdict":[{"test":{"test":{"test":["1"]}}}],"testdict2":{"test":{"test":{"test":["1"]}}},"testdictlist":{"test":["a","b","c"]},"assignments":[{"intent":"apply","target":{"@odata.type":"#test","groupName":"test-group","deviceAndAppManagementAssignmentFilterId":"test-filter","deviceAndAppManagementAssignmentFilterType":"test"}}]}',
             encoding="utf-8",
         )
         self.expected_data = "#test##testDescription:test###Assignments|intent|target|filtertype|filtername||------|----------|-----------|-----------||apply|test-group|test|test-filter|###Configuration|setting|value||------------|-------------------------------------------------------||Odatatype|test||Test|test||Name|test||Testvals|1,2||Testbool|False||Testlist|test<br/>||Testlistdict|**test:**<ul>**test:**<ul><li>1</li></ul></ul><br/>||Testdict2|**test**<ul>**test:**<ul><li>1</li></ul><br/></ul>||Testdictlist|**test:**<ul><li>a</li><li>b</li><li>c</li></ul>|"
 
         document_configs(
-            f"{self.directory.path}/config", f"{self.directory.path}/test.md", "test", 100, split=False, cleanup=True
+            f"{self.directory.path}/config",
+            f"{self.directory.path}/test.md",
+            "test",
+            100,
+            split=False,
+            cleanup=True,
+            decode=False,
         )
 
         with open(f"{self.directory.path}/test.md", "r") as f:
             self.data = f.read()
             self.result = "".join([line.strip() for line in self.data])
 
         self.assertEqual(self.result, self.expected_data)
```

### Comparing `IntuneCD-1.4.6b1/tests/test_get_added_removed.py` & `IntuneCD-1.4.7b1/tests/test_get_added_removed.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_get_authparams.py` & `IntuneCD-1.4.7b1/tests/test_get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_graph_batch.py` & `IntuneCD-1.4.7b1/tests/test_graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_graph_request.py` & `IntuneCD-1.4.7b1/tests/test_graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_group_report.py` & `IntuneCD-1.4.7b1/tests/test_group_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_load_file.py` & `IntuneCD-1.4.7b1/tests/test_load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_match.py` & `IntuneCD-1.4.7b1/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_remove_keys.py` & `IntuneCD-1.4.7b1/tests/test_remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_save_output.py` & `IntuneCD-1.4.7b1/tests/test_save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6b1/tests/test_update_frontend.py` & `IntuneCD-1.4.7b1/tests/test_update_frontend.py`

 * *Files identical despite different names*

