# Comparing `tmp/neon_speech-3.3.2a6-py3-none-any.whl.zip` & `tmp/neon_speech-3.3.2a7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17849 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1831 b- defN 23-May-25 16:29 neon_speech/__init__.py
--rw-r--r--  2.0 unx     2914 b- defN 23-May-25 16:29 neon_speech/__main__.py
--rw-r--r--  2.0 unx     5085 b- defN 23-May-25 16:29 neon_speech/cli.py
--rw-r--r--  2.0 unx    21078 b- defN 23-May-25 16:29 neon_speech/service.py
--rw-r--r--  2.0 unx     4459 b- defN 23-May-25 16:29 neon_speech/stt.py
--rw-r--r--  2.0 unx     4395 b- defN 23-May-25 16:29 neon_speech/utils.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-25 16:29 neon_speech-3.3.2a6.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2451 b- defN 23-May-25 16:29 neon_speech-3.3.2a6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 16:29 neon_speech-3.3.2a6.dist-info/WHEEL
--rw-r--r--  2.0 unx      111 b- defN 23-May-25 16:29 neon_speech-3.3.2a6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-May-25 16:29 neon_speech-3.3.2a6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      988 b- defN 23-May-25 16:29 neon_speech-3.3.2a6.dist-info/RECORD
-12 files, 45050 bytes uncompressed, 16191 bytes compressed:  64.1%
+Zip file size: 17841 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1831 b- defN 23-May-26 22:25 neon_speech/__init__.py
+-rw-r--r--  2.0 unx     2784 b- defN 23-May-26 22:25 neon_speech/__main__.py
+-rw-r--r--  2.0 unx     5171 b- defN 23-May-26 22:25 neon_speech/cli.py
+-rw-r--r--  2.0 unx    21078 b- defN 23-May-26 22:25 neon_speech/service.py
+-rw-r--r--  2.0 unx     4459 b- defN 23-May-26 22:25 neon_speech/stt.py
+-rw-r--r--  2.0 unx     4395 b- defN 23-May-26 22:25 neon_speech/utils.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-26 22:25 neon_speech-3.3.2a7.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2451 b- defN 23-May-26 22:25 neon_speech-3.3.2a7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 22:25 neon_speech-3.3.2a7.dist-info/WHEEL
+-rw-r--r--  2.0 unx      111 b- defN 23-May-26 22:25 neon_speech-3.3.2a7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-May-26 22:25 neon_speech-3.3.2a7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      988 b- defN 23-May-26 22:25 neon_speech-3.3.2a7.dist-info/RECORD
+12 files, 45006 bytes uncompressed, 16183 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: neon_speech/stt.py
 Comment: 
 
 Filename: neon_speech/utils.py
 Comment: 
 
-Filename: neon_speech-3.3.2a6.dist-info/LICENSE.md
+Filename: neon_speech-3.3.2a7.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_speech-3.3.2a6.dist-info/METADATA
+Filename: neon_speech-3.3.2a7.dist-info/METADATA
 Comment: 
 
-Filename: neon_speech-3.3.2a6.dist-info/WHEEL
+Filename: neon_speech-3.3.2a7.dist-info/WHEEL
 Comment: 
 
-Filename: neon_speech-3.3.2a6.dist-info/entry_points.txt
+Filename: neon_speech-3.3.2a7.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_speech-3.3.2a6.dist-info/top_level.txt
+Filename: neon_speech-3.3.2a7.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_speech-3.3.2a6.dist-info/RECORD
+Filename: neon_speech-3.3.2a7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_speech/__main__.py

```diff
@@ -23,33 +23,30 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from ovos_utils import wait_for_exit_signal
-from neon_utils.configuration_utils import init_config_dir
 from neon_utils.log_utils import init_log
 from neon_utils.process_utils import start_malloc, snapshot_malloc, print_malloc
 from ovos_utils.log import LOG
-from ovos_utils.process_utils import PIDLock as Lock
+from ovos_utils.process_utils import PIDLock, reset_sigint_handler
+from neon_speech.service import NeonSpeechClient
 
 
 def main(*args, **kwargs):
     # Initialize configuration
-    init_config_dir()
     init_log(log_name="voice")
     if kwargs.get("config"):
         LOG.warning("Found config kwarg, updating to 'speech_config'")
         kwargs["speech_config"] = kwargs.pop("config")
 
-    from ovos_utils.process_utils import reset_sigint_handler
-    from neon_speech.service import NeonSpeechClient
     reset_sigint_handler()
-    Lock("voice")
+    PIDLock("voice")
     malloc_running = start_malloc(stack_depth=4)
     service = NeonSpeechClient(*args, **kwargs)
     service.start()
     wait_for_exit_signal()
     if malloc_running:
         try:
             print_malloc(snapshot_malloc())
```

## neon_speech/cli.py

```diff
@@ -48,14 +48,17 @@
 @click.option("--module", "-m", default=None,
               help="STT Plugin to configure")
 @click.option("--package", "-p", default=None,
               help="STT package spec to install")
 @click.option("--force-install", "-f", default=False, is_flag=True,
               help="Force pip installation of configured module")
 def run(module, package, force_install):
+    from neon_utils.configuration_utils import init_config_dir
+    init_config_dir()
+
     from neon_speech.__main__ import main
     from ovos_config.config import Configuration
     speech_config = Configuration()
     if force_install or module or package:
         install_plugin(module, package, force_install)
     if module and module != speech_config["stt"]["module"]:
         click.echo("Updating runtime config with module and package")
```

## Comparing `neon_speech-3.3.2a6.dist-info/LICENSE.md` & `neon_speech-3.3.2a7.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_speech-3.3.2a6.dist-info/METADATA` & `neon_speech-3.3.2a7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: neon-speech
-Version: 3.3.2a6
+Version: 3.3.2a7
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ovos-dinkum-listener (>=0.0.2a21,~=0.0.1)
+Requires-Dist: ovos-dinkum-listener (>=0.0.2a24,~=0.0.1)
 Requires-Dist: ovos-bus-client (~=0.0.3)
 Requires-Dist: ovos-utils (~=0.0.30)
 Requires-Dist: ovos-plugin-manager (>=0.0.23a17,~=0.0.19)
 Requires-Dist: click (~=8.0)
 Requires-Dist: click-default-group (~=1.2)
 Requires-Dist: neon-utils[audio,network] (>=1.5.0a5,~=1.3)
 Requires-Dist: ovos-config (~=0.0.7)
```

