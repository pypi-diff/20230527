# Comparing `tmp/dcicutils-7.4.4.5b21.tar.gz` & `tmp/dcicutils-7.4.4.5b23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.4.4.5b21.tar", max compression
+gzip compressed data, was "dcicutils-7.4.4.5b23.tar", max compression
```

## Comparing `dcicutils-7.4.4.5b21.tar` & `dcicutils-7.4.4.5b23.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1098 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/README.rst
--rw-r--r--   0        0        0        0 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3723 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-05-25 16:55:12.990109 dcicutils-7.4.4.5b21/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46739 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27661 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    29607 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20234 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   156269 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    12771 2023-05-25 16:55:12.994109 dcicutils-7.4.4.5b21/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-05-25 16:55:12.998109 dcicutils-7.4.4.5b21/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-05-25 16:55:12.998109 dcicutils-7.4.4.5b21/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-05-25 16:55:12.998109 dcicutils-7.4.4.5b21/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-05-25 16:55:12.998109 dcicutils-7.4.4.5b21/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-05-25 16:55:12.998109 dcicutils-7.4.4.5b21/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3968 2023-05-25 16:55:12.998109 dcicutils-7.4.4.5b21/pyproject.toml
--rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 dcicutils-7.4.4.5b21/setup.py
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 dcicutils-7.4.4.5b21/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/README.rst
+-rw-r--r--   0        0        0        0 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3723 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-05-27 07:57:06.697004 dcicutils-7.4.4.5b23/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46739 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27661 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    30865 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20234 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   156269 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    12767 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-05-27 07:57:06.701004 dcicutils-7.4.4.5b23/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-05-27 07:57:06.705004 dcicutils-7.4.4.5b23/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-05-27 07:57:06.705004 dcicutils-7.4.4.5b23/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-05-27 07:57:06.705004 dcicutils-7.4.4.5b23/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-05-27 07:57:06.705004 dcicutils-7.4.4.5b23/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3968 2023-05-27 07:57:06.705004 dcicutils-7.4.4.5b23/pyproject.toml
+-rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 dcicutils-7.4.4.5b23/setup.py
+-rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 dcicutils-7.4.4.5b23/PKG-INFO
```

### Comparing `dcicutils-7.4.4.5b21/LICENSE.txt` & `dcicutils-7.4.4.5b23/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/README.rst` & `dcicutils-7.4.4.5b23/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/base.py` & `dcicutils-7.4.4.5b23/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/beanstalk_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/cloudformation_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/codebuild_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/command_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/common.py` & `dcicutils-7.4.4.5b23/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/creds_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/data_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/deployment_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/diff_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/docker_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/ecr_scripts.py` & `dcicutils-7.4.4.5b23/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/ecr_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/ecs_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/env_base.py` & `dcicutils-7.4.4.5b23/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/env_manager.py` & `dcicutils-7.4.4.5b23/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/env_scripts.py` & `dcicutils-7.4.4.5b23/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/env_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/env_utils_legacy.py` & `dcicutils-7.4.4.5b23/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/es_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/exceptions.py` & `dcicutils-7.4.4.5b23/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/ff_mocks.py` & `dcicutils-7.4.4.5b23/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/ff_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/function_cache_decorator.py` & `dcicutils-7.4.4.5b23/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/glacier_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/jh_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/kibana/dashboards.json` & `dcicutils-7.4.4.5b23/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/kibana/readme.md` & `dcicutils-7.4.4.5b23/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/lang_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/log_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/misc_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/obfuscation_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/opensearch_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/project_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/project_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import importlib
 import os
 import toml
 
 from pkg_resources import resource_filename
 from typing import Callable, Optional, Type
-from .misc_utils import PRINT, StorageCell, classproperty, environ_bool, ignored
+from .misc_utils import PRINT, StorageCell, classproperty, environ_bool, ignored, get_error_message
 from .lang_utils import conjoined_list, maybe_pluralize
 
 
 class ProjectNames:
 
     def __init__(self, *, PYPROJECT_NAME, NAME, PRETTY_NAME=None, REPO_NAME=None, PYPI_NAME=None,
                  PACKAGE_NAME=None, APP_NAME=None, APP_PRETTY_NAME=None):
@@ -19,15 +20,15 @@
         self.APP_NAME = APP_NAME = APP_NAME or self.appify(REPO_NAME)
         self.APP_PRETTY_NAME = APP_PRETTY_NAME or self.prettify(APP_NAME)
         self.PACKAGE_NAME = (PACKAGE_NAME
                              # This uses ProjectRegistry (not cls) because that part of the protocol is common to all
                              # classes and subclasses of that class. No need to worry about specialized classes.
                              # -kmp 19-May-2023
                              or self.infer_package_name(poetry_data=ProjectRegistry.POETRY_DATA,
-                                                        pypi_name=PYPI_NAME, pyproject_name=PYPROJECT_NAME))
+                                                        pyproject_name=PYPROJECT_NAME))
 
     @classmethod
     def prettify(cls, name: str) -> str:
         """
         Turns a token name (possibly hyphenated) into a pretty name with capitalized words.
         e.g, "foo-bar" => "Foo Bar"
 
@@ -55,23 +56,30 @@
         In this class, this is just an identity, but it might be customized in a subclass.
         For example, in the C4 projects, "dcicutils" uses the repo name "utils", and "dcicsnovault" uses
         the repo "snovault", so a subclass of this class might be customized to strip "dcic" from the name.
         """
         return name
 
     @classmethod
