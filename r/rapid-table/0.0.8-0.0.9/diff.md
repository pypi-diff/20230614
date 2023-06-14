# Comparing `tmp/rapid_table-0.0.8-py3-none-any.whl.zip` & `tmp/rapid_table-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 7076312 bytes, number of entries: 14
--rw-r--r--  2.0 unx      110 b- defN 23-Feb-12 06:42 rapid_table/__init__.py
--rw-r--r--  2.0 unx     3142 b- defN 23-Feb-12 06:42 rapid_table/rapid_table.py
+Zip file size: 7076416 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-19 02:02 rapid_table/__init__.py
+-rw-r--r--  2.0 unx     3142 b- defN 23-Apr-19 02:02 rapid_table/rapid_table.py
 -rw-r--r--  2.0 unx  7704409 b- defN 22-Dec-19 09:03 rapid_table/models/en_ppstructure_mobile_v2_SLANet.onnx
--rw-r--r--  2.0 unx      106 b- defN 23-Feb-12 06:42 rapid_table/table_matcher/__init__.py
--rw-r--r--  2.0 unx     6670 b- defN 23-Feb-12 06:42 rapid_table/table_matcher/matcher.py
--rw-r--r--  2.0 unx    10045 b- defN 23-Feb-12 06:42 rapid_table/table_matcher/utils.py
--rw-r--r--  2.0 unx      653 b- defN 23-Feb-12 06:42 rapid_table/table_structure/__init__.py
--rw-r--r--  2.0 unx     1945 b- defN 23-Feb-12 06:42 rapid_table/table_structure/table_structure.py
--rw-r--r--  2.0 unx    12116 b- defN 23-Feb-12 06:42 rapid_table/table_structure/utils.py
--rw-r--r--  2.0 unx     4568 b- defN 23-Feb-12 06:43 rapid_table-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-12 06:43 rapid_table-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 23-Feb-12 06:43 rapid_table-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Feb-12 06:43 rapid_table-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1260 b- defN 23-Feb-12 06:43 rapid_table-0.0.8.dist-info/RECORD
-14 files, 7745189 bytes uncompressed, 7074186 bytes compressed:  8.7%
+-rw-r--r--  2.0 unx      106 b- defN 23-Apr-19 02:02 rapid_table/table_matcher/__init__.py
+-rw-r--r--  2.0 unx     6670 b- defN 23-Apr-19 02:02 rapid_table/table_matcher/matcher.py
+-rw-r--r--  2.0 unx    10045 b- defN 23-Apr-19 02:02 rapid_table/table_matcher/utils.py
+-rw-r--r--  2.0 unx      653 b- defN 23-Apr-19 02:02 rapid_table/table_structure/__init__.py
+-rw-r--r--  2.0 unx     1945 b- defN 23-Apr-19 02:02 rapid_table/table_structure/table_structure.py
+-rw-r--r--  2.0 unx    12116 b- defN 23-Apr-19 02:02 rapid_table/table_structure/utils.py
+-rw-r--r--  2.0 unx     4883 b- defN 23-Apr-19 02:03 rapid_table-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 02:03 rapid_table-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 23-Apr-19 02:03 rapid_table-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-19 02:03 rapid_table-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1260 b- defN 23-Apr-19 02:03 rapid_table-0.0.9.dist-info/RECORD
+14 files, 7745504 bytes uncompressed, 7074290 bytes compressed:  8.7%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: rapid_table/table_structure/table_structure.py
 Comment: 
 
 Filename: rapid_table/table_structure/utils.py
 Comment: 
 
-Filename: rapid_table-0.0.8.dist-info/METADATA
+Filename: rapid_table-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: rapid_table-0.0.8.dist-info/WHEEL
+Filename: rapid_table-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_table-0.0.8.dist-info/entry_points.txt
+Filename: rapid_table-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_table-0.0.8.dist-info/top_level.txt
+Filename: rapid_table-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_table-0.0.8.dist-info/RECORD
+Filename: rapid_table-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rapid_table-0.0.8.dist-info/RECORD` & `rapid_table-0.0.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 rapid_table/models/en_ppstructure_mobile_v2_SLANet.onnx,sha256=LK4X0WoW-d9yKeIWZf4_vgbzyoWyAkdy7j4xQulVqmA,7704409
 rapid_table/table_matcher/__init__.py,sha256=MG5RnW1TllQdYPDoCEAWjhcAKEez44kaNHegLOW--Gk,106
 rapid_table/table_matcher/matcher.py,sha256=A8gVZ2XQJqWA87HK5b-_Ql8raY94rauS9g3QOjnha6w,6670
 rapid_table/table_matcher/utils.py,sha256=sqOCUuelNGzbfvs7mb8JHbKmn-pvNjQtHp2fhgDG6Fs,10045
 rapid_table/table_structure/__init__.py,sha256=N_1OGAgiMrF4LB5_sP_OSOrh6pnBGZrrnph8RfQ3VHA,653
 rapid_table/table_structure/table_structure.py,sha256=0QyKU9c6J-H5kCGET09NVjkHV-xa5pMC-JERvMnY-Ow,1945
 rapid_table/table_structure/utils.py,sha256=_aeKapmhI_U-DzmizrhyTZ4iK8YD-eefS3pFKuUy_oQ,12116
-rapid_table-0.0.8.dist-info/METADATA,sha256=zqQXXYslm4YRhuTgjHRuFty3blnenpU6vhqEvn_NSEg,4568
-rapid_table-0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-rapid_table-0.0.8.dist-info/entry_points.txt,sha256=a4UsMSxd7Ex1mZvdIT5AmkuiUAvB__awLj-NeYU8bsQ,61
-rapid_table-0.0.8.dist-info/top_level.txt,sha256=DkBPZpaze8SaoAvCufxilNpITY4n-rHH1lgHr6KHPgA,12
-rapid_table-0.0.8.dist-info/RECORD,,
+rapid_table-0.0.9.dist-info/METADATA,sha256=iH6zLmmBuOa8ZrNyvKBy3BLorndQup0wUCQmq6eJJFE,4883
+rapid_table-0.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rapid_table-0.0.9.dist-info/entry_points.txt,sha256=a4UsMSxd7Ex1mZvdIT5AmkuiUAvB__awLj-NeYU8bsQ,61
+rapid_table-0.0.9.dist-info/top_level.txt,sha256=DkBPZpaze8SaoAvCufxilNpITY4n-rHH1lgHr6KHPgA,12
+rapid_table-0.0.9.dist-info/RECORD,,
```

