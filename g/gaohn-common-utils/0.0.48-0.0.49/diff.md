# Comparing `tmp/gaohn-common-utils-0.0.48.tar.gz` & `tmp/gaohn-common-utils-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.48.tar", last modified: Tue Jun 13 10:34:35 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.49.tar", last modified: Wed Jun 14 10:08:38 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.48.tar` & `gaohn-common-utils-0.0.49.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:35.139596 gaohn-common-utils-0.0.48/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 10:34:35.139596 gaohn-common-utils-0.0.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:35.139596 gaohn-common-utils-0.0.48/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:35.139596 gaohn-common-utils-0.0.48/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:35.135596 gaohn-common-utils-0.0.48/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:35.139596 gaohn-common-utils-0.0.48/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:35.139596 gaohn-common-utils-0.0.48/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:35.139596 gaohn-common-utils-0.0.48/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:35.139596 gaohn-common-utils-0.0.48/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:35.139596 gaohn-common-utils-0.0.48/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:35.139596 gaohn-common-utils-0.0.48/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:34:35.139596 gaohn-common-utils-0.0.48/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 10:34:35.000000 gaohn-common-utils-0.0.48/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 10:34:35.000000 gaohn-common-utils-0.0.48/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:34:35.000000 gaohn-common-utils-0.0.48/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 10:34:35.000000 gaohn-common-utils-0.0.48/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 10:34:35.000000 gaohn-common-utils-0.0.48/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 10:34:16.000000 gaohn-common-utils-0.0.48/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 10:34:35.139596 gaohn-common-utils-0.0.48/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:38.095180 gaohn-common-utils-0.0.49/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 10:08:38.095180 gaohn-common-utils-0.0.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:38.095180 gaohn-common-utils-0.0.49/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:38.095180 gaohn-common-utils-0.0.49/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:38.091179 gaohn-common-utils-0.0.49/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:38.095180 gaohn-common-utils-0.0.49/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:38.095180 gaohn-common-utils-0.0.49/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:38.095180 gaohn-common-utils-0.0.49/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:38.095180 gaohn-common-utils-0.0.49/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:38.091179 gaohn-common-utils-0.0.49/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:38.095180 gaohn-common-utils-0.0.49/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:38.095180 gaohn-common-utils-0.0.49/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:38.095180 gaohn-common-utils-0.0.49/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 10:08:38.000000 gaohn-common-utils-0.0.49/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-14 10:08:38.000000 gaohn-common-utils-0.0.49/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:08:38.000000 gaohn-common-utils-0.0.49/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-14 10:08:38.000000 gaohn-common-utils-0.0.49/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 10:08:38.000000 gaohn-common-utils-0.0.49/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-14 10:08:14.000000 gaohn-common-utils-0.0.49/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 10:08:38.095180 gaohn-common-utils-0.0.49/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.48/LICENSE` & `gaohn-common-utils-0.0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.48/PKG-INFO` & `gaohn-common-utils-0.0.49/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,75 +1,81 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.48
+Version: 0.0.49
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# Continuous Integration
+# Common Utils
 
 [![Continuous Integration](https://github.com/gao-hongnan/common-utils/actions/workflows/ci.yaml/badge.svg?branch=continuous-integration)](https://github.com/gao-hongnan/common-utils/actions/workflows/ci.yaml)
 
-## Virtual Environment
+## TODOs
+
+1. Use own `Logger` once the class is finalized in all scripts.
+
+## Continuous Integration
+
+### Virtual Environment
 
 First, make a virtual environment with `make_venv.sh`:
 
 ```bash
 curl -s -o make_venv.sh \
   https://raw.githubusercontent.com/gao-hongnan/common-utils/main/scripts/devops/make_venv.sh && \
 bash make_venv.sh venv --pyproject --dev && \
 source venv/bin/activate && \
 rm make_venv.sh
 ```
 
-## Continue on error vs If Always
+### Continue on error vs If Always
 
 See [here](https://stackoverflow.com/questions/58858429/how-to-run-a-github-actions-step-even-if-the-previous-step-fails-while-still-f/58859404#58859404).
 
-## Run Bandit Security Check
+### Run Bandit Security Check
 
 ```bash
 bash ./scripts/devops/ci/ci_security_bandit.sh \
   --severity-level=low \
   --format=json \
   --output=bandit_results.json \
   common_utils
 ```
 
-## Run Linter Check
+### Run Linter Check
 
 ```bash
 bash ./scripts/devops/ci/ci_linter_pylint.sh \
   --rcfile=pyproject.toml \
   --fail-under=10 \
   --score=yes \
   --output-format=json:pylint_results.json,colorized \
   common_utils
 ```
 
-## Run Formatter Black Check
+### Run Formatter Black Check
 
 ```bash
 bash ./scripts/devops/ci/ci_formatter_black.sh \
   --check \
   --diff \
   --color \
   --verbose \
   common_utils
 ```
 
-## Run Formatter Isort Check
+### Run Formatter Isort Check
 
 ```bash
 bash ./scripts/devops/ci/ci_formatter_isort.sh \
   --check \
   --diff \
   --color \
   --verbose \
@@ -81,18 +87,18 @@
 ```bash
 bash ./scripts/devops/ci/ci_typing_mypy.sh \
   --config-file=pyproject.toml \
   common_utils \
   | tee mypy_results.log
 ```
 
-## Run Unit Test
+### Run Unit Test
 
 ## Run Integration Test
 
-## Run System Test
+### Run System Test
 
-## Run Acceptance Test
+### Run Acceptance Test
 
 https://madewithml.com/courses/mlops/testing/
 
-## Run Data Test (Great Expectations)
+### Run Data Test (Great Expectations)
```

### Comparing `gaohn-common-utils-0.0.48/README.md` & `gaohn-common-utils-0.0.49/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,66 @@
-# Continuous Integration
+# Common Utils
 
 [![Continuous Integration](https://github.com/gao-hongnan/common-utils/actions/workflows/ci.yaml/badge.svg?branch=continuous-integration)](https://github.com/gao-hongnan/common-utils/actions/workflows/ci.yaml)
 
-## Virtual Environment
+## TODOs
+
+1. Use own `Logger` once the class is finalized in all scripts.
+
+## Continuous Integration
+
+### Virtual Environment
 
 First, make a virtual environment with `make_venv.sh`:
 
 ```bash
 curl -s -o make_venv.sh \
   https://raw.githubusercontent.com/gao-hongnan/common-utils/main/scripts/devops/make_venv.sh && \
 bash make_venv.sh venv --pyproject --dev && \
 source venv/bin/activate && \
 rm make_venv.sh
 ```
 
-## Continue on error vs If Always
+### Continue on error vs If Always
 
 See [here](https://stackoverflow.com/questions/58858429/how-to-run-a-github-actions-step-even-if-the-previous-step-fails-while-still-f/58859404#58859404).
 
-## Run Bandit Security Check
+### Run Bandit Security Check
 
 ```bash
 bash ./scripts/devops/ci/ci_security_bandit.sh \
   --severity-level=low \
   --format=json \
   --output=bandit_results.json \
   common_utils
 ```
 
-## Run Linter Check
+### Run Linter Check
 
 ```bash
 bash ./scripts/devops/ci/ci_linter_pylint.sh \
   --rcfile=pyproject.toml \
   --fail-under=10 \
   --score=yes \
   --output-format=json:pylint_results.json,colorized \
   common_utils
 ```
 
-## Run Formatter Black Check
+### Run Formatter Black Check
 
 ```bash
 bash ./scripts/devops/ci/ci_formatter_black.sh \
   --check \
   --diff \
   --color \
   --verbose \
   common_utils
 ```
 
-## Run Formatter Isort Check
+### Run Formatter Isort Check
 
 ```bash
 bash ./scripts/devops/ci/ci_formatter_isort.sh \
   --check \
   --diff \
   --color \
   --verbose \
@@ -66,18 +72,18 @@
 ```bash
 bash ./scripts/devops/ci/ci_typing_mypy.sh \
   --config-file=pyproject.toml \
   common_utils \
   | tee mypy_results.log
 ```
 
-## Run Unit Test
+### Run Unit Test
 
 ## Run Integration Test
 
-## Run System Test
+### Run System Test
 
-## Run Acceptance Test
+### Run Acceptance Test
 
 https://madewithml.com/courses/mlops/testing/
 
-## Run Data Test (Great Expectations)
+### Run Data Test (Great Expectations)
```

### Comparing `gaohn-common-utils-0.0.48/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.49/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.48/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.49/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.48/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.49/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.48/common_utils/core/base.py` & `gaohn-common-utils-0.0.49/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.48/common_utils/core/common.py` & `gaohn-common-utils-0.0.49/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.48/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.49/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.48/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.49/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.48/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.49/common_utils/versioning/dvc/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 import shutil
 from pathlib import Path
 from typing import Dict
 
 from common_utils.core.base import Storage
 
 
+# pylint: disable=line-too-long
 class SimpleDVC:
     """
+    # TODO: try to see if we can make it work for local storage as well.
+
     LOCAL TREE
     pipeline-training/data
     ├── interim
     ├── processed
     └── raw
         ├── filtered_movies_incremental.csv             # filename
         └── filtered_movies_incremental.csv.json        # metadata for filename
```

### Comparing `gaohn-common-utils-0.0.48/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.49/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,75 +1,81 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.48
+Version: 0.0.49
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# Continuous Integration
+# Common Utils
 
 [![Continuous Integration](https://github.com/gao-hongnan/common-utils/actions/workflows/ci.yaml/badge.svg?branch=continuous-integration)](https://github.com/gao-hongnan/common-utils/actions/workflows/ci.yaml)
 
-## Virtual Environment
+## TODOs
+
+1. Use own `Logger` once the class is finalized in all scripts.
+
+## Continuous Integration
+
+### Virtual Environment
 
 First, make a virtual environment with `make_venv.sh`:
 
 ```bash
 curl -s -o make_venv.sh \
   https://raw.githubusercontent.com/gao-hongnan/common-utils/main/scripts/devops/make_venv.sh && \
 bash make_venv.sh venv --pyproject --dev && \
 source venv/bin/activate && \
 rm make_venv.sh
 ```
 
-## Continue on error vs If Always
+### Continue on error vs If Always
 
 See [here](https://stackoverflow.com/questions/58858429/how-to-run-a-github-actions-step-even-if-the-previous-step-fails-while-still-f/58859404#58859404).
 
-## Run Bandit Security Check
+### Run Bandit Security Check
 
 ```bash
 bash ./scripts/devops/ci/ci_security_bandit.sh \
   --severity-level=low \
   --format=json \
   --output=bandit_results.json \
   common_utils
 ```
 
-## Run Linter Check
+### Run Linter Check
 
 ```bash
 bash ./scripts/devops/ci/ci_linter_pylint.sh \
   --rcfile=pyproject.toml \
   --fail-under=10 \
   --score=yes \
   --output-format=json:pylint_results.json,colorized \
   common_utils
 ```
 
-## Run Formatter Black Check
+### Run Formatter Black Check
 
 ```bash
 bash ./scripts/devops/ci/ci_formatter_black.sh \
   --check \
   --diff \
   --color \
   --verbose \
   common_utils
 ```
 
-## Run Formatter Isort Check
+### Run Formatter Isort Check
 
 ```bash
 bash ./scripts/devops/ci/ci_formatter_isort.sh \
   --check \
   --diff \
   --color \
   --verbose \
@@ -81,18 +87,18 @@
 ```bash
 bash ./scripts/devops/ci/ci_typing_mypy.sh \
   --config-file=pyproject.toml \
   common_utils \
   | tee mypy_results.log
 ```
 
-## Run Unit Test
+### Run Unit Test
 
 ## Run Integration Test
 
-## Run System Test
+### Run System Test
 
-## Run Acceptance Test
+### Run Acceptance Test
 
 https://madewithml.com/courses/mlops/testing/
 
-## Run Data Test (Great Expectations)
+### Run Data Test (Great Expectations)
```

### Comparing `gaohn-common-utils-0.0.48/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.49/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,12 +10,15 @@
 common_utils/core/base.py
 common_utils/core/common.py
 common_utils/core/decorators.py
 common_utils/core/file_system_utils.py
 common_utils/core/logger.py
 common_utils/orchestrator/base.py
 common_utils/versioning/dvc/base.py
+common_utils/versioning/dvc/core.py
+common_utils/versioning/git/base.py
+common_utils/versioning/git/core.py
 gaohn_common_utils.egg-info/PKG-INFO
 gaohn_common_utils.egg-info/SOURCES.txt
 gaohn_common_utils.egg-info/dependency_links.txt
 gaohn_common_utils.egg-info/requires.txt
 gaohn_common_utils.egg-info/top_level.txt
```

### Comparing `gaohn-common-utils-0.0.48/pyproject.toml` & `gaohn-common-utils-0.0.49/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.48"
+version = "0.0.49"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -41,14 +41,16 @@
     "pytest==6.2.5",
     "mypy==1.3.0",
     "isort==5.12.0",
     "bandit==1.7.5",
     "mypy==1.3.0",
     "toml==0.10.2",
     "colorama==0.4.4",
+    "pytest-cov==4.0.0",
+    "coverage==7.0.5",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/gao-hongnan/common-utils"
 "Bug Tracker" = "https://github.com/gao-hongnan/common-utils/issues"
 
 [tool.black]
```

