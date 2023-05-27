# Comparing `tmp/varwizard-0.2.1.tar.gz` & `tmp/varwizard-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varwizard-0.2.1.tar", max compression
+gzip compressed data, was "varwizard-0.2.2.tar", max compression
```

## Comparing `varwizard-0.2.1.tar` & `varwizard-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      748 2023-05-25 12:00:28.451723 varwizard-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2048 2023-05-25 12:55:16.830778 varwizard-0.2.1/readme.md
--rw-r--r--   0        0        0       84 2023-05-25 12:30:46.711987 varwizard-0.2.1/varwizard/__init__.py
--rw-r--r--   0        0        0       59 2023-05-17 04:28:27.343893 varwizard-0.2.1/varwizard/__main__.py
--rw-r--r--   0        0        0     1675 2023-05-25 12:31:15.324437 varwizard-0.2.1/varwizard/cli.py
--rw-r--r--   0        0        0       51 2023-05-12 16:52:19.678029 varwizard-0.2.1/varwizard/config/__init__.py
--rw-r--r--   0        0        0      777 2023-05-25 12:36:46.261554 varwizard-0.2.1/varwizard/config/prefix_tuning.py
--rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2.1/varwizard/data/__init__.py
--rw-r--r--   0        0        0     3250 2023-05-25 12:39:09.295726 varwizard-0.2.1/varwizard/data/input_preparation.py
--rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2.1/varwizard/generation/__init__.py
--rw-r--r--   0        0        0     1305 2023-05-25 12:52:49.844575 varwizard-0.2.1/varwizard/generation/gen.py
--rw-r--r--   0        0        0   401536 2023-05-11 10:13:40.998948 varwizard-0.2.1/varwizard/libs/tree-sitter/c.so
--rw-r--r--   0        0        0  4076856 2023-05-11 10:13:41.242952 varwizard-0.2.1/varwizard/libs/tree-sitter/c_sharp.so
--rw-r--r--   0        0        0  2300056 2023-05-11 10:13:41.446956 varwizard-0.2.1/varwizard/libs/tree-sitter/cpp.so
--rw-r--r--   0        0        0   246152 2023-05-11 10:13:41.190951 varwizard-0.2.1/varwizard/libs/tree-sitter/go.so
--rw-r--r--   0        0        0   401704 2023-05-11 10:13:41.494956 varwizard-0.2.1/varwizard/libs/tree-sitter/java.so
--rw-r--r--   0        0        0   354200 2023-05-11 10:13:41.458956 varwizard-0.2.1/varwizard/libs/tree-sitter/javascript.so
--rw-r--r--   0        0        0   785016 2023-05-11 10:13:41.490956 varwizard-0.2.1/varwizard/libs/tree-sitter/php.so
--rw-r--r--   0        0        0   494864 2023-05-11 10:13:41.470956 varwizard-0.2.1/varwizard/libs/tree-sitter/python.so
--rw-r--r--   0        0        0  2130104 2023-05-11 10:13:41.090950 varwizard-0.2.1/varwizard/libs/tree-sitter/ruby.so
--rw-r--r--   0        0        0   849608 2023-05-11 10:13:41.238952 varwizard-0.2.1/varwizard/libs/tree-sitter/rust.so
--rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2.1/varwizard/models/__init__.py
--rw-r--r--   0        0        0      252 2023-05-11 10:13:41.090950 varwizard-0.2.1/varwizard/models/bloom.py
--rw-r--r--   0        0        0      261 2023-05-25 12:32:09.249284 varwizard-0.2.1/varwizard/models/codet5.py
--rw-r--r--   0        0        0     2795 2023-05-25 12:42:39.214988 varwizard-0.2.1/varwizard/models/varwizard.py
--rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2.1/varwizard/utils/__init__.py
--rw-r--r--   0        0        0    13556 2023-05-11 10:13:41.086950 varwizard-0.2.1/varwizard/utils/obfuscation.py
--rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 varwizard-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      748 2023-05-27 14:15:20.820183 varwizard-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2146 2023-05-27 18:09:39.864430 varwizard-0.2.2/readme.md
+-rw-r--r--   0        0        0       84 2023-05-27 14:15:32.832370 varwizard-0.2.2/varwizard/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-17 04:28:27.343893 varwizard-0.2.2/varwizard/__main__.py
+-rw-r--r--   0        0        0     1675 2023-05-25 12:31:15.324437 varwizard-0.2.2/varwizard/cli.py
+-rw-r--r--   0        0        0       51 2023-05-12 16:52:19.678029 varwizard-0.2.2/varwizard/config/__init__.py
+-rw-r--r--   0        0        0      777 2023-05-25 12:36:46.261554 varwizard-0.2.2/varwizard/config/prefix_tuning.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2.2/varwizard/data/__init__.py
+-rw-r--r--   0        0        0     4333 2023-05-27 17:41:16.101777 varwizard-0.2.2/varwizard/data/input_preparation.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2.2/varwizard/generation/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-27 18:07:37.166515 varwizard-0.2.2/varwizard/generation/gen.py
+-rw-r--r--   0        0        0   401536 2023-05-11 10:13:40.998948 varwizard-0.2.2/varwizard/libs/tree-sitter/c.so
+-rw-r--r--   0        0        0  4076856 2023-05-11 10:13:41.242952 varwizard-0.2.2/varwizard/libs/tree-sitter/c_sharp.so
+-rw-r--r--   0        0        0  2300056 2023-05-11 10:13:41.446956 varwizard-0.2.2/varwizard/libs/tree-sitter/cpp.so
+-rw-r--r--   0        0        0   246152 2023-05-11 10:13:41.190951 varwizard-0.2.2/varwizard/libs/tree-sitter/go.so
+-rw-r--r--   0        0        0   401704 2023-05-11 10:13:41.494956 varwizard-0.2.2/varwizard/libs/tree-sitter/java.so
+-rw-r--r--   0        0        0   354200 2023-05-11 10:13:41.458956 varwizard-0.2.2/varwizard/libs/tree-sitter/javascript.so
+-rw-r--r--   0        0        0   785016 2023-05-11 10:13:41.490956 varwizard-0.2.2/varwizard/libs/tree-sitter/php.so
+-rw-r--r--   0        0        0   494864 2023-05-11 10:13:41.470956 varwizard-0.2.2/varwizard/libs/tree-sitter/python.so
+-rw-r--r--   0        0        0  2130104 2023-05-11 10:13:41.090950 varwizard-0.2.2/varwizard/libs/tree-sitter/ruby.so
+-rw-r--r--   0        0        0   849608 2023-05-11 10:13:41.238952 varwizard-0.2.2/varwizard/libs/tree-sitter/rust.so
+-rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2.2/varwizard/models/__init__.py
+-rw-r--r--   0        0        0      252 2023-05-11 10:13:41.090950 varwizard-0.2.2/varwizard/models/bloom.py
+-rw-r--r--   0        0        0      261 2023-05-25 12:32:09.249284 varwizard-0.2.2/varwizard/models/codet5.py
+-rw-r--r--   0        0        0     2917 2023-05-27 17:04:49.895477 varwizard-0.2.2/varwizard/models/varwizard.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2.2/varwizard/utils/__init__.py
+-rw-r--r--   0        0        0    13557 2023-05-27 17:12:30.262652 varwizard-0.2.2/varwizard/utils/obfuscation.py
+-rw-r--r--   0        0        0     3142 1970-01-01 00:00:00.000000 varwizard-0.2.2/PKG-INFO
```

### Comparing `varwizard-0.2.1/pyproject.toml` & `varwizard-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=60",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 [tool.poetry]
 name="varwizard"
