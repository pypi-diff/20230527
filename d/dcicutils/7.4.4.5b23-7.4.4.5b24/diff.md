# Comparing `tmp/dcicutils-7.4.4.5b23.tar.gz` & `tmp/dcicutils-7.4.4.5b24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.4.4.5b23.tar", max compression
+gzip compressed data, was "dcicutils-7.4.4.5b24.tar", max compression
```

## Comparing `dcicutils-7.4.4.5b23.tar` & `dcicutils-7.4.4.5b24.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1098 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/README.rst
--rw-r--r--   0        0        0        0 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3723 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46739 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27661 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    30865 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20234 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   156269 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    12767 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-05-27 07:57:06.705004 dcicutils-7.4.4.5b23/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-05-27 07:57:06.705004 dcicutils-7.4.4.5b23/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-05-27 07:57:06.705004 dcicutils-7.4.4.5b23/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-05-27 07:57:06.705004 dcicutils-7.4.4.5b23/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3968 2023-05-27 07:57:06.705004 dcicutils-7.4.4.5b23/pyproject.toml
--rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 dcicutils-7.4.4.5b23/setup.py
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 dcicutils-7.4.4.5b23/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/README.rst
+-rw-r--r--   0        0        0        0 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3723 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-05-27 08:42:32.478693 dcicutils-7.4.4.5b24/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46739 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27661 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    30865 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20234 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   156269 2023-05-27 08:42:32.482693 dcicutils-7.4.4.5b24/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-05-27 08:42:32.486693 dcicutils-7.4.4.5b24/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-05-27 08:42:32.486693 dcicutils-7.4.4.5b24/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-05-27 08:42:32.486693 dcicutils-7.4.4.5b24/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    12767 2023-05-27 08:42:32.486693 dcicutils-7.4.4.5b24/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-05-27 08:42:32.486693 dcicutils-7.4.4.5b24/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-05-27 08:42:32.486693 dcicutils-7.4.4.5b24/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-05-27 08:42:32.486693 dcicutils-7.4.4.5b24/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-05-27 08:42:32.486693 dcicutils-7.4.4.5b24/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-05-27 08:42:32.486693 dcicutils-7.4.4.5b24/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3968 2023-05-27 08:42:32.486693 dcicutils-7.4.4.5b24/pyproject.toml
+-rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 dcicutils-7.4.4.5b24/setup.py
+-rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 dcicutils-7.4.4.5b24/PKG-INFO
```

### Comparing `dcicutils-7.4.4.5b23/LICENSE.txt` & `dcicutils-7.4.4.5b24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/README.rst` & `dcicutils-7.4.4.5b24/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/base.py` & `dcicutils-7.4.4.5b24/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/beanstalk_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/cloudformation_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/codebuild_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/command_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/common.py` & `dcicutils-7.4.4.5b24/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/creds_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/data_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/deployment_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/diff_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/docker_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/ecr_scripts.py` & `dcicutils-7.4.4.5b24/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/ecr_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/ecs_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/env_base.py` & `dcicutils-7.4.4.5b24/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/env_manager.py` & `dcicutils-7.4.4.5b24/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/env_scripts.py` & `dcicutils-7.4.4.5b24/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/env_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/env_utils_legacy.py` & `dcicutils-7.4.4.5b24/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/es_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/exceptions.py` & `dcicutils-7.4.4.5b24/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/ff_mocks.py` & `dcicutils-7.4.4.5b24/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/ff_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/function_cache_decorator.py` & `dcicutils-7.4.4.5b24/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/glacier_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/jh_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/kibana/dashboards.json` & `dcicutils-7.4.4.5b24/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/kibana/readme.md` & `dcicutils-7.4.4.5b24/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/lang_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/log_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/misc_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/obfuscation_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/opensearch_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/project_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/qa_checkers.py` & `dcicutils-7.4.4.5b24/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/qa_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/redis_tools.py` & `dcicutils-7.4.4.5b24/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/redis_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/s3_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.4.4.5b24/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/secrets_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/snapshot_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/task_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/dcicutils/trace_utils.py` & `dcicutils-7.4.4.5b24/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b23/pyproject.toml` & `dcicutils-7.4.4.5b24/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.4.4.5b23"  # to become 7.5.0
+version = "7.4.4.5b24"  # to become 7.5.0
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.4.4.5b23/setup.py` & `dcicutils-7.4.4.5b24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.4.4.5b23',
+    'version': '7.4.4.5b24',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.4.4.5b23/PKG-INFO` & `dcicutils-7.4.4.5b24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.4.4.5b23
+Version: 7.4.4.5b24
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

