# Comparing `tmp/aws_lambda_layer-0.2.3.tar.gz` & `tmp/aws_lambda_layer-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_layer-0.2.3.tar", last modified: Fri May 26 20:20:26 2023, max compression
+gzip compressed data, was "aws_lambda_layer-0.2.4.tar", last modified: Sat May 27 20:03:08 2023, max compression
```

## Comparing `aws_lambda_layer-0.2.3.tar` & `aws_lambda_layer-0.2.4.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 20:20:26.780949 aws_lambda_layer-0.2.3/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.3/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.3/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-05-13 04:31:27.000000 aws_lambda_layer-0.2.3/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-26 20:20:26.780815 aws_lambda_layer-0.2.3/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3045 2023-05-26 18:33:40.000000 aws_lambda_layer-0.2.3/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 20:20:26.779864 aws_lambda_layer-0.2.3/aws_lambda_layer/
--rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-26 15:58:40.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-26 20:19:05.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      395 2023-05-26 18:27:30.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/build_dist.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4224 2023-05-26 18:14:42.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/context.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    12038 2023-05-26 20:17:18.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/layer.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    12529 2023-05-26 20:00:24.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/source.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1459 2023-05-26 19:44:02.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 20:20:26.780425 aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-26 20:20:26.000000 aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      589 2023-05-26 20:20:26.000000 aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-26 20:20:26.000000 aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      169 2023-05-26 20:20:26.000000 aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       17 2023-05-26 20:20:26.000000 aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      989 2023-05-26 20:20:04.000000 aws_lambda_layer-0.2.3/pyproject.toml
--rw-r--r--   0 sanhehu    (501) staff       (20)     1949 2023-05-26 20:19:50.000000 aws_lambda_layer-0.2.3/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.3/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-05-16 01:23:43.000000 aws_lambda_layer-0.2.3/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-26 20:20:26.780990 aws_lambda_layer-0.2.3/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7662 2023-05-26 15:59:24.000000 aws_lambda_layer-0.2.3/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 20:20:26.780656 aws_lambda_layer-0.2.3/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      259 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.3/tests/test_import.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      577 2023-05-26 19:43:53.000000 aws_lambda_layer-0.2.3/tests/test_utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 20:03:08.059133 aws_lambda_layer-0.2.4/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.4/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.4/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-05-13 04:31:27.000000 aws_lambda_layer-0.2.4/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-27 20:03:08.058991 aws_lambda_layer-0.2.4/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3045 2023-05-26 18:33:40.000000 aws_lambda_layer-0.2.4/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 20:03:08.056888 aws_lambda_layer-0.2.4/aws_lambda_layer/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-26 15:58:40.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-27 19:59:46.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      412 2023-05-27 20:00:42.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4224 2023-05-26 18:14:42.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/context.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    13795 2023-05-27 19:54:58.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/layer.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    13006 2023-05-27 19:55:28.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/source.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      184 2023-05-27 19:51:13.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 20:03:08.058397 aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:46:28.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      650 2023-05-27 19:47:26.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/build_dist.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7590 2023-05-27 19:48:17.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/hashes.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 20:03:08.057617 aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-27 20:03:08.000000 aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      688 2023-05-27 20:03:08.000000 aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-27 20:03:08.000000 aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      169 2023-05-27 20:03:08.000000 aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       17 2023-05-27 20:03:08.000000 aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      989 2023-05-26 20:20:04.000000 aws_lambda_layer-0.2.4/pyproject.toml
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2239 2023-05-27 20:01:07.000000 aws_lambda_layer-0.2.4/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.4/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-05-16 01:23:43.000000 aws_lambda_layer-0.2.4/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-27 20:03:08.059172 aws_lambda_layer-0.2.4/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7662 2023-05-26 15:59:24.000000 aws_lambda_layer-0.2.4/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 20:03:08.058740 aws_lambda_layer-0.2.4/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      634 2023-05-27 20:02:07.000000 aws_lambda_layer-0.2.4/tests/test_import.py
```

### Comparing `aws_lambda_layer-0.2.3/LICENSE.txt` & `aws_lambda_layer-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.3/PKG-INFO` & `aws_lambda_layer-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws_lambda_layer
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts.
 Home-page: https://github.com/MacHu-GWU/aws_lambda_layer-project
-Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.3#downloads
+Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_lambda_layer-0.2.3/README.rst` & `aws_lambda_layer-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.3/aws_lambda_layer/build_dist.py` & `aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/build_dist.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.3/aws_lambda_layer/context.py` & `aws_lambda_layer-0.2.4/aws_lambda_layer/context.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.3/aws_lambda_layer/layer.py` & `aws_lambda_layer-0.2.4/aws_lambda_layer/layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,24 @@
     s3://bucket/${s3dir_lambda}/layer/000003/requirements.txt
 """
 
 import typing as T
 import glob
 import shutil
 import subprocess
+import dataclasses
 from pathlib import Path
 from urllib.parse import urlencode
 
 from s3pathlib import S3Path
 from func_args import NOTHING
 from boto_session_manager import BotoSesManager
 
-from . import utils
+from .vendor.better_pathlib import temp_cwd
+from .vendor.hashes import hashes
 from .context import BuildContext
 
 
 def get_latest_layer_version(
     bsm: "BotoSesManager",
     layer_name: str,
 ) -> T.Optional[int]:
@@ -106,15 +108,15 @@
     compatibility issues with certain C libraries.
 
     :param path_requirements: example: ``/path/to/requirements.txt``
     :param dir_build: example: ``/path/to/build/lambda``
     :param bin_pip: example: ``/path/to/.venv/bin/pip``
     :param quiet: whether you want to suppress the output of cli commands
 
-    :return: the layer content sha256
+    :return: the layer content sha256, it is sha256 of the requirements.txt file
     """
     build_context = BuildContext.new(dir_build=dir_build)
     path_requirements = Path(path_requirements).absolute()
     bin_pip = Path(bin_pip).absolute()
 
     # remove existing artifacts and temp folder
     build_context.path_layer_zip.unlink(missing_ok=True)
@@ -156,45 +158,47 @@
         f"{build_context.path_layer_zip}",
         "-r",
         "-9",
     ]
     if quiet:
         args.append("-q")
     # the glob command and zip command depends on the current working directory
-    with utils.temp_cwd(build_context.dir_build):
+    with temp_cwd(build_context.dir_build):
         args.extend(glob.glob("*"))
         args.append("-x")
         for package in ignore_package_list:
             args.append(f"python/{package}*")
         subprocess.run(args, check=True)
-    layer_sha256 = utils.sha256_of_bytes(path_requirements.read_bytes())
+    layer_sha256 = hashes.of_bytes(path_requirements.read_bytes())
     return layer_sha256
 
 
 def upload_layer_artifacts(
     bsm: "BotoSesManager",
     path_requirements: T.Union[str, Path],
     layer_sha256: str,
     dir_build: T.Union[str, Path],
     s3dir_lambda: T.Union[str, S3Path],
     metadata: T.Optional[T.Dict[str, str]] = NOTHING,
     tags: T.Optional[T.Dict[str, str]] = NOTHING,
-):
+) -> T.Tuple[S3Path, S3Path]:
     """
     Upload the recently built Lambda layer artifact from ``${dir_build}/layer.zip``
     to a temporary S3 folder. If the creation of a new layer from the temporary location
     is successful, copy it to the final location for the layer artifacts.
 
     :param bsm: boto session manager object
     :param path_requirements: example: ``/path/to/requirements.txt``
     :param layer_sha256: layer content sha256
     :param dir_build: example: ``/path/to/build/lambda``
     :param s3dir_lambda: example: ``s3://bucket/path/to/lambda/``
     :param metadata: S3 object metadata
     :param tags: S3 object tags
+
+    :return: s3path_tmp_layer_zip and s3path_tmp_layer_requirements_txt
     """
     build_context = BuildContext.new(dir_build=dir_build, s3dir_lambda=s3dir_lambda)
     path_requirements = Path(path_requirements).absolute()
 
     if metadata is NOTHING:
         metadata = {}
     metadata["layer_sha256"] = layer_sha256
@@ -218,23 +222,29 @@
         extra_args["Tagging"] = urlencode(tags)
     build_context.s3path_tmp_layer_requirements_txt.upload_file(
         path_requirements,
         overwrite=True,
         bsm=bsm,
         extra_args=extra_args,
     )
