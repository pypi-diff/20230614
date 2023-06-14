# Comparing `tmp/lightning_boost-1.0.0.tar.gz` & `tmp/lightning_boost-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning_boost-1.0.0.tar", max compression
+gzip compressed data, was "lightning_boost-1.0.1.tar", max compression
```

## Comparing `lightning_boost-1.0.0.tar` & `lightning_boost-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3531 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/README.md
--rw-r--r--   0        0        0       35 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/cli/__init__.py
--rw-r--r--   0        0        0     5429 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/cli/cli.py
--rw-r--r--   0        0        0        0 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/data/__init__.py
--rw-r--r--   0        0        0       44 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/data/datamodules/__init__.py
--rw-r--r--   0        0        0     6128 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/data/datamodules/base_datamodule.py
--rw-r--r--   0        0        0       38 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/data/datasets/__init__.py
--rw-r--r--   0        0        0     2392 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/data/datasets/base_dataset.py
--rw-r--r--   0        0        0       34 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/models/__init__.py
--rw-r--r--   0        0        0      651 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/models/base_model.py
--rw-r--r--   0        0        0        0 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/modules/__init__.py
--rw-r--r--   0        0        0       32 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/modules/loss/__init__.py
--rw-r--r--   0        0        0      949 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/modules/loss/task_loss.py
--rw-r--r--   0        0        0       36 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/modules/metrics/__init__.py
--rw-r--r--   0        0        0      801 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/modules/metrics/task_metric.py
--rw-r--r--   0        0        0       53 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/modules/optim/__init__.py
--rw-r--r--   0        0        0     1113 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/modules/optim/lr_scheduling_policy.py
--rw-r--r--   0        0        0      134 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/modules/preprocessing/__init__.py
--rw-r--r--   0        0        0     5452 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/modules/preprocessing/base_collator.py
--rw-r--r--   0        0        0      518 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/modules/preprocessing/base_transform.py
--rw-r--r--   0        0        0      847 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/modules/preprocessing/composite_transform.py
--rw-r--r--   0        0        0       36 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/systems/__init__.py
--rw-r--r--   0        0        0     9719 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/systems/base_system.py
--rw-r--r--   0        0        0     2662 2023-06-14 15:40:25.119694 lightning_boost-1.0.0/lightning_boost/systems/utils.py
--rw-r--r--   0        0        0     1108 2023-06-14 15:40:25.123694 lightning_boost-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4534 1970-01-01 00:00:00.000000 lightning_boost-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3531 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/README.md
+-rw-r--r--   0        0        0       35 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/cli/__init__.py
+-rw-r--r--   0        0        0     5429 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/cli/cli.py
+-rw-r--r--   0        0        0        0 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/data/__init__.py
+-rw-r--r--   0        0        0       44 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/data/datamodules/__init__.py
+-rw-r--r--   0        0        0     6128 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/data/datamodules/base_datamodule.py
+-rw-r--r--   0        0        0       38 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/data/datasets/__init__.py
+-rw-r--r--   0        0        0     2392 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/data/datasets/base_dataset.py
+-rw-r--r--   0        0        0       34 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/models/__init__.py
+-rw-r--r--   0        0        0      651 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/models/base_model.py
+-rw-r--r--   0        0        0        0 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/modules/__init__.py
+-rw-r--r--   0        0        0       32 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/modules/loss/__init__.py
+-rw-r--r--   0        0        0      949 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/modules/loss/task_loss.py
+-rw-r--r--   0        0        0       36 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/modules/metrics/__init__.py
+-rw-r--r--   0        0        0      801 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/modules/metrics/task_metric.py
+-rw-r--r--   0        0        0       53 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/modules/optim/__init__.py
+-rw-r--r--   0        0        0     1113 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/modules/optim/lr_scheduling_policy.py
+-rw-r--r--   0        0        0      134 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/modules/preprocessing/__init__.py
+-rw-r--r--   0        0        0     5452 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/modules/preprocessing/base_collator.py
+-rw-r--r--   0        0        0      518 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/modules/preprocessing/base_transform.py
+-rw-r--r--   0        0        0      847 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/modules/preprocessing/composite_transform.py
+-rw-r--r--   0        0        0       36 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/systems/__init__.py
+-rw-r--r--   0        0        0     9719 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/systems/base_system.py
+-rw-r--r--   0        0        0     2662 2023-06-14 15:53:29.662253 lightning_boost-1.0.1/lightning_boost/systems/utils.py
+-rw-r--r--   0        0        0     1108 2023-06-14 15:53:29.666253 lightning_boost-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4534 1970-01-01 00:00:00.000000 lightning_boost-1.0.1/PKG-INFO
```

### Comparing `lightning_boost-1.0.0/README.md` & `lightning_boost-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lightning_boost-1.0.0/lightning_boost/cli/cli.py` & `lightning_boost-1.0.1/lightning_boost/cli/cli.py`

 * *Files identical despite different names*

### Comparing `lightning_boost-1.0.0/lightning_boost/data/datamodules/base_datamodule.py` & `lightning_boost-1.0.1/lightning_boost/data/datamodules/base_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning_boost-1.0.0/lightning_boost/data/datasets/base_dataset.py` & `lightning_boost-1.0.1/lightning_boost/data/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `lightning_boost-1.0.0/lightning_boost/models/base_model.py` & `lightning_boost-1.0.1/lightning_boost/models/base_model.py`

 * *Files identical despite different names*

