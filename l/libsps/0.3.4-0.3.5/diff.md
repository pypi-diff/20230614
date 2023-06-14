# Comparing `tmp/libsps-0.3.4-cp38-cp38-win_amd64.whl.zip` & `tmp/libsps-0.3.5-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 244015 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   617984 b- defN 23-Jun-14 12:27 sps.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1088 b- defN 23-Jun-14 12:27 libsps-0.3.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      658 b- defN 23-Jun-14 12:27 libsps-0.3.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-14 12:27 libsps-0.3.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-14 12:27 libsps-0.3.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      461 b- defN 23-Jun-14 12:27 libsps-0.3.4.dist-info/RECORD
-6 files, 620295 bytes uncompressed, 243185 bytes compressed:  60.8%
+Zip file size: 243106 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat   616960 b- defN 23-Jun-14 14:10 sps.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-Jun-14 14:10 libsps-0.3.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      693 b- defN 23-Jun-14 14:10 libsps-0.3.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-14 14:10 libsps-0.3.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-14 14:10 libsps-0.3.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      461 b- defN 23-Jun-14 14:10 libsps-0.3.5.dist-info/RECORD
+6 files, 619306 bytes uncompressed, 242276 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: sps.cp38-win_amd64.pyd
+Filename: sps.cp39-win_amd64.pyd
 Comment: 
 
-Filename: libsps-0.3.4.dist-info/LICENSE
+Filename: libsps-0.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: libsps-0.3.4.dist-info/METADATA
+Filename: libsps-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: libsps-0.3.4.dist-info/WHEEL
+Filename: libsps-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: libsps-0.3.4.dist-info/top_level.txt
+Filename: libsps-0.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: libsps-0.3.4.dist-info/RECORD
+Filename: libsps-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `libsps-0.3.4.dist-info/LICENSE` & `libsps-0.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `libsps-0.3.4.dist-info/METADATA` & `libsps-0.3.5.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: libsps
-Version: 0.3.4
+Version: 0.3.5
 Summary: O(1) region count queries using sparse prefix sums
 Home-page: https://github.com/Siegel-Lab/libSps
 Author: Markus Schmidt
 Author-email: markus.rainer.schmidt@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
+License-File: LICENSE
 Provides-Extra: test
 Requires-Dist: pytest ; extra == 'test'
 
 
-O(1) region count queries using sparse prefix sums
-
+        O(1) region count queries using sparse prefix sums
+
```

