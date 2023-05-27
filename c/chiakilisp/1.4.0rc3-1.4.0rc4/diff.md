# Comparing `tmp/chiakilisp-1.4.0rc3-py3-none-any.whl.zip` & `tmp/chiakilisp-1.4.0rc4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 26692 bytes, number of entries: 19
+Zip file size: 27071 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 22-May-22 18:38 chiakilisp/__init__.py
 -rw-r--r--  2.0 unx    13791 b- defN 23-May-19 18:36 chiakilisp/lexer.py
 -rw-r--r--  2.0 unx     5943 b- defN 23-May-18 21:24 chiakilisp/parser.py
 -rw-r--r--  2.0 unx     1378 b- defN 23-May-19 18:48 chiakilisp/runtime.py
 -rw-r--r--  2.0 unx    11225 b- defN 23-May-18 22:30 chiakilisp/spec.py
--rw-r--r--  2.0 unx     3311 b- defN 23-May-15 20:31 chiakilisp/utils.py
+-rw-r--r--  2.0 unx     3311 b- defN 23-May-27 10:34 chiakilisp/utils.py
 -rw-r--r--  2.0 unx     7443 b- defN 23-May-23 21:25 chiakilisp/corelib/core.cl
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-13 11:18 chiakilisp/models/__init__.py
--rw-r--r--  2.0 unx    30784 b- defN 23-May-19 18:35 chiakilisp/models/expression.py
+-rw-r--r--  2.0 unx    31381 b- defN 23-May-27 16:44 chiakilisp/models/expression.py
 -rw-r--r--  2.0 unx      790 b- defN 23-May-15 20:31 chiakilisp/models/forward.py
 -rw-r--r--  2.0 unx     3778 b- defN 23-May-15 20:32 chiakilisp/models/literal.py
 -rw-r--r--  2.0 unx     1986 b- defN 23-May-15 20:31 chiakilisp/models/token.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-15 20:31 chiakilisp/proxies/__init__.py
 -rw-r--r--  2.0 unx      205 b- defN 23-May-15 20:31 chiakilisp/proxies/keyword.py
--rwxr-xr-x  2.0 unx    12909 b- defN 23-May-24 12:30 chiakilisp-1.4.0rc3.data/scripts/chiakilang
--rw-r--r--  2.0 unx     1408 b- defN 23-May-24 12:30 chiakilisp-1.4.0rc3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 12:30 chiakilisp-1.4.0rc3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-24 12:30 chiakilisp-1.4.0rc3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1559 b- defN 23-May-24 12:30 chiakilisp-1.4.0rc3.dist-info/RECORD
-19 files, 96613 bytes uncompressed, 24144 bytes compressed:  75.0%
+-rwxr-xr-x  2.0 unx    13359 b- defN 23-May-27 16:47 chiakilisp-1.4.0rc4.data/scripts/chiakilang
+-rw-r--r--  2.0 unx     1408 b- defN 23-May-27 16:47 chiakilisp-1.4.0rc4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-27 16:47 chiakilisp-1.4.0rc4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-27 16:47 chiakilisp-1.4.0rc4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1559 b- defN 23-May-27 16:47 chiakilisp-1.4.0rc4.dist-info/RECORD
+19 files, 97660 bytes uncompressed, 24523 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: chiakilisp/proxies/__init__.py
 Comment: 
 
 Filename: chiakilisp/proxies/keyword.py
 Comment: 
 
-Filename: chiakilisp-1.4.0rc3.data/scripts/chiakilang
+Filename: chiakilisp-1.4.0rc4.data/scripts/chiakilang
 Comment: 
 
-Filename: chiakilisp-1.4.0rc3.dist-info/METADATA
+Filename: chiakilisp-1.4.0rc4.dist-info/METADATA
 Comment: 
 
-Filename: chiakilisp-1.4.0rc3.dist-info/WHEEL
+Filename: chiakilisp-1.4.0rc4.dist-info/WHEEL
 Comment: 
 
-Filename: chiakilisp-1.4.0rc3.dist-info/top_level.txt
+Filename: chiakilisp-1.4.0rc4.dist-info/top_level.txt
 Comment: 
 
-Filename: chiakilisp-1.4.0rc3.dist-info/RECORD
+Filename: chiakilisp-1.4.0rc4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chiakilisp/models/expression.py

