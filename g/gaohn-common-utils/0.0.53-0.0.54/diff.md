# Comparing `tmp/gaohn-common-utils-0.0.53.tar.gz` & `tmp/gaohn-common-utils-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.53.tar", last modified: Wed Jun 14 11:05:34 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.54.tar", last modified: Wed Jun 14 12:13:04 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.53.tar` & `gaohn-common-utils-0.0.54.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:34.429039 gaohn-common-utils-0.0.53/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 11:05:34.429039 gaohn-common-utils-0.0.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:34.425039 gaohn-common-utils-0.0.53/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:34.425039 gaohn-common-utils-0.0.53/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:34.425039 gaohn-common-utils-0.0.53/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:34.425039 gaohn-common-utils-0.0.53/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:34.425039 gaohn-common-utils-0.0.53/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:34.425039 gaohn-common-utils-0.0.53/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:34.425039 gaohn-common-utils-0.0.53/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:34.425039 gaohn-common-utils-0.0.53/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:34.425039 gaohn-common-utils-0.0.53/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:34.425039 gaohn-common-utils-0.0.53/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:34.425039 gaohn-common-utils-0.0.53/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:34.429039 gaohn-common-utils-0.0.53/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 11:05:34.000000 gaohn-common-utils-0.0.53/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-14 11:05:34.000000 gaohn-common-utils-0.0.53/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:05:34.000000 gaohn-common-utils-0.0.53/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-14 11:05:34.000000 gaohn-common-utils-0.0.53/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 11:05:34.000000 gaohn-common-utils-0.0.53/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-14 11:05:17.000000 gaohn-common-utils-0.0.53/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:05:34.429039 gaohn-common-utils-0.0.53/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:13:04.140551 gaohn-common-utils-0.0.54/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 12:13:04.140551 gaohn-common-utils-0.0.54/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:13:04.136551 gaohn-common-utils-0.0.54/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:13:04.136551 gaohn-common-utils-0.0.54/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:13:04.132551 gaohn-common-utils-0.0.54/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:13:04.136551 gaohn-common-utils-0.0.54/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:13:04.136551 gaohn-common-utils-0.0.54/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:13:04.136551 gaohn-common-utils-0.0.54/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:13:04.136551 gaohn-common-utils-0.0.54/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:13:04.136551 gaohn-common-utils-0.0.54/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:13:04.136551 gaohn-common-utils-0.0.54/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:13:04.136551 gaohn-common-utils-0.0.54/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:13:04.136551 gaohn-common-utils-0.0.54/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:13:04.140551 gaohn-common-utils-0.0.54/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 12:13:04.000000 gaohn-common-utils-0.0.54/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-14 12:13:04.000000 gaohn-common-utils-0.0.54/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:13:04.000000 gaohn-common-utils-0.0.54/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-14 12:13:04.000000 gaohn-common-utils-0.0.54/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 12:13:04.000000 gaohn-common-utils-0.0.54/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-14 12:12:45.000000 gaohn-common-utils-0.0.54/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:13:04.140551 gaohn-common-utils-0.0.54/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.53/LICENSE` & `gaohn-common-utils-0.0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.53/PKG-INFO` & `gaohn-common-utils-0.0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.53
+Version: 0.0.54
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.53/README.md` & `gaohn-common-utils-0.0.54/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.53/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.54/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.53/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.54/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.53/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.54/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.53/common_utils/core/base.py` & `gaohn-common-utils-0.0.54/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.53/common_utils/core/common.py` & `gaohn-common-utils-0.0.54/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.53/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.54/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.53/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.54/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.53/common_utils/core/logger.py` & `gaohn-common-utils-0.0.54/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.53/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.54/common_utils/data_validator/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """This module aims to mimic the functionality of Great Expectations, but with a
-very minimalistic approach just to illustrate the concept."""
+very minimalistic approach just to illustrate the concept.
+
+TODO: https://cloud.google.com/architecture/mlops-continuous-delivery-and-automation-pipelines-in-machine-learning#data_and_model_validation
+    - Add more validation methods.
+"""
 from __future__ import annotations
+
 from typing import Any, Dict
 
 import pandas as pd
-import pytest
+from rich.pretty import pprint
 
 from common_utils.core.logger import Logger
 
 # Setup logging
 logger = Logger(
     module_name=__name__, propagate=False, log_root_dir=None, log_file=None
 ).logger
@@ -28,31 +33,38 @@
 
     def __init__(self, df: pd.DataFrame, schema: Dict[str, Any]) -> None:
         self.df = df
         self.schema = schema
 
     def check_missing(self) -> DataFrameValidator:
         """Check if there are missing values in the dataframe."""
-        missing_data = self.df.isnull().sum()
-        if missing_data.any():
+        logger.info("Checking missing values...")
+        total = self.df.isnull().sum().sort_values(ascending=False)
+        percent = (self.df.isnull().sum() / self.df.isnull().count()).sort_values(
+            ascending=False
+        )
+        missing_data = pd.concat([total, percent], axis=1, keys=["Total", "Percent"])
+        if missing_data["Total"].any():
             logger.warning("The following columns have missing data:")
-            logger.warning(missing_data[missing_data > 0])
+            pprint(missing_data[missing_data["Total"] > 0])
         return self
 
     def check_data_types(self) -> DataFrameValidator:
         """Check if the data types of the dataframe's columns match the expected schema."""
+        logger.info("Checking data types...")
         for column, dtype in self.schema.items():
             if self.df[column].dtype != dtype:
                 logger.warning(
                     f"The data type for {column} is not {dtype}, it's {self.df[column].dtype}"
                 )
         return self
 
     def check_schema(self) -> DataFrameValidator:
         """Check if the schema of the dataframe matches the expected schema."""
+        logger.info("Checking schema...")
         for column in self.schema.keys():
             if column not in self.df.columns:
                 logger.warning(
                     f"Expected {column} in the dataframe, but it's not present."
                 )
         for column in self.df.columns:
             if column not in self.schema.keys():
```

### Comparing `gaohn-common-utils-0.0.53/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.54/common_utils/versioning/dvc/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.53/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.54/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.53/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.54/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.53
+Version: 0.0.54
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.53/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.54/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.53/pyproject.toml` & `gaohn-common-utils-0.0.54/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.53"
+version = "0.0.54"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

