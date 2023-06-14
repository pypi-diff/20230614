# Comparing `tmp/e2eqavn-3.0-py2.py3-none-any.whl.zip` & `tmp/e2eqavn-3.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 36210 bytes, number of entries: 40
--rw-rw-r--  2.0 unx      496 b- defN 23-Jun-14 13:20 e2eqavn/__init__.py
--rw-rw-r--  2.0 unx     9282 b- defN 23-Jun-14 13:19 e2eqavn/cli.py
+Zip file size: 36201 bytes, number of entries: 40
+-rw-rw-r--  2.0 unx      496 b- defN 23-Jun-14 13:22 e2eqavn/__init__.py
+-rw-rw-r--  2.0 unx     9281 b- defN 23-Jun-14 13:22 e2eqavn/cli.py
 -rw-rw-r--  2.0 unx     2472 b- defN 23-May-25 07:49 e2eqavn/keywords.py
 -rw-rw-r--  2.0 unx     2973 b- defN 23-May-20 15:46 e2eqavn/datasets/MRCDataset.py
 -rw-rw-r--  2.0 unx     1386 b- defN 23-Apr-08 19:20 e2eqavn/datasets/TripletDataset.py
 -rw-rw-r--  2.0 unx      124 b- defN 23-May-02 14:04 e2eqavn/datasets/__init__.py
 -rw-rw-r--  2.0 unx     3660 b- defN 23-May-30 15:21 e2eqavn/datasets/data_collator.py
 -rw-rw-r--  2.0 unx       85 b- defN 23-Apr-08 14:59 e2eqavn/documents/__init__.py
 -rw-rw-r--  2.0 unx    12681 b- defN 23-Jun-12 11:14 e2eqavn/documents/corpus.py
@@ -30,13 +30,13 @@
 -rw-rw-r--  2.0 unx    10419 b- defN 23-May-25 09:03 e2eqavn/retrieval/sbert_retrieval.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-18 08:56 e2eqavn/utils/__init__.py
 -rw-rw-r--  2.0 unx    12493 b- defN 23-Jun-07 16:27 e2eqavn/utils/calculate.py
 -rw-rw-r--  2.0 unx      603 b- defN 23-May-31 16:18 e2eqavn/utils/io.py
 -rw-rw-r--  2.0 unx      998 b- defN 23-May-03 09:44 e2eqavn/utils/preprocess.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-19 07:27 test/__init__.py
 -rw-rw-r--  2.0 unx      334 b- defN 23-Apr-08 14:59 test/test_chunking.py
--rw-rw-r--  2.0 unx      677 b- defN 23-Jun-14 13:20 e2eqavn-3.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-14 13:20 e2eqavn-3.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       52 b- defN 23-Jun-14 13:20 e2eqavn-3.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       13 b- defN 23-Jun-14 13:20 e2eqavn-3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3367 b- defN 23-Jun-14 13:20 e2eqavn-3.0.dist-info/RECORD
-40 files, 107525 bytes uncompressed, 30814 bytes compressed:  71.3%
+-rw-rw-r--  2.0 unx      677 b- defN 23-Jun-14 13:22 e2eqavn-3.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-14 13:22 e2eqavn-3.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       52 b- defN 23-Jun-14 13:22 e2eqavn-3.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       13 b- defN 23-Jun-14 13:22 e2eqavn-3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3367 b- defN 23-Jun-14 13:22 e2eqavn-3.1.dist-info/RECORD
+40 files, 107524 bytes uncompressed, 30805 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -99,23 +99,23 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_chunking.py
 Comment: 
 
-Filename: e2eqavn-3.0.dist-info/METADATA
+Filename: e2eqavn-3.1.dist-info/METADATA
 Comment: 
 
-Filename: e2eqavn-3.0.dist-info/WHEEL
+Filename: e2eqavn-3.1.dist-info/WHEEL
 Comment: 
 
-Filename: e2eqavn-3.0.dist-info/entry_points.txt
+Filename: e2eqavn-3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: e2eqavn-3.0.dist-info/top_level.txt
+Filename: e2eqavn-3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: e2eqavn-3.0.dist-info/RECORD
+Filename: e2eqavn-3.1.dist-info/RECORD
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
-__version__ = '3.0'
+__version__ = '3.1'
```

## e2eqavn/cli.py

```diff
@@ -167,15 +167,15 @@
         predictions, ground_truth, list_questions = [], [], []
         ground_truth = []
         idx = 0
         for doc in eval_corpus.list_document:
             for pair_ques_ans in doc.list_pair_question_answers:
                 question = pair_ques_ans.question
                 list_questions.append(question)