```diff
@@ -2,14 +2,16 @@
 # pylint: disable=invalid-name
 # pylint: disable=line-too-long
 # pylint: disable=missing-module-docstring
 # pylint: disable=too-many-locals
 # pylint: disable=arguments-renamed
 # pylint: disable=too-many-branches
 # pylint: disable=too-many-statements
+# pylint: disable=raise-missing-from
+# pylint: disable=unnecessary-dunder-call
 # pylint: disable=too-many-return-statements
 
 import importlib
 from copy import deepcopy
 from typing import List, Any, Callable
 from chiakilisp.models.token import Token
 import chiakilisp.spec as s
@@ -17,24 +19,32 @@
 from chiakilisp.models.literal import\
     Literal, NotFound, Nil
 from chiakilisp.models.forward import\
     ExpressionType, CommonType
 from chiakilisp.utils import get_assertion_closure, pairs
 
 
+class Py3xError(Exception):
+
+    """Exception.execute() may throw this exception"""
+
+
 class ArityError(SyntaxError):
 
     """Stub class to display that there is an arity error"""
 
 
 NE_ASSERT = get_assertion_closure(NameError)  # <--------- raises NameError
 TE_ASSERT = get_assertion_closure(TypeError)  # <--------- raises TypeError
 SE_ASSERT = get_assertion_closure(SyntaxError)  # <----- raises SyntaxError
 RE_ASSERT = get_assertion_closure(RuntimeError)  # <--- raises RuntimeError
 
+MANAGED_ERRORS = (
+    Py3xError, ArityError, NameError, TypeError, SyntaxError, RuntimeError)
+
 
 def IDENTIFIER_ASSERT(lit: Literal, message: str) -> None:
 
     """Handy shortcut to make assertion that Literal is Identifier"""
 
     SE_ASSERT(lit.token().position(), lit.token().is_identifier(), message)
 
@@ -172,14 +182,15 @@
 
         """Execute here - is to return Python 3 value related to the expression: string, number, and vice versa"""
 
         head: Literal
 
         assert self.nodes(),              'Expression[execute]: current expression is empty, unable to execute it'
 
+        # TODO: implement something like chiakilisp.libs.core module to store symbols like `get` and `first` there
         get = environ.get('get')  # <------- some features like destructing or keyword-as-fn will require core/get
         first = environ.get('first')  # <----- some feature like inline function or others will require core/first
 
         head, *tail = self.nodes()
 
         where = head.token().position()  # <------------ when make assertions on expression head, this can be used
 
@@ -295,15 +306,14 @@
 
             return target.execute(environ, False)  # <----- at the end, return target' expression execution result
 
         if head.token().value().startswith('.') and not head.token().value() == '...':   # it could be an Ellipsis
             SE_ASSERT(where,
                       len(head.token().value()) > 1,    'Expression[execute]: dot-form: method name is mandatory')
             TAIL_IS_VALID(tail,                         'dot-form', where, 'Expression[execute]: dot-form: {why}')
-            handle_name: Literal  # <------------------------------------- assign handle name as a type of Literal
             handle_name, *method_args = tail  # <------------------------ parse dot-form handle name and arguments
             method_name = head.token().value()[1:]  # <------------------ parse handle name from the first literal
             handle_instance = handle_name.execute(environ, False)  # <--- get the handle instance from environment
             SE_ASSERT(where,
                       hasattr(handle_instance, '__class__'),
                       'Expression[execute]: dot-form: use object/method, module/method to invoke a static method')
             handle_alias = handle_instance.__class__.__name__  # <------------- get the actual instance class name
@@ -470,8 +480,13 @@
             environ[alias.split('/')[-1]] = environ.get('__require__')(alias)  # <----- assign to unqualified path
             return None  # <----------------------------------------------------------------------- and return nil
 
         handle = head.execute(environ, False)  # resolve handle object by its name, this could raise a 'NameError'
 
         self._assert_even_number_of_dict_literals()  # verify literals form arity before dictionary initialization
 
-        return handle(*tuple(map(lambda argument: argument.execute(environ,  False),  tail)))  # return the result
+        try:
+            return handle(*tuple(map(lambda argument: argument.execute(environ,  False), tail)))  # catch an error
+        except Exception as _error_:
+            if not isinstance(_error_, MANAGED_ERRORS):
+                raise Py3xError(f'{":".join(map(str, where))}: {_error_.__class__.__name__}: {_error_.__str__()}')
+            raise _error_  # re-raise the error if it's managed one, raise Py3xError if its arbitrary Python 3 one
```

## Comparing `chiakilisp-1.4.0rc3.data/scripts/chiakilang` & `chiakilisp-1.4.0rc4.data/scripts/chiakilang`

 * *Files 3% similar despite different names*

