# Comparing `tmp/libsps-0.3.2-cp39-cp39-win_amd64.whl.zip` & `tmp/libsps-0.3.3-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 2107 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1088 b- defN 23-Jun-13 15:10 libsps-0.3.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      848 b- defN 23-Jun-13 15:10 libsps-0.3.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-13 15:10 libsps-0.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-13 15:10 libsps-0.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      380 b- defN 23-Jun-13 15:10 libsps-0.3.2.dist-info/RECORD
-5 files, 2420 bytes uncompressed, 1397 bytes compressed:  42.3%
+Zip file size: 244226 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat   618496 b- defN 23-Jun-14 12:01 sps.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-Jun-14 12:01 libsps-0.3.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      846 b- defN 23-Jun-14 12:01 libsps-0.3.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-14 12:01 libsps-0.3.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-14 12:01 libsps-0.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      461 b- defN 23-Jun-14 12:01 libsps-0.3.3.dist-info/RECORD
+6 files, 620995 bytes uncompressed, 243396 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
-Filename: libsps-0.3.2.dist-info/LICENSE
+Filename: sps.cp39-win_amd64.pyd
 Comment: 
 
-Filename: libsps-0.3.2.dist-info/METADATA
+Filename: libsps-0.3.3.dist-info/LICENSE
 Comment: 
 
-Filename: libsps-0.3.2.dist-info/WHEEL
+Filename: libsps-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: libsps-0.3.2.dist-info/top_level.txt
+Filename: libsps-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: libsps-0.3.2.dist-info/RECORD
+Filename: libsps-0.3.3.dist-info/top_level.txt
+Comment: 
+
+Filename: libsps-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `libsps-0.3.2.dist-info/LICENSE` & `libsps-0.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `libsps-0.3.2.dist-info/METADATA` & `libsps-0.3.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsps
-Version: 0.3.2
+Version: 0.3.3
 Summary: O(1) region count queries using sparse prefix sums
 Home-page: https://github.com/Siegel-Lab/libSps
 Author: Markus Schmidt
 Author-email: markus.rainer.schmidt@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -17,10 +17,10 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 License-File: LICENSE
 Provides-Extra: test
 Requires-Dist: pytest ; extra == 'test'
 
 
-        # O(1) region count queries using sparse prefix sums
+        O(1) region count queries using sparse prefix sums
```