-    def infer_package_name(cls, poetry_data, pypi_name, pyproject_name):
+    def infer_package_name(cls, poetry_data, pyproject_name, as_dir=False):
         try:
             if poetry_data:
                 # We expect the first package in the declared packages to be the primary export
                 # Other exported dirs, such as scripts or tests should be in later entries.
-                return poetry_data['packages'][0]['include']
+                entry = poetry_data['packages'][0]
+                include = entry['include']
+                from_dir = entry.get('from', '.')
+                return os.path.join(from_dir, include) if as_dir else include
         except Exception:
             pass
-        return pypi_name or pyproject_name
+        result = pyproject_name
+        if not result:
+            raise ValueError(f"Unable to infer package name given"
+                             f" poetry_data={poetry_data!r} and pyproject_name={pyproject_name!r}.")
+        return result
 
     def items(self):
         """
         Given a ProjectNames instance, this returns a list of the form [(name_key1, name_val1), ...].
         """
         result = []
         for attr in sorted(dir(self)):
@@ -223,26 +231,26 @@
         which might be of this class or one of its subclasses.
         """
         return cls.PROJECT_REGISTRY_CLASS.app_project
 
     @classmethod
     def app_project_maker(cls):
         """
-        Makes an app_project function, a function of no arguments that returns the current app_project,
-        creating it on demand if necessary.
+        Returns a function that, when invoked, will yield the proper app project,
+        initializing that value in demand if it has not been previously initialized.
 
         NOTES:
-        * When using C4Project classes, please always use C4ProjectRegistry.app_project_maker() so that C4
-          policies will be applied upon demand-creation.
+        * When using C4Project classes, please always use <your-class>.app_project_maker() or
+          C4ProjectRegistry.app_project_maker() so that C4 policies will be applied upon demand-creation.
 
-        * The Project.app_project_maker() class method is deprecated. Please use
-          Please use Projectregistry.app_project_maker() or C4ProjectRegistry.app_project_maker(), instead.
+        * Note that by the time of first call to that function, the appropriate environment must be in place,
+          or an autoload will be attempted from your project's project_defs.py file.
+          If you want advance control of the specific environment in which the initialization will occur,
+          use <registry-class>.initialize().
         """
-        PRINT(f"{cls.__name__}.app_project_maker() called. This class method has been deprecated."
-              f" Please use {cls.PROJECT_REGISTRY_CLASS.__name__}.app_project_maker() instead.")
         return cls.PROJECT_REGISTRY_CLASS.app_project_maker()
 
     def project_filename(self, filename):
         """Returns a filename relative to given instance."""
         current_project = self.app_project
         if self is not current_project:
             raise RuntimeError(f"{self}.project_filename invoked,"
@@ -365,30 +373,32 @@
 
     @classproperty
     def PYPROJECT_NAME(cls) -> str:  # noQA - PyCharm thinks this should be 'self'
         if cls._PYPROJECT_NAME is None:
             cls._initialize_pyproject_name()
         result: Optional[str] = cls._PYPROJECT_NAME
         if result is None:
-            raise ValueError(f"{cls.__name__}.PROJECT_NAME not initialized properly.")
+            raise ValueError(f"{cls.__name__}.PYPROJECT_NAME not initialized properly.")
         return result
 
     @classmethod
     def _initialize_pyproject_name(cls, project_home=None, pyproject_toml_file=None,
                                    pyproject_toml=None, poetry_data=None, pyproject_name=None):
         if ProjectRegistry._PYPROJECT_NAME is None:
             # This isn't the home of Project, but the home of the Project-based application.
             # So in CGAP, for example, this would want to be the home of the CGAP application.
             # If not set, it will be assumed that the current working directory is that.
             # print("Setting up data.")
             if not project_home:
                 project_home = os.environ.get("APPLICATION_PROJECT_HOME", os.path.abspath(os.curdir))
             ProjectRegistry.APPLICATION_PROJECT_HOME = project_home
             if not pyproject_toml_file:
-                expected_pyproject_toml_file = os.path.join(project_home, "pyproject.toml")
+                expected_pyproject_toml_file = (os.path.join(project_home, "pyproject.toml")
+                                                if project_home
+                                                else "pyproject.toml")
                 pyproject_toml_file = (expected_pyproject_toml_file
                                        if os.path.exists(expected_pyproject_toml_file)
                                        else None)
             ProjectRegistry.PYPROJECT_TOML_FILE = pyproject_toml_file
             # print(f"Loading toml file {cls.PYPROJECT_TOML_FILE}")
             if not pyproject_toml:
                 ProjectRegistry.PYPROJECT_TOML = pyproject_toml = (toml.load(ProjectRegistry.PYPROJECT_TOML_FILE)
@@ -500,14 +510,24 @@
 
         NOTE: There is no need for this function to be called outside of this class except for testing.
               Really only one of these should be instantiated per running application, and that's
               done automatically by this class.
         """
         project_class: Optional[Type[Project]] = cls.find_pyproject(cls.PYPROJECT_NAME)
         if project_class is None:
