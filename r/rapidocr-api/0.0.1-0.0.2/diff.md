# Comparing `tmp/rapidocr_api-0.0.1-py3-none-any.whl.zip` & `tmp/rapidocr_api-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4228 bytes, number of entries: 7
--rw-r--r--  2.0 unx       74 b- defN 23-May-22 00:55 rapidocr_api/__init__.py
--rw-r--r--  2.0 unx     2082 b- defN 23-May-22 00:55 rapidocr_api/api.py
--rw-r--r--  2.0 unx     4563 b- defN 23-May-22 00:56 rapidocr_api-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 00:56 rapidocr_api-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 23-May-22 00:56 rapidocr_api-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 00:56 rapidocr_api-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      573 b- defN 23-May-22 00:56 rapidocr_api-0.0.1.dist-info/RECORD
-7 files, 7453 bytes uncompressed, 3202 bytes compressed:  57.0%
+Zip file size: 4222 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       74 b- defN 23-May-27 01:02 rapidocr_api/__init__.py
+-rw-r--r--  2.0 unx     2082 b- defN 23-May-27 01:02 rapidocr_api/api.py
+-rw-r--r--  2.0 unx     4553 b- defN 23-May-27 01:03 rapidocr_api-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-27 01:03 rapidocr_api-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 23-May-27 01:03 rapidocr_api-0.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-May-27 01:03 rapidocr_api-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      573 b- defN 23-May-27 01:03 rapidocr_api-0.0.2.dist-info/RECORD
+7 files, 7443 bytes uncompressed, 3196 bytes compressed:  57.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: rapidocr_api/__init__.py
 Comment: 
 
 Filename: rapidocr_api/api.py
 Comment: 
 
-Filename: rapidocr_api-0.0.1.dist-info/METADATA
+Filename: rapidocr_api-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: rapidocr_api-0.0.1.dist-info/WHEEL
+Filename: rapidocr_api-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: rapidocr_api-0.0.1.dist-info/entry_points.txt
+Filename: rapidocr_api-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapidocr_api-0.0.1.dist-info/top_level.txt
+Filename: rapidocr_api-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: rapidocr_api-0.0.1.dist-info/RECORD
+Filename: rapidocr_api-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rapidocr_api-0.0.1.dist-info/METADATA` & `rapidocr_api-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidocr-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: A cross platform OCR API Library based on OnnxRuntime.
 Home-page: https://github.com/RapidAI/RapidOCR
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Download-URL: https://github.com/RapidAI/RapidOCR.git
 Keywords: ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
@@ -25,17 +25,17 @@
     <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
     <a href="https://pypi.org/project/rapidocr-api/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rapidocr-api"></a>
     <a href="https://pepy.tech/project/rapidocr_api"><img src="https://static.pepy.tech/personalized-badge/rapidocr_api?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
 </p>
 
 ### Use
-1. Install`rapidocr_web[api]`
+1. Install`rapidocr_api`
    ```bash
-   $ pip install rapidocr_web[api]
+   $ pip install rapidocr_api
    ```
 2. Run
    - Usage:
        ```bash
        $ rapidocr_api -h
        usage: rapidocr_api [-h] [-ip IP] [-p PORT]
```

### html2text {}

