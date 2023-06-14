# Comparing `tmp/analyzr-sdk-python-1.2.56.tar.gz` & `tmp/analyzr-sdk-python-1.2.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analyzr-sdk-python-1.2.56.tar", last modified: Wed May 31 19:44:07 2023, max compression
+gzip compressed data, was "analyzr-sdk-python-1.2.57.tar", last modified: Wed Jun 14 16:57:43 2023, max compression
```

## Comparing `analyzr-sdk-python-1.2.56.tar` & `analyzr-sdk-python-1.2.57.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 19:44:07.430795 analyzr-sdk-python-1.2.56/
--rw-rw-rw-   0        0        0    11558 2022-10-21 16:54:33.000000 analyzr-sdk-python-1.2.56/LICENSE
--rw-rw-rw-   0        0        0     2280 2023-05-31 19:44:07.428803 analyzr-sdk-python-1.2.56/PKG-INFO
--rw-rw-rw-   0        0        0     1748 2023-05-31 11:48:21.000000 analyzr-sdk-python-1.2.56/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 19:44:07.380807 analyzr-sdk-python-1.2.56/analyzr_sdk_python.egg-info/
--rw-rw-rw-   0        0        0     2280 2023-05-31 19:44:07.000000 analyzr-sdk-python-1.2.56/analyzr_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-05-31 19:44:07.000000 analyzr-sdk-python-1.2.56/analyzr_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 19:44:07.000000 analyzr-sdk-python-1.2.56/analyzr_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 19:44:07.000000 analyzr-sdk-python-1.2.56/analyzr_sdk_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 19:44:07.425793 analyzr-sdk-python-1.2.56/analyzrclient/
--rw-rw-rw-   0        0        0      787 2023-03-08 22:15:55.000000 analyzr-sdk-python-1.2.56/analyzrclient/__init__.py
--rw-rw-rw-   0        0        0     2954 2023-05-31 13:20:37.000000 analyzr-sdk-python-1.2.56/analyzrclient/analyzer.py
--rw-rw-rw-   0        0        0     2943 2023-03-08 22:15:55.000000 analyzr-sdk-python-1.2.56/analyzrclient/client_basic_auth.py
--rw-rw-rw-   0        0        0     7613 2023-03-08 22:15:55.000000 analyzr-sdk-python-1.2.56/analyzrclient/client_saml_sso.py
--rw-rw-rw-   0        0        0     1407 2023-03-21 15:29:18.000000 analyzr-sdk-python-1.2.56/analyzrclient/constants.py
--rw-rw-rw-   0        0        0    19440 2023-03-29 19:46:12.000000 analyzr-sdk-python-1.2.56/analyzrclient/runner_base.py
--rw-rw-rw-   0        0        0    21393 2023-02-17 15:43:16.000000 analyzr-sdk-python-1.2.56/analyzrclient/runner_cluster.py
--rw-rw-rw-   0        0        0    25279 2023-02-17 14:52:41.000000 analyzr-sdk-python-1.2.56/analyzrclient/runner_propensity.py
--rw-rw-rw-   0        0        0    15891 2023-05-31 19:42:31.000000 analyzr-sdk-python-1.2.56/analyzrclient/runner_psm.py
--rw-rw-rw-   0        0        0    18644 2022-10-28 15:56:07.000000 analyzr-sdk-python-1.2.56/analyzrclient/runner_regression.py
--rw-rw-rw-   0        0        0     2963 2022-10-26 13:17:54.000000 analyzr-sdk-python-1.2.56/analyzrclient/runner_task.py
--rw-rw-rw-   0        0        0     9700 2022-10-24 20:38:31.000000 analyzr-sdk-python-1.2.56/analyzrclient/utils.py
--rw-rw-rw-   0        0        0      235 2022-10-25 12:57:59.000000 analyzr-sdk-python-1.2.56/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 19:44:07.431829 analyzr-sdk-python-1.2.56/setup.cfg
--rw-rw-rw-   0        0        0      771 2023-05-31 19:42:50.000000 analyzr-sdk-python-1.2.56/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:57:43.015370 analyzr-sdk-python-1.2.57/
+-rw-rw-rw-   0        0        0    11558 2022-10-21 16:54:33.000000 analyzr-sdk-python-1.2.57/LICENSE
+-rw-rw-rw-   0        0        0     2259 2023-06-14 16:57:43.013363 analyzr-sdk-python-1.2.57/PKG-INFO
+-rw-rw-rw-   0        0        0     1748 2023-05-31 11:48:21.000000 analyzr-sdk-python-1.2.57/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 16:57:42.961561 analyzr-sdk-python-1.2.57/analyzr_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0     2259 2023-06-14 16:57:42.000000 analyzr-sdk-python-1.2.57/analyzr_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      605 2023-06-14 16:57:42.000000 analyzr-sdk-python-1.2.57/analyzr_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 16:57:42.000000 analyzr-sdk-python-1.2.57/analyzr_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-14 16:57:42.000000 analyzr-sdk-python-1.2.57/analyzr_sdk_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 16:57:43.002842 analyzr-sdk-python-1.2.57/analyzrclient/
+-rw-rw-rw-   0        0        0      787 2023-03-08 22:15:55.000000 analyzr-sdk-python-1.2.57/analyzrclient/__init__.py
+-rw-rw-rw-   0        0        0     2954 2023-05-31 13:20:37.000000 analyzr-sdk-python-1.2.57/analyzrclient/analyzer.py
+-rw-rw-rw-   0        0        0     2943 2023-03-08 22:15:55.000000 analyzr-sdk-python-1.2.57/analyzrclient/client_basic_auth.py
+-rw-rw-rw-   0        0        0     7613 2023-03-08 22:15:55.000000 analyzr-sdk-python-1.2.57/analyzrclient/client_saml_sso.py
+-rw-rw-rw-   0        0        0     1407 2023-03-21 15:29:18.000000 analyzr-sdk-python-1.2.57/analyzrclient/constants.py
+-rw-rw-rw-   0        0        0    19440 2023-03-29 19:46:12.000000 analyzr-sdk-python-1.2.57/analyzrclient/runner_base.py
+-rw-rw-rw-   0        0        0    21393 2023-02-17 15:43:16.000000 analyzr-sdk-python-1.2.57/analyzrclient/runner_cluster.py
+-rw-rw-rw-   0        0        0    25279 2023-02-17 14:52:41.000000 analyzr-sdk-python-1.2.57/analyzrclient/runner_propensity.py
+-rw-rw-rw-   0        0        0    16563 2023-06-13 15:47:15.000000 analyzr-sdk-python-1.2.57/analyzrclient/runner_psm.py
+-rw-rw-rw-   0        0        0    18644 2022-10-28 15:56:07.000000 analyzr-sdk-python-1.2.57/analyzrclient/runner_regression.py
+-rw-rw-rw-   0        0        0     2963 2022-10-26 13:17:54.000000 analyzr-sdk-python-1.2.57/analyzrclient/runner_task.py
+-rw-rw-rw-   0        0        0     9700 2022-10-24 20:38:31.000000 analyzr-sdk-python-1.2.57/analyzrclient/utils.py
+-rw-rw-rw-   0        0        0      235 2022-10-25 12:57:59.000000 analyzr-sdk-python-1.2.57/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 16:57:43.016369 analyzr-sdk-python-1.2.57/setup.cfg
+-rw-rw-rw-   0        0        0      771 2023-06-14 16:49:05.000000 analyzr-sdk-python-1.2.57/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:57:43.010362 analyzr-sdk-python-1.2.57/tests/
+-rw-rw-rw-   0        0        0    34500 2023-06-12 21:24:03.000000 analyzr-sdk-python-1.2.57/tests/test_all.py
+-rw-rw-rw-   0        0        0    11110 2023-06-13 15:34:08.000000 analyzr-sdk-python-1.2.57/tests/test_quick.py
```

### Comparing `analyzr-sdk-python-1.2.56/LICENSE` & `analyzr-sdk-python-1.2.57/LICENSE`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.2.56/PKG-INFO` & `analyzr-sdk-python-1.2.57/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: analyzr-sdk-python
-Version: 1.2.56
+Version: 1.2.57
 Summary: Python SDK for Analyzr API
 Home-page: https://github.com/analyzr-ai/analyzr-sdk-python
 Author: Analyzr Team
 Author-email: support@analyzr.ai
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -52,8 +51,7 @@
 python -m unittest tests.test_quick -v # quick tests
 ```
 Make sure you update the `config.json` file first to include the name of your API tenant. 
 To run a single test case do:
 ```
 python -m unittest tests.test_all.PropensityTest.test_logistic_regression_classifier -v
 ```
