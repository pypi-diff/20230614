# Comparing `tmp/lk_logger-5.6.0-py3-none-any.whl.zip` & `tmp/lk_logger-5.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 37921 bytes, number of entries: 25
+Zip file size: 37980 bytes, number of entries: 25
 -rw-r--r--  2.0 unx      592 b- defN 80-Jan-01 00:00 lk_logger/__init__.py
 -rw-r--r--  2.0 unx      591 b- defN 80-Jan-01 00:00 lk_logger/_print.py
 -rw-r--r--  2.0 unx     1815 b- defN 80-Jan-01 00:00 lk_logger/cache.py
 -rw-r--r--  2.0 unx     5487 b- defN 80-Jan-01 00:00 lk_logger/config.py
 -rw-r--r--  2.0 unx     1563 b- defN 80-Jan-01 00:00 lk_logger/console.py
 -rw-r--r--  2.0 unx     4540 b- defN 80-Jan-01 00:00 lk_logger/control.py
 -rw-r--r--  2.0 unx     7360 b- defN 80-Jan-01 00:00 lk_logger/frame_info.py
 -rw-r--r--  2.0 unx    13617 b- defN 80-Jan-01 00:00 lk_logger/logger.py
 -rw-r--r--  2.0 unx    10446 b- defN 80-Jan-01 00:00 lk_logger/markup.py
--rw-r--r--  2.0 unx     7383 b- defN 80-Jan-01 00:00 lk_logger/message_builder.py
+-rw-r--r--  2.0 unx     7488 b- defN 80-Jan-01 00:00 lk_logger/message_builder.py
 -rw-r--r--  2.0 unx    10793 b- defN 80-Jan-01 00:00 lk_logger/message_formatter.py
 -rw-r--r--  2.0 unx     4034 b- defN 80-Jan-01 00:00 lk_logger/path_helper.py
 -rw-r--r--  2.0 unx     2559 b- defN 80-Jan-01 00:00 lk_logger/pipeline.py
 -rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 lk_logger/scanner/__init__.py
 -rw-r--r--  2.0 unx     6247 b- defN 80-Jan-01 00:00 lk_logger/scanner/analyser.py
 -rw-r--r--  2.0 unx     1128 b- defN 80-Jan-01 00:00 lk_logger/scanner/const.py
 -rw-r--r--  2.0 unx     1780 b- defN 80-Jan-01 00:00 lk_logger/scanner/exceptions.py
 -rw-r--r--  2.0 unx     9594 b- defN 80-Jan-01 00:00 lk_logger/scanner/scanner.py
 -rw-r--r--  2.0 unx     3238 b- defN 80-Jan-01 00:00 lk_logger/scanner/symbols.py
 -rw-r--r--  2.0 unx    19638 b- defN 80-Jan-01 00:00 lk_logger/scanner/text_scanner.py
 -rw-r--r--  2.0 unx      491 b- defN 80-Jan-01 00:00 lk_logger/scanner/typehint.py
 -rw-r--r--  2.0 unx      860 b- defN 80-Jan-01 00:00 lk_logger/shunt.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_logger-5.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx     4884 b- defN 80-Jan-01 00:00 lk_logger-5.6.0.dist-info/METADATA
-?rw-r--r--  2.0 unx     1996 b- defN 16-Jan-01 00:00 lk_logger-5.6.0.dist-info/RECORD
-25 files, 120795 bytes uncompressed, 34741 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_logger-5.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx     4884 b- defN 80-Jan-01 00:00 lk_logger-5.6.1.dist-info/METADATA
+?rw-r--r--  2.0 unx     1996 b- defN 16-Jan-01 00:00 lk_logger-5.6.1.dist-info/RECORD
+25 files, 120900 bytes uncompressed, 34800 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -60,17 +60,17 @@
 
 Filename: lk_logger/scanner/typehint.py
 Comment: 
 
 Filename: lk_logger/shunt.py
 Comment: 
 
-Filename: lk_logger-5.6.0.dist-info/WHEEL
+Filename: lk_logger-5.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: lk_logger-5.6.0.dist-info/METADATA
+Filename: lk_logger-5.6.1.dist-info/METADATA
 Comment: 
 
-Filename: lk_logger-5.6.0.dist-info/RECORD
+Filename: lk_logger-5.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lk_logger/__init__.py

```diff
@@ -17,8 +17,8 @@
 def __init():
     import traceback
     pipeline.add(traceback, bprint)
     setup(quiet=True)
 
 
 __init()
-__version__ = '5.6.0'
+__version__ = '5.6.1'
```

## lk_logger/message_builder.py

```diff
@@ -45,16 +45,18 @@
     _separator_b: Text
     
     def __init__(self, **kwargs) -> None:
         self.update_config(**kwargs)
     
     def update_config(self, **config) -> None:
         # https://fsymbols.com/signs/arrow/
-        self._separator_a = Text(' ➤ ', 'bright_black')
+        self._separator_a = Text('  ➤ ', 'bright_black')
         #   alternatives: ➤ ⪢ >> ⮕ -> ~> | │
+        #   note: if we use single char, make sure there are two whitespaces
+        #       before it.
         self._separator_b = Text(
             config.get('separator', ';   '), 'bright_black')
     
     # -------------------------------------------------------------------------
     
     def compose(
             self,
```

