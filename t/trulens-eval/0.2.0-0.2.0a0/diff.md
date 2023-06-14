# Comparing `tmp/trulens_eval-0.2.0-py3-none-any.whl.zip` & `tmp/trulens_eval-0.2.0a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 83643 bytes, number of entries: 32
+Zip file size: 83667 bytes, number of entries: 32
 -rw-rw-r--  2.0 unx     4799 b- defN 23-Jun-14 03:10 trulens_eval/Example_TruBot.py
 -rw-rw-r--  2.0 unx     3101 b- defN 23-Jun-14 03:10 trulens_eval/Leaderboard.py
--rw-rw-r--  2.0 unx     1136 b- defN 23-Jun-14 03:16 trulens_eval/__init__.py
+-rw-rw-r--  2.0 unx     1137 b- defN 23-Jun-14 03:12 trulens_eval/__init__.py
 -rw-rw-r--  2.0 unx     5401 b- defN 23-Jun-09 21:41 trulens_eval/benchmark.py
 -rw-rw-r--  2.0 unx     3443 b- defN 23-Jun-09 21:41 trulens_eval/feedback_prompts.py
 -rw-rw-r--  2.0 unx    18056 b- defN 23-Jun-14 03:10 trulens_eval/instruments.py
 -rw-rw-r--  2.0 unx      985 b- defN 23-Jun-09 21:41 trulens_eval/keys.py
 -rw-rw-r--  2.0 unx     3376 b- defN 23-Jun-14 03:10 trulens_eval/provider_apis.py
 -rw-rw-r--  2.0 unx     9474 b- defN 23-Jun-14 03:10 trulens_eval/schema.py
 -rw-rw-r--  2.0 unx    11241 b- defN 23-Jun-14 03:10 trulens_eval/slackbot.py
@@ -23,12 +23,12 @@
 -rw-rw-r--  2.0 unx     3828 b- defN 23-Jun-14 03:10 trulens_eval/utils/langchain.py
 -rw-rw-r--  2.0 unx     1450 b- defN 23-Jun-14 03:10 trulens_eval/utils/llama.py
 -rw-rw-r--  2.0 unx     1001 b- defN 23-Jun-14 03:10 trulens_eval/utils/notebook_utils.py
 -rw-rw-r--  2.0 unx      915 b- defN 23-Jun-09 21:41 trulens_eval/ux/add_logo.py
 -rw-rw-r--  2.0 unx     3511 b- defN 23-Jun-14 03:10 trulens_eval/ux/components.py
 -rw-rw-r--  2.0 unx     1213 b- defN 23-Jun-09 21:41 trulens_eval/ux/styles.py
 -rw-rw-r--  2.0 unx    29567 b- defN 23-Jun-09 21:41 trulens_eval/ux/trulens_logo.svg
--rw-rw-r--  2.0 unx    14320 b- defN 23-Jun-14 03:16 trulens_eval-0.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-14 03:16 trulens_eval-0.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 23-Jun-14 03:16 trulens_eval-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2675 b- defN 23-Jun-14 03:16 trulens_eval-0.2.0.dist-info/RECORD
-32 files, 254551 bytes uncompressed, 79377 bytes compressed:  68.8%
+-rw-rw-r--  2.0 unx    14322 b- defN 23-Jun-14 03:14 trulens_eval-0.2.0a0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-14 03:14 trulens_eval-0.2.0a0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       13 b- defN 23-Jun-14 03:14 trulens_eval-0.2.0a0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2683 b- defN 23-Jun-14 03:14 trulens_eval-0.2.0a0.dist-info/RECORD
+32 files, 254562 bytes uncompressed, 79385 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -78,20 +78,20 @@
 
 Filename: trulens_eval/ux/styles.py
 Comment: 
 
 Filename: trulens_eval/ux/trulens_logo.svg
 Comment: 
 
-Filename: trulens_eval-0.2.0.dist-info/METADATA
+Filename: trulens_eval-0.2.0a0.dist-info/METADATA
 Comment: 
 
-Filename: trulens_eval-0.2.0.dist-info/WHEEL
+Filename: trulens_eval-0.2.0a0.dist-info/WHEEL
 Comment: 
 
-Filename: trulens_eval-0.2.0.dist-info/top_level.txt
+Filename: trulens_eval-0.2.0a0.dist-info/top_level.txt
 Comment: 
 
-Filename: trulens_eval-0.2.0.dist-info/RECORD
+Filename: trulens_eval-0.2.0a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trulens_eval/__init__.py

