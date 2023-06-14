# Comparing `tmp/tpaw-0.0.1a2.tar.gz` & `tmp/tpaw-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpaw-0.0.1a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tpaw-0.0.1a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tpaw-0.0.1a2.tar` & `tpaw-0.0.1a3.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     3078 2023-06-14 03:45:27.697084 tpaw-0.0.1a2/.gitignore
--rw-r--r--   0        0        0     1296 2023-06-14 01:52:01.890982 tpaw-0.0.1a2/LICENSE
--rw-r--r--   0        0        0      351 2023-06-14 01:51:34.980692 tpaw-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-14 03:27:30.402948 tpaw-0.0.1a2/tests/__init__.py
--rw-r--r--   0        0        0    17029 2023-06-14 04:07:11.683947 tpaw-0.0.1a2/tests/data/groups.html
--rw-r--r--   0        0        0    35218 2023-06-14 06:34:57.679137 tpaw-0.0.1a2/tests/data/slash_new.html
--rw-r--r--   0        0        0     1766 2023-06-14 06:50:37.218088 tpaw-0.0.1a2/tests/test_tpaw.py
--rw-r--r--   0        0        0     6369 2023-06-14 07:10:58.211346 tpaw-0.0.1a2/tpaw.py
--rw-r--r--   0        0        0      230 1970-01-01 00:00:00.000000 tpaw-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0      149 2023-06-14 07:58:32.698840 tpaw-0.0.1a3/.flake8
+-rw-r--r--   0        0        0      993 2023-06-14 08:04:29.469030 tpaw-0.0.1a3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     3078 2023-06-14 03:45:27.697084 tpaw-0.0.1a3/.gitignore
+-rw-r--r--   0        0        0     1296 2023-06-14 01:52:01.890982 tpaw-0.0.1a3/LICENSE
+-rw-r--r--   0        0        0      524 2023-06-14 08:15:37.593983 tpaw-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 03:27:30.402948 tpaw-0.0.1a3/tests/__init__.py
+-rw-r--r--   0        0        0    17029 2023-06-14 04:07:11.683947 tpaw-0.0.1a3/tests/data/groups.html
+-rw-r--r--   0        0        0    35218 2023-06-14 06:34:57.679137 tpaw-0.0.1a3/tests/data/slash_new.html
+-rw-r--r--   0        0        0     1767 2023-06-14 07:41:59.421902 tpaw-0.0.1a3/tests/test_tpaw.py
+-rw-r--r--   0        0        0     6358 2023-06-14 08:16:01.054736 tpaw-0.0.1a3/tpaw.py
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 tpaw-0.0.1a3/PKG-INFO
```

### Comparing `tpaw-0.0.1a2/.gitignore` & `tpaw-0.0.1a3/.gitignore`

 * *Files identical despite different names*

### Comparing `tpaw-0.0.1a2/LICENSE` & `tpaw-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `tpaw-0.0.1a2/tests/data/groups.html` & `tpaw-0.0.1a3/tests/data/groups.html`

 * *Files identical despite different names*

### Comparing `tpaw-0.0.1a2/tests/data/slash_new.html` & `tpaw-0.0.1a3/tests/data/slash_new.html`

 * *Files identical despite different names*

### Comparing `tpaw-0.0.1a2/tests/test_tpaw.py` & `tpaw-0.0.1a3/tests/test_tpaw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from unittest.mock import Mock
 
 import pytest
-import tpaw
 from lxml.html import fragment_fromstring
 
+import tpaw
+
 
 def test_one_class():
     with pytest.raises(tpaw.TPAWError) as exception_info:
         tpaw.one_class(fragment_fromstring("<a>"), "notfound")
     assert len(exception_info.value.collection) == 0
 
     with pytest.raises(tpaw.TPAWError) as exception_info:
```

### Comparing `tpaw-0.0.1a2/tpaw.py` & `tpaw-0.0.1a3/tpaw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Tildes Python API Wrapper."""
 
-import sys
 from datetime import datetime, timedelta
 
-import requests
 import lxml.html
+import requests
 
-__version__ = "0.0.1a2"
+__version__ = "0.0.1a3"
 
 
 def one_class(element, class_selector, /):
     collection = element.find_class(class_selector)
     if len(collection) != 1:
         raise TPAWError(
             "Expected to find exactly 1 element", collection=collection, element=element
```

