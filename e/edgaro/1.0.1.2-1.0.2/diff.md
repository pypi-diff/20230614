# Comparing `tmp/edgaro-1.0.1.2.tar.gz` & `tmp/edgaro-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgaro-1.0.1.2.tar", last modified: Fri Jun  2 11:07:35 2023, max compression
+gzip compressed data, was "edgaro-1.0.2.tar", last modified: Wed Jun 14 17:47:01 2023, max compression
```

## Comparing `edgaro-1.0.1.2.tar` & `edgaro-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.747987 edgaro-1.0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-02 11:07:35.747987 edgaro-1.0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.739987 edgaro-1.0.1.2/edgaro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.739987 edgaro-1.0.1.2/edgaro/balancing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/balancing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/balancing/nested_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/balancing/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/balancing/transformer_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.739987 edgaro-1.0.1.2/edgaro/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/base/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/base/base_transformer_array.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.743987 edgaro-1.0.1.2/edgaro/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21672 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/data/dataset_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.743987 edgaro-1.0.1.2/edgaro/explain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/explain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/explain/explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/explain/explainer_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    23271 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/explain/explainer_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    27137 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/explain/explainer_result_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.743987 edgaro-1.0.1.2/edgaro/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25616 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/model/model_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.739987 edgaro-1.0.1.2/edgaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-02 11:07:35.000000 edgaro-1.0.1.2/edgaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-02 11:07:35.000000 edgaro-1.0.1.2/edgaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:07:35.000000 edgaro-1.0.1.2/edgaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 11:07:35.000000 edgaro-1.0.1.2/edgaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 11:07:35.000000 edgaro-1.0.1.2/edgaro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:07:35.747987 edgaro-1.0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.747987 edgaro-1.0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_balancing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_balancing_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_balancing_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_dataset_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_model_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.890451 edgaro-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 17:46:45.000000 edgaro-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-14 17:47:01.890451 edgaro-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-14 17:46:45.000000 edgaro-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.886450 edgaro-1.0.2/edgaro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.886450 edgaro-1.0.2/edgaro/balancing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/balancing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/balancing/nested_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/balancing/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/balancing/transformer_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.886450 edgaro-1.0.2/edgaro/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/base/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/base/base_transformer_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.886450 edgaro-1.0.2/edgaro/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21672 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/data/dataset_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.890451 edgaro-1.0.2/edgaro/explain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/explain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/explain/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/explain/explainer_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26093 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/explain/explainer_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/explain/explainer_result_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.890451 edgaro-1.0.2/edgaro/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25616 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/model/model_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.886450 edgaro-1.0.2/edgaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-14 17:47:01.000000 edgaro-1.0.2/edgaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-14 17:47:01.000000 edgaro-1.0.2/edgaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:47:01.000000 edgaro-1.0.2/edgaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 17:47:01.000000 edgaro-1.0.2/edgaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 17:47:01.000000 edgaro-1.0.2/edgaro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 17:47:01.890451 edgaro-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-14 17:46:45.000000 edgaro-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.890451 edgaro-1.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_balancing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_balancing_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_balancing_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_dataset_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_model_array.py
```

### Comparing `edgaro-1.0.1.2/LICENSE` & `edgaro-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/PKG-INFO` & `edgaro-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgaro
-Version: 1.0.1.2
+Version: 1.0.2
 Summary: Explainable imbalanceD learninG compARatOr
 Home-page: https://github.com/adrianstando/edgaro
 Author: Adrian Stańdo
 Author-email: adrian.j.stando@gmail.com
 Project-URL: Documentation, https://adrianstando.github.io/edgaro
 Project-URL: Code repository, https://github.com/adrianstando/edgaro
 Keywords: XAI,imbalance,machine learning,AI
```

### Comparing `edgaro-1.0.1.2/README.md` & `edgaro-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/edgaro/balancing/nested_transformer.py` & `edgaro-1.0.2/edgaro/balancing/nested_transformer.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/edgaro/balancing/transformer.py` & `edgaro-1.0.2/edgaro/balancing/transformer.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/edgaro/balancing/transformer_array.py` & `edgaro-1.0.2/edgaro/balancing/transformer_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/edgaro/base/base_transformer.py` & `edgaro-1.0.2/edgaro/base/base_transformer.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/edgaro/base/base_transformer_array.py` & `edgaro-1.0.2/edgaro/base/base_transformer_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/edgaro/data/dataset.py` & `edgaro-1.0.2/edgaro/data/dataset.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/edgaro/data/dataset_array.py` & `edgaro-1.0.2/edgaro/data/dataset_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/edgaro/explain/explainer.py` & `edgaro-1.0.2/edgaro/explain/explainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import numpy as np
 import pandas as pd
 import warnings
 import sys
 import os
 import multiprocessing
 