```diff
@@ -1,42 +1,42 @@
-Metadata-Version: 2.1 Name: rapidocr-api Version: 0.0.1 Summary: A cross
+Metadata-Version: 2.1 Name: rapidocr-api Version: 0.0.2 Summary: A cross
 platform OCR API Library based on OnnxRuntime. Home-page: https://github.com/
 RapidAI/RapidOCR Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Download-URL: https://github.com/RapidAI/RapidOCR.git Keywords:
 ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
 Platform: Any Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
 Python: >=3.7,<=3.10 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: rapidocr-onnxruntime Requires-Dist: fastapi Requires-
 Dist: uvicorn[standard] ## rapidocr-api
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
 static.pepy.tech/personalized-badge/
 rapidocr_api?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
-### Use 1. Install`rapidocr_web[api]` ```bash $ pip install rapidocr_web[api]
-``` 2. Run - Usage: ```bash $ rapidocr_api -h usage: rapidocr_api [-h] [-ip IP]
-[-p PORT] optional arguments: -h, --help show this help message and exit -ip
-IP, --ip IP IP Address -p PORT, --port PORT IP port ``` - Example: ```bash $
-rapidocr_api -ip 0.0.0.0 -p 9003 ``` 3. Use - with curl ```bash $ curl -
-F image_file=@1.png http://0.0.0.0:9003/ocr ``` - with python - Send image data
-by file format. ```python import requests url = 'http://localhost:9003/ocr'
-img_path = '../python/tests/test_files/ch_en_num.jpg' with open(img_path, 'rb')
-as f: file_dict = {'image_file': (img_path, f, 'image/png')} response =
-requests.post(url, files=file_dict, timeout=60) print(response.json()) ``` -
-Send image data by base64 format. ```python import base64 import requests url =
-'http://localhost:9003/ocr' img_path = '../python/tests/test_files/
-ch_en_num.jpg' with open(img_path, 'rb') as fa: img_str = base64.b64encode
-(fa.read()) payload = {'image_data': img_str} resp = requests.post(url,
-data=payload) print(resp.json()) ``` 4. Output  Click to expand ```json { "0":
-{ "rec_txt": "é¦æ¸¯æ·±å³æ½è¡ï¼", "dt_boxes": [ [265, 18], [472, 231],
-[431, 271], [223, 59] ], "score": "0.8175641223788261" }, "1": { "rec_txt":
-"ä¸ä¸æ¥æ§å«", "dt_boxes": [ [388, 15], [636, 257], [587, 307], [339, 65]
-], "score": "0.8293875356515249" }, "2": { "rec_txt": "ä¸ä¸é´å®Bè¶å",
-"dt_boxes": [ [215, 84], [509, 413], [453, 463], [159, 134] ], "score":
-"0.8626169338822365" }, "3": { "rec_txt": "bè¶ä»ªå¨æ¥æ§å«", "dt_boxes": [
-[128, 135], [430, 478], [366, 534], [64, 192] ], "score": "0.8449362441897392"
-}, "4": { "rec_txt": "å å¾®ä¿¡eee", "dt_boxes": [ [58, 189], [268, 450], [209,
-498], [0, 236] ], "score": "0.8176911813872201" }, "5": { "rec_txt":
-"å¯é®å¯", "dt_boxes": [ [493, 261], [617, 384], [577, 423], [454, 300] ],
-"score": "0.7494261413812637" } } ```  ### See details for [RapidOCR](https://
+### Use 1. Install`rapidocr_api` ```bash $ pip install rapidocr_api ``` 2. Run
+- Usage: ```bash $ rapidocr_api -h usage: rapidocr_api [-h] [-ip IP] [-p PORT]
+optional arguments: -h, --help show this help message and exit -ip IP, --ip IP
+IP Address -p PORT, --port PORT IP port ``` - Example: ```bash $ rapidocr_api -
+ip 0.0.0.0 -p 9003 ``` 3. Use - with curl ```bash $ curl -F image_file=@1.png
+http://0.0.0.0:9003/ocr ``` - with python - Send image data by file format.
+```python import requests url = 'http://localhost:9003/ocr' img_path = '../
+python/tests/test_files/ch_en_num.jpg' with open(img_path, 'rb') as f:
+file_dict = {'image_file': (img_path, f, 'image/png')} response = requests.post
+(url, files=file_dict, timeout=60) print(response.json()) ``` - Send image data
+by base64 format. ```python import base64 import requests url = 'http://
+localhost:9003/ocr' img_path = '../python/tests/test_files/ch_en_num.jpg' with
+open(img_path, 'rb') as fa: img_str = base64.b64encode(fa.read()) payload =
+{'image_data': img_str} resp = requests.post(url, data=payload) print(resp.json
+()) ``` 4. Output  Click to expand ```json { "0": { "rec_txt":
+"é¦æ¸¯æ·±å³æ½è¡ï¼", "dt_boxes": [ [265, 18], [472, 231], [431, 271], [223,
+59] ], "score": "0.8175641223788261" }, "1": { "rec_txt": "ä¸ä¸æ¥æ§å«",
+"dt_boxes": [ [388, 15], [636, 257], [587, 307], [339, 65] ], "score":
+"0.8293875356515249" }, "2": { "rec_txt": "ä¸ä¸é´å®Bè¶å", "dt_boxes": [
+[215, 84], [509, 413], [453, 463], [159, 134] ], "score": "0.8626169338822365"
+}, "3": { "rec_txt": "bè¶ä»ªå¨æ¥æ§å«", "dt_boxes": [ [128, 135], [430,
+478], [366, 534], [64, 192] ], "score": "0.8449362441897392" }, "4":
+{ "rec_txt": "å å¾®ä¿¡eee", "dt_boxes": [ [58, 189], [268, 450], [209, 498],
+[0, 236] ], "score": "0.8176911813872201" }, "5": { "rec_txt": "å¯é®å¯",
+"dt_boxes": [ [493, 261], [617, 384], [577, 423], [454, 300] ], "score":
+"0.7494261413812637" } } ```  ### See details for [RapidOCR](https://
 github.com/RapidAI/RapidOCR/tree/main/ocrweb).
```

