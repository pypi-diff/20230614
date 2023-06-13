# Comparing `tmp/msgram_core-1.2.0.tar.gz` & `tmp/msgram_core-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram_core-1.2.0.tar", last modified: Thu May 25 21:51:15 2023, max compression
+gzip compressed data, was "msgram_core-1.2.1.tar", last modified: Tue Jun 13 23:39:57 2023, max compression
```

## Comparing `msgram_core-1.2.0.tar` & `msgram_core-1.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.771896 msgram_core-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-05-25 21:50:59.000000 msgram_core-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-05-25 21:51:15.771896 msgram_core-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-25 21:50:59.000000 msgram_core-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-25 21:50:59.000000 msgram_core-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:51:15.771896 msgram_core-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.767895 msgram_core-1.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.767895 msgram_core-1.2.0/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/agregation.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/interpretation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/measures_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/weighting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.767895 msgram_core-1.2.0/src/msgram_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-05-25 21:51:15.000000 msgram_core-1.2.0/src/msgram_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 21:51:15.000000 msgram_core-1.2.0/src/msgram_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:51:15.000000 msgram_core-1.2.0/src/msgram_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 21:51:15.000000 msgram_core-1.2.0/src/msgram_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 21:51:15.000000 msgram_core-1.2.0/src/msgram_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.771896 msgram_core-1.2.0/src/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/parsers/sonarqube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.771896 msgram_core-1.2.0/src/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/resources/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.771896 msgram_core-1.2.0/src/staticfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/staticfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/staticfiles/default_pre_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/staticfiles/sonarqube_available_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/staticfiles/sonarqube_supported_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.771896 msgram_core-1.2.0/src/util/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/util/check_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/util/get_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.771896 msgram_core-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-25 21:50:59.000000 msgram_core-1.2.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.525076 msgram_core-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-06-13 23:39:33.000000 msgram_core-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-06-13 23:39:57.525076 msgram_core-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-13 23:39:33.000000 msgram_core-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-13 23:39:33.000000 msgram_core-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:39:57.525076 msgram_core-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.517076 msgram_core-1.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.521076 msgram_core-1.2.1/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/agregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/interpretation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/measures_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/weighting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.521076 msgram_core-1.2.1/src/msgram_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-06-13 23:39:57.000000 msgram_core-1.2.1/src/msgram_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-13 23:39:57.000000 msgram_core-1.2.1/src/msgram_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:39:57.000000 msgram_core-1.2.1/src/msgram_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 23:39:57.000000 msgram_core-1.2.1/src/msgram_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 23:39:57.000000 msgram_core-1.2.1/src/msgram_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.521076 msgram_core-1.2.1/src/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/parsers/sonarqube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.521076 msgram_core-1.2.1/src/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/resources/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.521076 msgram_core-1.2.1/src/staticfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/staticfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/staticfiles/default_pre_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/staticfiles/sonarqube_available_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/staticfiles/sonarqube_supported_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.525076 msgram_core-1.2.1/src/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/util/check_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/util/get_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.525076 msgram_core-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-13 23:39:33.000000 msgram_core-1.2.1/tests/test_helpers.py
```

### Comparing `msgram_core-1.2.0/LICENSE` & `msgram_core-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/PKG-INFO` & `msgram_core-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram_core
-Version: 1.2.0
+Version: 1.2.1
 Summary: The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram_core-1.2.0/README.md` & `msgram_core-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/pyproject.toml` & `msgram_core-1.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram_core"
-version = "1.2.0"
+version = "1.2.1"
 description = "The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis."
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `msgram_core-1.2.0/src/core/dataframe.py` & `msgram_core-1.2.1/src/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/src/core/interpretation_functions.py` & `msgram_core-1.2.1/src/core/interpretation_functions.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/src/core/measures_functions.py` & `msgram_core-1.2.1/src/core/measures_functions.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/src/core/schemas.py` & `msgram_core-1.2.1/src/core/schemas.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/src/msgram_core.egg-info/PKG-INFO` & `msgram_core-1.2.1/src/msgram_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-core
-Version: 1.2.0
+Version: 1.2.1
 Summary: The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram_core-1.2.0/src/msgram_core.egg-info/SOURCES.txt` & `msgram_core-1.2.1/src/msgram_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/src/parsers/sonarqube.py` & `msgram_core-1.2.1/src/parsers/sonarqube.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/src/staticfiles/sonarqube_available_metrics.py` & `msgram_core-1.2.1/src/staticfiles/sonarqube_available_metrics.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/src/staticfiles/sonarqube_supported_metrics.py` & `msgram_core-1.2.1/src/staticfiles/sonarqube_supported_metrics.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/src/util/check_functions.py` & `msgram_core-1.2.1/src/util/check_functions.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/src/util/constants.py` & `msgram_core-1.2.1/src/util/constants.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/src/util/exceptions.py` & `msgram_core-1.2.1/src/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/src/util/get_functions.py` & `msgram_core-1.2.1/src/util/get_functions.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.0/tests/test_helpers.py` & `msgram_core-1.2.1/tests/test_helpers.py`

 * *Files identical despite different names*