-from typing import List, Optional, Literal
+from typing import List, Optional, Literal, Callable
+from sklearn.metrics import balanced_accuracy_score
 
 from edgaro.data.dataset import Dataset
 from edgaro.model.model import Model
 from edgaro.explain.explainer_result import Explanation, ModelProfileExplanation, Curve, ModelPartsExplanation
 from edgaro.base.utils import print_unbuffered
 
 
@@ -40,14 +41,18 @@
     processes : int, default=1
         Number of processes for the calculation of explanations.
         If -1, it is replaced with the number of available CPU cores.
     random_state : int, optional, default=None
         Random state seed.
     B : int, optional, default=10
         Number of permutation rounds to perform on each variable - applicable only if explanation_type='VI'.
+    performance_metric_name : str, default='balanced_accuracy'
+        Name of the performance metric.
+    performance_metric : callable, default=balanced_accuracy_score
+        Name of the performance metric.
 
     Attributes
     ----------
     model : Model
         A Model object to calculate explanations on.
     name: str
         A name of the Explainer, by default it is a Model name.
@@ -63,34 +68,41 @@
     processes : int
         Number of processes for the calculation of explanations.
         If -1, it is replaced with the number of available CPU cores.
     random_state : int, optional
         Random state seed
     B : int, optional
         Number of permutation rounds to perform on each variable - applicable only if explanation_type='VI'.
+    performance_metric_name : str
+        Name of the performance metric.
+    performance_metric : callable
+        Name of the performance metric.
 
     References
     ----------
     .. [1] https://ema.drwhy.ai/partialDependenceProfiles.html
     .. [2] https://ema.drwhy.ai/accumulatedLocalProfiles.html
 
     """
 
     def __init__(self, model: Model, N: Optional[int] = None, explanation_type: Literal['PDP', 'ALE', 'VI'] = 'PDP',
                  verbose: bool = False, processes: int = 1, random_state: Optional[int] = None,
-                 B: Optional[int] = 10) -> None:
+                 B: Optional[int] = 10, performance_metric_name: str = 'balanced_accuracy',
+                 performance_metric: Callable[[pd.Series, pd.Series], float] = balanced_accuracy_score) -> None:
         self.model = model
         self.explainer = None
         self.name = model.name
         self.N = N
         self.explanation_type = explanation_type
         self.verbose = verbose
         self.processes = processes
         self.random_state = random_state
         self.B = B
+        self.performance_metric_name = performance_metric_name
+        self.performance_metric = performance_metric
 
         if self.processes == -1:
             self.processes = multiprocessing.cpu_count()
 
     def fit(self) -> None:
         """
         Fit the Explainer object and create an explainer attribute.
