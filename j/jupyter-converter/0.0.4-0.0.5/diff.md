# Comparing `tmp/jupyter_converter-0.0.4-py3-none-any.whl.zip` & `tmp/jupyter_converter-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9087 bytes, number of entries: 10
+Zip file size: 11008 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       21 b- defN 23-May-27 19:33 jupyter-converter/__init__.py
 -rw-r--r--  2.0 unx     8663 b- defN 23-May-27 19:29 jupyter-converter/cells.py
 -rw-r--r--  2.0 unx     3400 b- defN 23-May-27 19:29 jupyter-converter/converter.py
--rw-r--r--  2.0 unx       99 b- defN 23-May-27 19:55 jupyter_converter/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 23-May-27 19:59 jupyter_converter/__init__.py
 -rw-r--r--  2.0 unx     8663 b- defN 23-May-27 19:29 jupyter_converter/cells.py
--rw-r--r--  2.0 unx     3400 b- defN 23-May-27 19:29 jupyter_converter/converter.py
--rw-r--r--  2.0 unx      519 b- defN 23-May-27 19:56 jupyter_converter-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-27 19:56 jupyter_converter-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-May-27 19:56 jupyter_converter-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      845 b- defN 23-May-27 19:56 jupyter_converter-0.0.4.dist-info/RECORD
-10 files, 25720 bytes uncompressed, 7629 bytes compressed:  70.3%
+-rw-r--r--  2.0 unx    12015 b- defN 23-May-27 19:58 jupyter_converter/converter.py
+-rw-r--r--  2.0 unx      519 b- defN 23-May-27 19:59 jupyter_converter-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-27 19:59 jupyter_converter-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-May-27 19:59 jupyter_converter-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      846 b- defN 23-May-27 19:59 jupyter_converter-0.0.5.dist-info/RECORD
+10 files, 34282 bytes uncompressed, 9550 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: jupyter_converter/cells.py
 Comment: 
 
 Filename: jupyter_converter/converter.py
 Comment: 
 
-Filename: jupyter_converter-0.0.4.dist-info/METADATA
+Filename: jupyter_converter-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: jupyter_converter-0.0.4.dist-info/WHEEL
+Filename: jupyter_converter-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: jupyter_converter-0.0.4.dist-info/top_level.txt
+Filename: jupyter_converter-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: jupyter_converter-0.0.4.dist-info/RECORD
+Filename: jupyter_converter-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jupyter_converter/__init__.py

```diff
@@ -1,5 +1,2 @@
-__version__ = '0.0.4'
-__all__ = ["cells", "converter"]
-
-from . import cells
-from . import converter
+__version__ = '0.0.5'
+__all__ = ["converter"]
```

## jupyter_converter/converter.py

