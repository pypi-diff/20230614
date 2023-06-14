# Comparing `tmp/e2eqavn-2.2-py2.py3-none-any.whl.zip` & `tmp/e2eqavn-2.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 35719 bytes, number of entries: 40
--rw-rw-r--  2.0 unx      496 b- defN 23-Jun-07 13:55 e2eqavn/__init__.py
+Zip file size: 35733 bytes, number of entries: 40
+-rw-rw-r--  2.0 unx      496 b- defN 23-Jun-07 14:00 e2eqavn/__init__.py
 -rw-rw-r--  2.0 unx     7061 b- defN 23-May-25 09:03 e2eqavn/cli.py
 -rw-rw-r--  2.0 unx     2472 b- defN 23-May-25 07:49 e2eqavn/keywords.py
 -rw-rw-r--  2.0 unx     2973 b- defN 23-May-20 15:46 e2eqavn/datasets/MRCDataset.py
 -rw-rw-r--  2.0 unx     1386 b- defN 23-Apr-08 19:20 e2eqavn/datasets/TripletDataset.py
 -rw-rw-r--  2.0 unx      124 b- defN 23-May-02 14:04 e2eqavn/datasets/__init__.py
 -rw-rw-r--  2.0 unx     3660 b- defN 23-May-30 15:21 e2eqavn/datasets/data_collator.py
 -rw-rw-r--  2.0 unx       85 b- defN 23-Apr-08 14:59 e2eqavn/documents/__init__.py
@@ -30,13 +30,13 @@
 -rw-rw-r--  2.0 unx    10419 b- defN 23-May-25 09:03 e2eqavn/retrieval/sbert_retrieval.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-18 08:56 e2eqavn/utils/__init__.py
 -rw-rw-r--  2.0 unx    12402 b- defN 23-May-20 16:33 e2eqavn/utils/calculate.py
 -rw-rw-r--  2.0 unx      603 b- defN 23-May-31 16:18 e2eqavn/utils/io.py
 -rw-rw-r--  2.0 unx      998 b- defN 23-May-03 09:44 e2eqavn/utils/preprocess.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-19 07:27 test/__init__.py
 -rw-rw-r--  2.0 unx      334 b- defN 23-Apr-08 14:59 test/test_chunking.py
--rw-rw-r--  2.0 unx      649 b- defN 23-Jun-07 13:56 e2eqavn-2.2.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-07 13:56 e2eqavn-2.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       52 b- defN 23-Jun-07 13:56 e2eqavn-2.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       13 b- defN 23-Jun-07 13:56 e2eqavn-2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3367 b- defN 23-Jun-07 13:56 e2eqavn-2.2.dist-info/RECORD
-40 files, 105121 bytes uncompressed, 30323 bytes compressed:  71.2%
+-rw-rw-r--  2.0 unx      677 b- defN 23-Jun-07 14:02 e2eqavn-2.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-07 14:02 e2eqavn-2.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       52 b- defN 23-Jun-07 14:02 e2eqavn-2.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       13 b- defN 23-Jun-07 14:02 e2eqavn-2.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3367 b- defN 23-Jun-07 14:02 e2eqavn-2.3.dist-info/RECORD
+40 files, 105149 bytes uncompressed, 30337 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -99,23 +99,23 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_chunking.py
 Comment: 
 
-Filename: e2eqavn-2.2.dist-info/METADATA
+Filename: e2eqavn-2.3.dist-info/METADATA
 Comment: 
 
-Filename: e2eqavn-2.2.dist-info/WHEEL
+Filename: e2eqavn-2.3.dist-info/WHEEL
 Comment: 
 
-Filename: e2eqavn-2.2.dist-info/entry_points.txt
+Filename: e2eqavn-2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: e2eqavn-2.2.dist-info/top_level.txt
+Filename: e2eqavn-2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: e2eqavn-2.2.dist-info/RECORD
+Filename: e2eqavn-2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## e2eqavn/__init__.py

```diff
@@ -16,9 +16,9 @@
 
 stream_handler.setFormatter(formatted)
 logger.addHandler(stream_handler)
 logger.setLevel(logging.INFO)
 logger.propagate = False
 
 __author__ = 'khanhdm'
-__version__ = '2.2'
+__version__ = '2.3'
```