-version="0.2.1"
+version="0.2.2"
 license = "Apache-2.0"
 description = "An Automated Tool for Improving Code Quality Through Variable Name Refinement with Language Models"
 readme = "readme.md"
 homepage = "https://github.com/FSoft-AI4Code/VarWizard"
 repository = "https://github.com/FSoft-AI4Code/VarWizard"
 keywords = ["variable renaming", "language models", "code quality"]
 authors = ["FSoft-AI4Code <support.aic@fpt.com>"]
```

### Comparing `varwizard-0.2.1/varwizard/cli.py` & `varwizard-0.2.2/varwizard/cli.py`

 * *Files identical despite different names*

### Comparing `varwizard-0.2.1/varwizard/config/prefix_tuning.py` & `varwizard-0.2.2/varwizard/config/prefix_tuning.py`

 * *Files identical despite different names*

### Comparing `varwizard-0.2.1/varwizard/data/input_preparation.py` & `varwizard-0.2.2/varwizard/data/input_preparation.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,54 +2,74 @@
 from pkg_resources import resource_filename
 import varwizard
 
 from varwizard.utils.obfuscation import *
 
 from codetext.parser import GoParser, PhpParser, RubyParser, JavaParser, JavascriptParser, PythonParser, CppParser, CsharpParser, RustParser
 
