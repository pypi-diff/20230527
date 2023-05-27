# Comparing `tmp/simplejob-0.0.4-py3-none-any.whl.zip` & `tmp/simplejob-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 6519 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      138 b- defN 23-May-22 15:32 simplejob/__init__.py
--rw-rw-rw-  2.0 fat     9755 b- defN 23-May-25 15:26 simplejob/simplejob.py
--rw-rw-rw-  2.0 fat     1090 b- defN 23-May-25 15:47 simplejob-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5394 b- defN 23-May-25 15:47 simplejob-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-25 15:47 simplejob-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-25 15:47 simplejob-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      552 b- defN 23-May-25 15:47 simplejob-0.0.4.dist-info/RECORD
-7 files, 17031 bytes uncompressed, 5541 bytes compressed:  67.5%
+Zip file size: 7235 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      138 b- defN 23-May-26 20:52 simplejob/__init__.py
+-rw-rw-rw-  2.0 fat      878 b- defN 23-May-27 03:49 simplejob/__main__.py
+-rw-rw-rw-  2.0 fat    10127 b- defN 23-May-27 02:48 simplejob/simplejob.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 23-May-27 03:50 simplejob-0.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5658 b- defN 23-May-27 03:50 simplejob-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-27 03:50 simplejob-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-27 03:50 simplejob-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      630 b- defN 23-May-27 03:50 simplejob-0.0.5.dist-info/RECORD
+8 files, 18623 bytes uncompressed, 6139 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: simplejob/__init__.py
 Comment: 
 
+Filename: simplejob/__main__.py
+Comment: 
+
 Filename: simplejob/simplejob.py
 Comment: 
 
-Filename: simplejob-0.0.4.dist-info/LICENSE
+Filename: simplejob-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: simplejob-0.0.4.dist-info/METADATA
+Filename: simplejob-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: simplejob-0.0.4.dist-info/WHEEL
+Filename: simplejob-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: simplejob-0.0.4.dist-info/top_level.txt
+Filename: simplejob-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: simplejob-0.0.4.dist-info/RECORD
+Filename: simplejob-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplejob/simplejob.py

```diff
@@ -2,19 +2,20 @@
 # https://github.com/Hajime-Saitou/simplejob
 #
 # Copyright (c) 2023 Hajime Saito
 # MIT License
 import subprocess
 import threading
 import time
-from datetime import datetime, timedelta
+from datetime import datetime
 import enum
 import os
 import uuid
 from collections import Counter
+import json
 
 class JobRunningStatus(enum.IntEnum):
     Ready = 0
     Running = 1
     Completed = 2
     RetryOut = 3
 
@@ -50,14 +51,18 @@
         ids = { context["id"] for context in jobContexts }
         waitsIds = { id for context in jobContexts for id in context.get("waits", []) }
         return waitsIds - ids
     
     def detectInvalidIds(self, jobContexts:list) -> list:
         return [ index for index, context in enumerate(jobContexts) if not context.get("id", None) ]
 
+    def entryFromJson(self, filename:str):
+        with open(filename, "r") as f:
+            self.entry(json.load(f)["jobContexts"])
+
     def entry(self, jobContexts:list) -> None:
         elementIndices = self.detectInvalidIds(jobContexts)
         if len(elementIndices) > 0:
             raise ValueError(f"Invalid Id detected. element indices={elementIndices}")
 
         invalidWaitsIds = self.detectInvalidWaitsIds(jobContexts)
         if len(invalidWaitsIds) > 0:
@@ -83,59 +88,67 @@
             context["jobManager"] = self
             context["logOutputDirectory"] = self.logOutputDirecotry
             job.entry(**context)
             self.jobs.append(job)
 
         self.jobContexts = jobContexts
 
-    def rerun(self):
-        self.join()
+    def rerun(self, interval:float=1.0):
+        self.join(interval)
 
         for index, job in enumerate(self.jobs):
             if not job.hasError() and not job.retryOuted():
                 continue
 
             job = SimpleJob()
             context = self.jobContexts[index]
             context["jobManager"] = self
             context["logOutputDirectory"] = self.logOutputDirecotry
             job.entry(**context)
             self.jobs[index] = job
 
+        self.run(interval)
+
     def runAllReadyJobs(self) -> None:
         [ job.start() for job in self.jobs if job.ready() and not job.ident]
 
     def running(self) -> bool:
         return len([ job for job in self.jobs if job.running() ]) >= 1
 
-    def join(self, interval:int=1) -> None:
+    def join(self, interval:float=1.0) -> None:
         while self.running():
             time.sleep(interval)
 
-    def wait(self, interval:int=1) -> None:
-        while not self.completed():
+    def run(self, interval:float=1.0) -> None:
+        while True:
             self.runAllReadyJobs()
             if self.errorOccurred():
                 self.join(interval)
-                raise CalledJobError("Error occured")
+                break
+
+            if self.completed():
+                break
 
             time.sleep(interval)
 
+        if self.errorOccurred():
+            raise CalledJobError("Error occured")
+
     def completed(self) -> bool:
         return len([ job for job in self.jobs if job.completed() ]) == len(self.jobs)
 
     def errorOccurred(self) -> bool:
         return len([ job for job in self.jobs if job.completed() and job.hasError() ]) >= 1
 
     def report(self) -> dict:
         report = { "results": [] }
         for job in self.jobs:
             report["results"].append({ job.id: job.report() })
 
-        return report
+        return json.dumps(report, indent=4)
 
     def getRunningStatus(self):
         return Counter([ job.runningStatus.name for job in self.jobs ])
 
 class SimpleJob(threading.Thread):
     def entry(self, commandLine:str, id:str="", timeout:int=None, retry:int=1, delay:int=0, backoff:int=1, waits:list = [], logOutputDirectory:str="", jobManager:SimpleJobManager=None) -> None:
         if not jobManager and len(waits) > 0:
@@ -233,16 +246,17 @@
 
         with open(self.logFileName, "a", encoding="utf-8") as f:
             f.writelines(text)
 
     def report(self) -> dict:
         return {
             "runnigStatus": self.runningStatus.name,
-            "retried": self.retried if self.timeout is not None else None,
             "exitCode": self.exitCode if self.completed() else None,
+            "retried": self.retried if self.timeout is not None else None,
+            "commandLine": self.commandLine,
             "startDateTime": self.startDateTime.strftime('%Y/%m/%d %H:%M:%S.%f') if self.startDateTime is not None else None,
             "finishDateTime": self.finishDateTime.strftime('%Y/%m/%d %H:%M:%S.%f') if self.finishDateTime is not None else None,
             "elapsedTime": self.getElapsedTime()
         }
 
     def getElapsedTime(self) -> str:
         totalMilleSeconds = self.finishTime - self.startTime
```

