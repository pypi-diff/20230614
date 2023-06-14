# Comparing `tmp/meteva_base-0.1.0-py3-none-any.whl.zip` & `tmp/meteva_base-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 207720 bytes, number of entries: 74
+Zip file size: 207719 bytes, number of entries: 74
 -rw-rw-rw-  2.0 fat      174 b- defN 23-Apr-17 06:52 meteva_base/__init__.py
 -rw-rw-rw-  2.0 fat      141 b- defN 23-Apr-17 02:32 meteva_base/basicdata/__init__.py
 -rw-rw-rw-  2.0 fat     1199 b- defN 23-Jun-05 03:42 meteva_base/basicdata/const.py
 -rw-rw-rw-  2.0 fat     7385 b- defN 23-May-26 02:34 meteva_base/basicdata/ctl.py
 -rw-rw-rw-  2.0 fat    19260 b- defN 23-May-26 02:38 meteva_base/basicdata/dicts.py
 -rw-rw-rw-  2.0 fat    11163 b- defN 23-May-26 02:39 meteva_base/basicdata/grid.py
 -rw-rw-rw-  2.0 fat    32561 b- defN 23-May-26 02:58 meteva_base/basicdata/grid_data.py
@@ -64,13 +64,13 @@
 -rw-rw-rw-  2.0 fat    11227 b- defN 23-May-26 09:45 meteva_base/tool/math_tools.py
 -rw-rw-rw-  2.0 fat    12506 b- defN 23-Apr-17 02:32 meteva_base/tool/path_tools.py
 -rw-rw-rw-  2.0 fat   174805 b- defN 23-May-26 10:00 meteva_base/tool/plot_tools.py
 -rw-rw-rw-  2.0 fat    33020 b- defN 23-May-29 02:32 meteva_base/tool/plot_tools_adv.py
 -rw-rw-rw-  2.0 fat     4851 b- defN 23-Apr-17 02:32 meteva_base/tool/process_tools.py
 -rw-rw-rw-  2.0 fat     3816 b- defN 23-Apr-17 03:21 meteva_base/tool/station_tools.py
 -rw-rw-rw-  2.0 fat     5637 b- defN 23-Apr-17 02:32 meteva_base/tool/time_tools.py
--rw-rw-rw-  2.0 fat     1084 b- defN 23-Jun-14 01:56 meteva_base-0.1.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      825 b- defN 23-Jun-14 01:56 meteva_base-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-14 01:56 meteva_base-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-14 01:56 meteva_base-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     6482 b- defN 23-Jun-14 01:56 meteva_base-0.1.0.dist-info/RECORD
-74 files, 1064739 bytes uncompressed, 197466 bytes compressed:  81.5%
+-rw-rw-rw-  2.0 fat     1084 b- defN 23-Jun-14 02:14 meteva_base-0.1.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      825 b- defN 23-Jun-14 02:14 meteva_base-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-14 02:14 meteva_base-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-14 02:14 meteva_base-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     6482 b- defN 23-Jun-14 02:14 meteva_base-0.1.1.dist-info/RECORD
+74 files, 1064739 bytes uncompressed, 197465 bytes compressed:  81.5%
```

## zipnote {}

```diff
@@ -201,23 +201,23 @@
 
 Filename: meteva_base/tool/station_tools.py
 Comment: 
 
 Filename: meteva_base/tool/time_tools.py
 Comment: 
 
-Filename: meteva_base-0.1.0.dist-info/LICENSE.txt
+Filename: meteva_base-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: meteva_base-0.1.0.dist-info/METADATA
+Filename: meteva_base-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: meteva_base-0.1.0.dist-info/WHEEL
+Filename: meteva_base-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: meteva_base-0.1.0.dist-info/top_level.txt
+Filename: meteva_base-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: meteva_base-0.1.0.dist-info/RECORD
+Filename: meteva_base-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `meteva_base-0.1.0.dist-info/LICENSE.txt` & `meteva_base-0.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `meteva_base-0.1.0.dist-info/METADATA` & `meteva_base-0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteva-base
-Version: 0.1.0
+Version: 0.1.1
 Summary: base classes and functions of generally meteorogical usage, like Basic_class/IO/calculation/plot .etc
 Home-page: https://github.com/nmcdev/nimm
 Author: NMC_WFT
 Author-email: pangzide003@163.com
 License: MIT
 Requires-Dist: numpy (>=1.12.1)
 Requires-Dist: pandas (>=1.0.4)
```

## Comparing `meteva_base-0.1.0.dist-info/RECORD` & `meteva_base-0.1.1.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -63,12 +63,12 @@
 meteva_base/tool/math_tools.py,sha256=rbCh1tuo-6sWmFIFPcNOp4iI7mUbs8pzuNzI0RsSU-Y,11227
 meteva_base/tool/path_tools.py,sha256=iETXtI5Iq1f6fQ0yQJGVY7b9qjJRtL1Xq-BB0oBbYMY,12506
 meteva_base/tool/plot_tools.py,sha256=13gxGqBMrP2v5EH3ogO76GVzbzULia8g5HcEKoY2SrE,174805
 meteva_base/tool/plot_tools_adv.py,sha256=U0pJXOFl4fDgoWm1wRTLz2V-MGWB_VgpFESzkKWPfc0,33020
 meteva_base/tool/process_tools.py,sha256=DpKhLfb-NV0GUQQb3Gi_eG2xIUpCKtHWacB71KDUWJY,4851
 meteva_base/tool/station_tools.py,sha256=SEoFV3yBw5P-TWU-YNBLvI8dIhidwMGUSneXBTs0778,3816
 meteva_base/tool/time_tools.py,sha256=jqaFz_9fqgMn_9SYUW8lkXZIdvFjZAY0bjZ3bD1uq9w,5637
-meteva_base-0.1.0.dist-info/LICENSE.txt,sha256=u_GdHH9sIW5vgd8k1u8G2AAB6XOX6MB4inY_CaH7JaI,1084
-meteva_base-0.1.0.dist-info/METADATA,sha256=JxR_fglCRZs_CjosCwRynVQ6B5W0gt6LNItQBJdOtT0,825
-meteva_base-0.1.0.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-meteva_base-0.1.0.dist-info/top_level.txt,sha256=9xoeyXk97X89uUwYj_XV9UeCopr5XPlyacoJqhTh03k,12
-meteva_base-0.1.0.dist-info/RECORD,,
+meteva_base-0.1.1.dist-info/LICENSE.txt,sha256=u_GdHH9sIW5vgd8k1u8G2AAB6XOX6MB4inY_CaH7JaI,1084
+meteva_base-0.1.1.dist-info/METADATA,sha256=fKStCCrxYzPCsg_-PcbYquDViJubXY8AGGF5o-LAgJ8,825
+meteva_base-0.1.1.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+meteva_base-0.1.1.dist-info/top_level.txt,sha256=9xoeyXk97X89uUwYj_XV9UeCopr5XPlyacoJqhTh03k,12
+meteva_base-0.1.1.dist-info/RECORD,,
```

