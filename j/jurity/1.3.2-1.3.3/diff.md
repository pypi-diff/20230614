# Comparing `tmp/jurity-1.3.2.tar.gz` & `tmp/jurity-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jurity-1.3.2.tar", last modified: Thu Feb 10 19:21:32 2022, max compression
+gzip compressed data, was "jurity-1.3.3.tar", last modified: Wed Jun 14 01:15:14 2023, max compression
```

## Comparing `jurity-1.3.2.tar` & `jurity-1.3.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 a703204  (1381635968) staff       (20)        0 2022-02-10 19:21:32.735637 jurity-1.3.2/
--rw-r--r--   0 a703204  (1381635968) staff       (20)    11356 2022-02-10 19:19:39.000000 jurity-1.3.2/LICENSE
--rw-r--r--   0 a703204  (1381635968) staff       (20)      534 2022-02-10 19:19:39.000000 jurity-1.3.2/NOTICES
--rw-r--r--   0 a703204  (1381635968) staff       (20)     8777 2022-02-10 19:21:32.735123 jurity-1.3.2/PKG-INFO
--rw-r--r--   0 a703204  (1381635968) staff       (20)     8263 2022-02-10 19:19:39.000000 jurity-1.3.2/README.md
-drwxr-xr-x   0 a703204  (1381635968) staff       (20)        0 2022-02-10 19:21:32.715414 jurity-1.3.2/jurity/
--rw-r--r--   0 a703204  (1381635968) staff       (20)      108 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/__init__.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)      131 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/_version.py
-drwxr-xr-x   0 a703204  (1381635968) staff       (20)        0 2022-02-10 19:21:32.720842 jurity-1.3.2/jurity/classification/
--rw-r--r--   0 a703204  (1381635968) staff       (20)      417 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/classification/__init__.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     1254 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/classification/accuracy.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     1284 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/classification/auc.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)      153 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/classification/base.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     1506 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/classification/f1.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     1544 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/classification/precision.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     1497 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/classification/recall.py
-drwxr-xr-x   0 a703204  (1381635968) staff       (20)        0 2022-02-10 19:21:32.726192 jurity-1.3.2/jurity/fairness/
--rw-r--r--   0 a703204  (1381635968) staff       (20)     6527 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/fairness/__init__.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     3813 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/fairness/average_odds.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     6703 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/fairness/base.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     4082 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/fairness/disparate_impact.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     3451 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/fairness/equal_opportunity.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     3200 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/fairness/fnr_difference.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     4001 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/fairness/generalized_entropy.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     3413 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/fairness/predictive_equality.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     3056 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/fairness/statistical_parity.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     2650 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/fairness/theil_index.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     3706 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/hash_utils.py
-drwxr-xr-x   0 a703204  (1381635968) staff       (20)        0 2022-02-10 19:21:32.727848 jurity-1.3.2/jurity/mitigation/
--rw-r--r--   0 a703204  (1381635968) staff       (20)      403 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/mitigation/__init__.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     1169 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/mitigation/base.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)    19244 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/mitigation/equalized_odds.py
-drwxr-xr-x   0 a703204  (1381635968) staff       (20)        0 2022-02-10 19:21:32.734367 jurity-1.3.2/jurity/recommenders/
--rw-r--r--   0 a703204  (1381635968) staff       (20)      590 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/recommenders/__init__.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     7969 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/recommenders/auc.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     6387 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/recommenders/base.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     7184 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/recommenders/combined.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)    14465 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/recommenders/ctr.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)    30891 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/recommenders/diversity.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     8487 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/recommenders/map.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     7583 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/recommenders/ndcg.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     8062 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/recommenders/precision.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)     7588 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/recommenders/recall.py
--rw-r--r--   0 a703204  (1381635968) staff       (20)    17414 2022-02-10 19:19:39.000000 jurity-1.3.2/jurity/utils.py
-drwxr-xr-x   0 a703204  (1381635968) staff       (20)        0 2022-02-10 19:21:32.717460 jurity-1.3.2/jurity.egg-info/
--rw-r--r--   0 a703204  (1381635968) staff       (20)     8777 2022-02-10 19:21:32.000000 jurity-1.3.2/jurity.egg-info/PKG-INFO
--rw-r--r--   0 a703204  (1381635968) staff       (20)     1207 2022-02-10 19:21:32.000000 jurity-1.3.2/jurity.egg-info/SOURCES.txt
--rw-r--r--   0 a703204  (1381635968) staff       (20)        1 2022-02-10 19:21:32.000000 jurity-1.3.2/jurity.egg-info/dependency_links.txt
--rw-r--r--   0 a703204  (1381635968) staff       (20)       39 2022-02-10 19:21:32.000000 jurity-1.3.2/jurity.egg-info/requires.txt
--rw-r--r--   0 a703204  (1381635968) staff       (20)        7 2022-02-10 19:21:32.000000 jurity-1.3.2/jurity.egg-info/top_level.txt
--rw-r--r--   0 a703204  (1381635968) staff       (20)       38 2022-02-10 19:21:32.735804 jurity-1.3.2/setup.cfg
--rw-r--r--   0 a703204  (1381635968) staff       (20)     1035 2022-02-10 19:19:39.000000 jurity-1.3.2/setup.py
+drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-06-14 01:15:14.535531 jurity-1.3.3/
+-rw-r--r--   0 a640920  (1141242692) staff       (20)    11356 2021-03-03 02:15:09.000000 jurity-1.3.3/LICENSE
+-rw-r--r--   0 a640920  (1141242692) staff       (20)      534 2021-03-03 02:15:09.000000 jurity-1.3.3/NOTICES
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     8882 2023-06-14 01:15:14.534881 jurity-1.3.3/PKG-INFO
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     8368 2023-05-01 13:40:47.000000 jurity-1.3.3/README.md
+drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-06-14 01:15:14.468720 jurity-1.3.3/jurity/
+-rw-r--r--   0 a640920  (1141242692) staff       (20)      108 2021-03-03 02:15:09.000000 jurity-1.3.3/jurity/__init__.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)      131 2023-06-14 01:14:47.000000 jurity-1.3.3/jurity/_version.py
+drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-06-14 01:15:14.491451 jurity-1.3.3/jurity/classification/
+-rw-r--r--   0 a640920  (1141242692) staff       (20)      417 2021-03-03 02:15:09.000000 jurity-1.3.3/jurity/classification/__init__.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     1254 2021-03-03 02:15:09.000000 jurity-1.3.3/jurity/classification/accuracy.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     1284 2021-03-03 02:15:09.000000 jurity-1.3.3/jurity/classification/auc.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)      153 2021-03-03 02:15:09.000000 jurity-1.3.3/jurity/classification/base.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     1506 2021-03-03 02:15:09.000000 jurity-1.3.3/jurity/classification/f1.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     1544 2021-03-03 02:15:09.000000 jurity-1.3.3/jurity/classification/precision.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     1497 2021-03-03 02:15:09.000000 jurity-1.3.3/jurity/classification/recall.py
+drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-06-14 01:15:14.501037 jurity-1.3.3/jurity/fairness/
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     6456 2023-06-14 01:14:47.000000 jurity-1.3.3/jurity/fairness/__init__.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     3813 2023-06-14 01:14:47.000000 jurity-1.3.3/jurity/fairness/average_odds.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     6703 2023-06-14 01:14:47.000000 jurity-1.3.3/jurity/fairness/base.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     4082 2023-06-14 01:14:47.000000 jurity-1.3.3/jurity/fairness/disparate_impact.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     3451 2023-06-14 01:14:47.000000 jurity-1.3.3/jurity/fairness/equal_opportunity.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     3200 2023-06-14 01:14:47.000000 jurity-1.3.3/jurity/fairness/fnr_difference.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     4001 2023-06-14 01:14:47.000000 jurity-1.3.3/jurity/fairness/generalized_entropy.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     3413 2023-06-14 01:14:47.000000 jurity-1.3.3/jurity/fairness/predictive_equality.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     3056 2023-06-14 01:14:47.000000 jurity-1.3.3/jurity/fairness/statistical_parity.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     2650 2023-06-14 01:14:47.000000 jurity-1.3.3/jurity/fairness/theil_index.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     3706 2023-06-14 01:14:47.000000 jurity-1.3.3/jurity/hash_utils.py
+drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-06-14 01:15:14.509498 jurity-1.3.3/jurity/mitigation/
+-rw-r--r--   0 a640920  (1141242692) staff       (20)      403 2021-03-03 02:15:09.000000 jurity-1.3.3/jurity/mitigation/__init__.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     1169 2021-03-03 02:15:09.000000 jurity-1.3.3/jurity/mitigation/base.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)    19244 2021-03-03 02:15:09.000000 jurity-1.3.3/jurity/mitigation/equalized_odds.py
+drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-06-14 01:15:14.533728 jurity-1.3.3/jurity/recommenders/
+-rw-r--r--   0 a640920  (1141242692) staff       (20)      590 2022-02-28 22:25:41.000000 jurity-1.3.3/jurity/recommenders/__init__.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     7969 2021-07-14 19:32:13.000000 jurity-1.3.3/jurity/recommenders/auc.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     6387 2021-08-02 15:45:11.000000 jurity-1.3.3/jurity/recommenders/base.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     7184 2022-02-28 22:25:41.000000 jurity-1.3.3/jurity/recommenders/combined.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)    14465 2022-01-27 18:17:14.000000 jurity-1.3.3/jurity/recommenders/ctr.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)    30891 2022-02-28 22:25:41.000000 jurity-1.3.3/jurity/recommenders/diversity.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     8487 2022-01-27 18:17:14.000000 jurity-1.3.3/jurity/recommenders/map.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     7583 2021-08-02 15:45:14.000000 jurity-1.3.3/jurity/recommenders/ndcg.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     8062 2021-08-02 15:45:11.000000 jurity-1.3.3/jurity/recommenders/precision.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     7588 2021-08-02 15:45:11.000000 jurity-1.3.3/jurity/recommenders/recall.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)    17414 2023-06-14 01:14:47.000000 jurity-1.3.3/jurity/utils.py
+drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-06-14 01:15:14.474058 jurity-1.3.3/jurity.egg-info/
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     8882 2023-06-14 01:15:14.000000 jurity-1.3.3/jurity.egg-info/PKG-INFO
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     1207 2023-06-14 01:15:14.000000 jurity-1.3.3/jurity.egg-info/SOURCES.txt
+-rw-r--r--   0 a640920  (1141242692) staff       (20)        1 2023-06-14 01:15:14.000000 jurity-1.3.3/jurity.egg-info/dependency_links.txt
+-rw-r--r--   0 a640920  (1141242692) staff       (20)       39 2023-06-14 01:15:14.000000 jurity-1.3.3/jurity.egg-info/requires.txt
+-rw-r--r--   0 a640920  (1141242692) staff       (20)        7 2023-06-14 01:15:14.000000 jurity-1.3.3/jurity.egg-info/top_level.txt
+-rw-r--r--   0 a640920  (1141242692) staff       (20)       38 2023-06-14 01:15:14.535740 jurity-1.3.3/setup.cfg
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     1035 2021-03-03 02:15:09.000000 jurity-1.3.3/setup.py
```

### Comparing `jurity-1.3.2/LICENSE` & `jurity-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/NOTICES` & `jurity-1.3.3/NOTICES`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/PKG-INFO` & `jurity-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: jurity
-Version: 1.3.2
+Version: 1.3.3
 Summary: fairness and evaluation library
 Home-page: https://github.com/fidelity/jurity
 Author: FMR LLC
 License: UNKNOWN
 Project-URL: Source, https://github.com/fidelity/jurity
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICES
 
-[![ci](https://github.com/fidelity/jurity/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/fidelity/jurity/actions/workflows/ci.yml) [![PyPI version fury.io](https://badge.fury.io/py/jurity.svg)](https://pypi.python.org/pypi/jurity/) [![PyPI license](https://img.shields.io/pypi/l/jurity.svg)](https://pypi.python.org/pypi/jurity/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
+[![ci](https://github.com/fidelity/jurity/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/fidelity/jurity/actions/workflows/ci.yml) [![PyPI version fury.io](https://badge.fury.io/py/jurity.svg)](https://pypi.python.org/pypi/jurity/) [![PyPI license](https://img.shields.io/pypi/l/jurity.svg)](https://pypi.python.org/pypi/jurity/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![Downloads](https://static.pepy.tech/personalized-badge/jurity?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/jurity)
 
 
 # Jurity: Fairness & Evaluation Library
 
 Jurity is a research library that provides fairness metrics, recommender system evaluations, classification metrics and bias mitigation techniques. The library adheres to PEP-8 standards and is tested heavily.
 
 Jurity is developed by the Artificial Intelligence Center of Excellence at Fidelity Investments. Documentation is available at [fidelity.github.io/jurity](https://fidelity.github.io/jurity).
@@ -154,27 +154,25 @@
 ```python
 # Import classification metrics
 from jurity.classification import BinaryClassificationMetrics
 
 # Data
 labels = [1, 1, 0, 1, 0, 0, 1, 0]
 predictions = [0, 0, 0, 1, 1, 1, 1, 0]
