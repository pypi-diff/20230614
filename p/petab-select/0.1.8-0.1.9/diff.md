# Comparing `tmp/petab_select-0.1.8.tar.gz` & `tmp/petab_select-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petab_select-0.1.8.tar", last modified: Wed May 31 15:56:37 2023, max compression
+gzip compressed data, was "petab_select-0.1.9.tar", last modified: Tue Jun 13 09:37:24 2023, max compression
```

## Comparing `petab_select-0.1.8.tar` & `petab_select-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-31 15:56:37.946644 petab_select-0.1.8/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     1602 2021-08-31 13:20:42.000000 petab_select-0.1.8/LICENSE
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-05-31 15:56:37.946644 petab_select-0.1.8/PKG-INFO
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9256 2023-04-13 16:12:57.000000 petab_select-0.1.8/README.md
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-31 15:56:37.946644 petab_select-0.1.8/petab_select/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      263 2023-04-13 08:28:52.000000 petab_select-0.1.8/petab_select/__init__.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    52003 2023-05-31 15:52:41.000000 petab_select-0.1.8/petab_select/candidate_space.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    13247 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/cli.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     4460 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/constants.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     7225 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/criteria.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2443 2021-11-02 20:14:39.000000 petab_select-0.1.8/petab_select/descriptors.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     1076 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/handlers.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2438 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/misc.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    25976 2023-05-09 10:52:56.000000 petab_select-0.1.8/petab_select/model.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    11415 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/model_space.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    38364 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/model_subspace.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2254 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/petab.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     8571 2023-04-13 08:28:52.000000 petab_select-0.1.8/petab_select/problem.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    10226 2023-05-31 15:52:41.000000 petab_select-0.1.8/petab_select/ui.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      295 2021-11-03 18:08:02.000000 petab_select-0.1.8/petab_select/validators.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       80 2023-05-31 15:52:51.000000 petab_select-0.1.8/petab_select/version.py
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-31 15:56:37.946644 petab_select-0.1.8/petab_select.egg-info/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-05-31 15:56:37.000000 petab_select-0.1.8/petab_select.egg-info/PKG-INFO
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      658 2023-05-31 15:56:37.000000 petab_select-0.1.8/petab_select.egg-info/SOURCES.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)        1 2023-05-31 15:56:37.000000 petab_select-0.1.8/petab_select.egg-info/dependency_links.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       54 2023-05-31 15:56:37.000000 petab_select-0.1.8/petab_select.egg-info/entry_points.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      136 2023-05-31 15:56:37.000000 petab_select-0.1.8/petab_select.egg-info/requires.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       13 2023-05-31 15:56:37.000000 petab_select-0.1.8/petab_select.egg-info/top_level.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      281 2022-09-30 16:40:04.000000 petab_select-0.1.8/pyproject.toml
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       38 2023-05-31 15:56:37.946644 petab_select-0.1.8/setup.cfg
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2961 2023-04-13 16:12:57.000000 petab_select-0.1.8/setup.py
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-06-13 09:37:24.041004 petab_select-0.1.9/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     1602 2021-08-31 13:20:42.000000 petab_select-0.1.9/LICENSE
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-06-13 09:37:24.037004 petab_select-0.1.9/PKG-INFO
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9256 2023-04-13 16:12:57.000000 petab_select-0.1.9/README.md
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-06-13 09:37:24.037004 petab_select-0.1.9/petab_select/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      263 2023-04-13 08:28:52.000000 petab_select-0.1.9/petab_select/__init__.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    52003 2023-05-31 15:52:41.000000 petab_select-0.1.9/petab_select/candidate_space.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    13247 2022-09-30 16:40:04.000000 petab_select-0.1.9/petab_select/cli.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     4460 2022-09-30 16:40:04.000000 petab_select-0.1.9/petab_select/constants.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     7225 2022-09-30 16:40:04.000000 petab_select-0.1.9/petab_select/criteria.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2443 2021-11-02 20:14:39.000000 petab_select-0.1.9/petab_select/descriptors.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     1076 2022-09-30 16:40:04.000000 petab_select-0.1.9/petab_select/handlers.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2438 2022-09-30 16:40:04.000000 petab_select-0.1.9/petab_select/misc.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    25976 2023-05-09 10:52:56.000000 petab_select-0.1.9/petab_select/model.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    11415 2022-09-30 16:40:04.000000 petab_select-0.1.9/petab_select/model_space.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    38364 2022-09-30 16:40:04.000000 petab_select-0.1.9/petab_select/model_subspace.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2254 2022-09-30 16:40:04.000000 petab_select-0.1.9/petab_select/petab.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     8571 2023-04-13 08:28:52.000000 petab_select-0.1.9/petab_select/problem.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    10226 2023-05-31 15:52:41.000000 petab_select-0.1.9/petab_select/ui.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      295 2021-11-03 18:08:02.000000 petab_select-0.1.9/petab_select/validators.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       80 2023-06-13 09:37:02.000000 petab_select-0.1.9/petab_select/version.py
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-06-13 09:37:24.037004 petab_select-0.1.9/petab_select.egg-info/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-06-13 09:37:24.000000 petab_select-0.1.9/petab_select.egg-info/PKG-INFO
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      658 2023-06-13 09:37:24.000000 petab_select-0.1.9/petab_select.egg-info/SOURCES.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)        1 2023-06-13 09:37:24.000000 petab_select-0.1.9/petab_select.egg-info/dependency_links.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       54 2023-06-13 09:37:24.000000 petab_select-0.1.9/petab_select.egg-info/entry_points.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      136 2023-06-13 09:37:24.000000 petab_select-0.1.9/petab_select.egg-info/requires.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       13 2023-06-13 09:37:24.000000 petab_select-0.1.9/petab_select.egg-info/top_level.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      281 2022-09-30 16:40:04.000000 petab_select-0.1.9/pyproject.toml
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       38 2023-06-13 09:37:24.041004 petab_select-0.1.9/setup.cfg
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2961 2023-04-13 16:12:57.000000 petab_select-0.1.9/setup.py
```

### Comparing `petab_select-0.1.8/LICENSE` & `petab_select-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/PKG-INFO` & `petab_select-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab_select
-Version: 0.1.8
+Version: 0.1.9
 Summary: PEtab Select: an extension to PEtab for model selection.
 Home-page: https://github.com/PEtab-dev/petab_select
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `petab_select-0.1.8/README.md` & `petab_select-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select/candidate_space.py` & `petab_select-0.1.9/petab_select/candidate_space.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select/cli.py` & `petab_select-0.1.9/petab_select/cli.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select/constants.py` & `petab_select-0.1.9/petab_select/constants.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select/criteria.py` & `petab_select-0.1.9/petab_select/criteria.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select/descriptors.py` & `petab_select-0.1.9/petab_select/descriptors.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select/handlers.py` & `petab_select-0.1.9/petab_select/handlers.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select/misc.py` & `petab_select-0.1.9/petab_select/misc.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select/model.py` & `petab_select-0.1.9/petab_select/model.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select/model_space.py` & `petab_select-0.1.9/petab_select/model_space.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select/model_subspace.py` & `petab_select-0.1.9/petab_select/model_subspace.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select/petab.py` & `petab_select-0.1.9/petab_select/petab.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select/problem.py` & `petab_select-0.1.9/petab_select/problem.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select/ui.py` & `petab_select-0.1.9/petab_select/ui.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/petab_select.egg-info/PKG-INFO` & `petab_select-0.1.9/petab_select.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab-select
-Version: 0.1.8
+Version: 0.1.9
 Summary: PEtab Select: an extension to PEtab for model selection.
 Home-page: https://github.com/PEtab-dev/petab_select
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `petab_select-0.1.8/petab_select.egg-info/SOURCES.txt` & `petab_select-0.1.9/petab_select.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.8/setup.py` & `petab_select-0.1.9/setup.py`

 * *Files identical despite different names*

