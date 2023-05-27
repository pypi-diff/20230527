# Comparing `tmp/rtvc-0.1.0.tar.gz` & `tmp/rtvc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtvc-0.1.0.tar", last modified: Fri May 26 07:28:28 2023, max compression
+gzip compressed data, was "rtvc-0.1.1.tar", last modified: Sat May 27 01:13:14 2023, max compression
```

## Comparing `rtvc-0.1.0.tar` & `rtvc-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0       20 2023-05-26 04:39:35.864563 rtvc-0.1.0/README.md
--rw-r--r--   0        0        0     1099 2023-05-26 07:28:28.473027 rtvc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 04:45:22.845379 rtvc-0.1.0/rtvc/__init__.py
--rw-r--r--   0        0        0      437 2023-05-26 06:43:47.085759 rtvc-0.1.0/rtvc/__main__.py
--rw-r--r--   0        0        0      716 2023-05-26 06:43:46.859836 rtvc-0.1.0/rtvc/audio.py
--rw-r--r--   0        0        0     1067 2023-05-26 07:07:25.387820 rtvc-0.1.0/rtvc/config.py
--rw-r--r--   0        0        0    11281 2023-05-26 07:17:29.696986 rtvc-0.1.0/rtvc/gui.py
--rw-r--r--   0        0        0      876 2023-05-26 06:43:46.863686 rtvc-0.1.0/rtvc/i18n.py
--rw-r--r--   0        0        0      854 2023-05-26 07:14:19.866000 rtvc-0.1.0/rtvc/locales/en_US.yaml
--rw-r--r--   0        0        0      830 2023-05-26 07:21:24.961927 rtvc-0.1.0/rtvc/locales/zh_CN.yaml
--rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 rtvc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-26 07:34:56.775946 rtvc-0.1.1/LICENSE
+-rw-r--r--   0        0        0      562 2023-05-26 23:59:00.302765 rtvc-0.1.1/README.md
+-rw-r--r--   0        0        0     1437 2023-05-27 01:13:14.865999 rtvc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 04:45:22.845379 rtvc-0.1.1/rtvc/__init__.py
+-rw-r--r--   0        0        0      437 2023-05-26 06:43:47.085759 rtvc-0.1.1/rtvc/__main__.py
+-rw-r--r--   0        0        0   156997 2023-05-27 00:05:53.762257 rtvc-0.1.1/rtvc/assets/icon.png
+-rw-r--r--   0        0        0      734 2023-05-26 23:42:03.016172 rtvc-0.1.1/rtvc/audio.py
+-rw-r--r--   0        0        0     1950 2023-05-27 00:37:54.402972 rtvc-0.1.1/rtvc/config.py
+-rw-r--r--   0        0        0    18721 2023-05-27 00:37:54.410808 rtvc-0.1.1/rtvc/gui.py
+-rw-r--r--   0        0        0      907 2023-05-27 00:37:54.405152 rtvc-0.1.1/rtvc/i18n.py
+-rw-r--r--   0        0        0      977 2023-05-26 23:46:36.062919 rtvc-0.1.1/rtvc/locales/en_US.yaml
+-rw-r--r--   0        0        0      941 2023-05-26 23:46:45.823224 rtvc-0.1.1/rtvc/locales/zh_CN.yaml
+-rw-r--r--   0        0        0     1249 2023-05-26 23:41:55.884670 rtvc-0.1.1/tests/test_sola.py
+-rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 rtvc-0.1.1/PKG-INFO
```

### Comparing `rtvc-0.1.0/pyproject.toml` & `rtvc-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,62 @@
 [project]
 name = "rtvc"
-version = "0.1.0"
-description = ""
+version = "0.1.1"
+description = "Real-Time Voice Conversion GUI"
+readme = "README.md"
+requires-python = ">=3.10,<3.12"
+keywords = [
+    "voice-conversion",
+    "svc",
+]
 authors = [
     { name = "lengyue", email = "lengyue@lengyue.me" },
 ]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Programming Language :: Python :: 3.10",