@@ -130,14 +142,17 @@
         variables : list[str], optional
             List of variables for which the explanation should be calculated.
 
         Returns
         -------
         Explanation
         """
+        performance = self.model.evaluate(metrics_output_class=[self.performance_metric])
+        performance = performance['value'].iloc[0]
+
         if self.explainer is None:
             raise Exception('Explainer was not fitted!')
         category_colnames_base = self.model.get_category_colnames()
         dict_output = {}
 
         if variables is None:
             variables = list(self.model.get_train_dataset().data.columns)
@@ -152,24 +167,26 @@
             self.__transform_curve_category(dict_output, variables, category_colnames_base, explanation_type)
             self.__transform_curve_other(dict_output, variables, category_colnames_base, explanation_type)
 
             if self.verbose:
                 print_unbuffered(f'{self.explanation_type} was calculated calculated in {self.__repr__()} for '
                                  f'{self.model.get_test_dataset().name}')
 
-            return ModelProfileExplanation(dict_output, self.name, self.model.get_category_colnames())
+            return ModelProfileExplanation(dict_output, self.name, self.model.get_category_colnames(),
+                                           performance, self.performance_metric_name)
         elif self.explanation_type == 'VI':
             explanation_type = 'variable_importance'
             self.__transform_feature_importance(dict_output, variables, explanation_type)
 
             if self.verbose:
                 print_unbuffered(f'{self.explanation_type} was calculated calculated in {self.__repr__()} for '
                                  f'{self.model.get_test_dataset().name}')
 
-            return ModelPartsExplanation(dict_output, self.name)
+            return ModelPartsExplanation(dict_output, self.name,
+                                         performance, self.performance_metric_name)
         else:
             raise Exception('Wrong curve type!')
 
     def __transform_curve_category(self, dict_output, variables, category_colnames_base, explanation_type):
         category_colnames = list(set(variables).intersection(set(category_colnames_base)))
         if len(category_colnames) > 0:
             out_category = self.explainer.model_profile(verbose=False, variables=category_colnames,
```

### Comparing `edgaro-1.0.1.2/edgaro/explain/explainer_array.py` & `edgaro-1.0.2/edgaro/explain/explainer_array.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 import multiprocessing
+import pandas as pd
 
-from typing import Union, Optional, Literal
+from typing import Union, Optional, Literal, Callable
+from sklearn.metrics import balanced_accuracy_score
 
 from edgaro.model.model import Model
 from edgaro.model.model_array import ModelArray
 from edgaro.explain.explainer import Explainer
 from edgaro.explain.explainer_result_array import ExplanationArray, ModelProfileExplanationArray, \
     ModelPartsExplanationArray
 from edgaro.base.utils import print_unbuffered
@@ -31,14 +33,18 @@
     processes : int, default=1
         Number of processes for the calculation of explanations.
         If -1, it is replaced with the number of available CPU cores.
     random_state : int, optional, default=None
         Random state seed.
     B : int, optional, default=10
         Number of permutation rounds to perform on each variable - applicable only if explanation_type='VI'.
+    performance_metric_name : str
+        Name of the performance metric.
+    performance_metric : callable
+        Name of the performance metric.
 
     Attributes
     ----------
     models : Model, ModelArray
         A Model/ModelArray object to calculate the curves for.
     name: str
         A name of the ExplainerArray, by default it is a Model/ModelArray name.
@@ -54,47 +60,59 @@
     processes : int
         Number of processes for the calculation of explanations.
         If -1, it is replaced with the number of available CPU cores.
     random_state : int, optional
         Random state seed
     B : int, optional
         Number of permutation rounds to perform on each variable - applicable only if explanation_type='VI'.
+    performance_metric_name : str
+        Name of the performance metric.
+    performance_metric : callable
+        Name of the performance metric.
 
     """
 
     def __init__(self, models: Union[Model, ModelArray], N: Optional[int] = None,
                  explanation_type: Literal['PDP', 'ALE', 'VI'] = 'PDP', verbose: bool = False, processes: int = 1,
-                 random_state: Optional[int] = None, B: Optional[int] = 10) -> None:
+                 random_state: Optional[int] = None, B: Optional[int] = 10,
+                 performance_metric_name: str = 'balanced_accuracy',
+                 performance_metric: Callable[[pd.Series, pd.Series], float] = balanced_accuracy_score) -> None:
         self.models = models
         self.sub_calculators = None
         self.name = models.name
         self.N = N
         self.explanation_type = explanation_type
         self.verbose = verbose
 
         self.processes = processes
         self.random_state = random_state
         self.B = B
 
+        self.performance_metric_name = performance_metric_name
+        self.performance_metric = performance_metric
+
         if self.processes == -1:
             self.processes = multiprocessing.cpu_count()
 
     def fit(self) -> None:
         """
         Fit the ExplainerArray object and create an explainer attribute.
         """
 
         def create_sub_calculator(model: Union[Model, ModelArray]):
             if isinstance(model, Model):
                 calc = Explainer(model=model, N=self.N, explanation_type=self.explanation_type, verbose=self.verbose,
-                                 processes=self.processes, random_state=self.random_state, B=self.B)
+                                 processes=self.processes, random_state=self.random_state, B=self.B,
+                                 performance_metric_name=self.performance_metric_name,
+                                 performance_metric=self.performance_metric)
             else:
                 calc = ExplainerArray(models=model, N=self.N, explanation_type=self.explanation_type,
                                       verbose=self.verbose, processes=self.processes, random_state=self.random_state,
-                                      B=self.B)
+                                      B=self.B, performance_metric_name=self.performance_metric_name,
+                                      performance_metric=self.performance_metric)
 
             calc.fit()
             return calc
 
         self.sub_calculators = [create_sub_calculator(m) for m in self.models.get_models()]
 
         if self.verbose:
```

### Comparing `edgaro-1.0.1.2/edgaro/explain/explainer_result.py` & `edgaro-1.0.2/edgaro/explain/explainer_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,15 +48,19 @@
         pass
 
     @abstractmethod
     def plot(self) -> None:
         pass
 
     @abstractmethod
