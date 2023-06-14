# Comparing `tmp/BiocFrame-0.2.8.tar.gz` & `tmp/BiocFrame-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BiocFrame-0.2.8.tar", last modified: Mon Mar 20 17:17:18 2023, max compression
+gzip compressed data, was "BiocFrame-0.2.9.tar", last modified: Thu Mar 23 02:09:59 2023, max compression
```

## Comparing `BiocFrame-0.2.8.tar` & `BiocFrame-0.2.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-20 17:17:18.799723 BiocFrame-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/.coveragerc
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-20 17:17:18.787723 BiocFrame-0.2.8/.github/
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-20 17:17:18.791723 BiocFrame-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     3604 2023-03-20 17:17:18.799723 BiocFrame-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/README.md
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-20 17:17:18.795724 BiocFrame-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/docs/Makefile
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-20 17:17:18.795724 BiocFrame-0.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-20 17:17:18.799723 BiocFrame-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/setup.py
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-20 17:17:18.787723 BiocFrame-0.2.8/src/
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-20 17:17:18.795724 BiocFrame-0.2.8/src/BiocFrame.egg-info/
--rw-rw-rw-   0 runner    (1001) docker     (123)     3604 2023-03-20 17:17:18.000000 BiocFrame-0.2.8/src/BiocFrame.egg-info/PKG-INFO
--rw-rw-rw-   0 runner    (1001) docker     (123)      867 2023-03-20 17:17:18.000000 BiocFrame-0.2.8/src/BiocFrame.egg-info/SOURCES.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)        1 2023-03-20 17:17:18.000000 BiocFrame-0.2.8/src/BiocFrame.egg-info/dependency_links.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)        1 2023-03-20 17:17:18.000000 BiocFrame-0.2.8/src/BiocFrame.egg-info/not-zip-safe
--rw-rw-rw-   0 runner    (1001) docker     (123)       99 2023-03-20 17:17:18.000000 BiocFrame-0.2.8/src/BiocFrame.egg-info/requires.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)       10 2023-03-20 17:17:18.000000 BiocFrame-0.2.8/src/BiocFrame.egg-info/top_level.txt
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-20 17:17:18.799723 BiocFrame-0.2.8/src/biocframe/
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/src/biocframe/BiocFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/src/biocframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/src/biocframe/_validators.py
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-20 17:17:18.799723 BiocFrame-0.2.8/src/biocframe/io/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/src/biocframe/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/src/biocframe/io/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/src/biocframe/utils.py
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-20 17:17:18.799723 BiocFrame-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/tests/test_initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-03-20 17:15:58.000000 BiocFrame-0.2.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:09:59.532919 BiocFrame-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:09:59.508916 BiocFrame-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:09:59.520918 BiocFrame-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-03-23 02:09:59.532919 BiocFrame-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:09:59.520918 BiocFrame-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:09:59.520918 BiocFrame-0.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-23 02:09:59.532919 BiocFrame-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:09:59.512917 BiocFrame-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:09:59.524918 BiocFrame-0.2.9/src/BiocFrame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-03-23 02:09:59.000000 BiocFrame-0.2.9/src/BiocFrame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-23 02:09:59.000000 BiocFrame-0.2.9/src/BiocFrame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 02:09:59.000000 BiocFrame-0.2.9/src/BiocFrame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 02:09:59.000000 BiocFrame-0.2.9/src/BiocFrame.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-23 02:09:59.000000 BiocFrame-0.2.9/src/BiocFrame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-23 02:09:59.000000 BiocFrame-0.2.9/src/BiocFrame.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:09:59.528918 BiocFrame-0.2.9/src/biocframe/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/src/biocframe/BiocFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/src/biocframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/src/biocframe/_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:09:59.528918 BiocFrame-0.2.9/src/biocframe/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/src/biocframe/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/src/biocframe/io/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/src/biocframe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:09:59.532919 BiocFrame-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/tests/test_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-03-23 02:08:49.000000 BiocFrame-0.2.9/tox.ini
```

### Comparing `BiocFrame-0.2.8/.coveragerc` & `BiocFrame-0.2.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/.github/workflows/pypi-publish.yml` & `BiocFrame-0.2.9/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/.github/workflows/pypi-test.yml` & `BiocFrame-0.2.9/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/.gitignore` & `BiocFrame-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/CONTRIBUTING.md` & `BiocFrame-0.2.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/LICENSE.txt` & `BiocFrame-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/PKG-INFO` & `BiocFrame-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BiocFrame
-Version: 0.2.8
+Version: 0.2.9
 Summary: BiocFrame class to support complex types in Genomics. The goal is to not compete with `Pandas` but be inter-operable at some point.
 Home-page: https://github.com/BiocPy/biocframe
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/biocframe
 Project-URL: Source, https://github.com/BiocPy/biocframe