## Comparing `simplejob-0.0.4.dist-info/LICENSE` & `simplejob-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `simplejob-0.0.4.dist-info/METADATA` & `simplejob-0.0.5.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplejob
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple Batch job executor
 Home-page: https://github.com/Hajime-Saitou/simplejob
 Author: Hajime Saito
 Author-email: g.hajime.saitou@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/Hajime-Saitou/simplejob
 Keywords: batch,job
@@ -40,39 +40,42 @@
 
 ```
 from simplejob.simplejob import SimpleJobManager
 ```
 
 Prepare a job context consisting of job parameters and pass it as an argument to JobManager.entry().
 
-id ... Job ID (arbitrary name, if omitted, the base name of the first command line argument)
-command line ... command to execute and command line parameters
-Waiting list of other job IDs ... List of job IDs waiting to run
++ id ... Job ID (arbitrary name, if omitted, the base name of the first command line argument)
++ commandLine ... command to execute and command line parameters
+* Waits ... List of job IDs waiting to run
 
 ```
 jobContexts = [
     { "id": "hoge", "commandLine": r"timeout /t 1 /nobreak" },
     { "id": "piyo", "commandLine": r"timeout /t 3 /nobreak", "waits": [ "hoge" ] },
     { "id": "fuga", "commandLine": r"timeout /t 5 /nobreak", "waits": [ "hoge" ] },
-    { "id": "moga", "commandLine": r"timeout /t 2 /nobreak", "waits": [ "hoge", "fuga" ] },
+    { "id": "moga", "commandLine": r"timeout /t 2 /nobreak", "waits": [ "piyo", "fuga" ] },
 ]
 jobManager = SimpleJobManager()
 jobManager.entry(jobContexts)
 ```
 
 Run all jobs through JobManager.runAllReadyJobs() until all jobs are finished or an error occurs. If necessary, call an interval timer in the loop. The example calls a 1 second interval timer.
 
 ```
-while not jobManager.completed():
+while True:
     jobManager.runAllReadyJobs()
     if jobManager.errorOccurred():
         print("error occurred")
         jobManager.join()
         break
 
+    if jobManager.completed():
+        break
+
     time.sleep(1)
 ```
 
 It can be written on a single line using wait(). If error occred in the wait(), Raise CalledJobException.
 
 ```
 jobManager.wait()
@@ -86,70 +89,75 @@
 
 ```
 {
     "results": [
         {
             "hoge": {
                 "runnigStatus": "Completed",
-                "retried": null,
                 "exitCode": 0,
-                "startDateTime": "2023/05/26 00:12:39.741372",
-                "finishDateTime": "2023/05/26 00:12:40.204306",
-                "elapsedTime": "00:00:00.463711"
+                "retried": null,
+                "commandLine": "timeout /t 1 /nobreak",
+                "startDateTime": "2023/05/27 05:42:16.595910",
+                "finishDateTime": "2023/05/27 05:42:17.172984",
+                "elapsedTime": "00:00:00.580679"
             }
         },
         {
             "piyo": {
                 "runnigStatus": "Completed",
-                "retried": null,
                 "exitCode": 0,
-                "startDateTime": "2023/05/26 00:12:40.755401",
-                "finishDateTime": "2023/05/26 00:12:43.177881",
-                "elapsedTime": "00:00:02.422424"
+                "retried": null,
+                "commandLine": "timeout /t 3 /nobreak",
+                "startDateTime": "2023/05/27 05:42:17.589688",
+                "finishDateTime": "2023/05/27 05:42:20.131554",
+                "elapsedTime": "00:00:02.537245"
             }
         },
         {
             "fuga": {
                 "runnigStatus": "Completed",
-                "retried": null,
                 "exitCode": 0,
-                "startDateTime": "2023/05/26 00:12:40.762754",
-                "finishDateTime": "2023/05/26 00:12:41.122336",
-                "elapsedTime": "00:00:00.364163"
+                "retried": null,
+                "commandLine": "timeout /t 1 /nobreak",
+                "startDateTime": "2023/05/27 05:42:17.597681",
+                "finishDateTime": "2023/05/27 05:42:18.177357",
+                "elapsedTime": "00:00:00.584966"
             }
         },
         {
             "moga": {
                 "runnigStatus": "Completed",
-                "retried": null,
                 "exitCode": 0,
-                "startDateTime": "2023/05/26 00:12:43.800788",
-                "finishDateTime": "2023/05/26 00:12:45.155410",
-                "elapsedTime": "00:00:01.352033"
+                "retried": null,
+                "commandLine": "timeout /t 2 /nobreak",
+                "startDateTime": "2023/05/27 05:42:20.636437",
+                "finishDateTime": "2023/05/27 05:42:22.192478",
+                "elapsedTime": "00:00:01.556920"
             }
         }
     ]
 }
 ```
 
 ### Retry on timed out
 If the job fails by timed out, it can be retried. The retry parameters are as follows.Retry parameters can be set for individual jobs.
 
-retry ... Retry count (default is 0, no retry)
-timeout ... Number of seconds to timeout the job (default is None, no timeout)
-delay ... number of seconds to delay the job on retry (default 0, no delay)
-backkoff ... power to back off the retry interval (default 1)
++ retry ... Retry count (default is 0, no retry)
++ timeout ... Number of seconds to timeout the job (default is None, no timeout)
++ delay ... number of seconds to delay the job on retry (default 0, no delay)
++ backkoff ... power to back off the retry interval (default 1)
 
 The report for a failed retry is shown below.
 
 ```
 {
     "runnigStatus": "RetryOut",
-    "retried": 1,
     "exitCode": null,
+    "retried": 1,
+    "commandLine": "timeout /t 2 /nobreak",
     "startDateTime": "2023/05/18 21:47:38.528989",
     "finishDateTime": "2023/05/18 21:47:43.594701",
     "elapsedTime": "00:00:05.65712"
 }
 ```
 
 ### rerun
@@ -159,14 +167,12 @@
 ```
 jobManager.rerun()
 jobManager.wait()
 ```
 
 ## Output the job log
 
-## Output the job log
-
 To output logs, specify the logOutputDirectory parameter to constructor of SimpleJobManager class. The log file name is the job id with a "log" extension.
 
 ```
 jobManager = SimpleJobManager(r"C:\temp\log")
 ```
```