-
```

### Comparing `analyzr-sdk-python-1.2.56/README.md` & `analyzr-sdk-python-1.2.57/README.md`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.2.56/analyzr_sdk_python.egg-info/PKG-INFO` & `analyzr-sdk-python-1.2.57/analyzr_sdk_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: analyzr-sdk-python
-Version: 1.2.56
+Version: 1.2.57
 Summary: Python SDK for Analyzr API
 Home-page: https://github.com/analyzr-ai/analyzr-sdk-python
 Author: Analyzr Team
 Author-email: support@analyzr.ai
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -52,8 +51,7 @@
 python -m unittest tests.test_quick -v # quick tests
 ```
 Make sure you update the `config.json` file first to include the name of your API tenant. 
 To run a single test case do:
 ```
 python -m unittest tests.test_all.PropensityTest.test_logistic_regression_classifier -v
 ```
-
```

### Comparing `analyzr-sdk-python-1.2.56/analyzr_sdk_python.egg-info/SOURCES.txt` & `analyzr-sdk-python-1.2.57/analyzr_sdk_python.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -13,8 +13,10 @@
 analyzrclient/constants.py
 analyzrclient/runner_base.py
 analyzrclient/runner_cluster.py
 analyzrclient/runner_propensity.py
 analyzrclient/runner_psm.py
 analyzrclient/runner_regression.py
 analyzrclient/runner_task.py