```

### Comparing `BiocFrame-0.2.8/README.md` & `BiocFrame-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/docs/Makefile` & `BiocFrame-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/docs/conf.py` & `BiocFrame-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/docs/index.md` & `BiocFrame-0.2.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/setup.cfg` & `BiocFrame-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/setup.py` & `BiocFrame-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/src/BiocFrame.egg-info/PKG-INFO` & `BiocFrame-0.2.9/src/BiocFrame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BiocFrame
-Version: 0.2.8
+Version: 0.2.9
 Summary: BiocFrame class to support complex types in Genomics. The goal is to not compete with `Pandas` but be inter-operable at some point.
 Home-page: https://github.com/BiocPy/biocframe
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/biocframe
 Project-URL: Source, https://github.com/BiocPy/biocframe
```

### Comparing `BiocFrame-0.2.8/src/BiocFrame.egg-info/SOURCES.txt` & `BiocFrame-0.2.9/src/BiocFrame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/src/biocframe/BiocFrame.py` & `BiocFrame-0.2.9/src/biocframe/BiocFrame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-from typing import Any, List, Union, Sequence, Optional, Tuple, MutableMapping
+from typing import Any, Union, Sequence, Optional, Tuple, MutableMapping
 from .utils import match_to_indices
 
 from ._validators import validate_rows, validate_cols, validate_unique_list
 from collections import OrderedDict
 import pandas as pd
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 class BiocFrame:
     def __init__(
         self,
-        data: Optional[MutableMapping[str, Union[List[Any], MutableMapping]]] = None,
+        data: Optional[
+            MutableMapping[str, Union[Sequence[Any], MutableMapping]]
+        ] = None,
         numberOfRows: Optional[int] = None,
         rowNames: Optional[Sequence[str]] = None,
         columnNames: Optional[Sequence[str]] = None,
         metadata: Optional[MutableMapping] = None,
     ) -> None:
         """Initialize a BiocFrame object.
 
@@ -28,15 +30,15 @@
         as a column. This allows us to be flexible, e.g: nested data frames 
         or `BiocFrame` objects as columns.
 
         Raises:
             ValueError: if rows or columns mismatch from data.
 
         Args:
-            data (MutableMapping[str, Union[List[Any], MutableMapping]], optional): 
+            data (MutableMapping[str, Union[Sequence[Any], MutableMapping]], optional): 
                 a dictionary of colums and their values. all columns must have the 
                 same length. Defaults to None.
             numberOfRows (int, optional): Number of rows. Defaults to None.
             rowNames (Sequence[str], optional): Row index values . Defaults to None.
             columnNames (Sequence[str], optional): column names, if not provided, 
                 its automatically inferred from data. Defaults to None.
             metadata (MutableMapping, optional): metadata. Defaults to None.
@@ -57,25 +59,25 @@
         Raises:
             ValueError: when provided object does not contain columns of same length.
         """
 
         self._numberOfRows = validate_rows(
             self._numberOfRows, self._rowNames, self._data
         )
-        self._columnNames = validate_cols(self._columnNames, self._data)
+        self._columnNames, self._data = validate_cols(self._columnNames, self._data)
 
         self._numberOfColumns = len(self._columnNames)
 
         if self._numberOfRows is None:
             self._numberOfRows = 0
 
     def __str__(self) -> str:
         pattern = (
-            f"Class BiocFrame with {self.dims[0]} rows and {self.dims[1]} columns"
-            f"  columnNames: {self.columnNames}"
+            f"Class BiocFrame with {self.dims[0]} rows and {self.dims[1]} columns\n"
+            f"  columnNames: {self.columnNames}\n"
             f"  contains rowNames?: {self.rowNames is None}"
         )
         return pattern
 
     @property
     def dims(self) -> Tuple[int, int]:
         """Dimensions of the BiocFrame.
@@ -100,19 +102,19 @@
 
         Returns:
             Optional[Sequence[str]]: row index names if available else None.
         """
         return self._rowNames
 
     @property