-    def compare(self, other: List[Explanation]) -> List[Union[float, list]]:
+    def compare(self, other: List[Explanation]) -> List[Union[float, List]]:
+        pass
+
+    @abstractmethod
+    def compare_performance(self, other: List[Explanation], percent: bool = False) -> List[float]:
         pass
 
 
 class ModelProfileExplanation(Explanation):
     """
     The class which represent the PDP/ALE curves for all variables in one Model.
 
@@ -66,34 +70,45 @@
         A dictionary of pairs (column name, Curve object), which represents curves for all variables in one Model.
     name : str
         The name of ModelProfileExplanation. It is best if it is a Model name.
     categorical_columns : list[str]
         List of categorical variables.
     explanation_type : {'PDP', 'ALE'}, default='PDP'
         A curve type.
+    performance_metric_value : float
+        Value of the performance metric.
+    performance_metric_name : str
+        Name of the performance metric.
 
     Attributes
     ----------
     results : Dict[str, Curve]
         A dictionary of pairs (column name, Curve object), which represents curves for all variables in one Model.
     name : str
         The name of ModelProfileExplanation. It is best if it is a Model name.
     categorical_columns : list[str]
         List of categorical variables.
     explanation_type : {'PDP', 'ALE'}
         A curve type.
+    performance_metric_value : float, optional
+        Value of the performance metric.
+    performance_metric_name : str, optional
+        Name of the performance metric.
 
     """
 
     def __init__(self, results: Dict[str, Curve], name: str, categorical_columns: List[str],
+                 performance_metric_value: float, performance_metric_name: str,
                  explanation_type: Literal['PDP', 'ALE'] = 'PDP') -> None:
         self.results = results
         self.name = name
         self.categorical_columns = categorical_columns
         self.explanation_type = explanation_type
+        self.performance_metric_value = performance_metric_value
+        self.performance_metric_name = performance_metric_name
 
     def __getitem__(self, key: str) -> Optional[Curve]:
         if key in self.results.keys():
             return self.results[key]
         else:
             return None
 
@@ -281,14 +296,38 @@
             if isinstance(inp, list):
                 for inp_i in inp:
                     ModelProfileExplanation.__retrieve_explainer_results(inp_i, explain_results_in)
             else:
                 for inp_i in inp.results:
                     ModelProfileExplanation.__retrieve_explainer_results(inp_i, explain_results_in)
 
+    def compare_performance(self, other: List[ModelProfileExplanation], percent: bool = False) -> List[float]:
+        """
+        The function returns the difference between performance metric values. This object's value is subtracted
+        from other.
+
+        Parameters
+        ----------
+        other : list[ModelProfileExplanation]
+            List of ModelProfileExplanation objects to compare against.
+        percent : bool, default=False
+            If True, the percentage change will be returned instead of difference.
+
+        Returns
+        ----------
+        list[float]
+        """
+
+        tab = [elem.performance_metric_value - self.performance_metric_value for elem in other]
+
+        if percent:
+            tab = [tab[i] / self.performance_metric_value for i in range(len(tab))]
+
+        return tab
+
     def compare(self, other: List[ModelProfileExplanation], variable: Optional[Union[str, List[str]]] = None,
                 return_raw_per_variable: bool = False) -> List[Union[float, list]]:
         """
         The function calculates the metric to compare the curves for a given variable(s).
 
         Currently, there is only one comparison metric called `SDD` (Standard Deviation of Distances). It is the variance of
         the distances between curve in this object and curves in `other` in intermediate points.
@@ -385,29 +424,41 @@
     ----------
     results : Dict[str, float]
         A dictionary of pairs (column name, value), which represents Variable Importance for all variables in one Model.
     name : str
         The name of ModelProfileExplanation. It is best if it is a Model name.
     explanation_type : {'VI'}, default='VI'
         An explanation type.
+    performance_metric_value : float
+        Value of the performance metric.
+    performance_metric_name : str
+        Name of the performance metric.
 
     Attributes
     ----------
     results : Dict[str, float]
         A dictionary of pairs (column name, value), which represents Variable Importance for all variables in one Model.
     name : str
         The name of ModelProfileExplanation. It is best if it is a Model name.
     explanation_type : {'VI'}, default='VI'
         An explanation type.
+    performance_metric_value : float
+        Value of the performance metric.
+    performance_metric_name : str
+        Name of the performance metric.
+
     """
 
-    def __init__(self, results: Dict[str, float], name: str, explanation_type: Literal['VI'] = 'VI') -> None:
+    def __init__(self, results: Dict[str, float], name: str, performance_metric_value: float,
+                 performance_metric_name: str, explanation_type: Literal['VI'] = 'VI') -> None:
         self.results = results
         self.name = name
         self.explanation_type = explanation_type
+        self.performance_metric_value = performance_metric_value
+        self.performance_metric_name = performance_metric_name
 
     def __getitem__(self, key: str) -> Optional[float]:
         if key in self.results.keys():
             return self.results[key]
         else:
             return None
 
@@ -525,14 +576,38 @@
                     ax.text(
                         x_min + 0.7 * (x_max - x_min),
                         y_min + 0.2 * (y_max - y_min),
                         text,
                         fontsize='medium'
                     )
 