### Comparing `lightning_boost-1.0.0/lightning_boost/modules/loss/task_loss.py` & `lightning_boost-1.0.1/lightning_boost/modules/loss/task_loss.py`

 * *Files identical despite different names*

### Comparing `lightning_boost-1.0.0/lightning_boost/modules/metrics/task_metric.py` & `lightning_boost-1.0.1/lightning_boost/modules/metrics/task_metric.py`

 * *Files identical despite different names*

### Comparing `lightning_boost-1.0.0/lightning_boost/modules/optim/lr_scheduling_policy.py` & `lightning_boost-1.0.1/lightning_boost/modules/optim/lr_scheduling_policy.py`

 * *Files identical despite different names*

### Comparing `lightning_boost-1.0.0/lightning_boost/modules/preprocessing/base_collator.py` & `lightning_boost-1.0.1/lightning_boost/modules/preprocessing/base_collator.py`

 * *Files identical despite different names*

### Comparing `lightning_boost-1.0.0/lightning_boost/modules/preprocessing/base_transform.py` & `lightning_boost-1.0.1/lightning_boost/modules/preprocessing/base_transform.py`

 * *Files identical despite different names*

### Comparing `lightning_boost-1.0.0/lightning_boost/modules/preprocessing/composite_transform.py` & `lightning_boost-1.0.1/lightning_boost/modules/preprocessing/composite_transform.py`

 * *Files identical despite different names*

### Comparing `lightning_boost-1.0.0/lightning_boost/systems/base_system.py` & `lightning_boost-1.0.1/lightning_boost/systems/base_system.py`

 * *Files identical despite different names*

### Comparing `lightning_boost-1.0.0/lightning_boost/systems/utils.py` & `lightning_boost-1.0.1/lightning_boost/systems/utils.py`

 * *Files identical despite different names*

### Comparing `lightning_boost-1.0.0/pyproject.toml` & `lightning_boost-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lightning-boost"
-version = "v1.0.0"
+version = "v1.0.1"
 description = "PyTorch Lightning extension for faster model development."
 authors = ["Fabrice von der Lehr <fabrice.vonderlehr222@gmail.com>"]
 license = "mit"
 readme = "README.md"
 repository = "https://github.com/f-lair/lightning-boost"
 documentation = "https://lightning-boost.readthedocs.io/en/latest/"
 packages = [{include = "lightning_boost"}]
```

### Comparing `lightning_boost-1.0.0/PKG-INFO` & `lightning_boost-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-boost
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyTorch Lightning extension for faster model development.
 Home-page: https://github.com/f-lair/lightning-boost
 License: MIT
 Author: Fabrice von der Lehr
 Author-email: fabrice.vonderlehr222@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