## Comparing `lk_logger-5.6.0.dist-info/METADATA` & `lk_logger-5.6.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lk-logger
-Version: 5.6.0
+Version: 5.6.1
 Summary: Python advanced print with varnames.
 Home-page: https://github.com/likianta/lk-logger
 License: MIT
 Author: Likianta
 Author-email: likianta@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `lk_logger-5.6.0.dist-info/RECORD` & `lk_logger-5.6.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-lk_logger/__init__.py,sha256=PDvdrJlKEL6SPrj_2Xyww6DTCcWX27aaPBGzsdV8O2w,592
+lk_logger/__init__.py,sha256=Oq_DtanPTD5Y-HeLXCK2wBvZoujKoyoZt2BsZo2SFns,592
 lk_logger/_print.py,sha256=Q0WdJ-TxOcQy1aKxEgaxaCrixq9GdXqQVF7YTw-jELo,591
 lk_logger/cache.py,sha256=83bH8DTfZszNt5X59nLQcvYG07h23J83HB4FpQ7UoOY,1815
 lk_logger/config.py,sha256=mmM6x2vlR5setLz_5dhWKHzwL4tvY-oESsNDl5FOLr4,5487
 lk_logger/console.py,sha256=GSoFWXBybfNuF7S7b3_OJL70h52OSlTPnCbpay1pL60,1563
 lk_logger/control.py,sha256=wEGJzOOb4KE2dMVBnpC-IHRDCaMBCx7N3Tii8NUd8qU,4540
 lk_logger/frame_info.py,sha256=PzuZL0DkCmly8z061ZyeAMdgEY9cfurL4WhlBGa4cB0,7360
 lk_logger/logger.py,sha256=w1sPcYrzdcuxIkvpJ78gUnJLE4HgvuZ4cgjMlKK2Cv0,13617
 lk_logger/markup.py,sha256=FIDjNJ-q-Fb3T2FDCjhMDwyUrkH1mdY5_nFE1bSze20,10446
-lk_logger/message_builder.py,sha256=TvhZayAp5a2wDULiW84_Lg4zXg98h-aFSI9Xz0FmrLA,7383
+lk_logger/message_builder.py,sha256=0nnOnbxE4uDHYz7bQ2oLJMxJx_1E9vCCH_NOQavrqXQ,7488
 lk_logger/message_formatter.py,sha256=ZStrTjNUh0owDYnz-6jjzz347mC3jsLIklMFNqvkNhI,10793
 lk_logger/path_helper.py,sha256=LAZOe5XK_51I0YPA6rUuY0_DKtaMtHyz52xcHqRbxY0,4034
 lk_logger/pipeline.py,sha256=bo-Z9367i2TxxJOCS5_Rk_6CFccFyJYgp3-uw9q9LzQ,2559
 lk_logger/scanner/__init__.py,sha256=er6nQAKVaYpdk30878kEDo5vKTSa6CzR-CdxNJiaODo,71
 lk_logger/scanner/analyser.py,sha256=tbI48nDcBPthZoD8jlnpap7S6FIHs4u8pUMQpsmh6r4,6247
 lk_logger/scanner/const.py,sha256=pRfHUK2huF2oLkd-ZpGtGUKQ2T4K3EnlSI0pUGGnp6Q,1128
 lk_logger/scanner/exceptions.py,sha256=G1wpgEIzTLLrD6Q_m0qGD85v5KnlPm3CV1ZxgvGCVd8,1780
 lk_logger/scanner/scanner.py,sha256=7Ase1WyHD87cBr4k9zYehe9LgL91r0L1_XlgKHg1_Eg,9594
 lk_logger/scanner/symbols.py,sha256=ibW1-n7Xigo9LvowUSn6dIrx-UmiJyuxN321bSCilSg,3238
 lk_logger/scanner/text_scanner.py,sha256=84ese30Bh-H1ZVxT0jcNhsTwM1nLDkZOrUO1LSdjV6k,19638
 lk_logger/scanner/typehint.py,sha256=Vr929B1w9UGiLVEMIJJIyE6gULjd_NxmNVpssyZW_JI,491
 lk_logger/shunt.py,sha256=-2uc2STfSIABrY-yAC7qIBh3uBgEx0iL1CGB_9rcwzg,860
-lk_logger-5.6.0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-lk_logger-5.6.0.dist-info/METADATA,sha256=qx90GAC-In2d5a4QaG0LVwiBgjJ9EPs0HE0WpIUPMrs,4884
-lk_logger-5.6.0.dist-info/RECORD,,
+lk_logger-5.6.1.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+lk_logger-5.6.1.dist-info/METADATA,sha256=JD_5e5OVkVOLdEmM0yThI6hb-AcXllXjqT0rID_pibA,4884
+lk_logger-5.6.1.dist-info/RECORD,,
```