+    s3path_tmp_layer_zip = build_context.s3path_tmp_layer_zip
+    s3path_tmp_layer_requirements_txt = build_context.s3path_tmp_layer_requirements_txt
+    return (
+        s3path_tmp_layer_zip,
+        s3path_tmp_layer_requirements_txt,
+    )
 
 
 def publish_layer(
     bsm: "BotoSesManager",
     layer_name: str,
     python_versions: T.List[str],
     dir_build: T.Union[str, Path],
     s3dir_lambda: T.Union[str, S3Path],
-) -> str:
+) -> T.Tuple[int, str, S3Path, S3Path,]:
     """
     Publish a new lambda layer version from AWS S3.
 
     :param bsm: boto session manager object
     :param layer_name: the lambda layer name
     :param python_version: example: ``["python3.8",]``
     :param dir_build: example: ``/path/to/build/lambda``
@@ -269,29 +279,52 @@
         s3path_layer_zip,
         overwrite=False,
     )
     build_context.s3path_tmp_layer_requirements_txt.copy_to(
         s3path_layer_requirements_txt,
         overwrite=False,
     )
-    return layer_version_arn
+    return (
+        layer_version,
+        layer_version_arn,
+        s3path_layer_zip,
+        s3path_layer_requirements_txt,
+    )
+
+
+@dataclasses.dataclass
+class LayerDeployment:
+    """
+    Layer deployment information.
+
+    :param layer_sha256: the layer content sha256, it is sha256 of the requirements.txt file
+    :param layer_version: integer layer version
+    :param layer_version_arn: lambda layer arn
+    :param s3path_layer_zip: the S3Path object of the layer.zip file
+    :param s3path_layer_requirements_txt: the S3Path object of the requirements.txt file
+    """
+    layer_sha256: str = dataclasses.field()
+    layer_version: int = dataclasses.field()
+    layer_version_arn: str = dataclasses.field()
+    s3path_layer_zip: S3Path = dataclasses.field()
+    s3path_layer_requirements_txt: S3Path = dataclasses.field()
 
 
 def deploy_layer(
     bsm: "BotoSesManager",
     layer_name: str,
     python_versions: T.List[str],
     path_requirements: T.Union[str, Path],
     dir_build: T.Union[str, Path],
     s3dir_lambda: T.Union[str, S3Path],
     bin_pip: T.Union[str, Path],
     quiet: bool = False,
     metadata: T.Optional[T.Dict[str, str]] = NOTHING,
     tags: T.Optional[T.Dict[str, str]] = NOTHING,
-) -> T.Optional[str]:
+) -> T.Optional[LayerDeployment]:
     """
     Assemble the following functions together to build and deploy a new
     Lambda layer version if necessary.
 
     - :func:`get_latest_layer_version`
     - :func:`is_current_layer_the_same_as_latest_one`
     - :func:`build_layer_artifacts`
@@ -310,16 +343,16 @@
     :param dir_build: example: ``/path/to/build/lambda``
     :param s3dir_lambda: example: ``s3://bucket/path/to/lambda/``
     :param bin_pip: example: ``/path/to/.venv/bin/pip``
     :param quiet: whether you want to suppress the output of cli commands
     :param metadata: S3 object metadata
     :param tags: S3 object tags
 
