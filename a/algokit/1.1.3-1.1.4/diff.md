# Comparing `tmp/algokit-1.1.3-py3-none-any.whl.zip` & `tmp/algokit-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 43508 bytes, number of entries: 31
+Zip file size: 43511 bytes, number of entries: 31
 -rw-r--r--  2.0 unx     1168 b- defN 80-Jan-01 00:00 algokit/__init__.py
 -rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 algokit/__main__.py
 -rw-r--r--  2.0 unx     1511 b- defN 80-Jan-01 00:00 algokit/cli/__init__.py
 -rw-r--r--  2.0 unx     1778 b- defN 80-Jan-01 00:00 algokit/cli/bootstrap.py
 -rw-r--r--  2.0 unx     6065 b- defN 80-Jan-01 00:00 algokit/cli/completions.py
 -rw-r--r--  2.0 unx      296 b- defN 80-Jan-01 00:00 algokit/cli/config.py
 -rw-r--r--  2.0 unx     5802 b- defN 80-Jan-01 00:00 algokit/cli/doctor.py
@@ -21,13 +21,13 @@
 -rw-r--r--  2.0 unx     3520 b- defN 80-Jan-01 00:00 algokit/core/proc.py
 -rw-r--r--  2.0 unx     1970 b- defN 80-Jan-01 00:00 algokit/core/questionary_extensions.py
 -rw-r--r--  2.0 unx    10504 b- defN 80-Jan-01 00:00 algokit/core/sandbox.py
 -rw-r--r--  2.0 unx     4025 b- defN 80-Jan-01 00:00 algokit/core/typed_client_generation.py
 -rw-r--r--  2.0 unx      508 b- defN 80-Jan-01 00:00 algokit/core/utils.py
 -rw-r--r--  2.0 unx     4174 b- defN 80-Jan-01 00:00 algokit/core/version_prompt.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit/py.typed
--rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 algokit-1.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    13733 b- defN 80-Jan-01 00:00 algokit-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit-1.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 algokit-1.1.3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2478 b- defN 16-Jan-01 00:00 algokit-1.1.3.dist-info/RECORD
-31 files, 115665 bytes uncompressed, 39580 bytes compressed:  65.8%
+-rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 algokit-1.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13733 b- defN 80-Jan-01 00:00 algokit-1.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit-1.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 algokit-1.1.4.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2478 b- defN 16-Jan-01 00:00 algokit-1.1.4.dist-info/RECORD
+31 files, 115665 bytes uncompressed, 39583 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -72,23 +72,23 @@
 
 Filename: algokit/core/version_prompt.py
 Comment: 
 
 Filename: algokit/py.typed
 Comment: 
 
-Filename: algokit-1.1.3.dist-info/LICENSE
+Filename: algokit-1.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: algokit-1.1.3.dist-info/METADATA
+Filename: algokit-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: algokit-1.1.3.dist-info/WHEEL
+Filename: algokit-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: algokit-1.1.3.dist-info/entry_points.txt
+Filename: algokit-1.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: algokit-1.1.3.dist-info/RECORD
+Filename: algokit-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit/core/typed_client_generation.py

```diff
@@ -9,15 +9,15 @@
 import algokit_client_generator
 import click
 
 from algokit.core import proc
 
 logger = logging.getLogger(__name__)
 
-TYPESCRIPT_NPX_PACKAGE = "@algorandfoundation/algokit-client-generator@^2.1"
+TYPESCRIPT_NPX_PACKAGE = "@algorandfoundation/algokit-client-generator@^2.2"
 
 
 def _snake_case(s: str) -> str:
     s = s.replace("-", " ")
     s = re.sub(r"([A-Z]+)([A-Z][a-z])", r"\1_\2", s)
     s = re.sub(r"([a-z\d])([A-Z])", r"\1_\2", s)
     return re.sub(r"[-\s]", "_", s).lower()
```

## Comparing `algokit-1.1.3.dist-info/LICENSE` & `algokit-1.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit-1.1.3.dist-info/METADATA` & `algokit-1.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit
-Version: 1.1.3
+Version: 1.1.4
 Summary: Algorand development kit command-line interface
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit-1.1.3.dist-info/RECORD` & `algokit-1.1.4.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 algokit/core/conf.py,sha256=oWSlSAvTUviSK_AdS-H_G6DMqVOvBe_jCC-vJfgrkBI,1380
 algokit/core/doctor.py,sha256=I2BKoupBPot26Y-4OTMFJp0mATLfp9Nlz8XXv1N7i8Y,4711
 algokit/core/init.py,sha256=7y_EwVtuMfqZG_CGDR08K0f2SOOeFq6y1d8ihZgG3Uo,1159
 algokit/core/log_handlers.py,sha256=IT9mo8NhiLl2rzH6t6F9kEflmmFbOfOhKaPzRp7CVTM,5128
 algokit/core/proc.py,sha256=aJ3BGyXmI0oguOE1WbAyirCW2_IIBYuPOFutCX7cXnE,3520
 algokit/core/questionary_extensions.py,sha256=QvUGXL_GxcPvdGemy_5-Fza4d1PSJ2ml7aZAS3r4M20,1970
 algokit/core/sandbox.py,sha256=5iYxaJXqXhPSm69Y5mChEBYuc6C7kUjMgnoSG-WYsZc,10504
-algokit/core/typed_client_generation.py,sha256=ITKs3FyJT_XMln9ssPkyBFtJ66favkgYu0zY_cBGqSg,4025
+algokit/core/typed_client_generation.py,sha256=zfE-OH-lSnhoe25iNwngZyy_9jo6rU9tlBiqtbkE65c,4025
 algokit/core/utils.py,sha256=hgemlB8znOsGCO090BQOydnbq4ZRAsD9CzMbApEMGY8,508
 algokit/core/version_prompt.py,sha256=yf63811ilKPoJfusxKBmxoZetrCKMKvGoSODI1-kaek,4174
 algokit/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit-1.1.3.dist-info/LICENSE,sha256=CPjn5HTZL3VUJ8E1lxtdBx6SLzNnQlOoezdFYom9R24,1081
-algokit-1.1.3.dist-info/METADATA,sha256=1fDzkCOR3x8TN0xQySg97MJGx8sTeelQojxE_ejwQUM,13733
-algokit-1.1.3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-algokit-1.1.3.dist-info/entry_points.txt,sha256=JJtH-iaVJa6YUrN69B7AMycsg9-q6OwV52olGIU65rc,47
-algokit-1.1.3.dist-info/RECORD,,
+algokit-1.1.4.dist-info/LICENSE,sha256=CPjn5HTZL3VUJ8E1lxtdBx6SLzNnQlOoezdFYom9R24,1081
+algokit-1.1.4.dist-info/METADATA,sha256=eLwfE3080HoYYOxgcThS0le41uWThx7AtRMfFA7IhiQ,13733
+algokit-1.1.4.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+algokit-1.1.4.dist-info/entry_points.txt,sha256=JJtH-iaVJa6YUrN69B7AMycsg9-q6OwV52olGIU65rc,47
+algokit-1.1.4.dist-info/RECORD,,
```