-def beautify(function_root, function_bytes, vmap, new_function_bytes = None, offset = 0):
+def beautify(function_root, function_bytes, vmap, new_function_bytes = None, offset = 0, keyword = 'identifier'):
     if len(function_root.children) == 0:
         node_token = function_bytes[function_root.start_byte: function_root.end_byte].decode()
-        if function_root.type == 'identifier': 
+        if function_root.type == keyword: 
             if node_token in vmap:
                 if new_function_bytes is None:
                     new_function_bytes = function_bytes
                 new_function_bytes = new_function_bytes[:function_root.start_byte + offset] + vmap[node_token].encode() + new_function_bytes[function_root.end_byte + offset:]
                 offset += len(vmap[node_token].encode()) - function_root.end_byte + function_root.start_byte
                 return new_function_bytes, offset
     for child in function_root.children:
-        new_function_bytes, offset = beautify(child, function_bytes, vmap, new_function_bytes, offset)
+        new_function_bytes, offset = beautify(child, function_bytes, vmap, new_function_bytes, offset, keyword)
     return new_function_bytes, offset
 def prepare_input(input, lang, tokenizer, base_model_name, max_input_len: int = 400, prompt = ' Output var0 ='):
     parser = Parser()
     so_path = resource_filename('varwizard', f'libs/tree-sitter/{lang}.so')
     parser.set_language(Language(so_path, lang))
     
     bytes = input.encode()
     root = parser.parse(bytes).root_node
     code_parser = lang.replace('_', '')
+    if code_parser == 'c':
+        code_parser = 'cpp'
     code_parser = code_parser[0].upper() + code_parser[1:] + "Parser"
     code_parser = eval(code_parser)
     function_lst = code_parser.get_function_list(root)
-    for function_node in function_lst:
+    last_start_byte = 0
+    function_node = None
+    num_functions = len(function_lst)
+    assert num_functions > 0, "Not found any functions"
+    keyword = 'name' if lang == 'php' else 'identifier'
+    for fid, function_node in enumerate(function_lst):
         function_bytes = bytes[function_node.start_byte: function_node.end_byte]
-        new_function_bytes = function_bytes[:]
+        if lang == 'java':
+            before_class = 'public class A{\n'.encode()
+            after_class = '\n}'.encode()
+            function_bytes = before_class + function_bytes + after_class
+        elif lang == 'php':
+            before_class = '<?php\n'.encode()
+            after_class = '\n?>'.encode()
+            function_bytes = before_class + function_bytes + after_class
         function_root = parser.parse(function_bytes).root_node
         idens = {'var_num': 0, 'vars': {}}
         idens = eval(f'get_{lang}_var_names')(function_root, function_bytes, idens)
         chosen_vars = [x for x in idens['vars'] if x != x.upper()]
         chosen_ids = list(map(idens['vars'].get, chosen_vars))
         chosen_tup = sorted(list(zip(chosen_vars, chosen_ids)), key = lambda x: x[1])
         vmap = {}
         for i, var_name in enumerate(chosen_tup):
             vmap[var_name[0]] = f'var{i}'
-        new_function_bytes, _ = beautify(function_root, function_bytes, vmap)
+        new_function_bytes, _ = beautify(function_root, function_bytes, vmap, keyword = keyword)
+        if lang in ['java', 'php']:
+            new_function_bytes = new_function_bytes[len(before_class):-len(after_class)]
         function_code = new_function_bytes.decode()
+        # print('new', function_code)
         if 'bloom' in base_model_name:
             source_tokens = tokenizer.tokenize(function_code, truncation = True, max_length = max_input_len)
             prompt_tokens = tokenizer.tokenize(prompt)
             input_tokens = source_tokens + prompt_tokens
             input_ids = [tokenizer.bos_token_id] + tokenizer.convert_tokens_to_ids(input_tokens)
         elif 'codet5' in base_model_name:
             input_tokens = tokenizer.tokenize(function_code, truncation = True, max_length = max_input_len)
             input_ids = [tokenizer.bos_token_id] + tokenizer.convert_tokens_to_ids(input_tokens) + [tokenizer.eos_token_id]
