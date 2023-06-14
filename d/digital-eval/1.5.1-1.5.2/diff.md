# Comparing `tmp/digital-eval-1.5.1.tar.gz` & `tmp/digital-eval-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-eval-1.5.1.tar", last modified: Mon Apr 17 09:32:25 2023, max compression
+gzip compressed data, was "digital-eval-1.5.2.tar", last modified: Wed Jun  7 14:35:46 2023, max compression
```

## Comparing `digital-eval-1.5.1.tar` & `digital-eval-1.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-04-17 09:32:25.754415 digital-eval-1.5.1/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1107 2022-07-13 13:34:42.000000 digital-eval-1.5.1/LICENSE
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       11 2022-11-16 10:06:15.000000 digital-eval-1.5.1/MANIFEST.in
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5495 2023-04-17 09:32:25.754415 digital-eval-1.5.1/PKG-INFO
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     4903 2023-04-17 09:05:33.000000 digital-eval-1.5.1/README.md
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       87 2022-11-15 13:27:11.000000 digital-eval-1.5.1/pyproject.toml
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      942 2023-04-17 09:32:25.758415 digital-eval-1.5.1/setup.cfg
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-04-17 09:32:25.754415 digital-eval-1.5.1/src/
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-04-17 09:32:25.754415 digital-eval-1.5.1/src/digital_eval/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        6 2023-04-17 09:31:50.000000 digital-eval-1.5.1/src/digital_eval/VERSION
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      609 2023-03-28 09:38:32.000000 digital-eval-1.5.1/src/digital_eval/__init__.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     7484 2022-11-15 13:27:11.000000 digital-eval-1.5.1/src/digital_eval/cli.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    28362 2023-03-28 09:38:32.000000 digital-eval-1.5.1/src/digital_eval/evaluation.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    16203 2023-04-17 08:22:56.000000 digital-eval-1.5.1/src/digital_eval/metrics.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    26481 2023-03-28 09:38:32.000000 digital-eval-1.5.1/src/digital_eval/model.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    14939 2022-11-15 13:27:11.000000 digital-eval-1.5.1/src/digital_eval/model_legacy.py
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-04-17 09:32:25.754415 digital-eval-1.5.1/src/digital_eval.egg-info/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5495 2023-04-17 09:32:25.000000 digital-eval-1.5.1/src/digital_eval.egg-info/PKG-INFO
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      559 2023-04-17 09:32:25.000000 digital-eval-1.5.1/src/digital_eval.egg-info/SOURCES.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        1 2023-04-17 09:32:25.000000 digital-eval-1.5.1/src/digital_eval.egg-info/dependency_links.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       86 2023-04-17 09:32:25.000000 digital-eval-1.5.1/src/digital_eval.egg-info/entry_points.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       31 2023-04-17 09:32:25.000000 digital-eval-1.5.1/src/digital_eval.egg-info/requires.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       22 2023-04-17 09:32:25.000000 digital-eval-1.5.1/src/digital_eval.egg-info/top_level.txt
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-04-17 09:32:25.754415 digital-eval-1.5.1/src/ocr_util/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       21 2023-03-28 09:38:32.000000 digital-eval-1.5.1/src/ocr_util/__init__.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     2690 2023-04-17 08:33:00.000000 digital-eval-1.5.1/src/ocr_util/cli.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     4120 2023-04-17 08:29:20.000000 digital-eval-1.5.1/src/ocr_util/frame.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-06-07 14:35:46.469941 digital-eval-1.5.2/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1107 2022-07-13 13:34:42.000000 digital-eval-1.5.2/LICENSE
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       11 2022-11-16 10:06:15.000000 digital-eval-1.5.2/MANIFEST.in
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5798 2023-06-07 14:35:46.469941 digital-eval-1.5.2/PKG-INFO
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5206 2023-04-17 10:19:40.000000 digital-eval-1.5.2/README.md
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       87 2022-11-15 13:27:11.000000 digital-eval-1.5.2/pyproject.toml
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      942 2023-06-07 14:35:46.469941 digital-eval-1.5.2/setup.cfg
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-06-07 14:35:46.461941 digital-eval-1.5.2/src/
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-06-07 14:35:46.465941 digital-eval-1.5.2/src/digital_eval/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        6 2023-06-07 14:00:52.000000 digital-eval-1.5.2/src/digital_eval/VERSION
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      617 2023-06-07 13:56:39.000000 digital-eval-1.5.2/src/digital_eval/__init__.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     8552 2023-06-07 14:00:16.000000 digital-eval-1.5.2/src/digital_eval/cli.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    28362 2023-03-28 09:38:32.000000 digital-eval-1.5.2/src/digital_eval/evaluation.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    17660 2023-06-07 14:05:05.000000 digital-eval-1.5.2/src/digital_eval/metrics.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    26481 2023-03-28 09:38:32.000000 digital-eval-1.5.2/src/digital_eval/model.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    14939 2022-11-15 13:27:11.000000 digital-eval-1.5.2/src/digital_eval/model_legacy.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-06-07 14:35:46.465941 digital-eval-1.5.2/src/digital_eval.egg-info/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5798 2023-06-07 14:35:46.000000 digital-eval-1.5.2/src/digital_eval.egg-info/PKG-INFO
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      559 2023-06-07 14:35:46.000000 digital-eval-1.5.2/src/digital_eval.egg-info/SOURCES.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        1 2023-06-07 14:35:46.000000 digital-eval-1.5.2/src/digital_eval.egg-info/dependency_links.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       86 2023-06-07 14:35:46.000000 digital-eval-1.5.2/src/digital_eval.egg-info/entry_points.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       31 2023-06-07 14:35:46.000000 digital-eval-1.5.2/src/digital_eval.egg-info/requires.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       22 2023-06-07 14:35:46.000000 digital-eval-1.5.2/src/digital_eval.egg-info/top_level.txt
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-06-07 14:35:46.465941 digital-eval-1.5.2/src/ocr_util/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       21 2023-03-28 09:38:32.000000 digital-eval-1.5.2/src/ocr_util/__init__.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     2690 2023-04-17 08:33:00.000000 digital-eval-1.5.2/src/ocr_util/cli.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     4120 2023-04-17 08:29:20.000000 digital-eval-1.5.2/src/ocr_util/frame.py
```

### Comparing `digital-eval-1.5.1/LICENSE` & `digital-eval-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `digital-eval-1.5.1/PKG-INFO` & `digital-eval-1.5.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-eval
-Version: 1.5.1
+Version: 1.5.2
 Summary: Evaluate Mass Digitalization Data
 Author: Universitäts- und Landesbibliothek Sachsen-Anhalt
 Author-email: development@bibliothek.uni-halle.de
 Maintainer: Uwe Hartwig
 Maintainer-email: uwe.hartwig@bibliothek.uni-halle.de
 Project-URL: Homepage, https://github.com/ulb-sachsen-anhalt/digital-eval
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # digital eval
 
 ![example workflow](https://github.com/ulb-sachsen-anhalt/digital-eval/actions/workflows/python-app.yml/badge.svg)
+[![PyPi version](https://badgen.net/pypi/v/digital-eval/)](https://pypi.org/project/digital-eval) ![PyPI - Downloads](https://img.shields.io/pypi/dm/digital-eval) ![PyPI - License](https://img.shields.io/pypi/l/digital-eval) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/digital-eval)
 
 Python3 Tool to report evaluation outcomes from mass digitalization workflows.
 
 ## Features
 
 * match automatically groundtruth (i.e. reference data) and candidates by filename
 * use geometric information to evaluate only specific frame (i.e. specific column or region from large page) of
```