+            inferred_package = ProjectNames.infer_package_name(poetry_data=cls.POETRY_DATA,
+                                                               pyproject_name=cls.PYPROJECT_NAME,
+                                                               as_dir=True)
+            PRINT(f"Autoloading pyproject {cls.PYPROJECT_NAME!r} from inferred package {inferred_package!r}.")
+            try:
+                importlib.import_module(name=".project_defs", package=inferred_package)
+            except Exception as e:
+                PRINT(f"Autoload failed: {get_error_message(e)}")
+            project_class: Optional[Type[Project]] = cls.find_pyproject(cls.PYPROJECT_NAME)
+        if project_class is None:
             raise ValueError(f"Missing project class for pyproject {cls.PYPROJECT_NAME!r}.")
         if not issubclass(project_class, cls.PROJECT_BASE_CLASS):
             raise ValueError(f"Registered pyproject {cls.PYPROJECT_NAME!r} ({project_class.__name__})"
                              f" is not a subclass of {cls.PROJECT_BASE_CLASS.__name__}.")
         project: Project = project_class()
         return project  # instantiate and return
 
@@ -535,25 +555,24 @@
 
     @classmethod
     def app_project_maker(cls) -> Callable[[], Project]:
         """
         Returns a function that, when invoked, will yield the proper app project,
         initializing that value in demand if it has not been previously initialized.
 
-        Note that by the time of first call to that function, the appropriate environment must be in place.
-        If you want advance control of the specific environment in which the initialization will occur,
-        use <registry-class>.initialize().
-        """
+        NOTES:
+        * When using C4Project classes, please always use <your-class>.app_project_maker() or
+          C4ProjectRegistry.app_project_maker() so that C4 policies will be applied upon demand-creation.
 
+        * Note that by the time of first call to that function, the appropriate environment must be in place,
+          or an autoload will be attempted from your project's project_defs.py file.
+          If you want advance control of the specific environment in which the initialization will occur,
+          use <registry-class>.initialize().
+        """
         def app_project() -> Project:
-            if cls == Project:
-                raise Exception("Please do not use ProjectRegistry.app_project_maker()."
-                                " For DBMI users, use C4ProjectRegistry."
-                                " For others, make a subclass of ProjectRegistry and use that.")
-
             return cls.app_project
 
         return app_project
 
 
 Project.declare_project_registry_class(ProjectRegistry)  # Finalize a circular dependency
```

### Comparing `dcicutils-7.4.4.5b21/dcicutils/qa_checkers.py` & `dcicutils-7.4.4.5b23/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/qa_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/redis_tools.py` & `dcicutils-7.4.4.5b23/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/redis_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/s3_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.4.4.5b23/dcicutils/scripts/publish_to_pypi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Script to publish the Python package in the CURRENT git repo to PyPi.
-# Does the following checks before allowing a publish:
+# Does the following checks before allowing poetry to publish:
 #
 # 0. Current directory MUST be a git repo.
 # 1. The git repo MUST NOT contain unstaged changes.
 # 2. The git repo MUST NOT contain staged but uncommitted changes.
 # 3. The git repo MUST NOT contain committed but unpushed changes.
 # 4. The git repo package directories MUST NOT contain untracked files,
 #    OR if they do contain untracked files then you must confirm this is OK.
@@ -30,14 +30,15 @@
 # would be if publishing only happened via GitHub actions.
 
 import argparse
 import os
 import requests
 import subprocess
 import toml
+
 from typing import Tuple, Union
 
 
 PYPI_BASE_URL = "https://pypi.org"
 DEBUG = False
 
 
@@ -316,16 +317,15 @@
     Exits this process immediately with status 1;
     first prints a message saying no action was taken.
     """
     PRINT("Exiting without taking action.")
     exit(1)
 
 
-def PRINT(s):
-    print(s)
+PRINT = print
 
 
 def WARNING_PRINT(s):
     PRINT(f"WARNING: {s}")
 
 
 def ERROR_PRINT(s):
```

### Comparing `dcicutils-7.4.4.5b21/dcicutils/secrets_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/snapshot_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/task_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/dcicutils/trace_utils.py` & `dcicutils-7.4.4.5b23/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4.5b21/pyproject.toml` & `dcicutils-7.4.4.5b23/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.4.4.5b21"  # to become 7.5.0
+version = "7.4.4.5b23"  # to become 7.5.0
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.4.4.5b21/setup.py` & `dcicutils-7.4.4.5b23/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.4.4.5b21',
+    'version': '7.4.4.5b23',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.4.4.5b21/PKG-INFO` & `dcicutils-7.4.4.5b23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.4.4.5b21
+Version: 7.4.4.5b23
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