-likelihoods = [0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.1]
-is_member = [0, 0, 0, 0, 1, 1, 1, 1]
 
 # Available: Accuracy, F1, Precision, Recall, and AUC
 f1_score = BinaryClassificationMetrics.F1()
 
 print('F1 score is', f1_score.get_score(predictions, labels))
 ```
 
 
 ## Installation
 
-Jurity is available to install as `pip install jurity`. It can also be installed by building from source by following the instructions in our [documentation](https://fidelity.github.io/jurity/install.html).
+Jurity requires **Python 3.7+** and can be installed from PyPI using ``pip install jurity`` or by building from source as shown in [installation instructions](https://fidelity.github.io/jurity/install.html).
 
 ## Support
 Please submit bug reports and feature requests as [Issues](https://github.com/fidelity/jurity/issues).
 
 ## License
 Jurity is licensed under the [Apache License 2.0.](https://github.com/fidelity/jurity/blob/master/LICENSE)
```

### Comparing `jurity-1.3.2/README.md` & `jurity-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![ci](https://github.com/fidelity/jurity/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/fidelity/jurity/actions/workflows/ci.yml) [![PyPI version fury.io](https://badge.fury.io/py/jurity.svg)](https://pypi.python.org/pypi/jurity/) [![PyPI license](https://img.shields.io/pypi/l/jurity.svg)](https://pypi.python.org/pypi/jurity/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
+[![ci](https://github.com/fidelity/jurity/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/fidelity/jurity/actions/workflows/ci.yml) [![PyPI version fury.io](https://badge.fury.io/py/jurity.svg)](https://pypi.python.org/pypi/jurity/) [![PyPI license](https://img.shields.io/pypi/l/jurity.svg)](https://pypi.python.org/pypi/jurity/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![Downloads](https://static.pepy.tech/personalized-badge/jurity?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/jurity)
 
 
 # Jurity: Fairness & Evaluation Library
 
 Jurity is a research library that provides fairness metrics, recommender system evaluations, classification metrics and bias mitigation techniques. The library adheres to PEP-8 standards and is tested heavily.
 
 Jurity is developed by the Artificial Intelligence Center of Excellence at Fidelity Investments. Documentation is available at [fidelity.github.io/jurity](https://fidelity.github.io/jurity).
@@ -137,26 +137,24 @@
 ```python
 # Import classification metrics
 from jurity.classification import BinaryClassificationMetrics
 
 # Data
 labels = [1, 1, 0, 1, 0, 0, 1, 0]
 predictions = [0, 0, 0, 1, 1, 1, 1, 0]
-likelihoods = [0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.1]
-is_member = [0, 0, 0, 0, 1, 1, 1, 1]
 
 # Available: Accuracy, F1, Precision, Recall, and AUC
 f1_score = BinaryClassificationMetrics.F1()
 
 print('F1 score is', f1_score.get_score(predictions, labels))
 ```
 
 
 ## Installation
 
-Jurity is available to install as `pip install jurity`. It can also be installed by building from source by following the instructions in our [documentation](https://fidelity.github.io/jurity/install.html).
+Jurity requires **Python 3.7+** and can be installed from PyPI using ``pip install jurity`` or by building from source as shown in [installation instructions](https://fidelity.github.io/jurity/install.html).
 
 ## Support
 Please submit bug reports and feature requests as [Issues](https://github.com/fidelity/jurity/issues).
 
 ## License
 Jurity is licensed under the [Apache License 2.0.](https://github.com/fidelity/jurity/blob/master/LICENSE)
```

### Comparing `jurity-1.3.2/jurity/classification/accuracy.py` & `jurity-1.3.3/jurity/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/classification/auc.py` & `jurity-1.3.3/jurity/classification/auc.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/classification/f1.py` & `jurity-1.3.3/jurity/classification/f1.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/classification/precision.py` & `jurity-1.3.3/jurity/classification/precision.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/classification/recall.py` & `jurity-1.3.3/jurity/classification/recall.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/fairness/__init__.py` & `jurity-1.3.3/jurity/fairness/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,19 +78,17 @@
                 score = instance.get_score(labels, predictions)
             else:
                 score = instance.get_score(labels, predictions, is_member, membership_label)
 
             if score is None:
                 score = np.nan
             score = np.round(score, 3)
-            df = df.append({"Metric": instance.name,
-                            "Value": score,
-                            "Lower Bound": instance.lower_bound,
-                            "Ideal Value": instance.ideal_value,
-                            "Upper Bound": instance.upper_bound}, ignore_index=True)
+            df = pd.concat([df, pd.DataFrame(
+                [[instance.name, score, instance.ideal_value, instance.lower_bound, instance.upper_bound]],
+                columns=df.columns)], axis=0, ignore_index=True)
 
         df = df.set_index("Metric")
 
         return df
 
 
 class MultiClassFairnessMetrics(NamedTuple):
@@ -154,11 +152,11 @@
             for position, class_ in enumerate(list_of_classes):
                 append_dict[class_] = scores[position]
 
             append_dict["Lower Bound"] = multi_instance.lower_bound
             append_dict["Ideal Value"] = multi_instance.ideal_value
             append_dict["Upper Bound"] = multi_instance.upper_bound
 
-            df = df.append(append_dict, ignore_index=True)
+            df = pd.concat([df, pd.DataFrame([append_dict])], ignore_index=True)
 
         df = df.set_index("Metric")
         return df
```

### Comparing `jurity-1.3.2/jurity/fairness/average_odds.py` & `jurity-1.3.3/jurity/fairness/average_odds.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/fairness/base.py` & `jurity-1.3.3/jurity/fairness/base.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/fairness/disparate_impact.py` & `jurity-1.3.3/jurity/fairness/disparate_impact.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/fairness/equal_opportunity.py` & `jurity-1.3.3/jurity/fairness/equal_opportunity.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/fairness/fnr_difference.py` & `jurity-1.3.3/jurity/fairness/fnr_difference.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/fairness/generalized_entropy.py` & `jurity-1.3.3/jurity/fairness/generalized_entropy.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/fairness/predictive_equality.py` & `jurity-1.3.3/jurity/fairness/predictive_equality.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/fairness/statistical_parity.py` & `jurity-1.3.3/jurity/fairness/statistical_parity.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/fairness/theil_index.py` & `jurity-1.3.3/jurity/fairness/theil_index.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/hash_utils.py` & `jurity-1.3.3/jurity/hash_utils.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/mitigation/base.py` & `jurity-1.3.3/jurity/mitigation/base.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/mitigation/equalized_odds.py` & `jurity-1.3.3/jurity/mitigation/equalized_odds.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/recommenders/__init__.py` & `jurity-1.3.3/jurity/recommenders/__init__.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/recommenders/auc.py` & `jurity-1.3.3/jurity/recommenders/auc.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/recommenders/base.py` & `jurity-1.3.3/jurity/recommenders/base.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/recommenders/combined.py` & `jurity-1.3.3/jurity/recommenders/combined.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/recommenders/ctr.py` & `jurity-1.3.3/jurity/recommenders/ctr.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/recommenders/diversity.py` & `jurity-1.3.3/jurity/recommenders/diversity.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/recommenders/map.py` & `jurity-1.3.3/jurity/recommenders/map.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/recommenders/ndcg.py` & `jurity-1.3.3/jurity/recommenders/ndcg.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/recommenders/precision.py` & `jurity-1.3.3/jurity/recommenders/precision.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/recommenders/recall.py` & `jurity-1.3.3/jurity/recommenders/recall.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity/utils.py` & `jurity-1.3.3/jurity/utils.py`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/jurity.egg-info/PKG-INFO` & `jurity-1.3.3/jurity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: jurity
-Version: 1.3.2
+Version: 1.3.3
 Summary: fairness and evaluation library
 Home-page: https://github.com/fidelity/jurity
 Author: FMR LLC
 License: UNKNOWN
 Project-URL: Source, https://github.com/fidelity/jurity
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICES
 
-[![ci](https://github.com/fidelity/jurity/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/fidelity/jurity/actions/workflows/ci.yml) [![PyPI version fury.io](https://badge.fury.io/py/jurity.svg)](https://pypi.python.org/pypi/jurity/) [![PyPI license](https://img.shields.io/pypi/l/jurity.svg)](https://pypi.python.org/pypi/jurity/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
+[![ci](https://github.com/fidelity/jurity/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/fidelity/jurity/actions/workflows/ci.yml) [![PyPI version fury.io](https://badge.fury.io/py/jurity.svg)](https://pypi.python.org/pypi/jurity/) [![PyPI license](https://img.shields.io/pypi/l/jurity.svg)](https://pypi.python.org/pypi/jurity/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![Downloads](https://static.pepy.tech/personalized-badge/jurity?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/jurity)
 
 
 # Jurity: Fairness & Evaluation Library
 
 Jurity is a research library that provides fairness metrics, recommender system evaluations, classification metrics and bias mitigation techniques. The library adheres to PEP-8 standards and is tested heavily.
 
 Jurity is developed by the Artificial Intelligence Center of Excellence at Fidelity Investments. Documentation is available at [fidelity.github.io/jurity](https://fidelity.github.io/jurity).
@@ -154,27 +154,25 @@
 ```python
 # Import classification metrics
 from jurity.classification import BinaryClassificationMetrics
 
 # Data
 labels = [1, 1, 0, 1, 0, 0, 1, 0]
 predictions = [0, 0, 0, 1, 1, 1, 1, 0]
-likelihoods = [0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.1]
-is_member = [0, 0, 0, 0, 1, 1, 1, 1]
 
 # Available: Accuracy, F1, Precision, Recall, and AUC
 f1_score = BinaryClassificationMetrics.F1()
 
 print('F1 score is', f1_score.get_score(predictions, labels))
 ```
 
 
 ## Installation
 
-Jurity is available to install as `pip install jurity`. It can also be installed by building from source by following the instructions in our [documentation](https://fidelity.github.io/jurity/install.html).
+Jurity requires **Python 3.7+** and can be installed from PyPI using ``pip install jurity`` or by building from source as shown in [installation instructions](https://fidelity.github.io/jurity/install.html).
 
 ## Support
 Please submit bug reports and feature requests as [Issues](https://github.com/fidelity/jurity/issues).
 
 ## License
 Jurity is licensed under the [Apache License 2.0.](https://github.com/fidelity/jurity/blob/master/LICENSE)
```

### Comparing `jurity-1.3.2/jurity.egg-info/SOURCES.txt` & `jurity-1.3.3/jurity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jurity-1.3.2/setup.py` & `jurity-1.3.3/setup.py`

 * *Files identical despite different names*

