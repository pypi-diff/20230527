# Comparing `tmp/versioner.py-1.1.0-py3-none-any.whl.zip` & `tmp/versioner.py-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5133 bytes, number of entries: 11
+Zip file size: 5091 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat      952 b- defN 22-Dec-02 20:29 versioner/Exceptions.py
--rw-rw-rw-  2.0 fat     1131 b- defN 22-Dec-02 18:07 versioner/Functions.py
+-rw-rw-rw-  2.0 fat     1131 b- defN 23-May-05 19:44 versioner/Functions.py
 -rw-rw-rw-  2.0 fat      520 b- defN 22-Dec-02 20:44 versioner/Units.py
--rw-rw-rw-  2.0 fat     2688 b- defN 22-Dec-30 18:00 versioner/Version.py
--rw-rw-rw-  2.0 fat      306 b- defN 22-Dec-30 17:54 versioner/__init__.py
--rw-rw-rw-  2.0 fat      966 b- defN 22-Dec-30 18:01 versioner/__main__.py
--rw-rw-rw-  2.0 fat     1085 b- defN 22-Dec-30 18:01 versioner.py-1.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      366 b- defN 22-Dec-30 18:01 versioner.py-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Dec-30 18:01 versioner.py-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 22-Dec-30 18:01 versioner.py-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      873 b- defN 22-Dec-30 18:01 versioner.py-1.1.0.dist-info/RECORD
-11 files, 8989 bytes uncompressed, 3657 bytes compressed:  59.3%
+-rw-rw-rw-  2.0 fat     2394 b- defN 23-May-27 14:43 versioner/Version.py
+-rw-rw-rw-  2.0 fat      283 b- defN 23-May-27 14:43 versioner/__init__.py
+-rw-rw-rw-  2.0 fat      966 b- defN 23-May-05 19:44 versioner/__main__.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-May-27 14:43 versioner.py-1.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      366 b- defN 23-May-27 14:43 versioner.py-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-27 14:43 versioner.py-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-27 14:43 versioner.py-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      873 b- defN 23-May-27 14:43 versioner.py-1.1.1.dist-info/RECORD
+11 files, 8672 bytes uncompressed, 3615 bytes compressed:  58.3%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: versioner/__init__.py
 Comment: 
 
 Filename: versioner/__main__.py
 Comment: 
 
-Filename: versioner.py-1.1.0.dist-info/LICENSE
+Filename: versioner.py-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: versioner.py-1.1.0.dist-info/METADATA
+Filename: versioner.py-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: versioner.py-1.1.0.dist-info/WHEEL
+Filename: versioner.py-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: versioner.py-1.1.0.dist-info/top_level.txt
+Filename: versioner.py-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: versioner.py-1.1.0.dist-info/RECORD
+Filename: versioner.py-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## versioner/Version.py

```diff
@@ -1,32 +1,27 @@
 from vbml import Pattern
 from typing import Dict, Any, List
 # * Local Imports
-try:
-    from .Functions import get_patterns, handling_variations, is_equal_keys, parse_version_data
-    from .Exceptions import ParsingError, ParsingKeysError
-    from .Units import STANDART_PATTERNS, STANDART_VARIATIONS, STANDART_VERSION_DATA
-except:
-    from Functions import get_patterns, handling_variations, is_equal_keys, parse_version_data
-    from Exceptions import ParsingError, ParsingKeysError
-    from Units import STANDART_PATTERNS, STANDART_VARIATIONS, STANDART_VERSION_DATA
+from .Functions import get_patterns, handling_variations, is_equal_keys, parse_version_data
+from .Exceptions import ParsingError, ParsingKeysError
+from .Units import STANDART_PATTERNS, STANDART_VARIATIONS, STANDART_VERSION_DATA
 
 # ! Version Class
 class Version:
     def __init__(
         self,
         version: str,
         version_data: Dict[str, int]
     ) -> None:
         self.version = version
         self.version_data = version_data
         self.hash_data = [hash(i) for i in self.version_data.values()]
     
     def __str__(self) -> str: return self.version
-    def __repr__(self) -> str: return f"{self.__class__.__name__}('{self.__str__()}')"
+    def __repr__(self) -> str: return f"'{self.__str__()}'"
     def similar_to(self, version) -> bool: return is_equal_keys(self.version_data, version.version_data)
     def __eq__(self, other) -> bool:
         if self.similar_to(other):
             return min([(i[0] == i[1]) for i in list(zip(self.hash_data, other.hash_data))])
         raise ParsingKeysError()
     def __lt__(self, other) -> bool:
         if self.similar_to(other):
```