-    :return: The published lambda layer version ARN. If returns None,
-        then no deployment happened.
+    :return: The :class:`LayerDeployment` object. If returns None, then no
+        deployment happened.
     """
     latest_layer_version = get_latest_layer_version(bsm=bsm, layer_name=layer_name)
 
     if is_current_layer_the_same_as_latest_one(
         bsm=bsm,
         latest_layer_version=latest_layer_version,
         path_requirements=path_requirements,
@@ -330,24 +363,40 @@
     layer_sha256 = build_layer_artifacts(
         path_requirements=path_requirements,
         dir_build=dir_build,
         bin_pip=bin_pip,
         quiet=quiet,
     )
 
-    upload_layer_artifacts(
+    (
+        s3path_tmp_layer_zip,
+        s3path_tmp_layer_requirements_txt,
+    ) = upload_layer_artifacts(
         bsm=bsm,
         path_requirements=path_requirements,
         layer_sha256=layer_sha256,
         dir_build=dir_build,
         s3dir_lambda=s3dir_lambda,
         metadata=metadata,
         tags=tags,
     )
 
-    return publish_layer(
+    (
+        layer_version,
+        layer_version_arn,
+        s3path_layer_zip,
+        s3path_layer_requirements_txt,
+    ) = publish_layer(
         bsm=bsm,
         layer_name=layer_name,
         python_versions=python_versions,
         dir_build=dir_build,
         s3dir_lambda=s3dir_lambda,
     )
+
+    return LayerDeployment(
+        layer_sha256=layer_sha256,
+        layer_version=layer_version,
+        layer_version_arn=layer_version_arn,
+        s3path_layer_zip=s3path_layer_zip,
+        s3path_layer_requirements_txt=s3path_layer_requirements_txt,
+    )
```

### Comparing `aws_lambda_layer-0.2.3/aws_lambda_layer/source.py` & `aws_lambda_layer-0.2.4/aws_lambda_layer/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,30 @@
     s3://bucket/${s3dir_lambda}/source/0.1.3/source.zip
 """
 
 import typing as T
 import glob
 import shutil
 import subprocess
+import dataclasses
 from pathlib import Path
 from urllib.parse import urlencode
 
 from s3pathlib import S3Path
 from func_args import NOTHING
 from boto_session_manager import BotoSesManager
 