```diff
@@ -1,12 +1,231 @@
 import os
 import copy
 import codecs
 import json
-from cells import Cell
+
+
+# 코드 입력 문구 (코드를 삭제하고 출력을 박제하는 Cell)
+code_input_msgs = [
+    '# 코드입력',
+    '# 코드를 입력하세요.',
+    '# 코드를 입력해 주세요',
+]
+
+# 검증코드 (출력 값을 삭제하지 않음)
+validation_msgs =  [
+    '# 검증코드',
+    '# 코드 검증',
+    '# 코드검증',
+]
+
+option_msgs = {
+    'code': code_input_msgs, 
+    'validation': validation_msgs,
+}
+
+css_table_align_left = [
+    'div.output_area .rendered_html table {\n',
+    '   margin-left: 0;\n',
+    '   margin-right: 0;\n',
+    '}\n'
+]
+
+fixed_code_input_text = '# ▼ 코드를 입력해 주세요 ▼ #'
+
+class Cell():
+    def __init__(self, json_obj, option_msgs=option_msgs, remain_code=False, add_solution=False, use_fixed_code_input_text=True, clear_cell_output=True):
+        """
+        json_obj: ipynb json Object
+        option_msgs: # 코드입력, # 코드검증과 같은 메시지
+        remain_code: # 코드입력 Cell 의 코드 삭제 여부. True: 유지, False: 삭제. 기본값: False
+        add_solution: 정답지 출력을 마크다운 셀로 추가 생성
+        use_fixed_code_input_text: 고정된 코드를 입력해 주세요 문구 출력 여부. True: 고정 문구 출력, False: 첫 문장을 문구로 출력
+        clear_cell_output: 모든 셀의 출력 값을 Clear 여부. 기본값: True(초기화)        
+        """
+        self.json_obj = json_obj
+        
+        # cell_type: 'code' or 'markdown'
+        self.cell_type = json_obj['cell_type']
+        
+        # 코드입력 / 검증코드 문구
+        self.option_msgs = option_msgs
+        
+        # input_type: None, 'code', 'validation'
+        self.input_type = None
+        
+        # 코드입력 Cell 의 코드 삭제 여부
+        self.remain_code = remain_code
+        
+        # 출력(output) 존재 여부
+        self.outputs = None
+        
+        # 정답 코드
+        self.answer_code = None
+        
+        # 정답지 표기 여부
+        self.add_solution = add_solution
+        
+        # 코드를 입력해 주세요 고정 문구 활용 여부
+        self.use_fixed_code_input_text = use_fixed_code_input_text
+        
+        # 일반 Cell의 출력 초기화
+        self.clear_cell_output = clear_cell_output
+        
+        # 초기화 진행
+        self.initialize()
+        
+    def initialize(self):
+        if 'execution_count' in self.json_obj:
+            self.json_obj['execution_count'] = None
+        
+        msg_idx = 0
+        
+        # Source 코드가 존재하는 경우
+        if 'source' in self.json_obj:
+            for i, source in enumerate(self.json_obj['source']):
+                for msg in self.option_msgs['code']:
+                    if msg in source:
+                        self.input_type = 'code'
+                        msg_idx = i
+                        break
+                    
+                for msg in self.option_msgs['validation']:
+                    if msg in source:
+                        self.input_type = 'validation'
+                        break
+                    
+        # 코드 입력창 초기화 처리
+        if self.input_type == 'validation' and 'outputs' in self.json_obj:
+            pass
+        
+        elif self.input_type == 'code' and 'source' in self.json_obj:
+            # '코드입력' or '코드를 입력해 주세요' 문구 등의 처리
+            code_input_header = self.json_obj['source'][msg_idx]
+            
+            # 정답을 추가하여 출력 생성하는 경우
+            if self.add_solution:
+                answer_code = copy.deepcopy(self.json_obj['source'])
+                answer_code.pop(msg_idx)
+                self.answer_code = answer_code
+                    
+            
+            if self.remain_code == False:
+                self.json_obj['source'].clear()
+                
+                if self.use_fixed_code_input_text:
+                    self.json_obj['source'].append(fixed_code_input_text)
+                else:
+                    self.json_obj['source'].append(code_input_header)
+                self.json_obj['source'].append('\n')
+            else:
+                if self.use_fixed_code_input_text:
+                    self.json_obj['source'][0] = fixed_code_input_text + '\n'
+            
+        elif 'outputs' in self.json_obj and self.clear_cell_output:
+            self.json_obj['outputs'].clear()
+            
+        # 출력창 처리
+        if self.input_type == 'code' and 'outputs' in self.json_obj and len(self.json_obj['outputs']) > 0:
+            if 'data' in self.json_obj['outputs'][0]:
+                # Series, DataFrame 출력
+                # data = self.json_obj['outputs'][0]['data']
+                for output_ in self.json_obj['outputs']:
+                    data = output_['data']
+                    if 'text/html' in data:
+                        # DataFrame 출력
+                        html = data['text/html']
+                        html.insert(0, '<p><strong>[출력 결과]</strong></p>')
+                        replaced_html = []
+                        for row in html:
+                            row = row.replace(r'<div>', r'<div class="output_subarea output_html rendered_html output_result">')
+                            row = row.replace(r'class="dataframe"', r'class="dataframe" style="margin-left: 0; margin-right: 0;"')
+                            replaced_html.append(row)
+                        
+                        self.outputs = replaced_html
+                        # break
+                        
+                    elif 'text/plain' in data:
+                        # print('test/plain FOUND!!')
+                        # Plain TEXT 출력
+                        plain_text = data['text/plain']
+                        if len(plain_text) > 0 and plain_text[0].startswith('<Figure'):
+                            self.outputs = None
+                            # continue
+                        else:
+                            plain_text[0] = '<pre>' + plain_text[0]
+                            plain_text[len(plain_text)-1] = plain_text[len(plain_text)-1] + '</pre>'
+                            plain_text.insert(0, '<p><strong>[출력 결과]</strong></p>')
+                            self.outputs = plain_text
+                            
+                    if 'image/png' in data:
+                        # print('IMAGE FOUND!!')
+                        # pyplot 그래프
+                        plain_image = data['image/png']
+                        plain_image = '<img style="margin-left: 0; margin-right: 0;" src="data:image/png;base64,' + plain_image.replace('\n','') + '"/>'
+                        self.outputs = []
+                        self.outputs.insert(0, '<p><strong>[출력 결과]</strong></p>')
+                        self.outputs.append(plain_image)
+                        break
+                    
+            elif 'text' in self.json_obj['outputs'][0]:
+                # Series 형태의 TEXT output
+                text = self.json_obj['outputs'][0]['text']
+                if len(text) > 0 and text[0].startswith('<Figure'):
+                    self.outputs = None
+                else:
+                    text[0] = '<pre>' + text[0]
+                    text[len(text)-1] = text[len(text)-1] + '</pre>'
+                    text.insert(0, '<p><strong>[출력 결과]</strong></p>')
+                    self.outputs = text
+    
+    def create_answer_output(self):
+        if self.answer_code is not None:
+            answer_output = [
+                '<details>\n',
+                '<summary>\n',
+                '<b>▼ [정답 확인] ▼</b>\n',
+                '</summary>\n',
+                '<div class="markdown">\n',
+                '<span><pre><code>',
+                # import pandas as pd
+
+            # pd.read_csv('data.csv')
+                
+            ]
+            answer_output.extend(self.answer_code)
+            answer_output.append('\n</code></pre></span></div></details>\n',)
+            return answer_output
+        else:
+            return None
+        
+    def get_type(self):
+        return self.cell_type
+    
+    def get_input_type(self):
+        return self.input_type
+    
+    def get(self, tag):
+        if tag in self.json_obj:
+            return self.json_obj[tag]
+        else:
+            return None
+        
+    def set(self, tag, value):
+        if tag in self.json_obj:
+            self.json_obj[tag] = value
+            return True
+        else:
+            return False
+        
+    def keys(self):
+        return self.json_obj.keys()
+    
+    def __call__(self):
+        return self.json_obj
 
 
 def convert_notebook(src_file, tgt_file=None, post_fix='-(변환).ipynb', folder_path='실습', remain_code=False, add_solution=False):
     if add_solution:
         post_fix = post_fix[:-6] + '-(정답추가)' + '.ipynb'
         
     if remain_code:
```