## Comparing `e2eqavn-2.2.dist-info/METADATA` & `e2eqavn-2.3.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2eqavn
-Version: 2.2
+Version: 2.3
 Summary: e2eqavn is end to end pipeline for question answering
 Author: khanhdm
 Author-email: khanhc1k36@gmail.com
 Requires-Python: >3.6.0
 Requires-Dist: numpy
 Requires-Dist: PyYAML
 Requires-Dist: sentence-transformers
@@ -20,8 +20,9 @@
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: accelerate
 Requires-Dist: protobuf (==3.20)
 Requires-Dist: colorlog
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
+Requires-Dist: pymongo[srv]
```

## Comparing `e2eqavn-2.2.dist-info/RECORD` & `e2eqavn-2.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-e2eqavn/__init__.py,sha256=RtpYQtJhM6lSCIOlq0LV3qkwHGg92yhRC7d2hw4Qnuk,496
+e2eqavn/__init__.py,sha256=t6-eteS47JcH0VwXcsZUHgFdYgaCqjvba9cgNAyTlPE,496
 e2eqavn/cli.py,sha256=VzQxgKWkDt-hiqJx3tSAzlzwRZ82MwvnZcX0JnHWO48,7061
 e2eqavn/keywords.py,sha256=HzbuUmSAh1lZemWm4GHiQo3VZ5tN4kBZIhJS9_BPvfo,2472
 e2eqavn/datasets/MRCDataset.py,sha256=q0TDZ0dOR3O63hzzD_b1mAkPSb7jpHpnh5ywuJIXOuA,2973
 e2eqavn/datasets/TripletDataset.py,sha256=UalsiPb-sVq79gE923C_Gu8mqih_KJ-NCAI2MEV-VCY,1386
 e2eqavn/datasets/__init__.py,sha256=PVd6KkEbmwFhGlSdv8lCnLcyIT6MrIOU2zeLEDnNBQM,124
 e2eqavn/datasets/data_collator.py,sha256=i1eE-WHBmLH2uI8CIv-WZpAjhzwbKTwTtgr9Ytw5FAA,3660
 e2eqavn/documents/__init__.py,sha256=KhJ-7DiMYhKRaNBXpMFooJ4EioOOXKxFqjTVB__1JG8,85
@@ -29,12 +29,12 @@
 e2eqavn/retrieval/sbert_retrieval.py,sha256=KhdDq2CBF_E9nhWpQExyNtcjQOtxvOaZybj1ZAV7idQ,10419
 e2eqavn/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 e2eqavn/utils/calculate.py,sha256=dFQCipyqcBWlQeq_aQgON2Rg06rYjMhfzByYtUSjifQ,12402
 e2eqavn/utils/io.py,sha256=StKqF8nRhuApqlI0vPlme8Y50Do4epId8KeW4oJ5uTI,603
 e2eqavn/utils/preprocess.py,sha256=1yhNSGZ5FRzIglW0IRiZyxS1b3Rr5CNzLN78lQsRQjQ,998
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_chunking.py,sha256=tW3Cg_Ll8mtfYjmPmNy5MgElUSe8eIKhcWAND20SRDA,334
-e2eqavn-2.2.dist-info/METADATA,sha256=IgH-zvJu9pQngAZg61ZCqS-7gtS8xSol5-04Unn5ldc,649
-e2eqavn-2.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-e2eqavn-2.2.dist-info/entry_points.txt,sha256=pPUmMeBtyeitA4rbQwBo_glm5HRGPLREjN9eeAGu_Bk,52
-e2eqavn-2.2.dist-info/top_level.txt,sha256=Qu5Dlk8CtzRo5i3_O722D1zBatiVaNkiPAbSDCOA2pA,13
-e2eqavn-2.2.dist-info/RECORD,,
+e2eqavn-2.3.dist-info/METADATA,sha256=jgqlCCQJZBcrxYQBgHx6LIpfEwsixr6UBwr0OxU_zV4,677
+e2eqavn-2.3.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+e2eqavn-2.3.dist-info/entry_points.txt,sha256=pPUmMeBtyeitA4rbQwBo_glm5HRGPLREjN9eeAGu_Bk,52
+e2eqavn-2.3.dist-info/top_level.txt,sha256=Qu5Dlk8CtzRo5i3_O722D1zBatiVaNkiPAbSDCOA2pA,13
+e2eqavn-2.3.dist-info/RECORD,,
```