-from . import utils
-from .context import BuildContext
-from .build_dist import (
-    build_dist_with_python,
+from .vendor.better_pathlib import temp_cwd
+from .vendor.hashes import hashes
+from .vendor.build_dist import (
     build_dist_with_python_build,
     build_dist_with_poetry_build,
 )
+from .utils import ensure_exact_one_true
+from .context import BuildContext
 
 
 def _build_source_from_tar_gz(
     package_name: str,
     dir_dist: Path,
     dir_tmp: Path,
     dir_deploy: Path,
@@ -109,15 +111,15 @@
     :param use_pathlib: do you want to use pathlib to build your source?
     :param verbose: whether you want to suppress the output of cli commands
 
     :return: tuple of two item, first one is the code sha256 hash of the source artifacts,
         second one is the path to the source.zip file
     """
     # validate arguments
-    utils.ensure_exact_one_true(
+    ensure_exact_one_true(
         [
             use_pip,
             use_build,
             use_poetry,
             use_pathlib,
         ]
     )
@@ -134,15 +136,15 @@
 
     # clean up existing files in build folder
     shutil.rmtree(build_context.dir_build, ignore_errors=True)
     build_context.dir_deploy.mkdir(parents=True, exist_ok=True)
 
     # install python library
     if use_pip:
-        with utils.temp_cwd(dir_project_root):
+        with temp_cwd(dir_project_root):
             args = [
                 f"{path_bin_python}",
                 "-m",
                 "pip",
                 "install",
                 f"{dir_project_root}",
                 "--no-dependencies",
@@ -207,19 +209,19 @@
         "-r",
         "-9",
     ]
     if verbose is False:
         args.append("-q")
 
     # has to cd to the deploy dir to run the glob command
-    with utils.temp_cwd(build_context.dir_deploy):
+    with temp_cwd(build_context.dir_deploy):
         args.extend(glob.glob("*"))
         subprocess.run(args, check=True)
 
-    source_sha256 = utils.sha256_of_paths([build_context.dir_deploy])
+    source_sha256 = hashes.of_paths([build_context.dir_deploy])
     path_source_zip = build_context.path_source_zip
     return source_sha256, path_source_zip
 
 
 def upload_source_artifacts(
     bsm: "BotoSesManager",
     version: str,
@@ -259,14 +261,28 @@
         overwrite=True,
         bsm=bsm,
         extra_args=extra_args,
     )
     return s3path_source_zip
 
 
+@dataclasses.dataclass
+class SourceArtifactsDeployment:
+    """
+    Source artifacts deployment information.
+
+    :param source_sha256: code sha256 hash of the source artifacts
+    :param path_source_zip: path to the source.zip file on local
+    :param s3path_source_zip: S3Path object of the source.zip file
+    """
+    source_sha256: str = dataclasses.field()
+    path_source_zip: Path = dataclasses.field()
+    s3path_source_zip: S3Path = dataclasses.field()
+
+
 def publish_source_artifacts(
     bsm: "BotoSesManager",
     path_setup_py_or_pyproject_toml: T.Union[str, Path],
     package_name: str,
     path_lambda_function: T.Union[str, Path],
     version: str,
     dir_build: T.Union[str, Path],
@@ -276,15 +292,15 @@
     metadata: T.Optional[T.Dict[str, str]] = NOTHING,
     tags: T.Optional[T.Dict[str, str]] = NOTHING,
     use_pip: bool = False,
     use_build: bool = False,
     use_poetry: bool = False,
     use_pathlib: bool = False,
     verbose: bool = True,
-) -> T.Tuple[str, Path, S3Path]:
+) -> SourceArtifactsDeployment:
     """
     Assemble the following functions together to build and then upload the
     source artifacts to S3.
 
     - :func:`build_source_artifacts`
     - :func:`upload_source_artifacts`
 
@@ -305,17 +321,15 @@
     :param tags: S3 object tags
     :param use_pip: do you want to use pip to build your source?
     :param use_build: do you want to use python-build to build your source?
     :param use_poetry: do you want to use python-poetry to build your source?
     :param use_pathlib: do you want to use pathlib to build your source?
     :param verbose: whether you want to suppress the output of cli commands
 
-    :return: tuple of three item, first one is the code sha256 hash of the source artifacts,
-        second one is the path to the source.zip file, the third one is the S3 path
-        of the uploaded ``source.zip`` file.
+    :return: :class:`SourceArtifactsDeployment` object.
     """
     source_sha256, path_source_zip = build_source_artifacts(
         path_setup_py_or_pyproject_toml=path_setup_py_or_pyproject_toml,
         package_name=package_name,
         path_lambda_function=path_lambda_function,
         dir_build=dir_build,
         path_bin_python=path_bin_python,
@@ -331,8 +345,12 @@
         version=version,
         source_sha256=source_sha256,
         dir_build=dir_build,
         s3dir_lambda=s3dir_lambda,
         metadata=metadata,
         tags=tags,
     )
-    return source_sha256, path_source_zip, s3path_source_zip
+    return SourceArtifactsDeployment(
+        source_sha256=source_sha256,
+        path_source_zip=path_source_zip,
+        s3path_source_zip=s3path_source_zip,
+    )
```

### Comparing `aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/PKG-INFO` & `aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws-lambda-layer
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts.
 Home-page: https://github.com/MacHu-GWU/aws_lambda_layer-project
-Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.3#downloads
+Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/SOURCES.txt` & `aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 release-history.rst
 requirements-test.txt
 requirements.txt
 setup.py
 aws_lambda_layer/__init__.py
 aws_lambda_layer/_version.py
 aws_lambda_layer/api.py
-aws_lambda_layer/build_dist.py
 aws_lambda_layer/context.py
 aws_lambda_layer/layer.py
 aws_lambda_layer/source.py
 aws_lambda_layer/utils.py
 aws_lambda_layer.egg-info/PKG-INFO
 aws_lambda_layer.egg-info/SOURCES.txt
 aws_lambda_layer.egg-info/dependency_links.txt
 aws_lambda_layer.egg-info/requires.txt
 aws_lambda_layer.egg-info/top_level.txt
-tests/test_import.py
-tests/test_utils.py
+aws_lambda_layer/vendor/__init__.py
+aws_lambda_layer/vendor/better_pathlib.py
+aws_lambda_layer/vendor/build_dist.py
+aws_lambda_layer/vendor/hashes.py
+tests/test_import.py
```

### Comparing `aws_lambda_layer-0.2.3/pyproject.toml` & `aws_lambda_layer-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.3/release-history.rst` & `aws_lambda_layer-0.2.4/release-history.rst`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.2.4 (2023-05-27)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Minor Improvements**
+
+- now the ``deploy_layer`` method returns a ``LayerDeployment`` object.
+- now the ``publish_source_artifacts`` method returns a ``SourceArtifactsDeployment`` object.
+
+
 0.2.3 (2023-05-26)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - also add source sha256 and layer sha256 to S3 object metadata for integrity check.
```

### Comparing `aws_lambda_layer-0.2.3/setup.py` & `aws_lambda_layer-0.2.4/setup.py`

 * *Files identical despite different names*