+    def compare_performance(self, other: List[ModelPartsExplanation], percent: bool = False) -> List[float]:
+        """
+        The function returns the difference between performance metric values. This object's value is subtracted
+        from other.
+
+        Parameters
+        ----------
+        other : list[ModelPartsExplanation]
+            List of ModelPartsExplanation objects to compare against.
+        percent : bool, default=False
+            If True, the percentage change will be returned instead of difference.
+
+        Returns
+        ----------
+        list[float]
+        """
+
+        tab = [elem.performance_metric_value - self.performance_metric_value for elem in other]
+
+        if percent:
+            tab = [tab[i] / self.performance_metric_value for i in range(len(tab))]
+
+        return tab
+
     def compare(self, other: List[ModelPartsExplanation], variable: Optional[Union[str, List[str]]] = None,
                 max_variables: Optional[int] = None, return_raw: bool = True) -> List[Union[float, list]]:
         """
         The function calculates the metric to compare model parts of two or more models.
 
         Currently, there is only one metric based on the Wilcoxon statistical test [3]_. The metric value is the
         p-value of this test, where the inputs are variable importance values.
```

### Comparing `edgaro-1.0.1.2/edgaro/explain/explainer_result_array.py` & `edgaro-1.0.2/edgaro/explain/explainer_result_array.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 
 import math
 import re
 
 from abc import ABC, abstractmethod
+
+import matplotlib.axes
 import matplotlib.pyplot as plt
 import numpy as np
 
 from typing import List, Literal, Optional, Union, Tuple
+
+import pandas as pd
 from matplotlib.axes import Axes
 from statsmodels.stats.multitest import fdrcorrection
 
 from edgaro.explain.explainer_result import ModelProfileExplanation, ModelPartsExplanation
 
 
 class ExplanationArray(ABC):
@@ -26,14 +30,18 @@
     def compare(self) -> List[Union[float, list]]:
         pass
 
     @abstractmethod
     def plot_summary(self) -> None:
         pass
 
+    @abstractmethod
+    def compare_performance(self) -> List[Union[float, List]]:
+        pass
+
 
 class ModelProfileExplanationArray(ExplanationArray):
     """
     The class which represent the PDP/ALE curves for all variables in Model/ModelArray object.
 
     Parameters
     ----------
@@ -177,14 +185,75 @@
                 centered=centered
             )
 
         fig.tight_layout(rect=[0, 0.05, 1, 0.97])
         fig.legend([x.name for x in results], ncol=n_col, loc='lower center')
         plt.suptitle(f"{self.explanation_type} curves for {self.name}", fontsize=18)
 
+    def __filter_for_comparing(self, index_base, model_filter):
+        if isinstance(index_base, int) and index_base < 0:
+            index_base = self.results.index(self.results[index_base])
+
+        def filter_objects(obj):
+            if model_filter is not None and \
+                    re.search(model_filter, obj.name) is None:
+                return False
+            return True
+
+        def flatten(lst):
+            out = []
+            for i in range(len(lst)):
+                if not (isinstance(lst[i], list) or isinstance(lst[i], ModelProfileExplanationArray)):
+                    out.append(lst[i])
+                else:
+                    tmp = flatten(lst[i])
+                    out = out + tmp
+            return out
+
+        base_model = self[index_base]
+        if base_model is None:
+            raise Exception('Wrong index_base argument!')
+
+        res = flatten(self.results)
+        res.remove(self.results[index_base])
+
+        tab = [res[i] for i in range(len(res)) if filter_objects(res[i])]
+        return base_model, tab
+
+    def compare_performance(self, index_base: Union[str, int] = -1, model_filter: Optional[str] = None,
+                            percent: bool = False) -> List[Union[float, List]]:
+        """
+        The function returns the difference between performance metric values. index_base-object's value is subtracted
+        from others.
+
+        Parameters
+        ----------
+        index_base : int, str, default=-1
+                    Index of a curve to be a base for comparisons.
+        model_filter : str, optional, default=None
+            A regex expression to filter the names of the ModelProfileExplanation objects for comparing.
+        percent : bool, default=False
+            If True, the percentage change will we returned instead of difference.
+
+        Returns
+        ----------
+        list[float, list]
+        """
+
+        if isinstance(self.results[index_base], ModelProfileExplanation):
+            base_model, tab = self.__filter_for_comparing(index_base, model_filter)
+            return base_model.compare_performance(tab, percent=percent)
+        elif np.alltrue([isinstance(res, ModelProfileExplanationArray) for res in self.results]):
+            return [
+                res.compare_performance(index_base=index_base, model_filter=model_filter, percent=percent)
+                for res in self.results
+            ]
+        else:
+            raise Exception('Wrong result structure!')
+
     def compare(self, variable: Optional[Union[str, List[str]]] = None, index_base: Union[str, int] = -1,
                 return_raw: bool = True, return_raw_per_variable: bool = True, model_filter: Optional[str] = None) \
             -> List[Union[float, List]]:
         """
         The function compares the curves in the array.
 
         Parameters
@@ -204,56 +273,28 @@
         Returns
         -------
         list[float, list]
 
         """
 
         if isinstance(self.results[index_base], ModelProfileExplanation):
