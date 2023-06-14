# Comparing `tmp/rapid_layout-0.0.8-py3-none-any.whl.zip` & `tmp/rapid_layout-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6834194 bytes, number of entries: 10
--rw-r--r--  2.0 unx      646 b- defN 22-Dec-19 06:15 rapid_layout/__init__.py
--rw-r--r--  2.0 unx      517 b- defN 22-Dec-19 06:15 rapid_layout/config.yaml
--rw-r--r--  2.0 unx     2998 b- defN 22-Dec-19 06:15 rapid_layout/rapid_layout.py
--rw-r--r--  2.0 unx    15141 b- defN 22-Dec-19 06:15 rapid_layout/utils.py
+Zip file size: 6834192 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      646 b- defN 23-Jan-09 01:19 rapid_layout/__init__.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Jan-09 01:19 rapid_layout/config.yaml
+-rw-r--r--  2.0 unx     2998 b- defN 23-Jan-09 01:19 rapid_layout/rapid_layout.py
+-rw-r--r--  2.0 unx    15141 b- defN 23-Jan-09 01:19 rapid_layout/utils.py
 -rw-r--r--  2.0 unx  7423528 b- defN 22-Nov-19 19:32 rapid_layout/models/layout_cdla.onnx
--rw-r--r--  2.0 unx     1742 b- defN 22-Dec-19 06:15 rapid_layout-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-19 06:15 rapid_layout-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 22-Dec-19 06:15 rapid_layout-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 22-Dec-19 06:15 rapid_layout-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      838 b- defN 22-Dec-19 06:15 rapid_layout-0.0.8.dist-info/RECORD
-10 files, 7445580 bytes uncompressed, 6832760 bytes compressed:  8.2%
+-rw-r--r--  2.0 unx     1742 b- defN 23-Jan-09 01:19 rapid_layout-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jan-09 01:19 rapid_layout-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 23-Jan-09 01:19 rapid_layout-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jan-09 01:19 rapid_layout-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      838 b- defN 23-Jan-09 01:19 rapid_layout-0.0.9.dist-info/RECORD
+10 files, 7445580 bytes uncompressed, 6832758 bytes compressed:  8.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: rapid_layout/utils.py
 Comment: 
 
 Filename: rapid_layout/models/layout_cdla.onnx
 Comment: 
 
-Filename: rapid_layout-0.0.8.dist-info/METADATA
+Filename: rapid_layout-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: rapid_layout-0.0.8.dist-info/WHEEL
+Filename: rapid_layout-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_layout-0.0.8.dist-info/entry_points.txt
+Filename: rapid_layout-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_layout-0.0.8.dist-info/top_level.txt
+Filename: rapid_layout-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_layout-0.0.8.dist-info/RECORD
+Filename: rapid_layout-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rapid_layout-0.0.8.dist-info/METADATA` & `rapid_layout-0.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid-layout
-Version: 0.0.8
+Version: 0.0.9
 Summary: RapidLayout
 Home-page: https://github.com/RapidAI/RapidOCR
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: ppstructure,layout,rapidocr,rapid_layout
 Platform: Any
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapid-layout Version: 0.0.8 Summary: RapidLayout
+Metadata-Version: 2.1 Name: rapid-layout Version: 0.0.9 Summary: RapidLayout
 Home-page: https://github.com/RapidAI/RapidOCR Author: SWHL Author-email:
 liekkaskono@163.com License: Apache-2.0 Keywords:
 ppstructure,layout,rapidocr,rapid_layout Platform: Any Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown Requires-
 Dist: PyYAML (>=6.0) Requires-Dist: numpy (>=1.21.6) Requires-Dist: onnxruntime
```

