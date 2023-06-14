# Comparing `tmp/pytest-jira-xfail-1.0.0.tar.gz` & `tmp/pytest-jira-xfail-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-jira-xfail-1.0.0.tar", last modified: Mon Nov  7 11:46:12 2022, max compression
+gzip compressed data, was "pytest-jira-xfail-1.0.1.tar", last modified: Thu Dec  1 18:28:47 2022, max compression
```

## Comparing `pytest-jira-xfail-1.0.0.tar` & `pytest-jira-xfail-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:46:12.227522 pytest-jira-xfail-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-11-07 11:46:01.000000 pytest-jira-xfail-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-11-07 11:46:12.227522 pytest-jira-xfail-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-11-07 11:46:01.000000 pytest-jira-xfail-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:46:12.227522 pytest-jira-xfail-1.0.0/pytest_jira_xfail/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:46:01.000000 pytest-jira-xfail-1.0.0/pytest_jira_xfail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-11-07 11:46:01.000000 pytest-jira-xfail-1.0.0/pytest_jira_xfail/annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3935 2022-11-07 11:46:01.000000 pytest-jira-xfail-1.0.0/pytest_jira_xfail/jira_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:46:12.227522 pytest-jira-xfail-1.0.0/pytest_jira_xfail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-11-07 11:46:12.000000 pytest-jira-xfail-1.0.0/pytest_jira_xfail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-11-07 11:46:12.000000 pytest-jira-xfail-1.0.0/pytest_jira_xfail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 11:46:12.000000 pytest-jira-xfail-1.0.0/pytest_jira_xfail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-07 11:46:12.000000 pytest-jira-xfail-1.0.0/pytest_jira_xfail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-07 11:46:12.000000 pytest-jira-xfail-1.0.0/pytest_jira_xfail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 11:46:12.227522 pytest-jira-xfail-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-11-07 11:46:01.000000 pytest-jira-xfail-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 18:28:47.789439 pytest-jira-xfail-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2022-12-01 18:28:36.000000 pytest-jira-xfail-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2022-12-01 18:28:47.789439 pytest-jira-xfail-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2022-12-01 18:28:36.000000 pytest-jira-xfail-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 18:28:47.789439 pytest-jira-xfail-1.0.1/pytest_jira_xfail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 18:28:36.000000 pytest-jira-xfail-1.0.1/pytest_jira_xfail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-01 18:28:36.000000 pytest-jira-xfail-1.0.1/pytest_jira_xfail/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2022-12-01 18:28:36.000000 pytest-jira-xfail-1.0.1/pytest_jira_xfail/jira_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 18:28:47.789439 pytest-jira-xfail-1.0.1/pytest_jira_xfail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2022-12-01 18:28:47.000000 pytest-jira-xfail-1.0.1/pytest_jira_xfail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2022-12-01 18:28:47.000000 pytest-jira-xfail-1.0.1/pytest_jira_xfail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-01 18:28:47.000000 pytest-jira-xfail-1.0.1/pytest_jira_xfail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-01 18:28:47.000000 pytest-jira-xfail-1.0.1/pytest_jira_xfail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-01 18:28:47.000000 pytest-jira-xfail-1.0.1/pytest_jira_xfail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-01 18:28:47.789439 pytest-jira-xfail-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2022-12-01 18:28:36.000000 pytest-jira-xfail-1.0.1/setup.py
```

### Comparing `pytest-jira-xfail-1.0.0/LICENSE` & `pytest-jira-xfail-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-jira-xfail-1.0.0/PKG-INFO` & `pytest-jira-xfail-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-jira-xfail
-Version: 1.0.0
+Version: 1.0.1
 Summary: Plugin skips (xfail) tests if unresolved Jira issue(s) linked
 Home-page: https://github.com/JamalZeynalov/pytest-jira-xfail
 Author: Jamal Zeinalov
 Author-email: jamal.zeynalov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytest-jira-xfail-1.0.0/README.md` & `pytest-jira-xfail-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest-jira-xfail-1.0.0/pytest_jira_xfail/annotations.py` & `pytest-jira-xfail-1.0.1/pytest_jira_xfail/annotations.py`

 * *Files identical despite different names*

### Comparing `pytest-jira-xfail-1.0.0/pytest_jira_xfail/jira_helper.py` & `pytest-jira-xfail-1.0.1/pytest_jira_xfail/jira_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import pytest
 from _pytest.mark import Mark
 from jira import JIRA
 from singleton_decorator import singleton
+from selenium.common.exceptions import *
+from requests import *
 
 
 @singleton
 class PytestJiraHelper:
     def __init__(
         self,
         jira_url: str,
```

### Comparing `pytest-jira-xfail-1.0.0/pytest_jira_xfail.egg-info/PKG-INFO` & `pytest-jira-xfail-1.0.1/pytest_jira_xfail.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-jira-xfail
-Version: 1.0.0
+Version: 1.0.1
 Summary: Plugin skips (xfail) tests if unresolved Jira issue(s) linked
 Home-page: https://github.com/JamalZeynalov/pytest-jira-xfail
 Author: Jamal Zeinalov
 Author-email: jamal.zeynalov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytest-jira-xfail-1.0.0/setup.py` & `pytest-jira-xfail-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pytest-jira-xfail",
-    version="1.0.0",
+    version="1.0.1",
     author="Jamal Zeinalov",
     author_email="jamal.zeynalov@gmail.com",
     description='Plugin skips (xfail) tests if unresolved Jira issue(s) linked',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JamalZeynalov/pytest-jira-xfail",
     packages=find_packages(),
@@ -21,10 +21,11 @@
     install_requires=[
         "pytest~=7.2.0",
         "requests~=2.28.1",
         "setuptools~=65.5.1",
         "jira~=3.4.1",
         "singleton-decorator~=1.0.0",
         "allure-pytest~=2.11.1",
+        "selenium>=4.6.0",
     ],
     python_requires=">=3.9",
 )
```