## Comparing `jupyter_converter-0.0.4.dist-info/METADATA` & `jupyter_converter-0.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-converter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Jupyter Notebook exam generator written by TeddyNote
 Home-page: https://github.com/teddylee777
 Author: teddylee777
 Author-email: teddylee777@gmail.com
 Keywords: teddynote,teddylee777,jupyter notebook converter,exam generator
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `jupyter_converter-0.0.4.dist-info/RECORD` & `jupyter_converter-0.0.5.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 jupyter-converter/__init__.py,sha256=07NzQXBgNlnw5kSN6ZYxE9By-_RuH3Jyy58Z74sIio0,21
 jupyter-converter/cells.py,sha256=swa3-i205cvPIcnZj0HSXYKDdMSeryxVjSMbxScYGJs,8663
 jupyter-converter/converter.py,sha256=hAOFIQrRB_jOsBCS9YeioQUtpwBvcNEXgikkCe0ete8,3400
-jupyter_converter/__init__.py,sha256=6Z015FrqN4GdIgDIA7QADWHOhSVFbe3A4GAS4f6UBwA,99
+jupyter_converter/__init__.py,sha256=l6ThgMGVhn-rIUhEVFiZYE8RJKKqHwBMUJv5q1GOCEg,45
 jupyter_converter/cells.py,sha256=swa3-i205cvPIcnZj0HSXYKDdMSeryxVjSMbxScYGJs,8663
-jupyter_converter/converter.py,sha256=hAOFIQrRB_jOsBCS9YeioQUtpwBvcNEXgikkCe0ete8,3400
-jupyter_converter-0.0.4.dist-info/METADATA,sha256=e_Z8joezRjAM22KCCqAAZ8rwLZRyMr_-62BmR-Jk3gc,519
-jupyter_converter-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-jupyter_converter-0.0.4.dist-info/top_level.txt,sha256=mF9jQPCYgLEtCGesnHuO-eP1XKlbsIk-4qLtEF2CpE4,18
-jupyter_converter-0.0.4.dist-info/RECORD,,
+jupyter_converter/converter.py,sha256=5pqIJ8x3nEkPxyEyKZBaG1qfz0z9gE-GCGxF6XZOhyg,12015
+jupyter_converter-0.0.5.dist-info/METADATA,sha256=eJJ4w8vEw-dzYNhDGc50TZBNh15zVozhzwgPFEhOmyY,519
+jupyter_converter-0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+jupyter_converter-0.0.5.dist-info/top_level.txt,sha256=mF9jQPCYgLEtCGesnHuO-eP1XKlbsIk-4qLtEF2CpE4,18
+jupyter_converter-0.0.5.dist-info/RECORD,,
```

