# Comparing `tmp/neon_enclosure-1.4.3a2-py3-none-any.whl.zip` & `tmp/neon_enclosure-1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13817 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1831 b- defN 23-May-25 16:56 neon_enclosure/__init__.py
--rw-r--r--  2.0 unx     2832 b- defN 23-May-25 16:56 neon_enclosure/__main__.py
--rw-r--r--  2.0 unx     3152 b- defN 23-May-25 16:56 neon_enclosure/cli.py
--rw-r--r--  2.0 unx     3660 b- defN 23-May-25 16:56 neon_enclosure/service.py
--rw-r--r--  2.0 unx     1832 b- defN 23-May-25 16:56 neon_enclosure/admin/__init__.py
--rw-r--r--  2.0 unx     2839 b- defN 23-May-25 16:56 neon_enclosure/admin/__main__.py
--rw-r--r--  2.0 unx     2406 b- defN 23-May-25 16:56 neon_enclosure/admin/service.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-25 16:56 neon_enclosure-1.4.3a2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2702 b- defN 23-May-25 16:56 neon_enclosure-1.4.3a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 16:56 neon_enclosure-1.4.3a2.dist-info/WHEEL
--rw-r--r--  2.0 unx      126 b- defN 23-May-25 16:56 neon_enclosure-1.4.3a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-May-25 16:56 neon_enclosure-1.4.3a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1131 b- defN 23-May-25 16:56 neon_enclosure-1.4.3a2.dist-info/RECORD
-13 files, 24252 bytes uncompressed, 11909 bytes compressed:  50.9%
+Zip file size: 13786 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1831 b- defN 23-May-26 23:48 neon_enclosure/__init__.py
+-rw-r--r--  2.0 unx     2832 b- defN 23-May-26 23:48 neon_enclosure/__main__.py
+-rw-r--r--  2.0 unx     3152 b- defN 23-May-26 23:48 neon_enclosure/cli.py
+-rw-r--r--  2.0 unx     3660 b- defN 23-May-26 23:48 neon_enclosure/service.py
+-rw-r--r--  2.0 unx     1832 b- defN 23-May-26 23:48 neon_enclosure/admin/__init__.py
+-rw-r--r--  2.0 unx     2839 b- defN 23-May-26 23:48 neon_enclosure/admin/__main__.py
+-rw-r--r--  2.0 unx     2406 b- defN 23-May-26 23:48 neon_enclosure/admin/service.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-26 23:48 neon_enclosure-1.5.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2695 b- defN 23-May-26 23:48 neon_enclosure-1.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 23:48 neon_enclosure-1.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      127 b- defN 23-May-26 23:48 neon_enclosure-1.5.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-May-26 23:48 neon_enclosure-1.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1119 b- defN 23-May-26 23:49 neon_enclosure-1.5.0.dist-info/RECORD
+13 files, 24234 bytes uncompressed, 11902 bytes compressed:  50.9%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: neon_enclosure/admin/__main__.py
 Comment: 
 
 Filename: neon_enclosure/admin/service.py
 Comment: 
 
-Filename: neon_enclosure-1.4.3a2.dist-info/LICENSE.md
+Filename: neon_enclosure-1.5.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_enclosure-1.4.3a2.dist-info/METADATA
+Filename: neon_enclosure-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: neon_enclosure-1.4.3a2.dist-info/WHEEL
+Filename: neon_enclosure-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: neon_enclosure-1.4.3a2.dist-info/entry_points.txt
+Filename: neon_enclosure-1.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_enclosure-1.4.3a2.dist-info/top_level.txt
+Filename: neon_enclosure-1.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_enclosure-1.4.3a2.dist-info/RECORD
+Filename: neon_enclosure-1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `neon_enclosure-1.4.3a2.dist-info/LICENSE.md` & `neon_enclosure-1.5.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_enclosure-1.4.3a2.dist-info/METADATA` & `neon_enclosure-1.5.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.4.3a2
+Version: 1.5.0
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
 Requires-Dist: ovos-PHAL (~=0.0.4)
 Requires-Dist: neon-utils[network] (~=1.3)
 Requires-Dist: ovos-utils[extras] (~=0.0.32)
 Requires-Dist: ovos-bus-client (~=0.0.3)
 Requires-Dist: ovos-backend-client (~=0.0.6)
 Provides-Extra: docker
 Requires-Dist: ovos-phal-plugin-homeassistant (~=0.0.1) ; extra == 'docker'
@@ -51,7 +51,9 @@
 -e PULSE_SERVER=unix:${XDG_RUNTIME_DIR}/pulse/native \
 -e PULSE_COOKIE=/home/neon/.config/pulse/cookie \
 neon_enclosure
 ```
 
 >*Note:* The above example assumes Docker data is stored in the standard user locations `~/.local/share` and `~/.config`.
 > You may want to change these values to some other path to separate container and host system data.
+
+
```

## Comparing `neon_enclosure-1.4.3a2.dist-info/RECORD` & `neon_enclosure-1.5.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 neon_enclosure/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
 neon_enclosure/__main__.py,sha256=v0iXqgiP-OXIHMoReuZ3v_3cCm7SVKsvlEyobaldfv0,2832
 neon_enclosure/cli.py,sha256=hrt0DltcdUypm-g08OFDG8ojbMXSANkgRw1OAVk_10g,3152
 neon_enclosure/service.py,sha256=ntd4ky4nfdtDEkWEKn8wRJkrqQFX1_N9l0HDXQwDcfI,3660
 neon_enclosure/admin/__init__.py,sha256=FCW9FTGwZxZm9BbxptD2ri02MXw5mq0YtuIfJ0Rm0SA,1832
 neon_enclosure/admin/__main__.py,sha256=bMiOyKwsqEyqXlgOSiy64lT1pqCw7hq5pvrTUXGVZdE,2839
 neon_enclosure/admin/service.py,sha256=UrD0RLVFi-27A0wnFFfQjVlmo-GHWxEyma1Q0W8TLqE,2406
-neon_enclosure-1.4.3a2.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_enclosure-1.4.3a2.dist-info/METADATA,sha256=exB9f5HzPBmZO-LAvwcEK82GvFOu7h0eYB2qPQViNQ0,2702
-neon_enclosure-1.4.3a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_enclosure-1.4.3a2.dist-info/entry_points.txt,sha256=xIujp8DylZvh005eOZ7canZhQr2JdIepZhoV2SXRnEI,126
-neon_enclosure-1.4.3a2.dist-info/top_level.txt,sha256=JyzbDWcL_LA7RBt9baW_93Ep9FDpe-ukXCsowuQm2Ug,15
-neon_enclosure-1.4.3a2.dist-info/RECORD,,
+neon_enclosure-1.5.0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_enclosure-1.5.0.dist-info/METADATA,sha256=lkr-sTgG_zSqGRAx5KJOohphZDjTTyRmdyDO5_4_ysc,2695
+neon_enclosure-1.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_enclosure-1.5.0.dist-info/entry_points.txt,sha256=6Jj4lPTnz0a89img-7ynoJRUxlX7ye2o4hPVmwhC_hc,127
+neon_enclosure-1.5.0.dist-info/top_level.txt,sha256=JyzbDWcL_LA7RBt9baW_93Ep9FDpe-ukXCsowuQm2Ug,15
+neon_enclosure-1.5.0.dist-info/RECORD,,
```