-        yield input_ids, {v: k for k, v in vmap.items()}
+        before_context = bytes[last_start_byte:function_node.start_byte].decode()
+        after_context = bytes[function_node.end_byte:].decode() if fid == num_functions - 1 else None
+        last_start_byte = function_node.end_byte
+        yield input_ids, {v: k for k, v in vmap.items()}, before_context, after_context
```

### Comparing `varwizard-0.2.1/varwizard/generation/gen.py` & `varwizard-0.2.2/varwizard/generation/gen.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,12 +15,13 @@
         start_pos = prediction.find('var0')
         prediction = prediction[start_pos:].replace('</s>', '')
         new_code = tokenizer.decode(input_ids[0]).replace('<s>', '').replace('</s>', '')
     pred_coms = prediction.split()
     new_vmap = {}
     for i in range(len(pred_coms) // 3):
         key, _, value = pred_coms[3 * i: 3 * i + 3]
+        if value.startswith('var') or value.startswith('$var'): continue
         new_vmap[key] = value
     vmap.update(new_vmap)
     for key, value in vmap.items():
         new_code = new_code.replace(key, value)
     return new_code
```

### Comparing `varwizard-0.2.1/varwizard/libs/tree-sitter/c.so` & `varwizard-0.2.2/varwizard/libs/tree-sitter/c.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2.1/varwizard/libs/tree-sitter/c_sharp.so` & `varwizard-0.2.2/varwizard/libs/tree-sitter/c_sharp.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2.1/varwizard/libs/tree-sitter/cpp.so` & `varwizard-0.2.2/varwizard/libs/tree-sitter/cpp.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2.1/varwizard/libs/tree-sitter/go.so` & `varwizard-0.2.2/varwizard/libs/tree-sitter/go.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2.1/varwizard/libs/tree-sitter/java.so` & `varwizard-0.2.2/varwizard/libs/tree-sitter/java.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2.1/varwizard/libs/tree-sitter/javascript.so` & `varwizard-0.2.2/varwizard/libs/tree-sitter/javascript.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2.1/varwizard/libs/tree-sitter/php.so` & `varwizard-0.2.2/varwizard/libs/tree-sitter/php.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2.1/varwizard/libs/tree-sitter/python.so` & `varwizard-0.2.2/varwizard/libs/tree-sitter/python.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2.1/varwizard/libs/tree-sitter/ruby.so` & `varwizard-0.2.2/varwizard/libs/tree-sitter/ruby.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2.1/varwizard/libs/tree-sitter/rust.so` & `varwizard-0.2.2/varwizard/libs/tree-sitter/rust.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2.1/varwizard/models/varwizard.py` & `varwizard-0.2.2/varwizard/models/varwizard.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,21 +43,23 @@
 	@torch.inference_mode()
 	def make_new_code(self, input, lang, output_path = None, max_input_len: int = 400, max_new_tokens: int = 100, penalty_alpha: float = 0.6, top_k: int = 4, device = 'cpu'):
 		if os.path.exists(input):
 			with open(input) as f:
 				input = f.read()
 		input = input.strip()
 		all_predictions = []
-		for input_ids, vmap in self.prepare_input(input, lang, base_model_name = self.base_model_name, max_input_len = max_input_len):
+		for input_ids, vmap, before_context, after_context in self.prepare_input(input, lang, base_model_name = self.base_model_name, max_input_len = max_input_len):
 			input_ids = torch.tensor(input_ids)
 			input_ids = input_ids.to(device)
 			self.model.device = device
 			self.model.to(device)
 			input_ids = input_ids.unsqueeze(0)
 			prediction = self.generate(input_ids, vmap, max_new_tokens = max_new_tokens, penalty_alpha = penalty_alpha, top_k = top_k)
-			all_predictions.append(prediction)
-		prediction = '\n'.join(all_predictions)
+			all_predictions.extend([before_context, prediction])
+			if after_context is not None:
+				all_predictions.append(after_context)
+		prediction = ''.join(all_predictions)
 		if output_path is not None:
 			with open(output_path, 'w') as f:
 				f.write(prediction)
 		return prediction
```

### Comparing `varwizard-0.2.1/varwizard/utils/obfuscation.py` & `varwizard-0.2.2/varwizard/utils/obfuscation.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             idens['var_num'] += 1
         return idens
     for child in children:
         get_c_var_names(child, bytes, idens)
     return idens
 def get_php_var_names(root, bytes, idens = {'var_num': 0, 'vars': {}}, KEYWORDS = ['A', '__CLASS__', '__METHOD__', '__FUNCTION__', 'GLOBAL']):
     children = root.children
-    if root.type == 'method_declaration':
+    if root.type == 'function_definition':
         _children = []
         for child in children:
             if child.type == 'name':
                 node_token = bytes[child.start_byte:child.end_byte].decode()
                 idens['func'] = node_token
             else:
                 _children.append(child)
```