### Comparing `digital-eval-1.5.1/README.md` & `digital-eval-1.5.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # digital eval
 
 ![example workflow](https://github.com/ulb-sachsen-anhalt/digital-eval/actions/workflows/python-app.yml/badge.svg)
+[![PyPi version](https://badgen.net/pypi/v/digital-eval/)](https://pypi.org/project/digital-eval) ![PyPI - Downloads](https://img.shields.io/pypi/dm/digital-eval) ![PyPI - License](https://img.shields.io/pypi/l/digital-eval) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/digital-eval)
 
 Python3 Tool to report evaluation outcomes from mass digitalization workflows.
 
 ## Features
 
 * match automatically groundtruth (i.e. reference data) and candidates by filename
 * use geometric information to evaluate only specific frame (i.e. specific column or region from large page) of
```

### Comparing `digital-eval-1.5.1/setup.cfg` & `digital-eval-1.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [options]
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 install_requires = 
-	rapidfuzz<3
+	rapidfuzz>3
 	numpy
 	nltk
 	shapely
 
 [options.packages.find]
 where = src
```

### Comparing `digital-eval-1.5.1/src/digital_eval/__init__.py` & `digital-eval-1.5.2/src/digital_eval/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     report_stdout,
     ocr_to_text,
 )
 
 from .metrics import (
     accuracy_for,
     error_for,
-    UC_NORMALIZATION,
+    UC_NORMALIZATION_DEFAULT,
     MetricChars,
     MetricLetters,
     MetricWords,
     MetricBoW,
     MetricIRPre,
     MetricIRRec,
     MetricIRFM,
```

### Comparing `digital-eval-1.5.1/src/digital_eval/cli.py` & `digital-eval-1.5.2/src/digital_eval/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,89 +4,105 @@
 import argparse
 import os
 import sys
 
 import datetime as dt
 
 from typing import (
-    List
+    List, Type
 )
 
 from digital_eval import (
     find_groundtruth,
     gather_candidates,
     Evaluator,
     report_stdout,
     ocr_to_text,
-    UC_NORMALIZATION,
+    UC_NORMALIZATION_DEFAULT,
     accuracy_for,
     error_for,
     MetricChars,
     MetricLetters,
     MetricWords,
     MetricBoW,
     MetricIRPre,
     MetricIRRec,
     MetricIRFM
 )
+from digital_eval.metrics import OCRDifferenceMetric, accuracy_for_bow, error_for_bow
 
 # script constants
 DEFAULT_VERBOSITY = 0
 VERBOSITY = DEFAULT_VERBOSITY
 EVAL_VERBOSITY = DEFAULT_VERBOSITY
 
 # calculations
 DEFAULT_CALCULCATION = 'acc'
 CALC_DICT = {
-    'acc' : accuracy_for,
-    'accuracy' : accuracy_for,
-    'err' : error_for, 
-    'error' : error_for,
+    'acc': accuracy_for,
+    'accuracy': accuracy_for,
+    'err': error_for,
+    'error': error_for,
 }
-DEFAULT_UTF8_NORM = UC_NORMALIZATION
+
+CALC_DICT_BOW = {
+    'acc': accuracy_for_bow,
+    'accuracy': accuracy_for_bow,
+    'err': error_for_bow,
+    'error': error_for_bow,
+}
+
+DEFAULT_UTF8_NORM = UC_NORMALIZATION_DEFAULT
 
 # metrics
 DEFAULT_OCR_METRICS = 'Cs,Ls'
 DEFAULT_OCR_METRIC_PREPROCESSINGS = ''
 DEFAULT_OCR_METRIC_POSTPROCESSINGS = ''
 METRIC_DICT = {
-    'Cs' : MetricChars,
-    'Characters' : MetricChars,
-    'Ls' : MetricLetters,
-    'Letters' : MetricLetters,
-    'Ws' : MetricWords,
-    'Words' : MetricWords,
-    'BoWs' : MetricBoW,
-    'BagOfWords' : MetricBoW,
-    'IRPre' : MetricIRPre,
+    'Cs': MetricChars,
+    'Characters': MetricChars,
+    'Ls': MetricLetters,
+    'Letters': MetricLetters,
+    'Ws': MetricWords,
+    'Words': MetricWords,
+    'BoWs': MetricBoW,
+    'BagOfWords': MetricBoW,
+    'IRPre': MetricIRPre,
     'Pre': MetricIRPre,
-    'Precision' : MetricIRPre,
-    'IRRec' : MetricIRRec,
+    'Precision': MetricIRPre,
+    'IRRec': MetricIRRec,
     'Rec': MetricIRRec,
-    'IRFMeasure' : MetricIRFM,
-    'FM' : MetricIRFM,
+    'IRFMeasure': MetricIRFM,
+    'FM': MetricIRFM,
 }
 
 
 def _get_info():
     here = os.path.abspath(os.path.dirname(__file__))
     _v = ''
     _t = ''
     _fp = os.path.join(here, 'VERSION')
     with open(_fp) as fp:
         _v = fp.read()
     _t = dt.datetime.fromtimestamp(os.stat(_fp).st_mtime).strftime("%Y-%m-%d")
     return f'v{_v}/{_t}'
 
 
-def _initialize_metrics(the_metrics, norm, calc) -> List:
+def _initialize_metrics(the_metrics, norm, calc) -> List[OCRDifferenceMetric]:
     _tokens = the_metrics.split(',')
     try:
-        return [METRIC_DICT[m](normalization=norm, calc_func=CALC_DICT[calc]) 
-                for m in _tokens]
+        metric_objects: List[OCRDifferenceMetric] = []
+        for m in _tokens:
+            clazz: Type[OCRDifferenceMetric] = METRIC_DICT[m]
+            calc_func = CALC_DICT[calc]
+            if m == 'BoWs' or m == 'BagOfWords':
+                calc_func = CALC_DICT_BOW[calc]
+            metric_inst: OCRDifferenceMetric = clazz(normalization=norm, calc_func=calc_func)
+            metric_objects.append(metric_inst)
+        return metric_objects
     except KeyError as _err:
         _keys = ','.join(METRIC_DICT.keys()) + ','.join(CALC_DICT.keys())
         _msg = f"Unknown: '{_err.args[0]}'.\nPlease use one of the following keys: '{_keys}'."
         print(_msg)
         sys.exit(1)
 
 
@@ -97,15 +113,15 @@
 
     # create basic evaluator instance
     evaluator = Evaluator(path_candidates, VERBOSITY, xtra)
     evaluator.metrics = _initialize_metrics(metrics, norm=utf8norm, calc=calc)
     evaluator.calc = calc
     if VERBOSITY >= 1:
         print(f"[DEBUG] text normalized using '{utf8norm}' calculate '{calc}' metric values for '{metrics}'")
-    
+
     if is_legacy:
         evaluator.to_text_func = ocr_to_text
     evaluator.is_sequential = is_sequential
     evaluator.domain_reference = path_reference
 
     # gather structure information
     candidates = gather_candidates(path_candidates)
@@ -119,15 +135,15 @@
         if gt:
             entry.path_g = gt
 
     # remove all paths where no groundtruth exists
     gt_entries = [c for c in candidates if c.path_g]
     n_entries = len(candidates)
     n_diff = n_entries - len(gt_entries)
-    gt_missing = set(gt_entries) ^ set (candidates)
+    gt_missing = set(gt_entries) ^ set(candidates)
     rnd_str = f" ({gt_missing})" if gt_missing else ""
     if VERBOSITY >= 1:
         print(f'[DEBUG] from "{n_entries}" filtered "{n_diff}" candidates missing groundtruth{rnd_str}')
 
     # trigger actual evaluation
     evaluator.eval_all(gt_entries)
 
@@ -146,57 +162,57 @@
 
 
 def start():
     PARSER = argparse.ArgumentParser(description=f"""
         Evaluate Mass Digital Data. ({_get_info()})
         """)
     PARSER.add_argument(
-        "candidates", 
+        "candidates",
         help="Root Directory to inspect"
-        )
-    PARSER.add_argument("-ref", "--reference", 
-        required=False,
-        help="Root Reference directory for Groundtruth or alike (optional)"
-        )
-    PARSER.add_argument("-v", "--VERBOSITY", 
-        action='count', 
-        default=DEFAULT_VERBOSITY,
-        required=False, 
-        help=f"Verbosity flag. To increase, append multiple 'v's (optional; default: '{DEFAULT_VERBOSITY}')"
-        )
-    PARSER.add_argument("--calc", 
-        default=DEFAULT_CALCULCATION,
-        required=False,
-        help=f"Calculation to perform (optional; default: '{DEFAULT_CALCULCATION}'; available: '{','.join(CALC_DICT.keys())}')"
-        )
+    )
+    PARSER.add_argument("-ref", "--reference",
+                        required=False,
+                        help="Root Reference directory for Groundtruth or alike (optional)"
+                        )
+    PARSER.add_argument("-v", "--VERBOSITY",
+                        action='count',
+                        default=DEFAULT_VERBOSITY,
+                        required=False,
+                        help=f"Verbosity flag. To increase, append multiple 'v's (optional; default: '{DEFAULT_VERBOSITY}')"
+                        )
+    PARSER.add_argument("--calc",
+                        default=DEFAULT_CALCULCATION,
+                        required=False,
+                        help=f"Calculation to perform (optional; default: '{DEFAULT_CALCULCATION}'; available: '{','.join(CALC_DICT.keys())}')"
+                        )
     # metrics
     PARSER.add_argument("--metrics",
-        default=DEFAULT_OCR_METRICS,
-        required=False, 
-        help=f"List of metrics to use (optional, default: '{DEFAULT_OCR_METRICS}'; available: '{','.join(METRIC_DICT.keys())}')"
-        )
-    PARSER.add_argument("--legacy", 
-        action='store_true',
-        required=False,
-        help="legacy evaluation with naive rectangular geometry (optional; default: 'False')", 
-        )
+                        default=DEFAULT_OCR_METRICS,
+                        required=False,
+                        help=f"List of metrics to use (optional, default: '{DEFAULT_OCR_METRICS}'; available: '{','.join(METRIC_DICT.keys())}')"
+                        )
+    PARSER.add_argument("--legacy",
+                        action='store_true',
+                        required=False,
+                        help="legacy evaluation with naive rectangular geometry (optional; default: 'False')",
+                        )
     PARSER.add_argument("--utf8",
-        default=DEFAULT_UTF8_NORM,
-        required=False,
-        help=f"UTF-8 Unicode Python Normalization (optional; default: '{DEFAULT_UTF8_NORM}'; available: 'NFC','NFKC','NFD','NFKD')",
-        )
-    PARSER.add_argument("--sequential", 
-        action='store_true',
-        required=False,
-        help="Execute calculations sequentially (optional; default: 'False')", 
-        )
-    PARSER.add_argument("-x", "--extra", 
-        required=False, 
-        help="pass additional information to evaluation, like 'ignore_geometry' (compare only text, ignore coords)"
-        )
+                        default=DEFAULT_UTF8_NORM,
+                        required=False,
+                        help=f"UTF-8 Unicode Python Normalization (optional; default: '{DEFAULT_UTF8_NORM}'; available: 'NFC','NFKC','NFD','NFKD')",
+                        )
+    PARSER.add_argument("--sequential",
+                        action='store_true',
+                        required=False,
+                        help="Execute calculations sequentially (optional; default: 'False')",
+                        )
+    PARSER.add_argument("-x", "--extra",
+                        required=False,
+                        help="pass additional information to evaluation, like 'ignore_geometry' (compare only text, ignore coords)"
+                        )
     PARSER.set_defaults(legacy=False)
     PARSER.set_defaults(sequential=False)
 
     ARGS = vars(PARSER.parse_args())
     path_candidates = ARGS["candidates"]
     path_reference = ARGS["reference"]
     global VERBOSITY
