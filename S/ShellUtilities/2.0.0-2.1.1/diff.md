# Comparing `tmp/ShellUtilities-2.0.0.tar.gz` & `tmp/ShellUtilities-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ShellUtilities-2.0.0.tar", last modified: Mon May 22 17:11:08 2023, max compression
+gzip compressed data, was "ShellUtilities-2.1.1.tar", last modified: Fri May 26 14:55:52 2023, max compression
```

## Comparing `ShellUtilities-2.0.0.tar` & `ShellUtilities-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 17:11:08.000000 ShellUtilities-2.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 17:11:08.000000 ShellUtilities-2.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 17:11:08.000000 ShellUtilities-2.0.0/src/ShellUtilities/
--rw-r--r--   0 root         (0) root         (0)     8119 2023-04-05 16:00:52.000000 ShellUtilities-2.0.0/src/ShellUtilities/Shell.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-04-05 16:00:52.000000 ShellUtilities-2.0.0/src/ShellUtilities/ShellCommandException.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-05 16:00:52.000000 ShellUtilities-2.0.0/src/ShellUtilities/ShellCommandResults.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:00:52.000000 ShellUtilities-2.0.0/src/ShellUtilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 17:11:08.000000 ShellUtilities-2.0.0/src/ShellUtilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-22 17:11:08.000000 ShellUtilities-2.0.0/src/ShellUtilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-05-22 17:11:08.000000 ShellUtilities-2.0.0/src/ShellUtilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 17:11:08.000000 ShellUtilities-2.0.0/src/ShellUtilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-22 17:11:08.000000 ShellUtilities-2.0.0/src/ShellUtilities.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:00:52.000000 ShellUtilities-2.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)      965 2023-05-22 16:56:42.000000 ShellUtilities-2.0.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-22 17:11:08.000000 ShellUtilities-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 17:11:08.000000 ShellUtilities-2.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 14:55:52.700048 ShellUtilities-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-05-26 14:55:52.700048 ShellUtilities-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-05-26 14:46:02.000000 ShellUtilities-2.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 14:55:52.700048 ShellUtilities-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      965 2023-05-26 14:55:01.000000 ShellUtilities-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 14:55:52.698047 ShellUtilities-2.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 14:55:52.699048 ShellUtilities-2.1.1/src/ShellUtilities/
+-rw-r--r--   0 root         (0) root         (0)     8324 2023-05-26 14:18:39.000000 ShellUtilities-2.1.1/src/ShellUtilities/Shell.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-04-05 16:00:52.000000 ShellUtilities-2.1.1/src/ShellUtilities/ShellCommandException.py
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-05 16:00:52.000000 ShellUtilities-2.1.1/src/ShellUtilities/ShellCommandResults.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:00:52.000000 ShellUtilities-2.1.1/src/ShellUtilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 14:55:52.700048 ShellUtilities-2.1.1/src/ShellUtilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-05-26 14:55:52.000000 ShellUtilities-2.1.1/src/ShellUtilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-26 14:55:52.000000 ShellUtilities-2.1.1/src/ShellUtilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 14:55:52.000000 ShellUtilities-2.1.1/src/ShellUtilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-26 14:55:52.000000 ShellUtilities-2.1.1/src/ShellUtilities.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ShellUtilities-2.0.0/src/ShellUtilities/Shell.py` & `ShellUtilities-2.1.1/src/ShellUtilities/Shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,68 +6,72 @@
 import os
 import threading
 import queue
 import asyncio
 
 logger = logging.getLogger(__name__).parent
 
-def __execute_shell_command(command, env, cwd):
+def __execute_shell_command(command, env, cwd, executable=None):
     # Create the process and wait for the exit
-    process = __execute_shell_command_async(command, env, cwd)
+    process = __execute_shell_command_async(command, env, cwd, executable)
     (stdout, stderr) = process.communicate()
     exitcode = process.returncode
 
     # The stderr and stdout are byte objects... lets change them to strings
     stdout = stdout.decode()
     stderr = stderr.decode()
 
     # Sanitize the variables and remove trailing newline characters
     stdout = stdout.rstrip("\n")
     stderr = stderr.rstrip("\n")
 
     return exitcode, stdout, stderr
 
 
-def __execute_shell_command_async(command, env, cwd):
+def __execute_shell_command_async(command, env, cwd, executable=None):
 
     args = [command]
     kwargs = {
         "stdout": subprocess.PIPE,
         "stderr": subprocess.PIPE,
         "shell": True,
-        "close_fds": 'posix'
+        "close_fds": 'posix',
     }
+    logging.debug(f"Executable set to: {executable}")
+
+    if executable:
+        kwargs["executable"] = executable
     if env:
         kwargs["env"] = env
     if cwd:
         kwargs["cwd"] = cwd
 
     # Create the process
     process = subprocess.Popen(*args, **kwargs)
 
     return process
 
 
-def execute_shell_command(command, max_retries=1, retry_delay=1, env=None, cwd=None, blocking=True):
+def execute_shell_command(command, max_retries=1, retry_delay=1, env=None, cwd=None, blocking=True, executable=None):
 
     try:
 
         if cwd and not os.path.isdir(cwd):
             raise Exception("The working directory '{0}' does not exist.".format(cwd))
 
         logging.debug("Running shell command:")
         logging.debug(command)
 
         for i in range(0, max_retries):
 
             # Run the shell command
             if blocking:
-                exitcode, stdout_string, stderr_string = __execute_shell_command(command, env, cwd)
+                exitcode, stdout_string, stderr_string = __execute_shell_command(command, env, cwd, executable)
             else:
-                process = __execute_shell_command_async(command, env, cwd)
+                process = __execute_shell_command_async(command, env, cwd, executable)
                 return process
 
             # Set the exit code and return
             if exitcode == 0:
                 return ShellCommandResults(command, stdout_string, stderr_string, exitcode)
 
             # If an error occured we need to determine if this is the last retry attempt
@@ -186,14 +190,15 @@
     stderr_read_thread = threading.Thread(target=read_from_queue, args=[stderr_queue, stderr_func, stderr_lock])
     stdout_read_thread.start()
     stderr_read_thread.start()
 
     threads = (stdout_enqueue_thread, stderr_enqueue_thread, stdout_read_thread, stderr_read_thread)
     return threads
 
+
 def wait(shell_process, output_handling_threads):
 
     # This is a blocking function which will safely wait for the shell process and handling threads to complete
 
     # Wait for the process to exit
     shell_process.wait()
```

### Comparing `ShellUtilities-2.0.0/setup.py` & `ShellUtilities-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open('README.md', "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="ShellUtilities",
-    version="2.0.0",
+    version="2.1.1",
     author="tschneider",
     author_email="tschneider@live.com",
     description="A library for executing shell commands in either a blocking or non-blocking way.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(source_code_dir),
     package_dir={
```