-            if isinstance(index_base, int) and index_base < 0:
-                index_base = self.results.index(self.results[index_base])
-
-            def filter_objects(obj):
-                if model_filter is not None and \
-                        re.search(model_filter, obj.name) is None:
-                    return False
-                return True
-
-            def flatten(lst):
-                out = []
-                for i in range(len(lst)):
-                    if not (isinstance(lst[i], list) or isinstance(lst[i], ModelProfileExplanationArray)):
-                        out.append(lst[i])
-                    else:
-                        tmp = flatten(lst[i])
-                        out = out + tmp
-                return out
-
-            base_model = self[index_base]
-            if base_model is None:
-                raise Exception('Wrong index_base argument!')
-
-            res = flatten(self.results)
-            res.remove(self.results[index_base])
+            base_model, res = self.__filter_for_comparing(index_base, model_filter)
 
             if return_raw:
                 out = []
                 for i in range(len(res)):
-                    if not filter_objects(res[i]):
-                        continue
-
                     if not return_raw_per_variable:
                         out.append(base_model.compare(res[i], variable=variable,
                                                       return_raw_per_variable=False)[0])
                     else:
                         out.append(base_model.compare(res[i], variable=variable,
                                                       return_raw_per_variable=True))
                 return out
             else:
-                tab = [res[i] for i in range(len(res)) if filter_objects(res[i])]
-                return base_model.compare(tab, variable=variable, return_raw_per_variable=return_raw_per_variable)
+                return base_model.compare(res, variable=variable, return_raw_per_variable=return_raw_per_variable)
         elif np.alltrue([isinstance(res, ModelProfileExplanationArray) for res in self.results]):
             return [
                 res.compare(variable=variable, index_base=index_base, return_raw=return_raw,
                             return_raw_per_variable=return_raw_per_variable, model_filter=model_filter)
                 for res in self.results
             ]
         else:
@@ -330,14 +371,110 @@
                     raise Exception('Incorrect length of filter_labels!')
             else:
                 plt.boxplot(results, patch_artist=True, labels=model_filters)
 
         if return_df:
             return results
 
