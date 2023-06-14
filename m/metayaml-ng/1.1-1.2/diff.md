# Comparing `tmp/metayaml-ng-1.1.tar.gz` & `tmp/metayaml-ng-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metayaml-ng-1.1.tar", last modified: Thu Jun  1 14:41:52 2023, max compression
+gzip compressed data, was "metayaml-ng-1.2.tar", last modified: Wed Jun 14 19:18:13 2023, max compression
```

## Comparing `metayaml-ng-1.1.tar` & `metayaml-ng-1.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.185858 metayaml-ng-1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.173858 metayaml-ng-1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.177857 metayaml-ng-1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-01 14:41:42.000000 metayaml-ng-1.1/.github/workflows/ci-cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-01 14:41:42.000000 metayaml-ng-1.1/.github/workflows/sync.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-06-01 14:41:42.000000 metayaml-ng-1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-01 14:41:52.185858 metayaml-ng-1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7910 2023-06-01 14:41:42.000000 metayaml-ng-1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.177857 metayaml-ng-1.1/metayaml/
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-01 14:41:42.000000 metayaml-ng-1.1/metayaml/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-06-01 14:41:42.000000 metayaml-ng-1.1/metayaml/exception.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2402 2023-06-01 14:41:42.000000 metayaml-ng-1.1/metayaml/jinja_eval.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12482 2023-06-01 14:41:42.000000 metayaml-ng-1.1/metayaml/metayaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.181858 metayaml-ng-1.1/metayaml_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-01 14:41:52.000000 metayaml-ng-1.1/metayaml_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-01 14:41:52.000000 metayaml-ng-1.1/metayaml_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:41:52.000000 metayaml-ng-1.1/metayaml_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-01 14:41:52.000000 metayaml-ng-1.1/metayaml_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 14:41:52.000000 metayaml-ng-1.1/metayaml_ng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 14:41:42.000000 metayaml-ng-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 14:41:42.000000 metayaml-ng-1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-01 14:41:52.185858 metayaml-ng-1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.181858 metayaml-ng-1.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5031 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.185858 metayaml-ng-1.1/tests/test_files/
--rwxr-xr-x   0 runner    (1001) docker     (123)      390 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/cp.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      228 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/dict_update.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/f1.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/f2.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/f3.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/foo_data.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/inherit.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/inherit_deepcp.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       98 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/inherit_subst.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      133 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/list_eval.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/test.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/test_multi.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/test_order.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/undef.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/undef2.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:18:13.892625 metayaml-ng-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:18:13.884625 metayaml-ng-1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:18:13.884625 metayaml-ng-1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-14 19:17:57.000000 metayaml-ng-1.2/.github/workflows/ci-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-14 19:17:57.000000 metayaml-ng-1.2/.github/workflows/sync.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-06-14 19:17:57.000000 metayaml-ng-1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-14 19:17:57.000000 metayaml-ng-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-06-14 19:18:13.892625 metayaml-ng-1.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7910 2023-06-14 19:17:57.000000 metayaml-ng-1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:18:13.884625 metayaml-ng-1.2/metayaml/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-14 19:17:57.000000 metayaml-ng-1.2/metayaml/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-06-14 19:17:57.000000 metayaml-ng-1.2/metayaml/exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2402 2023-06-14 19:17:57.000000 metayaml-ng-1.2/metayaml/jinja_eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12482 2023-06-14 19:17:57.000000 metayaml-ng-1.2/metayaml/metayaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:18:13.888625 metayaml-ng-1.2/metayaml_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-06-14 19:18:13.000000 metayaml-ng-1.2/metayaml_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-14 19:18:13.000000 metayaml-ng-1.2/metayaml_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:18:13.000000 metayaml-ng-1.2/metayaml_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-14 19:18:13.000000 metayaml-ng-1.2/metayaml_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 19:18:13.000000 metayaml-ng-1.2/metayaml_ng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-14 19:17:57.000000 metayaml-ng-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 19:17:57.000000 metayaml-ng-1.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-14 19:18:13.892625 metayaml-ng-1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:18:13.888625 metayaml-ng-1.2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5031 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:18:13.892625 metayaml-ng-1.2/tests/test_files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      390 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/cp.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      228 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/dict_update.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/f1.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/f2.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/f3.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/foo_data.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/inherit.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/inherit_deepcp.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       98 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/inherit_subst.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      133 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/list_eval.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/test.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/test_multi.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/test_order.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/undef.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tests/test_files/undef2.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-06-14 19:17:57.000000 metayaml-ng-1.2/tox.ini
```

### Comparing `metayaml-ng-1.1/.github/workflows/ci-cd.yml` & `metayaml-ng-1.2/.github/workflows/ci-cd.yml`

 * *Files identical despite different names*

### Comparing `metayaml-ng-1.1/.github/workflows/sync.yml` & `metayaml-ng-1.2/.github/workflows/sync.yml`

 * *Files identical despite different names*

### Comparing `metayaml-ng-1.1/PKG-INFO` & `metayaml-ng-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: metayaml-ng
-Version: 1.1
+Version: 1.2
 Summary: Enhancements of yaml format to support include and python expression
 Download-URL: https://pypi.org/project/metayaml-ng/
 Author: Anton Tagunov
 Maintainer: William Barnhart
 Maintainer-email: williambbarnhart@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Other Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
 
 =========
 Meta Yaml
 =========
 
 Note: This is a fork of the project at https://bitbucket.org/atagunov/metayaml.
```

### Comparing `metayaml-ng-1.1/README.rst` & `metayaml-ng-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `metayaml-ng-1.1/metayaml/exception.py` & `metayaml-ng-1.2/metayaml/exception.py`

 * *Files identical despite different names*

### Comparing `metayaml-ng-1.1/metayaml/jinja_eval.py` & `metayaml-ng-1.2/metayaml/jinja_eval.py`

 * *Files identical despite different names*

### Comparing `metayaml-ng-1.1/metayaml/metayaml.py` & `metayaml-ng-1.2/metayaml/metayaml.py`

 * *Files identical despite different names*

### Comparing `metayaml-ng-1.1/metayaml_ng.egg-info/PKG-INFO` & `metayaml-ng-1.2/metayaml_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: metayaml-ng
-Version: 1.1
+Version: 1.2
 Summary: Enhancements of yaml format to support include and python expression
 Download-URL: https://pypi.org/project/metayaml-ng/
 Author: Anton Tagunov
 Maintainer: William Barnhart
 Maintainer-email: williambbarnhart@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Other Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
 
 =========
 Meta Yaml
 =========
 
 Note: This is a fork of the project at https://bitbucket.org/atagunov/metayaml.
```

### Comparing `metayaml-ng-1.1/metayaml_ng.egg-info/SOURCES.txt` & `metayaml-ng-1.2/metayaml_ng.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+LICENSE
 README.rst
 pyproject.toml
 requirements-dev.txt
 setup.cfg
 tox.ini
 .github/workflows/ci-cd.yml
 .github/workflows/sync.yml
```

### Comparing `metayaml-ng-1.1/setup.cfg` & `metayaml-ng-1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `metayaml-ng-1.1/tests/test.py` & `metayaml-ng-1.2/tests/test.py`

 * *Files identical despite different names*