@@ -228,14 +244,15 @@
         if _base_can != _base_ref:
             print(f"[WARN ] start domains '{_base_can}' and '{_base_ref}' mismatch, summary might be inaccurate!")
 
     # some diagnostics
     if VERBOSITY >= 2:
         args = f"{path_candidates}, {path_reference}, {VERBOSITY}, {xtra}"
         print(f'[DEBUG] called with {args}')
-    
+
     # here we go
-    _main(path_candidates, path_reference, metrics, utf8norm, calc, xtra, is_legacy=IS_LEGACY, is_sequential=IS_SEQUENTIAL)
+    _main(path_candidates, path_reference, metrics, utf8norm, calc, xtra, is_legacy=IS_LEGACY,
+          is_sequential=IS_SEQUENTIAL)
 
 
 if __name__ == "__main__":
     start()
```

### Comparing `digital-eval-1.5.1/src/digital_eval/evaluation.py` & `digital-eval-1.5.2/src/digital_eval/evaluation.py`

 * *Files identical despite different names*

### Comparing `digital-eval-1.5.1/src/digital_eval/metrics.py` & `digital-eval-1.5.2/src/digital_eval/metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
 """Metrics Module"""
 
+from __future__ import annotations
+
 from collections import (
     Counter
 )
 from functools import partial
 
 import string
 
 from typing import (
     List,
-    Set,
+    Set, Callable,
 )
 
 import unicodedata
 
 from nltk import (
     download,
 )
