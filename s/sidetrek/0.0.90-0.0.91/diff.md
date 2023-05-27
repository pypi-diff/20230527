# Comparing `tmp/sidetrek-0.0.90.tar.gz` & `tmp/sidetrek-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidetrek-0.0.90.tar", max compression
+gzip compressed data, was "sidetrek-0.0.91.tar", max compression
```

## Comparing `sidetrek-0.0.90.tar` & `sidetrek-0.0.91.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.90/README.md
--rw-r--r--   0        0        0      776 2023-05-27 14:50:52.319726 sidetrek-0.0.90/pyproject.toml
--rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.90/sidetrek/__init__.py
--rw-r--r--   0        0        0     1850 2023-05-23 22:57:40.497644 sidetrek-0.0.90/sidetrek/cli.py
--rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.90/sidetrek/cli_commands/__init__.py
--rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.90/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      308 2023-05-23 22:40:50.433399 sidetrek-0.0.90/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0    10270 2023-05-26 21:33:27.204243 sidetrek-0.0.90/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0        0        0     2857 2023-05-26 23:29:03.067762 sidetrek-0.0.90/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.90/sidetrek/cli_commands/constants.py
--rw-r--r--   0        0        0    11999 2023-05-26 21:33:20.619575 sidetrek-0.0.90/sidetrek/cli_commands/helpers.py
--rw-r--r--   0        0        0     4065 2023-05-27 14:50:45.612612 sidetrek-0.0.90/sidetrek/cli_commands/workflow.py
--rw-r--r--   0        0        0    21676 2023-05-24 17:24:59.596079 sidetrek-0.0.90/sidetrek/collect_env.py
--rw-r--r--   0        0        0       37 2023-04-02 20:04:34.987724 sidetrek-0.0.90/sidetrek/constants.py
--rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.90/sidetrek/datapipes.py
--rw-r--r--   0        0        0     4354 2023-05-26 15:36:54.943156 sidetrek-0.0.90/sidetrek/dataset.py
--rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.90/sidetrek/flyte/__init__.py
--rw-r--r--   0        0        0      874 2023-05-09 03:56:32.928519 sidetrek-0.0.90/sidetrek/global_fns.py
--rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.90/sidetrek/loggers.py
--rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.90/sidetrek/types/__init__.py
--rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.90/sidetrek/types/dataset.py
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 sidetrek-0.0.90/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.91/README.md
+-rw-r--r--   0        0        0      776 2023-05-27 14:53:06.799077 sidetrek-0.0.91/pyproject.toml
+-rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.91/sidetrek/__init__.py
+-rw-r--r--   0        0        0     1850 2023-05-23 22:57:40.497644 sidetrek-0.0.91/sidetrek/cli.py
+-rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.91/sidetrek/cli_commands/__init__.py
+-rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.91/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      308 2023-05-23 22:40:50.433399 sidetrek-0.0.91/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0    10270 2023-05-26 21:33:27.204243 sidetrek-0.0.91/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0     2857 2023-05-26 23:29:03.067762 sidetrek-0.0.91/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.91/sidetrek/cli_commands/constants.py
+-rw-r--r--   0        0        0    11999 2023-05-26 21:33:20.619575 sidetrek-0.0.91/sidetrek/cli_commands/helpers.py
+-rw-r--r--   0        0        0     3937 2023-05-27 14:53:02.645504 sidetrek-0.0.91/sidetrek/cli_commands/workflow.py
+-rw-r--r--   0        0        0    21676 2023-05-24 17:24:59.596079 sidetrek-0.0.91/sidetrek/collect_env.py
+-rw-r--r--   0        0        0       37 2023-04-02 20:04:34.987724 sidetrek-0.0.91/sidetrek/constants.py
+-rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.91/sidetrek/datapipes.py
+-rw-r--r--   0        0        0     4354 2023-05-26 15:36:54.943156 sidetrek-0.0.91/sidetrek/dataset.py
+-rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.91/sidetrek/flyte/__init__.py
+-rw-r--r--   0        0        0      874 2023-05-09 03:56:32.928519 sidetrek-0.0.91/sidetrek/global_fns.py
+-rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.91/sidetrek/loggers.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.91/sidetrek/types/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.91/sidetrek/types/dataset.py
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 sidetrek-0.0.91/PKG-INFO
```

### Comparing `sidetrek-0.0.90/pyproject.toml` & `sidetrek-0.0.91/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sidetrek"
-version = "0.0.90"
+version = "0.0.91"
 description = ""
 authors = ["Seungchan Lee <seunggs@gmail.com>"]
 readme = "README.md"
 exclude = ["sidetrek/test/**"]
 
 [tool.poetry.scripts]
 sidetrek = "sidetrek.cli:app"
```

### Comparing `sidetrek-0.0.90/sidetrek/__init__.py` & `sidetrek-0.0.91/sidetrek/__init__.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.90/sidetrek/cli.py` & `sidetrek-0.0.91/sidetrek/cli.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.90/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc` & `sidetrek-0.0.91/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.90/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc` & `sidetrek-0.0.91/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.90/sidetrek/cli_commands/helpers.py` & `sidetrek-0.0.91/sidetrek/cli_commands/helpers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.90/sidetrek/cli_commands/workflow.py` & `sidetrek-0.0.91/sidetrek/cli_commands/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,16 +63,14 @@
         print(f"[green]✔️ [white]Workflow generated [grey89]({time_elapsed}s) - {wf_file_path.as_posix()}")
 
         # Get aws credentials and set it as env var for execution (grants temporary local s3 access)
         aws_creds = get_aws_creds()
         if aws_creds is None:
             raise Exception("Failed to get aws credentials")
 
-        print(f"AWS_ACCESS_KEY_ID={aws_creds['AccessKeyId']}")
-        print(f"AWS_SECRET_ACCESS_KEY={aws_creds['SecretKey']}")
         aws_env = {**os.environ, "AWS_ACCESS_KEY_ID": aws_creds["AccessKeyId"], "AWS_SECRET_ACCESS_KEY": aws_creds["SecretKey"], "AWS_SESSION_TOKEN": aws_creds["SessionToken"]}
 
         wf_execution_step = progress.add_task(description="Executing the workflow...", total=None)
         # print(" ".join(["pyflyte", "run", wf_file_path.as_posix(), generated_wf_name, "--_wf_args", workflow_args]))
         with subprocess.Popen(
             ["pyflyte", "run", wf_file_path, generated_wf_name, "--_wf_args", workflow_args],
             cwd=get_generated_local_sidetrek_dir_path(),
```

### Comparing `sidetrek-0.0.90/sidetrek/collect_env.py` & `sidetrek-0.0.91/sidetrek/collect_env.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.90/sidetrek/datapipes.py` & `sidetrek-0.0.91/sidetrek/datapipes.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.90/sidetrek/dataset.py` & `sidetrek-0.0.91/sidetrek/dataset.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.90/sidetrek/global_fns.py` & `sidetrek-0.0.91/sidetrek/global_fns.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.90/sidetrek/loggers.py` & `sidetrek-0.0.91/sidetrek/loggers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.90/sidetrek/types/dataset.py` & `sidetrek-0.0.91/sidetrek/types/dataset.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.90/PKG-INFO` & `sidetrek-0.0.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidetrek
-Version: 0.0.90
+Version: 0.0.91
 Summary: 
 Author: Seungchan Lee
 Author-email: seunggs@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