+    def plot_performance_gain_analysis(self, model_filters: Optional[List[str]] = None, filter_labels: [List[str]] = None,
+                                       variables: Optional[List[str]] = None, figsize: Optional[Tuple[int, int]] = None,
+                                       index_base: Union[str, int] = -1, return_df: bool = False, percent: bool = False,
+                                       ax: Optional[matplotlib.axes.Axes] = None):
+        """
+        The function plots performance gain analysis plot which compares ASDD values and
+        difference in performance metric values.
+
+        Parameters
+        ----------
+        variables : list[str], optional, default=None
+            Variables for which the plot should be generated. If None, plots for all variables are generated if all the
+            available ModelProfileExplanation objects have exactly the same set of column names.
+        figsize : tuple(int, int), optional, default=None
+            The size of a figure.
+        model_filters : list[str], optional, default=None
+            List of regex expressions to filter the names of the ModelProfileExplanation objects for comparing.
+            Each element in the list creates a new boxplot. If None, one boxplot of all results is plotted.
+        filter_labels : list[str], optional, default=None
+            Labels of model filters.
+        index_base : int, str, default=-1
+            Index of a curve to be a base for comparisons.
+        return_df : bool, default=False
+            If True, the method returns a dataframe on which a plot is created.
+        percent : bool, default=False
+            If True, the percentage change will be plotted instead of difference.
+        ax : matplotlib.axes.Axes, optional
+            ax to plot on
+        """
+        x = self.results
+        while not isinstance(x, ModelProfileExplanation):
+            x = x[0]
+        performance_metric_name = x.performance_metric_name
+
+        if ax is None:
+            fig, ax = plt.subplots(figsize=figsize)
+
+        plt.title(f'Performance gain analysis of {self.explanation_type}\nfor {self.name} with {performance_metric_name} metric')
+        plt.xlabel('Performance gain')
+        plt.ylabel(r'ASDD values [$10^{-3}$]')
+
+        def format_func(value, tick_number):
+            return str(int(value * 10 ** 3))
+
+        def flatten(lst):
+            out = []
+            for i in range(len(lst)):
+                if not isinstance(lst[i], list):
+                    out.append(lst[i])
+                else:
+                    tmp = flatten(lst[i])
+                    out = out + tmp
+            return out
+
+        ax.yaxis.set_major_formatter(plt.FuncFormatter(format_func))
+
+        if model_filters is None:
+            results = self.compare(variable=variables, index_base=index_base,
+                                   return_raw=True, return_raw_per_variable=False)
+            results = flatten(results)
+
+            performance = self.compare_performance(index_base=index_base, percent=percent)
+            performance = flatten(performance)
+
+            if filter_labels is not None and len(filter_labels) == 1:
+                plt.scatter(x=performance, y=results, label=filter_labels[0])
+                plt.legend()
+            else:
+                plt.scatter(x=performance, y=results)
+
+        else:
+            results = []
+            performance = []
+            for i in range(len(model_filters)):
+                f = model_filters[i]
+                tmp_res = self.compare(variable=variables, index_base=index_base, model_filter=f,
+                                       return_raw=True, return_raw_per_variable=False)
+                tmp_res = flatten(tmp_res)
+                results.append(tmp_res)
+
+                tmp_per = self.compare_performance(index_base=index_base, percent=percent, model_filter=f)
+                tmp_per = flatten(tmp_per)
+                performance.append(tmp_per)
+
+                if filter_labels is not None:
+                    if len(filter_labels) == len(model_filters):
+                        plt.scatter(x=tmp_per, y=tmp_res, label=filter_labels[i], c=i)
+                    else:
+                        raise Exception('Incorrect length of filter_labels!')
+                else:
+                    plt.scatter(x=tmp_per, y=tmp_res, c=i)
+            plt.legend()
+
+        if return_df:
+            return results, performance
+
     def __str__(self) -> str:
         return f"ModelProfileExplanationArray {self.name} for {len(self.results)} variables: {list(self.results)} with {self.explanation_type} curve type"
 
     def __repr__(self) -> str:
         return f"<ModelProfileExplanationArray {self.name} with {self.explanation_type} curve type>"
 
 
@@ -425,14 +562,65 @@
         plots = self.results.copy()
         plots.remove(base)
         plots = ModelPartsExplanationArray.__flatten(plots)
 
         base.plot(variable=variable, figsize=figsize, max_variables=max_variables,
                   add_plot=plots, ax=ax, show_legend=show_legend, x_lim=x_lim, metric_precision=metric_precision)
 
+    def __filter_for_comparing(self, index_base, model_filter):
+        if isinstance(index_base, int) and index_base < 0:
+            index_base = self.results.index(self.results[index_base])
+
+        def filter_objects(obj):
+            if model_filter is not None and \
+                    re.search(model_filter, obj.name) is None:
+                return False
+            return True
+
+        base_model = self[index_base]
+        if base_model is None:
+            raise Exception('Wrong index_base argument!')
+
+        res = ModelPartsExplanationArray.__flatten(self.results)
+        res.remove(self.results[index_base])
+
+        tab = [res[i] for i in range(len(res)) if filter_objects(res[i])]
+        return base_model, tab
+
+    def compare_performance(self, index_base: Union[str, int] = -1, model_filter: Optional[str] = None,
+                            percent: bool = False) -> List[Union[float, List]]:
+        """
+        The function returns the difference between performance metric values. index_base-object's value is subtracted
+        from others.
+
+        Parameters
+        ----------
+        index_base : int, str, default=-1
+                    Index of a curve to be a base for comparisons.
+        model_filter : str, optional, default=None
+            A regex expression to filter the names of the ModelProfileExplanation objects for comparing.
+        percent : bool, default=False
+            If True, the percentage change will we returned instead of difference.
+
+        Returns
+        ----------
+        list[float, list]
+        """
+
+        if isinstance(self.results[index_base], ModelProfileExplanation):
+            base_model, tab = self.__filter_for_comparing(index_base, model_filter)
+            return base_model.compare_performance(tab, percent=percent)
+        elif np.alltrue([isinstance(res, ModelProfileExplanationArray) for res in self.results]):
+            return [
+                res.compare_performance(index_base=index_base, model_filter=model_filter, percent=percent)
+                for res in self.results
+            ]
+        else:
+            raise Exception('Wrong result structure!')
+
     def compare(self, variable: Optional[Union[str, List[str]]] = None, max_variables: Optional[int] = None,
                 return_raw: bool = True, index_base: Union[str, int] = -1, model_filter: Optional[str] = None) \
             -> List[Union[float, list]]:
         """
         The function compares variable importance in the array.
 
         Parameters
@@ -452,31 +640,15 @@
         Returns
         -------
         list[float, list]
 
         """
 
         if isinstance(self.results[index_base], ModelPartsExplanation):