```diff
@@ -27,15 +27,15 @@
     - `provider_apis.py` `feedback_prompts.py`
 
     - `schema.py`
 
     - `util.py` `keys.py`
 """
 
-__version__ = "0.2.0"
+__version__ = "0.2.0a"
 
 from trulens_eval.schema import FeedbackMode
 from trulens_eval.schema import Query
 from trulens_eval.tru import Tru
 from trulens_eval.tru_chain import TruChain
 from trulens_eval.tru_feedback import Feedback
 from trulens_eval.tru_feedback import Huggingface
```

## Comparing `trulens_eval-0.2.0.dist-info/METADATA` & `trulens_eval-0.2.0a0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trulens-eval
-Version: 0.2.0
+Version: 0.2.0a0
 Summary: Library with langchain instrumentation to evaluate LLM based applications.
 Home-page: https://www.trulens.org
 Author: Truera Inc
 Author-email: all@truera.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

## Comparing `trulens_eval-0.2.0.dist-info/RECORD` & `trulens_eval-0.2.0a0.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 trulens_eval/Example_TruBot.py,sha256=5kJxiRuRcEteSZBjReD92yVHSrW4iuJQb2thiVWiaQQ,4799
 trulens_eval/Leaderboard.py,sha256=mfoILz_zmw_XyOXk7afm6iWwRUFb4YxRjADgXwjMm1s,3101
-trulens_eval/__init__.py,sha256=JBxgbuLAGPrtb2ml0YUYvuH7wdfzGpt7rEmHo0YY_mo,1136
+trulens_eval/__init__.py,sha256=PIqjmGmYanF9qTxSkuT0O0Ia3QffFBpuiZtaGaOwGwc,1137
 trulens_eval/benchmark.py,sha256=LHVnqYTudYpOJ2iry7De41jLfO2FImZqprUlaUkOiKA,5401
 trulens_eval/feedback_prompts.py,sha256=DgW4_f_4g018tYNwca1D1taJhhdwaf2fDR9J8s0Upls,3443
 trulens_eval/instruments.py,sha256=c16xGkLGReoJKwsyvWzIm0NpHULZghQ4ALGlubuhtig,18056
 trulens_eval/keys.py,sha256=n8v1LSi9u25RZe1EkhNULdUmMrvupce9C96i0rNYcnE,985
 trulens_eval/provider_apis.py,sha256=IRJrJiOs7Effjn-VtFwTONde0oGfUyGyzihDMi_wKM4,3376
 trulens_eval/schema.py,sha256=6arjAS-ouNAg_pj5kckyLsdRvs2FkHqNmdJHcy-dwSU,9474
 trulens_eval/slackbot.py,sha256=pTOIUlBcwEOeo98l1oMTSU8Ho46bGr0bcqAxqtmwsvA,11241
@@ -22,11 +22,11 @@
 trulens_eval/utils/langchain.py,sha256=GfeKB88ZHyN833pMQoHGCnZUehOmfNj2z1DDqj9LjeU,3828
 trulens_eval/utils/llama.py,sha256=ktDJNoM4wrUyJb2cUYLulgueqOp9pLKiuD5GNAetGeQ,1450
 trulens_eval/utils/notebook_utils.py,sha256=QTB2tedjSNF5d25sfrJEg20aqcK3Kx3MfcteeWcRzxQ,1001
 trulens_eval/ux/add_logo.py,sha256=Pwl6mfzAX1VSi2VTOZsMBoCstaBuVGoSrs7P5tomP4U,915
 trulens_eval/ux/components.py,sha256=8Cdus2FCcAHDHSI2-Hrt9zM_GZx7JWVfzXI-5qhuxwI,3511
 trulens_eval/ux/styles.py,sha256=23_Chwh8W8JzJiur_wa2GHJYkQ9rYovTWIEgLdUKuRM,1213
 trulens_eval/ux/trulens_logo.svg,sha256=92RLTgG0YDPEtZcQWWI7aXTYZAW4wAOAkIIgKUbTiW8,29567
-trulens_eval-0.2.0.dist-info/METADATA,sha256=OJEB0tXy6zN9q9JFdlpmmU7M2WrjZMtLSwH9KDFWEG8,14320
-trulens_eval-0.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-trulens_eval-0.2.0.dist-info/top_level.txt,sha256=AKIBExe5S-v-TbsBrhe1ctF06PubKoYmWNS9rJ1Rb_o,13
-trulens_eval-0.2.0.dist-info/RECORD,,
+trulens_eval-0.2.0a0.dist-info/METADATA,sha256=yPqTEKlBS3sLz2Zlu8yla4OGsg0Nn9aZzFTQ7cH520M,14322
+trulens_eval-0.2.0a0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+trulens_eval-0.2.0a0.dist-info/top_level.txt,sha256=AKIBExe5S-v-TbsBrhe1ctF06PubKoYmWNS9rJ1Rb_o,13
+trulens_eval-0.2.0a0.dist-info/RECORD,,
```