-analyzrclient/utils.py
+analyzrclient/utils.py
+tests/test_all.py
+tests/test_quick.py
```

### Comparing `analyzr-sdk-python-1.2.56/analyzrclient/__init__.py` & `analyzr-sdk-python-1.2.57/analyzrclient/__init__.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.2.56/analyzrclient/analyzer.py` & `analyzr-sdk-python-1.2.57/analyzrclient/analyzer.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.2.56/analyzrclient/client_basic_auth.py` & `analyzr-sdk-python-1.2.57/analyzrclient/client_basic_auth.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.2.56/analyzrclient/client_saml_sso.py` & `analyzr-sdk-python-1.2.57/analyzrclient/client_saml_sso.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.2.56/analyzrclient/constants.py` & `analyzr-sdk-python-1.2.57/analyzrclient/constants.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.2.56/analyzrclient/runner_base.py` & `analyzr-sdk-python-1.2.57/analyzrclient/runner_base.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.2.56/analyzrclient/runner_cluster.py` & `analyzr-sdk-python-1.2.57/analyzrclient/runner_cluster.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.2.56/analyzrclient/runner_propensity.py` & `analyzr-sdk-python-1.2.57/analyzrclient/runner_propensity.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.2.56/analyzrclient/runner_psm.py` & `analyzr-sdk-python-1.2.57/analyzrclient/runner_psm.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,24 +57,25 @@
                     # Load encoding keys
                     keys = self._keys_load(model_id=model_id, verbose=verbose)
                     if keys is None:
                         print('ERROR! Keys not found. ')
                         return None
                 else:
                     keys = {}