## Comparing `simplejob-0.0.4.dist-info/RECORD` & `simplejob-0.0.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 simplejob/__init__.py,sha256=6uL_mCITP-B5IsHQnH_EdLOuOra_h8qhcsc4JzwQg5Y,138
-simplejob/simplejob.py,sha256=vC26GyLPioE4UTR3vy75pBzWKvlmOy_lcpD_fBeb5aI,9755
-simplejob-0.0.4.dist-info/LICENSE,sha256=Vagqa5lmdjnJU04Y4FZYFRpvkLGv8mB_8XGGXQ1ODg0,1090
-simplejob-0.0.4.dist-info/METADATA,sha256=vbLgLxHJRIEwpTlV-_eSsvL62Smw4zIHWkZcIHluAos,5394
-simplejob-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-simplejob-0.0.4.dist-info/top_level.txt,sha256=YTc5tkhXcB0dLc0EIlpQRHYmt8Q63ucEgdP0-QSAFng,10
-simplejob-0.0.4.dist-info/RECORD,,
+simplejob/__main__.py,sha256=P6WnVLNpP-OlOzQckCtLOPzQnNDQUnLEoQTcAnWHR5w,878
+simplejob/simplejob.py,sha256=8Pw2osHzIicE6apgbN29T7l6hZ0uZkS7o8Cyo7Dcdq8,10127
+simplejob-0.0.5.dist-info/LICENSE,sha256=Vagqa5lmdjnJU04Y4FZYFRpvkLGv8mB_8XGGXQ1ODg0,1090
+simplejob-0.0.5.dist-info/METADATA,sha256=NkeI7yCRrb0HtWoDlrOm9Vi-ON_9qFz7xVHCa53nCcA,5658
+simplejob-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+simplejob-0.0.5.dist-info/top_level.txt,sha256=YTc5tkhXcB0dLc0EIlpQRHYmt8Q63ucEgdP0-QSAFng,10
+simplejob-0.0.5.dist-info/RECORD,,
```

