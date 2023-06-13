# Comparing `tmp/viam_sdk-0.4.1-py3-none-manylinux2014_x86_64.whl.zip` & `tmp/viam_sdk-0.4.1rc1-py3-none-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9847294 bytes, number of entries: 375
+Zip file size: 9847321 bytes, number of entries: 375
 -rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx     1411 b- defN 80-Jan-01 00:00 viam/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 viam/components/__init__.py
 -rw-r--r--  2.0 unx     1075 b- defN 80-Jan-01 00:00 viam/components/arm/__init__.py
 -rw-r--r--  2.0 unx     2870 b- defN 80-Jan-01 00:00 viam/components/arm/arm.py
 -rw-r--r--  2.0 unx     3734 b- defN 80-Jan-01 00:00 viam/components/arm/client.py
 -rw-r--r--  2.0 unx     4951 b- defN 80-Jan-01 00:00 viam/components/arm/service.py
@@ -366,12 +366,12 @@
 -rw-r--r--  2.0 unx     1633 b- defN 80-Jan-01 00:00 viam/services/slam/slam.py
 -rw-r--r--  2.0 unx      426 b- defN 80-Jan-01 00:00 viam/services/vision/__init__.py
 -rw-r--r--  2.0 unx     5176 b- defN 80-Jan-01 00:00 viam/services/vision/client.py
 -rw-r--r--  2.0 unx     5076 b- defN 80-Jan-01 00:00 viam/services/vision/service.py
 -rw-r--r--  2.0 unx     4996 b- defN 80-Jan-01 00:00 viam/services/vision/vision.py
 -rw-r--r--  2.0 unx     5149 b- defN 80-Jan-01 00:00 viam/sessions_client.py
 -rw-r--r--  2.0 unx     7927 b- defN 80-Jan-01 00:00 viam/utils.py
--rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 viam_sdk-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     8335 b- defN 80-Jan-01 00:00 viam_sdk-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 viam_sdk-0.4.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    34597 b- defN 16-Jan-01 00:00 viam_sdk-0.4.1.dist-info/RECORD
-375 files, 30152660 bytes uncompressed, 9791580 bytes compressed:  67.5%
+-rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 viam_sdk-0.4.1rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8338 b- defN 80-Jan-01 00:00 viam_sdk-0.4.1rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 viam_sdk-0.4.1rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    34609 b- defN 16-Jan-01 00:00 viam_sdk-0.4.1rc1.dist-info/RECORD
+375 files, 30152675 bytes uncompressed, 9791583 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -1107,20 +1107,20 @@
 
 Filename: viam/sessions_client.py
 Comment: 
 
 Filename: viam/utils.py
 Comment: 
 
-Filename: viam_sdk-0.4.1.dist-info/LICENSE
+Filename: viam_sdk-0.4.1rc1.dist-info/LICENSE
 Comment: 
 
-Filename: viam_sdk-0.4.1.dist-info/METADATA
+Filename: viam_sdk-0.4.1rc1.dist-info/METADATA
 Comment: 
 
-Filename: viam_sdk-0.4.1.dist-info/WHEEL
+Filename: viam_sdk-0.4.1rc1.dist-info/WHEEL
 Comment: 
 
-Filename: viam_sdk-0.4.1.dist-info/RECORD
+Filename: viam_sdk-0.4.1rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `viam_sdk-0.4.1.dist-info/LICENSE` & `viam_sdk-0.4.1rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `viam_sdk-0.4.1.dist-info/METADATA` & `viam_sdk-0.4.1rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viam-sdk
-Version: 0.4.1
+Version: 0.4.1rc1
 Summary: Viam Robotics Python SDK
 License: Apache-2.0
 Author: Naveed
 Author-email: naveed@viam.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `viam_sdk-0.4.1.dist-info/RECORD` & `viam_sdk-0.4.1rc1.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -365,11 +365,11 @@
 viam/services/slam/slam.py,sha256=872OV9JvSEvwWRBDiX-P8Zs87fNBp-5mbMx4ruot-gY,1633
 viam/services/vision/__init__.py,sha256=8DPwRKggv0cMb3Z4R5-pAHvbAIIMBfNYWUktuh58gyE,426
 viam/services/vision/client.py,sha256=EHiVW1R2JgS_DzyenmJzcIhQdtiegeUUBy2lYBpKemg,5176
 viam/services/vision/service.py,sha256=ae0zUVBi-QiNYoxfT7KurCUvdy0umdUdFVqMLprF_3c,5076
 viam/services/vision/vision.py,sha256=MFeEWjiS2Dp7ttqL3lmHTznxmGpoVEkIgYbWTuiZPPg,4996
 viam/sessions_client.py,sha256=GUSKFmJnafDabxMsQQG2nuHPaiCUgjw42iHWJGg9qNA,5149
 viam/utils.py,sha256=gGoMOLkeJSerDIH2nPDydTfL7-p2AWqZCMU4jQEp0go,7927
-viam_sdk-0.4.1.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
-viam_sdk-0.4.1.dist-info/METADATA,sha256=2ZICUoSpIvmH6PNS10FnEiQJD78KTEQiF86u45z3kVM,8335
-viam_sdk-0.4.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-viam_sdk-0.4.1.dist-info/RECORD,,
+viam_sdk-0.4.1rc1.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
+viam_sdk-0.4.1rc1.dist-info/METADATA,sha256=VVyVGi71g7aanlg7RBr8JORT32DsO7k_SuI7UgvI5EY,8338
+viam_sdk-0.4.1rc1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+viam_sdk-0.4.1rc1.dist-info/RECORD,,
```