-            if isinstance(index_base, int) and index_base < 0:
-                index_base = self.results.index(self.results[index_base])
-
-            def filter_objects(obj):
-                if model_filter is not None and \
-                        re.search(model_filter, obj.name) is None:
-                    return False
-                return True
-
-            base_model = self[index_base]
-            if base_model is None:
-                raise Exception('Wrong index_base argument!')
-
-            res = ModelPartsExplanationArray.__flatten(self.results)
-            res.remove(self.results[index_base])
-
-            res_filtered = [res[i] for i in range(len(res)) if filter_objects(res[i])]
+            base_model, res_filtered = self.__filter_for_comparing(index_base, model_filter)
             return base_model.compare(other=res_filtered, variable=variable, max_variables=max_variables,
                                       return_raw=return_raw)
         elif np.alltrue([isinstance(res, ModelPartsExplanationArray) for res in self.results]):
             return [
                 res.compare(variable=variable, max_variables=max_variables, return_raw=return_raw,
                             index_base=index_base, model_filter=model_filter)
                 for res in self.results
```

### Comparing `edgaro-1.0.1.2/edgaro/model/model.py` & `edgaro-1.0.2/edgaro/model/model.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/edgaro/model/model_array.py` & `edgaro-1.0.2/edgaro/model/model_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/edgaro.egg-info/PKG-INFO` & `edgaro-1.0.2/edgaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgaro
-Version: 1.0.1.2
+Version: 1.0.2
 Summary: Explainable imbalanceD learninG compARatOr
 Home-page: https://github.com/adrianstando/edgaro
 Author: Adrian Stańdo
 Author-email: adrian.j.stando@gmail.com
 Project-URL: Documentation, https://adrianstando.github.io/edgaro
 Project-URL: Code repository, https://github.com/adrianstando/edgaro
 Keywords: XAI,imbalance,machine learning,AI
```

### Comparing `edgaro-1.0.1.2/edgaro.egg-info/SOURCES.txt` & `edgaro-1.0.2/edgaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/setup.py` & `edgaro-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="edgaro",
-    version="1.0.1.2",
+    version="1.0.2",
     description="Explainable imbalanceD learninG compARatOr",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/adrianstando/edgaro",
     author="Adrian Stańdo",
     author_email="adrian.j.stando@gmail.com",
     classifiers=[
```

### Comparing `edgaro-1.0.1.2/test/test_balancing.py` & `edgaro-1.0.2/test/test_balancing.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/test/test_balancing_array.py` & `edgaro-1.0.2/test/test_balancing_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/test/test_balancing_nested.py` & `edgaro-1.0.2/test/test_balancing_nested.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/test/test_dataset.py` & `edgaro-1.0.2/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/test/test_dataset_array.py` & `edgaro-1.0.2/test/test_dataset_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/test/test_explain.py` & `edgaro-1.0.2/test/test_explain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+import copy
 
 from imblearn.under_sampling import RandomUnderSampler
 from sklearn.metrics import accuracy_score
 from copy import deepcopy
 
 from edgaro.data.dataset import DatasetFromOpenML, Dataset
 from edgaro.balancing.transformer import TransformerFromIMBLEARN, RandomUnderSampler as RUS
@@ -331,14 +332,30 @@
     column = rf.get_models()[0].get_train_dataset().data.columns[0]
     try:
         t[2].plot_summary(variables=column, model_filters=[f"^{name_1}", f"^{name_2}"])
     except (Exception,):
         assert False
 
 
+def test_array_of_arrays_plot_performance_gain(model_array2):
+    rf, t = model_array2
+
+    # simulate more results
+    t = copy.deepcopy(t)
+    t = t[[0, 1]]
+    t.results[1] = t[0]
+    t.results.append(t[0])
+    t.results.append(t[0])
+
+    try:
+        t.plot_performance_gain_analysis()
+    except (Exception,):
+        assert False
+
+
 def test_array_of_arrays_compare(model_array2):
     rf, t = model_array2
     column = rf.get_models()[0].get_train_dataset().data.columns[0]
     column1 = rf.get_models()[0].get_train_dataset().data.columns[1]
     try:
         t1 = deepcopy(t)
         t1[0].results[column].y += 0.1
```

### Comparing `edgaro-1.0.1.2/test/test_model.py` & `edgaro-1.0.2/test/test_model.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.2/test/test_model_array.py` & `edgaro-1.0.2/test/test_model_array.py`

 * *Files identical despite different names*