-    def data(self) -> MutableMapping[str, Union[List[Any], MutableMapping]]:
+    def data(self) -> MutableMapping[str, Union[Sequence[Any], MutableMapping]]:
         """Access data (as dictionary).
 
         Returns:
-            MutableMapping[str, Union[List[Any], MutableMapping]]: 
+            MutableMapping[str, Union[Sequence[Any], MutableMapping]]: 
                 dictionary of columns and their values.
         """
         return self._data
 
     @rowNames.setter
     def rowNames(self, names: Optional[Sequence[str]]):
         """Set new index.
@@ -305,15 +307,15 @@
 
         # slice the columns and data
         if colIndicesOrNames is not None:
             new_column_indices = match_to_indices(self._columnNames, colIndicesOrNames)
 
             if isinstance(new_column_indices, slice):
                 new_columnNames = new_columnNames[new_column_indices]
-            elif isinstance(new_column_indices, list):
+            elif isinstance(new_column_indices, Sequence):
                 new_columnNames = [new_columnNames[i] for i in new_column_indices]
             else:
                 raise TypeError("Column Slice: Unknown match_to_indices type")
 
         for col in new_columnNames:
             new_data[col] = self._data[col]
 
@@ -321,15 +323,15 @@
         if rowIndicesOrNames is not None:
             new_row_indices = rowIndicesOrNames
             if self._rowNames is not None:
                 new_row_indices = match_to_indices(self._rowNames, rowIndicesOrNames)
 
                 if isinstance(new_row_indices, slice):
                     new_rowNames = new_rowNames[new_row_indices]
-                elif isinstance(new_row_indices, list):
+                elif isinstance(new_row_indices, Sequence):
                     new_rowNames = [new_rowNames[i] for i in new_row_indices]
                 else:
                     raise TypeError("Row Slice: Unknown match_to_indices type")
 
             # since row names are not set, the
             # only option here is to slice by index
             if isinstance(new_row_indices, slice):
@@ -414,15 +416,15 @@
 
     # TODO: implement inplace, view
     def __setitem__(self, key: str, newvalue: Sequence[Any]):
         """Set/Assign a value to a column.
 
         Args:
             key (str): Column name.
-            newvalue (List[Any]): New value to set.
+            newvalue (Sequence[Any]): New value to set.
 
         Raises:
             ValueError: If length of `newvalue` does not match the length of the object.
         """
         if len(newvalue) != self._numberOfRows:
             raise ValueError(
                 f"new column:{key} has incorrect number of values. need to be {self._numberOfRows} but provided {len(newvalue)}"
```

### Comparing `BiocFrame-0.2.8/src/biocframe/__init__.py` & `BiocFrame-0.2.9/src/biocframe/__init__.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/src/biocframe/_validators.py` & `BiocFrame-0.2.9/src/biocframe/_validators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import Any, List, Union, Optional, MutableMapping, Sequence
+from typing import Any, Union, MutableMapping, Sequence
 from collections import OrderedDict
 
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 def validate_rows(
     numberOfRows: int,
     rowNames: Sequence[str],
-    data: MutableMapping[str, Union[List[Any], MutableMapping]],
+    data: MutableMapping[str, Union[Sequence[Any], MutableMapping]],
 ) -> int:
     """Validate rows of BiocFrame object.
 
     Args:
         numberOfRows (int, optional): Number of rows. Defaults to None.
         rowNames (Sequence[str], optional): Row index values . Defaults to None.
-        data (MutableMapping[str, Union[List[Any], MutableMapping]], optional): 
+        data (MutableMapping[str, Union[Sequence[Any], MutableMapping]], optional): 
             a dictionary of colums and their values. all columns must have the 
             same length. Defaults to {}.
 
     Raises:
         ValueError: when `numberOfRows` and `data` do not agree.
 
     Returns:
@@ -54,22 +54,22 @@
                 raise ValueError("length of `rowNames` and `numberOfRows` do not match")
 
     return numberOfRows
 
 
 def validate_cols(
     columnNames: Sequence[str],
-    data: MutableMapping[str, Union[List[Any], MutableMapping]],
+    data: MutableMapping[str, Union[Sequence[Any], MutableMapping]],
 ) -> Sequence[str]:
     """Validate columns of a BiocFrame object.
 
     Args:
         columnNames (Sequence[str], optional): column names, if not provided, 
             its automatically inferred from data. Defaults to None.
-        data (MutableMapping[str, Union[List[Any], MutableMapping]], optional): 
+        data (MutableMapping[str, Union[Sequence[Any], MutableMapping]], optional): 
             a dictionary of colums and their values. all columns must have the 
             same length. Defaults to {}.. Defaults to {}.
 
     Raises:
         ValueError: when `columnNames` and `data` do not agree.
 
     Returns:
@@ -79,24 +79,37 @@
         columnNames = list(data.keys())
     else:
         if len(columnNames) != len(data.keys()):
             raise ValueError(
                 "Number of columns mismatch between `columnNames` and `data`"
             )
 
-        # Technically should throw an error but
-        # lets just fix it
-        # colnames and dict order should be the same
-        new_odata = OrderedDict()
-        for k in columnNames:
-            new_odata[k] = data[k]
+    # Technically should throw an error but
+    # lets just fix it
+    # colnames and dict order should be the same
+    incorrect_types = []
+    new_odata = OrderedDict()
+    for k in columnNames:
+        # check for types
+        col_value = data[k]
+
+        if not (hasattr(col_value, "__len__") and hasattr(col_value, "__getitem__")):
+            incorrect_types.append(k)
+
+        new_odata[k] = data[k]
+
+    if len(incorrect_types) > 0:
+        raise TypeError(
+            "All columns in data must support `len` and "
+            f"`slice` operations. Columns: {incorrect_types} do not."
+        )
 
-        data = new_odata
+    data = new_odata
 
-    return columnNames
+    return columnNames, data
 
 
 def validate_unique_list(values: Sequence) -> bool:
     """Validate if a list has unique values.
 
     Args:
         values (Sequence): list of values to check.
```

### Comparing `BiocFrame-0.2.8/src/biocframe/utils.py` & `BiocFrame-0.2.9/src/biocframe/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-from typing import Any, List, Union, Sequence
+from typing import Any, Union, Sequence
 
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 def match_to_indices(
-    data: Sequence[Any], indices: Union[List[int], slice, List[str]]
+    data: Sequence[Any], indices: Union[Sequence[int], slice, Sequence[str]]
 ) -> Union[slice, Sequence[Any]]:
     """slice an array
 
     Args:
         data (Sequence[Any]): input data array to slice
-        indices (Union[List[int], slice, List[str]): either a slice or a list of indices to keep
+        indices (Union[Sequence[int], slice, Sequence[str]): either a slice or 
+            a list of indices to keep
 
     Returns:
         Union[slice, Sequence[Any]]: either a slice or list of indices
     """
 
     if isinstance(indices, slice):
         return indices
-    elif isinstance(indices, list):
+    elif isinstance(indices, Sequence):
         all_strs = all([isinstance(k, str) for k in indices])
         # slice by value
         if all_strs:
             diff = list(set(indices).difference(set(data)))
             if len(diff) > 0:
                 raise ValueError(
                     f"Cannot slice by value since {diff} do not exist in {data}"
                 )
 
             return [i for i in range(len(indices)) if indices[i] in data]
         else:
             return indices
 
-    raise TypeError(f"`indices` is neither a `list` nor a `slice`")
+    raise TypeError("`indices` is neither a `list` nor a `slice`")
```

### Comparing `BiocFrame-0.2.8/tests/test_initialize.py` & `BiocFrame-0.2.9/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/tests/test_methods.py` & `BiocFrame-0.2.9/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/tests/test_readme.py` & `BiocFrame-0.2.9/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.2.8/tox.ini` & `BiocFrame-0.2.9/tox.ini`

 * *Files identical despite different names*

