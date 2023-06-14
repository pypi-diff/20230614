# Comparing `tmp/abd_clam-0.9.0.dev1.tar.gz` & `tmp/abd_clam-0.9.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abd_clam-0.9.0.dev1.tar", max compression
+gzip compressed data, was "abd_clam-0.9.0.dev5.tar", max compression
```

## Comparing `abd_clam-0.9.0.dev1.tar` & `abd_clam-0.9.0.dev5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1064 2023-06-14 02:22:05.045870 abd_clam-0.9.0.dev1/LICENSE
--rw-r--r--   0        0        0     2482 2023-06-14 02:22:05.045870 abd_clam-0.9.0.dev1/README.md
--rw-r--r--   0        0        0      776 2023-06-14 02:22:05.045870 abd_clam-0.9.0.dev1/pyproject.toml
--rw-r--r--   0        0        0      141 2023-06-14 02:22:05.045870 abd_clam-0.9.0.dev1/python/abd_clam/__init__.py
--rw-r--r--   0        0        0      295 2023-06-14 02:22:05.045870 abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/__init__.py
--rw-r--r--   0        0        0     1738 2023-06-14 02:22:05.045870 abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/anomaly_dataset.py
--rw-r--r--   0        0        0     2307 2023-06-14 02:22:05.045870 abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/anomaly_space.py
--rw-r--r--   0        0        0    11437 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/chaoda.py
--rw-r--r--   0        0        0     9281 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/graph_scorers.py
--rw-r--r--   0        0        0     4931 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/meta_ml.py
--rw-r--r--   0        0        0    14627 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/pretrained_models.py
--rw-r--r--   0        0        0    10205 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/training.py
--rw-r--r--   0        0        0       35 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/classification/__init__.py
--rw-r--r--   0        0        0     3247 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/classification/classifier.py
--rw-r--r--   0        0        0      414 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/core/__init__.py
--rw-r--r--   0        0        0    23491 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/core/cluster.py
--rw-r--r--   0        0        0     1463 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/core/cluster_criteria.py
--rw-r--r--   0        0        0     5983 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/core/dataset.py
--rw-r--r--   0        0        0    13554 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/core/graph.py
--rw-r--r--   0        0        0     7323 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/core/graph_criteria.py
--rw-r--r--   0        0        0     3678 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/core/metric.py
--rw-r--r--   0        0        0     7834 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/core/space.py
--rw-r--r--   0        0        0       25 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/search/__init__.py
--rw-r--r--   0        0        0     8645 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/search/cakes.py
--rw-r--r--   0        0        0      105 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/utils/__init__.py
--rw-r--r--   0        0        0     1358 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/utils/constants.py
--rw-r--r--   0        0        0     1533 2023-06-14 02:22:05.049870 abd_clam-0.9.0.dev1/python/abd_clam/utils/helpers.py
--rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 abd_clam-0.9.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-14 02:40:32.998701 abd_clam-0.9.0.dev5/LICENSE
+-rw-r--r--   0        0        0     2482 2023-06-14 02:40:32.998701 abd_clam-0.9.0.dev5/README.md
+-rw-r--r--   0        0        0      776 2023-06-14 02:40:33.002702 abd_clam-0.9.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0      169 2023-06-14 02:40:33.002702 abd_clam-0.9.0.dev5/python/abd_clam/__init__.py
+-rw-r--r--   0        0        0      295 2023-06-14 02:40:33.002702 abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/__init__.py
+-rw-r--r--   0        0        0     1738 2023-06-14 02:40:33.002702 abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/anomaly_dataset.py
+-rw-r--r--   0        0        0     2307 2023-06-14 02:40:33.002702 abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/anomaly_space.py
+-rw-r--r--   0        0        0    11437 2023-06-14 02:40:33.002702 abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/chaoda.py
+-rw-r--r--   0        0        0     9281 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/graph_scorers.py
+-rw-r--r--   0        0        0     4931 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/meta_ml.py
+-rw-r--r--   0        0        0    14627 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/pretrained_models.py
+-rw-r--r--   0        0        0    10205 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/training.py
+-rw-r--r--   0        0        0       35 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/classification/__init__.py
+-rw-r--r--   0        0        0     3247 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/classification/classifier.py
+-rw-r--r--   0        0        0      414 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/core/__init__.py
+-rw-r--r--   0        0        0    23491 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/core/cluster.py
+-rw-r--r--   0        0        0     1463 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/core/cluster_criteria.py
+-rw-r--r--   0        0        0     5983 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/core/dataset.py
+-rw-r--r--   0        0        0    13554 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/core/graph.py
+-rw-r--r--   0        0        0     7323 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/core/graph_criteria.py
+-rw-r--r--   0        0        0     3678 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/core/metric.py
+-rw-r--r--   0        0        0     7834 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/core/space.py
+-rw-r--r--   0        0        0       25 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/search/__init__.py
+-rw-r--r--   0        0        0     8645 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/search/cakes.py
+-rw-r--r--   0        0        0      105 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/utils/__init__.py
+-rw-r--r--   0        0        0     1358 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/utils/constants.py
+-rw-r--r--   0        0        0     1533 2023-06-14 02:40:33.006702 abd_clam-0.9.0.dev5/python/abd_clam/utils/helpers.py
+-rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 abd_clam-0.9.0.dev5/PKG-INFO
```

### Comparing `abd_clam-0.9.0.dev1/LICENSE` & `abd_clam-0.9.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/README.md` & `abd_clam-0.9.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/pyproject.toml` & `abd_clam-0.9.0.dev5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abd-clam"
-version = "0.9.0-dev1"
+version = "0.9.0-dev5"
 description = "Clustered Learning of Approximate Manifolds"
 authors = [
     "Najib Ishaq <najib_ishaq@zoho.com>",
     "Tom Howard <info@tomhoward.codes>",
     "Noah Daniels <noah_daniels@uri.edu>",
     "Morgan Prior <morgan_prior@uri.edu>",
     "Isaac Chen <ijchen@uri.edu>",
```

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/anomaly_dataset.py` & `abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/anomaly_dataset.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/anomaly_space.py` & `abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/anomaly_space.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/chaoda.py` & `abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/chaoda.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/graph_scorers.py` & `abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/graph_scorers.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/meta_ml.py` & `abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/meta_ml.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/pretrained_models.py` & `abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/pretrained_models.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/anomaly_detection/training.py` & `abd_clam-0.9.0.dev5/python/abd_clam/anomaly_detection/training.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/classification/classifier.py` & `abd_clam-0.9.0.dev5/python/abd_clam/classification/classifier.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/core/cluster.py` & `abd_clam-0.9.0.dev5/python/abd_clam/core/cluster.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/core/cluster_criteria.py` & `abd_clam-0.9.0.dev5/python/abd_clam/core/cluster_criteria.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/core/dataset.py` & `abd_clam-0.9.0.dev5/python/abd_clam/core/dataset.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/core/graph.py` & `abd_clam-0.9.0.dev5/python/abd_clam/core/graph.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/core/graph_criteria.py` & `abd_clam-0.9.0.dev5/python/abd_clam/core/graph_criteria.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/core/metric.py` & `abd_clam-0.9.0.dev5/python/abd_clam/core/metric.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/core/space.py` & `abd_clam-0.9.0.dev5/python/abd_clam/core/space.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/search/cakes.py` & `abd_clam-0.9.0.dev5/python/abd_clam/search/cakes.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/utils/constants.py` & `abd_clam-0.9.0.dev5/python/abd_clam/utils/constants.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/python/abd_clam/utils/helpers.py` & `abd_clam-0.9.0.dev5/python/abd_clam/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `abd_clam-0.9.0.dev1/PKG-INFO` & `abd_clam-0.9.0.dev5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abd-clam
-Version: 0.9.0.dev1
+Version: 0.9.0.dev5
 Summary: Clustered Learning of Approximate Manifolds
 License: MIT
 Author: Najib Ishaq
 Author-email: najib_ishaq@zoho.com
 Requires-Python: >=3.9.0,<3.10.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