@@ -23,71 +25,74 @@
 )
 from nltk.metrics import (
     recall,
     f_measure
 )
 from nltk.metrics import precision as nltk_precision
 
-from rapidfuzz.string_metric import (
-    levenshtein
+from rapidfuzz.distance import (
+    Levenshtein
 )
 
-
 # Python3 standard Unicode Normalization
 #
-UC_NORMALIZATION = 'NFKD'
-
+UC_NORMALIZATION_DEFAULT = 'NFC'
+UC_NORMALIZATION_NFKD = 'NFKD'
 
 # whitespaces
 #
 # usual spatium and special control sequences
 WHITESPACES = string.whitespace
 
+WHITESPACES_EXCLUDING_BLANK_CHARS = WHITESPACES[1:]
 
 # punctuations
 #
 #   * regular ASCII-punctuations
 #   * Dashes        \u2012-2017
 #   * Quotations    \u2018-201F
 PUNCTUATIONS = string.punctuation + '\u2012' + '\u2013' + '\u2014' + '\u2015' + '\u2016' + \
-    '\u2017' + '\u2018' + '\u2019' + '\u201A' + '\u201B' + \
-    '\u201C' + '\u201D' + '\u201E' + '\u201F'
+               '\u2017' + '\u2018' + '\u2019' + '\u201A' + '\u201B' + \
+               '\u201C' + '\u201D' + '\u201E' + '\u201F'
 # no special line break delimiter
 PUNCTUATIONS = PUNCTUATIONS + '\u2E17'  # DOUBLE OBLIQUE HYPHEN
 # no spaces
 PUNCTUATIONS = PUNCTUATIONS + '\u0020' + '\u00a0' + '\u2000' + \
-    '\u2001' + '\u2002' + '\u2003' + '\u2004' + '\u2005' + \
-    '\u2006' + '\u2007' + '\u2008' + '\u2009' + \
-    '\u200a' + '\u2028' + '\u205f' + '\u3000'
-
+               '\u2001' + '\u2002' + '\u2003' + '\u2004' + '\u2005' + \
+               '\u2006' + '\u2007' + '\u2008' + '\u2009' + \
+               '\u200a' + '\u2028' + '\u205f' + '\u3000'
 
 # digits
 #
 #   * ASCII digits
 #   * arabic digits
 #   * persian / indic digits
 DIGITS = string.digits + '\u0660' + '\u0661' + '\u0662' + '\u0663' + \
-    '\u0664' + '\u0665' + '\u0666' + '\u0667' + '\u0668' + '\u0669'
+         '\u0664' + '\u0665' + '\u0666' + '\u0667' + '\u0668' + '\u0669'
 # persian indic digits
 DIGITS = DIGITS + '\u06f0' + '\u06f1' + '\u06f2' + '\u06f3' + \
-    '\u06f4' + '\u06f5' + '\u06f6' + '\u06f7' + '\u06f8' + '\u06f9'
-
+         '\u06f4' + '\u06f5' + '\u06f6' + '\u06f7' + '\u06f8' + '\u06f9'
 
 # filter mechanics
 #
 # via Python3 string translation maps
 WHITESPACE_TRANSLATOR = str.maketrans('', '', WHITESPACES)
+WHITESPACE_EXCLUDING_BLANK_CHARS_TRANSLATOR = str.maketrans('', '', WHITESPACES_EXCLUDING_BLANK_CHARS)
 PUNCT_TRANLATOR = str.maketrans('', '', PUNCTUATIONS)
 DIGIT_TRANSLATOR = str.maketrans('', '', DIGITS)
 
 
 def _filter_whitespaces(a_str) -> str:
     return a_str.translate(WHITESPACE_TRANSLATOR)
 
 
+def _filter_whitespaces_excluding_blank_chars(a_str) -> str:
+    return a_str.translate(WHITESPACE_EXCLUDING_BLANK_CHARS_TRANSLATOR)
+
+
 def _filter_puncts(a_str) -> str:
     return a_str.translate(PUNCT_TRANLATOR)
 
 
 def _filter_digits(a_str) -> str:
     return a_str.translate(DIGIT_TRANSLATOR)
 
@@ -138,15 +143,15 @@
     return tokens - get_stopwords(languages=languages)
 
 
 def _strip_stopwords_for(languages):
     return partial(_strip_languages_stopwords, languages=languages)
 
 
-def normalize_unicode(input_str: str, uc_norm_by=UC_NORMALIZATION) -> str:
+def normalize_unicode(input_str: str, uc_norm_by=UC_NORMALIZATION_DEFAULT) -> str:
     """Apply basic unicode normalization
     """
 
     if uc_norm_by is not None:
         input_str = unicodedata.normalize(uc_norm_by, input_str)
     return input_str
 
@@ -179,75 +184,85 @@
             raise DigitalEvalMetricException(f"invalid diff: {_diff}!")
         if _ref is None or _ref < 0:
             raise DigitalEvalMetricException(f"invalid ref: {_ref}!")
     except AttributeError as _ae:
         raise DigitalEvalMetricException(_ae.args[0]) from _ae
 
 
-def accuracy_for(the_obj) -> float:
+def accuracy_for(metric_obj: OCRDifferenceMetric) -> float:
     """Calculate accuracy as ratio of
     correct items, with correct items
     being expected items minus
     number of differences.
 
     Respect following corner cases:
     * if less correct items than differences => 0
     * if both correct items and differences eq zero => 1
       means: nothing to find and it did detect nothing
       (i.e. no false-positives)
 
     Args:
-        the_obj (object): object containing information
+        metric_obj (OCRDifferenceMetric): object containing information
         about reference data and difference
 
     Returns:
         float: accuracy in range 0.0 - 1.0
     """
 
-    _inspect_calculation_object(the_obj)
-    diffs = the_obj.diff
-    n_refs = len(the_obj._data_reference)
-    if (n_refs - diffs) < 0:
-        return 0.0
-    if n_refs == 0 and diffs == 0:
-        return 1.0
-    elif n_refs > 0:
-        return (n_refs - diffs) / n_refs
-    else:
-        return 0.0
+    _inspect_calculation_object(metric_obj)
+    diffs = metric_obj.diff
+    n_refs = len(metric_obj._data_reference)
+    return _calculate(lambda d, n: (n - d) / n, diffs, n_refs)
+
 
+def error_for_bow(metric_obj: OCRDifferenceMetric) -> float:
+    _inspect_calculation_object(metric_obj)
+    diffs = metric_obj.diff
+    n_refs = len(metric_obj._data_reference) + len(metric_obj._data_candidate)
+    return _calculate(lambda d, n: d / n, diffs, n_refs)
 
-def error_for(the_obj) -> float:
+
+def accuracy_for_bow(metric_obj: OCRDifferenceMetric) -> float:
+    _inspect_calculation_object(metric_obj)
+    diffs = metric_obj.diff
+    n_refs = len(metric_obj._data_reference) + len(metric_obj._data_candidate)
+    return _calculate(lambda d, n: 1 - (d / n), diffs, n_refs)
+
+
+def error_for(metric_obj: OCRDifferenceMetric) -> float:
     """Calculate error as ratio of
     difference and number of
     expected items.
 
     Respect following corner cases:
     * if less expected items than differences => 0
     * if both expected items and differences eq zero => 1
       means: nothing to find and detected nothing
       (i.e. no false-positives)
 
     Args:
-        the_obj (object): object containing information
+        metric_obj (OCRDifferenceMetric): object containing information
         about reference data and difference
 
     Returns:
         float: error in range 0.0 - 1.0
     """
+    _inspect_calculation_object(metric_obj)
+    diffs = metric_obj.diff
+    n_refs = len(metric_obj._data_reference)
+    return _calculate(lambda d, n: d / n, diffs, n_refs)
 
-    _inspect_calculation_object(the_obj)
-    diffs = the_obj.diff
-    n_refs = len(the_obj._data_reference)
+
+def _calculate(calculate: Callable[[int, int], float], diffs: int, n_refs: int) -> float:
     if (n_refs - diffs) < 0:
         return 0.0
     if n_refs == 0 and diffs == 0:
         return 1.0
     elif n_refs > 0:
-        return diffs / n_refs
+        return calculate(diffs, n_refs)
     else:
         return 0.0
 
 
 def norm_to_scale(value, scale_by) -> float:
     """Normalize outcome in range 0 - scale_by"""
     return value * scale_by
@@ -257,16 +272,22 @@
     """Normalize value in between 0 - 100"""
     return partial(norm_to_scale, scale_by=100)(value)
 
 
 class OCRDifferenceMetric:
     """Basic definition of a OCRDifferenceMetric"""
 
-    def __init__(self, precision, normalization, calc_func,
-                 preprocessings=None, postprocessings=None) -> None:
+    def __init__(
+            self,
+            precision=2,
+            normalization=UC_NORMALIZATION_DEFAULT,
+            calc_func=accuracy_for,
+            preprocessings=None,
+            postprocessings=None
+    ) -> None:
         self.precision = precision
         self._value = None
         self.diff = None
         self._label = None
         self.unicode_normalization = normalization
         self.preprocessings = []
         if isinstance(preprocessings, list):
@@ -348,36 +369,36 @@
         remember this needs further refinement"""
         raise NotImplementedError
 
 
 class MetricChars(OCRDifferenceMetric):
     """Calculate plain sequent character based metric"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
                  preprocessings=None, postprocessings=None):
         super().__init__(
             precision,
             normalization,
             calc_func,
             preprocessings,
             postprocessings)
         self._label = 'Cs'
         self.name = 'Characters'