+]
 dependencies = [
     "noisereduce>=2.0.1",
     "sounddevice>=0.4.6",
-    "torch>=2.0.1",
-    "torchaudio>=2.0.2",
     "pyyaml>=6.0",
     "PyQt6>=6.5.0",
     "pyqtdarktheme==2.1.0",
+    "requests>=2.31.0",
 ]
-requires-python = ">=3.10,<3.12"
-readme = "README.md"
 
 [project.license]
 text = "MIT"
 
-[project.scripts]
+[project.urls]
+repository = "https://github.com/fishaudio/realtime-vc-gui"
+
+[project.gui-scripts]
 rtvc = "rtvc.__main__:main"
 
 [tool.pdm.build]
 includes = [
     "rtvc",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort>=5.12.0",
     "black>=23.3.0",
     "pytest>=7.3.1",
-    "PySimpleGUI>=4.60.5",
+    "torch>=2.0.1",
+    "pyinstaller>=5.11.0",
 ]
 
 [tool.pdm.scripts.lint]
 shell = "black . && isort ."
 
+[tool.pdm.scripts.lint-check]
+shell = "black --check . && isort --check ."
+
 [tool.pdm.scripts.test]
 shell = "PYTHONPATH=. pytest -n=auto -q tests"
 
 [tool.pdm.scripts.docs]
 shell = "sphinx-autobuild docs docs/_build/html"
 
 [[tool.pdm.source]]
```

### Comparing `rtvc-0.1.0/rtvc/i18n.py` & `rtvc-0.1.1/rtvc/i18n.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pathlib import Path
 
 import yaml
 
-from rtvc.config import config
+from rtvc.config import application_path, config
 
 # Load i18n files from locales/ directory
-i18n_path = Path(__file__).parent / "locales"
+i18n_path = application_path / "locales"
 i18n_files = list(i18n_path.glob("*.yaml"))
 
 i18n_map = {}
 for i18n_file in i18n_files:
-    with open(i18n_file, "r") as f:
+    with open(i18n_file, "r", encoding="utf-8") as f:
         i18n_map[i18n_file.stem] = yaml.safe_load(f.read())
 
 
 def _t(key: str | list[str], locale: str | None = None, fallback: str = "en_US") -> str:
     if locale is None:
         locale = config.locale
```

### Comparing `rtvc-0.1.0/rtvc/locales/en_US.yaml` & `rtvc-0.1.1/rtvc/locales/en_US.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 i18n:
   language: "Language"
   restart_msg: "Configuration changed, do you want to restart the app to take effect?"
 
 backend:
   name: "Backend"
   test: "Test"
+  test_succeed: "Successfully connected to backend."
+  test_failed: "Failed to connect to backend in 5s."
 
 audio_device:
   name: "Audio Device (Please use same kind of device for input and output)"
   input: "Input (Recording)"
   output: "Output (Playback)"
 
 audio:
@@ -30,7 +32,8 @@
   input_denoise: "Input Denoise"
   output_denoise: "Output Denoise"
 
 action:
   start: "Start Voice Conversion"
   stop: "Stop Voice Conversion"
   latency: "Latency: {latency:.2f} ms"
+  error: "Error"
```

### Comparing `rtvc-0.1.0/rtvc/locales/zh_CN.yaml` & `rtvc-0.1.1/rtvc/locales/zh_CN.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 i18n:
   language: "语言"
   restart_msg: "配置已更改，是否要重新启动应用程序以使其生效?"
 
 backend:
   name: "后端"
   test: "测试"
+  test_succeed: "成功连接到后端。"
+  test_failed: "5 秒内无法连接到后端。"
 
 audio_device:
   name: "音频设备（请对输入和输出使用同类设备）"
   input: "输入（录音）"
   output: "输出（播放）"
 
 audio:
@@ -30,7 +32,8 @@
   input_denoise: "输入降噪"
   output_denoise: "输出降噪"
 
 action:
   start: "开始语音转换"
   stop: "停止语音转换"
   latency: "延迟: {latency:.2f} ms"
+  error: "错误"
```