-                atx, raw, misc = self.__retrieve_train_results(
+                atx, raw, misc, bins = self.__retrieve_train_results(
                         request_id=model_id,
                         client_id=client_id,
                         fref=keys['fref_exp'] if encoding else {},
                         zref=keys['zref'] if encoding else {}, 
                         verbose=verbose,
                         encoding=encoding)
                 res1['atx'] = atx
                 res1['raw'] = raw
                 res1['misc'] = misc
+                res1['bins'] = bins
             if res2['status'] in ['Complete', 'Failed']:
                 self._buffer_clear(
                     request_id=model_id, client_id=client_id,
                     verbose=verbose)
         return res1
 
     def train(self, df, client_id=None,
@@ -134,14 +135,15 @@
         :type encoding: boolean, optional
         :return: JSON object with the following attributes, as applicable:
                     `model_id` (UUID provided with initial request),
                     `atx` (average treatment effects),
                     `raw` (dataset stats prior to matching),
                     `misc` (miscellaneous error stats including accuracy, precision, recall,
                     F1, AUC, Gini),
+                    `bins` (histogram of matched propensity scores)
         """
 
         # Encode data
         request_id = self._get_request_id()
         if verbose: print('Model ID: {}'.format(request_id))
         if encoding:
             data, xref, zref, rref, fref, fref_exp, bref = self._encode(
@@ -186,15 +188,15 @@
                         'client_id': client_id,
                         'command': 'task-status'
                     },
                     timeout=timeout,
                     step=step,
                     verbose=verbose)
                 if res2['response']['status'] in ['Complete']:
-                    atx, raw, misc = self.__retrieve_train_results(
+                    atx, raw, misc, bins = self.__retrieve_train_results(
                         request_id=request_id,
                         client_id=client_id,
                         fref=fref_exp if encoding else {},
                         zref=zref if encoding else {},
                         outcome_var=outcome_var,
                         verbose=verbose,
                         encoding=encoding)
@@ -212,14 +214,15 @@
         if verbose and not poll: print('Training job started with polling disabled. You will need to request results for this model ID.')
         res5 = {}
         res5['model_id'] = request_id
         if poll:
             res5['atx'] = atx
             res5['raw'] = raw
             res5['misc'] = misc
+            res5['bins'] = bins
         return res5
 
     def __train(self, request_id=None, client_id=None,
             idx_field=None, outcome_var=None, treatment_var=None, categorical_fields=[],
             verbose=False, staging=False):
         """
         :param request_id:
@@ -232,15 +235,15 @@
         :param categorical_fields:
         :param verbose: Set to true for verbose output
         :param staging:
         :return:
         """
         if verbose: print('Training propensity score matching model using data in buffer...')
         res = self._client._post(self.__uri, {
-            'command': 'psm-train',
+            'command': 'matching-train',
             'request_id': request_id,
             'client_id': client_id,
             'idx_field': idx_field,
             'outcome_var': outcome_var,
             'treatment_var': treatment_var,
             'categorical_fields': categorical_fields,
             'staging': staging,
@@ -294,17 +297,28 @@
         if verbose: print('    Retrieving miscellaneous stats...')
         misc = self._buffer_read(
             request_id=request_id, client_id=client_id, dataframe_name='misc',
             verbose=verbose)
         if not misc.empty:
             misc['Value'] = misc['Value'].astype('float')
         else:
-            if verbose: print('WARNING! Raw stats dataframe is empty')
+            if verbose: print('WARNING! Miscellaneous stats dataframe is empty')
 
-        return atx, raw, misc 
+        # Binned stats
+        if verbose: print('    Retrieving binned stats...')
+        bins = self._buffer_read(
+            request_id=request_id, client_id=client_id, dataframe_name='bins',
+            verbose=verbose)
+        if not bins.empty:
+            bins['count_treated'] = bins['count_treated'].astype('int')
+            bins['count_untreated'] = bins['count_untreated'].astype('int')
+        else:
+            if verbose: print('WARNING! Binned stats dataframe is empty')
+
+        return atx, raw, misc, bins 
 
     def __decode_raw_stats(self, raw, fref={}, zref={}, outcome_var=None, verbose=False):
         """
         Decode raw stats. Note that homomorphic encryption is only homomorphic with averages. 
         Other stats are set to None durign decryption.
 
         :param raw:
```

### Comparing `analyzr-sdk-python-1.2.56/analyzrclient/runner_regression.py` & `analyzr-sdk-python-1.2.57/analyzrclient/runner_regression.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.2.56/analyzrclient/runner_task.py` & `analyzr-sdk-python-1.2.57/analyzrclient/runner_task.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.2.56/analyzrclient/utils.py` & `analyzr-sdk-python-1.2.57/analyzrclient/utils.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.2.56/setup.py` & `analyzr-sdk-python-1.2.57/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name='analyzr-sdk-python',
-    version='1.2.56',
+    version='1.2.57',
     description='Python SDK for Analyzr API',
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/analyzr-ai/analyzr-sdk-python",
     author='Analyzr Team',
     author_email='support@analyzr.ai',
     license='Apache 2.0',
```