## versioner/__init__.py

```diff
@@ -1,15 +1,14 @@
 from .Version import (
-    Versioner,
-    Version,
-    ParsingError,
-    ParsingKeysError,
+    Versioner, Version
+)
+from .Units import (
     STANDART_PATTERNS,
     STANDART_VARIATIONS,
     STANDART_VERSION_DATA
 )
 
 __name__ = "versioner.py"
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 __author__ = "Romanin"
 __email__ = "semina054@gmail.com"
 __licence__ = "MIT"
```

## Comparing `versioner.py-1.1.0.dist-info/LICENSE` & `versioner.py-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `versioner.py-1.1.0.dist-info/RECORD` & `versioner.py-1.1.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 versioner/Exceptions.py,sha256=g1UT2ay-a0bhBAH-gDO7s-E90aO43QmdNRW_1rXCwwQ,952
 versioner/Functions.py,sha256=CDY6veHsJhlkwdaXFyPi1oaIDvy8CXei2_6f-QB7pJ8,1131
 versioner/Units.py,sha256=vlD_9tjmMIn_uVYNireMXt9tQlad6SXILxAVC17rJow,520
-versioner/Version.py,sha256=hfO2hkrbXq-kYls3cNPFvEM-tWFHbuqPvdzLexGw8lc,2688
-versioner/__init__.py,sha256=afsEsc4Pad0sJXmH37VY7PztB8giLFZFlbap37TprF0,306
+versioner/Version.py,sha256=jJXRZZWGDL1lH_IcdmKlqn1CQdb-zJJHyp60WO0Tdwg,2394
+versioner/__init__.py,sha256=e91wHiLmcjeJrp0t-BXI__pjHSQlsnAYb0q4rJTgq34,283
 versioner/__main__.py,sha256=ALWRnbdVMnMtHR7FrtUj74jUa0k2wMpG-jTaOUOZIoE,966
-versioner.py-1.1.0.dist-info/LICENSE,sha256=spNP9-xRNk_f344KMfxONAblI58MMrpPasaQ5sXdwe4,1085
-versioner.py-1.1.0.dist-info/METADATA,sha256=tTmfEWryAjlvNBXFKoex9Ddl8YVxD-XWKltTajlKsA4,366
-versioner.py-1.1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-versioner.py-1.1.0.dist-info/top_level.txt,sha256=7lke3tKWLLL9eOFxui2M8Bx6OxbHIZKbLtcXqwwkQhg,10
-versioner.py-1.1.0.dist-info/RECORD,,
+versioner.py-1.1.1.dist-info/LICENSE,sha256=spNP9-xRNk_f344KMfxONAblI58MMrpPasaQ5sXdwe4,1085
+versioner.py-1.1.1.dist-info/METADATA,sha256=QkqT7EzQ3OXGrSJ2hiA-tp6PW4AzuwGd6jpxs8iHgO8,366
+versioner.py-1.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+versioner.py-1.1.1.dist-info/top_level.txt,sha256=7lke3tKWLLL9eOFxui2M8Bx6OxbHIZKbLtcXqwwkQhg,10
+versioner.py-1.1.1.dist-info/RECORD,,
```