-        self.preprocessings = [_filter_whitespaces]
+        self.preprocessings = [_filter_whitespaces_excluding_blank_chars]
         self.postprocessings = [norm_percentual]
 
     def _forward(self):
         self.diff = edit_distance(self._data_reference, self._data_candidate)
 
 
 class MetricLetters(OCRDifferenceMetric):
     """Calculate metric for only a certain sub-set of
     character sequence"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
                  preprocessings=None, postprocessings=None):
         super().__init__(
             precision,
             normalization,
             calc_func,
             preprocessings,
             postprocessings)
@@ -390,15 +411,15 @@
     def _forward(self):
         self.diff = edit_distance(self._data_reference, self._data_candidate)
 
 
 class MetricWords(OCRDifferenceMetric):
     """Calculate metric for a sequence of word tokens"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
                  preprocessings=None, postprocessings=None):
         super().__init__(
             precision,
             normalization,
             calc_func,
             preprocessings,
             postprocessings)
@@ -408,15 +429,15 @@
     def _forward(self):
         self.diff = edit_distance(self._data_reference, self._data_candidate)
 
 
 class MetricBoW(OCRDifferenceMetric):
     """Calculate metric for a multiset of word tokens"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
                  preprocessings=None, postprocessings=None):
         super().__init__(
             precision,
             normalization,
             calc_func,
             preprocessings,
             postprocessings)
@@ -426,15 +447,15 @@
     def _forward(self):
         self.diff = bag_of_tokens(self._data_reference, self._data_candidate)
 
 
 class MetricIR(OCRDifferenceMetric):
     """Calculate information retrival metrics"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
                  preprocessings=None, postprocessings=None, languages=None):
         super().__init__(
             precision,
             normalization,
             calc_func,
             preprocessings,
             postprocessings)