```diff
@@ -242,14 +242,20 @@
 
     ENVIRONMENT.update({
         n: getattr(BUILTINS, n, None)
         for n in
         filter(lambda k: k not in ['__import__', '__loader__', '__name__', '__package__', '__spec__'],
                dir(BUILTINS))})  # proxy only allowed builtin Python 3 symbols, others are proven to cause bugs
 
+    del ENVIRONMENT['__doc__']   # <-- no need to proxy this built-in var, as it's unlikely be accessed by user
+    del ENVIRONMENT['__debug__']  # <- we will proxy this built-in boolean variable by `running-in-debug-mode?`
+    del ENVIRONMENT['__build_class__']   # <-- no need to proxy this built-in method, as there is `type` exists
+
+    ENVIRONMENT['running-in-debug-mode?'] =  __debug__  # <---------------- proxy `__debug__` built-in variable
+
     if not args.coreless:
         if os.path.exists('chiakilisp/corelib/core.cl'):
             require('chiakilisp/corelib/core.cl', use_global_env=True)  # <------- load ChiakiLisp core library
         else:
             execute(
                 pkgutil.get_data('chiakilisp', 'corelib/core.cl').decode('utf-8'),  'corelib.cl',  silent=True)
```

## Comparing `chiakilisp-1.4.0rc3.dist-info/METADATA` & `chiakilisp-1.4.0rc4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiakilisp
-Version: 1.4.0rc3
+Version: 1.4.0rc4
 Summary: ChiakiLisp - Yet another LISP
 Home-page: https://chiakilisp.jedi2light.moe
 Author: @jedi2light
 Author-email: jedi2light@jedi2light.moe
 Maintainer: @jedi2light
 Maintainer-email: jedi2light@jedi2light.moe
 License: WTFPL
```

## Comparing `chiakilisp-1.4.0rc3.dist-info/RECORD` & `chiakilisp-1.4.0rc4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 chiakilisp/lexer.py,sha256=FnLU7DPtpVRLP2rkMQ3h1INQ4KC-MLy_vAjSrvPG9vg,13791
 chiakilisp/parser.py,sha256=aPAa3U8D28DO15NzwUliLTOZeCaQEu5giOpzCnPBSs8,5943
 chiakilisp/runtime.py,sha256=J69abrFy4RdcA6oU9z2Pv4ok4A7h5X8lR9VM1l28kk4,1378
 chiakilisp/spec.py,sha256=4_hvO1HYm3RGnky1q85q72we1L3wpjufDgoVU_kcTwk,11225
 chiakilisp/utils.py,sha256=lYwdSJY_y5QEBAM9rEd02Z9ra9ZADJ_yO8JIfsS2WAM,3311
 chiakilisp/corelib/core.cl,sha256=a-vhEjziW_vQy9kfWFF_SJbNPdL4O0sx23AwaUvAdR4,7443
 chiakilisp/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-chiakilisp/models/expression.py,sha256=xoOR1QQhTq19KwlVRmaedJnUL0u3Aqo5wwIk-eCBvTw,30784
+chiakilisp/models/expression.py,sha256=yRBvimRfmTRUYiO4GeLSZdlY1GFnsZeAfsKTeeKfmMs,31381
 chiakilisp/models/forward.py,sha256=ykZjLoXxONjvoCZ3h2itUieAFteh5TUiAuk4f8NoiZs,790
 chiakilisp/models/literal.py,sha256=0m0FRZ9YLq23pH_DKjSSObey5gZIo73BUJP37F5svsA,3778
 chiakilisp/models/token.py,sha256=TYfdqCVn3_74aBCn6m5gPikjpwixUW65FeKrMLuvpvE,1986
 chiakilisp/proxies/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chiakilisp/proxies/keyword.py,sha256=fMVWpRxk_Sk_6CXE08IFnFTtMbvhadUSe2IYgin_h60,205
-chiakilisp-1.4.0rc3.data/scripts/chiakilang,sha256=kv-yjMEWm0XIoCB2DjaLrvLHX_lobI_IhZywiLuHYvM,12909
-chiakilisp-1.4.0rc3.dist-info/METADATA,sha256=g_iIekRgTknUTXJJ9NFuR3jhSZcbP0lG2Ew8x2HH_z4,1408
-chiakilisp-1.4.0rc3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-chiakilisp-1.4.0rc3.dist-info/top_level.txt,sha256=uV87HteR3vUsfEm7HlxKG0Fh7zkoke2RetMtgLu97Bc,11
-chiakilisp-1.4.0rc3.dist-info/RECORD,,
+chiakilisp-1.4.0rc4.data/scripts/chiakilang,sha256=-vbv8w6RFangekz5zoX-FBDYFabYX_Ad4VvvPD8Hvro,13359
+chiakilisp-1.4.0rc4.dist-info/METADATA,sha256=KYbur4Dz8kwHeDMLhQbsEHT5K_hmcTtWZ4XQFfX5A4g,1408
+chiakilisp-1.4.0rc4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+chiakilisp-1.4.0rc4.dist-info/top_level.txt,sha256=uV87HteR3vUsfEm7HlxKG0Fh7zkoke2RetMtgLu97Bc,11
+chiakilisp-1.4.0rc4.dist-info/RECORD,,
```