-                answers = [ans[eval_corpus[ANSWER_KEY]] for ans in pair_ques_ans.list_dict_answer]
+                answers = [ans[eval_corpus.answer_key] for ans in pair_ques_ans.list_dict_answer]
                 ground_truth.append(
                     {
                         'answers': {'text': answers},
                         'id': str(idx)
                     }
                 )
                 idx += 1
```

## Comparing `e2eqavn-3.0.dist-info/METADATA` & `e2eqavn-3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2eqavn
-Version: 3.0
+Version: 3.1
 Summary: e2eqavn is end to end pipeline for question answering
 Author: khanhdm
 Author-email: khanhc1k36@gmail.com
 Requires-Python: >3.6.0
 Requires-Dist: numpy
 Requires-Dist: PyYAML
 Requires-Dist: sentence-transformers
```

## Comparing `e2eqavn-3.0.dist-info/RECORD` & `e2eqavn-3.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-e2eqavn/__init__.py,sha256=EsOFgP0GPlGhtJIAYUQIpcl9U3kUUt8TapwKDoJRG8Y,496
-e2eqavn/cli.py,sha256=kfbn6dXlkFinIG87sBZk42oW-ZK0c_IWRfVlu2ZY1fc,9282
+e2eqavn/__init__.py,sha256=dPM-sA6jn4B6zXvx__KcpdXiG-Sw_W4IYDj46RboGWk,496
+e2eqavn/cli.py,sha256=8bo-z8UBgm_0eiRxLFV3WOMFGfvkA_RDjQd0vDkw4Wc,9281
 e2eqavn/keywords.py,sha256=HzbuUmSAh1lZemWm4GHiQo3VZ5tN4kBZIhJS9_BPvfo,2472
 e2eqavn/datasets/MRCDataset.py,sha256=q0TDZ0dOR3O63hzzD_b1mAkPSb7jpHpnh5ywuJIXOuA,2973
 e2eqavn/datasets/TripletDataset.py,sha256=UalsiPb-sVq79gE923C_Gu8mqih_KJ-NCAI2MEV-VCY,1386
 e2eqavn/datasets/__init__.py,sha256=PVd6KkEbmwFhGlSdv8lCnLcyIT6MrIOU2zeLEDnNBQM,124
 e2eqavn/datasets/data_collator.py,sha256=i1eE-WHBmLH2uI8CIv-WZpAjhzwbKTwTtgr9Ytw5FAA,3660
 e2eqavn/documents/__init__.py,sha256=KhJ-7DiMYhKRaNBXpMFooJ4EioOOXKxFqjTVB__1JG8,85
 e2eqavn/documents/corpus.py,sha256=mKMcqgpmH8kYylhWI-fXVQ8Zp9hl-_o3V7-BvIkGfN8,12681
@@ -29,12 +29,12 @@
 e2eqavn/retrieval/sbert_retrieval.py,sha256=KhdDq2CBF_E9nhWpQExyNtcjQOtxvOaZybj1ZAV7idQ,10419
 e2eqavn/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 e2eqavn/utils/calculate.py,sha256=yf5HPZyPodws38PNr2Zl3u7aqe_MTfQt1kAE0wHxuSk,12493
 e2eqavn/utils/io.py,sha256=StKqF8nRhuApqlI0vPlme8Y50Do4epId8KeW4oJ5uTI,603
 e2eqavn/utils/preprocess.py,sha256=1yhNSGZ5FRzIglW0IRiZyxS1b3Rr5CNzLN78lQsRQjQ,998
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_chunking.py,sha256=tW3Cg_Ll8mtfYjmPmNy5MgElUSe8eIKhcWAND20SRDA,334
-e2eqavn-3.0.dist-info/METADATA,sha256=0-i6FAtvUXb4llCjNoKF6ORglZHzRb5yGLXl8qzOuOc,677
-e2eqavn-3.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-e2eqavn-3.0.dist-info/entry_points.txt,sha256=pPUmMeBtyeitA4rbQwBo_glm5HRGPLREjN9eeAGu_Bk,52
-e2eqavn-3.0.dist-info/top_level.txt,sha256=Qu5Dlk8CtzRo5i3_O722D1zBatiVaNkiPAbSDCOA2pA,13
-e2eqavn-3.0.dist-info/RECORD,,
+e2eqavn-3.1.dist-info/METADATA,sha256=Lm8g1yL6-VRX1lDNYn_TtgAiY2rjMXBa1XuNUw3WQ2U,677
+e2eqavn-3.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+e2eqavn-3.1.dist-info/entry_points.txt,sha256=pPUmMeBtyeitA4rbQwBo_glm5HRGPLREjN9eeAGu_Bk,52
+e2eqavn-3.1.dist-info/top_level.txt,sha256=Qu5Dlk8CtzRo5i3_O722D1zBatiVaNkiPAbSDCOA2pA,13
+e2eqavn-3.1.dist-info/RECORD,,
```