@@ -451,15 +472,15 @@
         """to remind that this class needs further refinement"""
         raise NotImplementedError
 
 
 class MetricIRPre(MetricIR):
     """Calculate precision"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
                  preprocessings=None, postprocessings=None, languages=None):
         super().__init__(
             precision,
             normalization,
             calc_func,
             preprocessings,
             postprocessings,
@@ -469,15 +490,15 @@
     def _forward(self):
         self.diff = ir_precision(self._data_reference, self._data_candidate)
 
 
 class MetricIRRec(MetricIR):
     "Calculate recall"
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
                  preprocessings=None, postprocessings=None, languages=None):
         super().__init__(
             precision,
             normalization,
             calc_func,
             preprocessings,
             postprocessings,
@@ -487,15 +508,15 @@
     def _forward(self):
         self.diff = ir_recall(self._data_reference, self._data_candidate)
 
 
 class MetricIRFM(MetricIR):
     """Calculate harmonic mean for precision/recall"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
                  preprocessings=None, postprocessings=None, languages=None):
         super().__init__(
             precision,
             normalization,
             calc_func,
             preprocessings,
             postprocessings,
@@ -514,24 +535,25 @@
     Works with characters and word-like tokens, where
     tokens correspond also to:
     * abbreviations  (like "Nr." or "Etg.")
     * numbers/years  (like "1899")
     * split-up words (line endings/beginnings)
     """
 
-    return levenshtein(reference_data, candidate_data)
+    return Levenshtein.distance(reference_data, candidate_data)
 
 
 def bag_of_tokens(reference_tokens: List[str],
                   candidate_tokens: List[str]) -> int:
     """Calculate intersection/difference
     between reference and candidate token list
     """
-
-    return len(_diff(reference_tokens, candidate_tokens))
+    false_negatives: List[str] = _diff(reference_tokens, candidate_tokens)
+    false_positives: List[str] = _diff(candidate_tokens, reference_tokens)
+    return len(false_negatives) + len(false_positives)
 
 
 def _diff(gt_tokens, cd_tokens) -> List[str]:
     return list((Counter(gt_tokens) - Counter(cd_tokens)).elements())
 
 
 def ir_precision(reference_data, candidate_data) -> float:
```

### Comparing `digital-eval-1.5.1/src/digital_eval/model.py` & `digital-eval-1.5.2/src/digital_eval/model.py`

 * *Files identical despite different names*

### Comparing `digital-eval-1.5.1/src/digital_eval/model_legacy.py` & `digital-eval-1.5.2/src/digital_eval/model_legacy.py`

 * *Files identical despite different names*

### Comparing `digital-eval-1.5.1/src/digital_eval.egg-info/PKG-INFO` & `digital-eval-1.5.2/src/digital_eval.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-eval
-Version: 1.5.1
+Version: 1.5.2
 Summary: Evaluate Mass Digitalization Data
 Author: Universitäts- und Landesbibliothek Sachsen-Anhalt
 Author-email: development@bibliothek.uni-halle.de
 Maintainer: Uwe Hartwig
 Maintainer-email: uwe.hartwig@bibliothek.uni-halle.de
 Project-URL: Homepage, https://github.com/ulb-sachsen-anhalt/digital-eval
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # digital eval
 
 ![example workflow](https://github.com/ulb-sachsen-anhalt/digital-eval/actions/workflows/python-app.yml/badge.svg)
+[![PyPi version](https://badgen.net/pypi/v/digital-eval/)](https://pypi.org/project/digital-eval) ![PyPI - Downloads](https://img.shields.io/pypi/dm/digital-eval) ![PyPI - License](https://img.shields.io/pypi/l/digital-eval) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/digital-eval)
 
 Python3 Tool to report evaluation outcomes from mass digitalization workflows.
 
 ## Features
 
 * match automatically groundtruth (i.e. reference data) and candidates by filename
 * use geometric information to evaluate only specific frame (i.e. specific column or region from large page) of
```

### Comparing `digital-eval-1.5.1/src/digital_eval.egg-info/SOURCES.txt` & `digital-eval-1.5.2/src/digital_eval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digital-eval-1.5.1/src/ocr_util/cli.py` & `digital-eval-1.5.2/src/ocr_util/cli.py`

 * *Files identical despite different names*

### Comparing `digital-eval-1.5.1/src/ocr_util/frame.py` & `digital-eval-1.5.2/src/ocr_util/frame.py`

 * *Files identical despite different names*

