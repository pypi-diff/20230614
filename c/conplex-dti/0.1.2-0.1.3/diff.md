# Comparing `tmp/conplex_dti-0.1.2.tar.gz` & `tmp/conplex_dti-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conplex_dti-0.1.2.tar", max compression
+gzip compressed data, was "conplex_dti-0.1.3.tar", max compression
```

## Comparing `conplex_dti-0.1.2.tar` & `conplex_dti-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1074 2023-03-11 16:53:19.162872 conplex_dti-0.1.2/LICENSE
--rw-r--r--   0        0        0     3723 2023-06-12 16:38:19.603868 conplex_dti-0.1.2/README.md
--rw-r--r--   0        0        0     3510 2023-04-27 20:13:59.889524 conplex_dti-0.1.2/conplex_dti/MAIN_OLD.txt
--rw-r--r--   0        0        0      399 2023-06-12 16:38:19.605660 conplex_dti-0.1.2/conplex_dti/__init__.py
--rw-r--r--   0        0        0     1070 2023-06-12 16:38:19.607396 conplex_dti-0.1.2/conplex_dti/__main__.py
--rw-r--r--   0        0        0    23714 2023-04-27 20:13:59.892315 conplex_dti-0.1.2/conplex_dti/architectures.py
--rw-r--r--   0        0        0      166 2023-04-27 20:13:59.893555 conplex_dti-0.1.2/conplex_dti/cli/__init__.py
--rw-r--r--   0        0        0     1316 2023-04-27 20:13:59.894669 conplex_dti-0.1.2/conplex_dti/cli/download.py
--rw-r--r--   0        0        0    19492 2023-06-13 20:17:18.168303 conplex_dti-0.1.2/conplex_dti/cli/train.py
--rw-r--r--   0        0        0      171 2023-04-27 20:13:59.897366 conplex_dti-0.1.2/conplex_dti/dataset/__init__.py
--rw-r--r--   0        0        0    24290 2023-06-12 16:38:19.611383 conplex_dti-0.1.2/conplex_dti/dataset/datamodules.py
--rw-r--r--   0        0        0      421 2023-04-27 20:13:59.900173 conplex_dti-0.1.2/conplex_dti/featurizer/__init__.py
--rw-r--r--   0        0        0     7731 2023-04-27 20:13:59.901288 conplex_dti-0.1.2/conplex_dti/featurizer/base.py
--rw-r--r--   0        0        0    11422 2023-04-27 20:13:59.902654 conplex_dti-0.1.2/conplex_dti/featurizer/molecule.py
--rw-r--r--   0        0        0    11493 2023-04-27 21:09:39.865982 conplex_dti-0.1.2/conplex_dti/featurizer/protein.py
--rw-r--r--   0        0        0        0 2023-04-27 20:13:59.904417 conplex_dti-0.1.2/conplex_dti/model/__init__.py
--rw-r--r--   0        0        0    23789 2023-04-27 20:13:59.906381 conplex_dti-0.1.2/conplex_dti/model/architectures.py
--rw-r--r--   0        0        0     2125 2023-04-27 20:13:59.907393 conplex_dti-0.1.2/conplex_dti/model/margin.py
--rw-r--r--   0        0        0     4022 2023-04-27 20:13:59.908432 conplex_dti-0.1.2/conplex_dti/utils.py
--rw-r--r--   0        0        0     4177 2023-06-13 20:17:36.998182 conplex_dti-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5325 1970-01-01 00:00:00.000000 conplex_dti-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-11 16:53:19.162872 conplex_dti-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3723 2023-06-13 23:34:46.686358 conplex_dti-0.1.3/README.md
+-rw-r--r--   0        0        0     3510 2023-06-14 01:47:41.847038 conplex_dti-0.1.3/conplex_dti/MAIN_OLD.txt
+-rw-r--r--   0        0        0      399 2023-06-14 01:47:41.848725 conplex_dti-0.1.3/conplex_dti/__init__.py
+-rw-r--r--   0        0        0     1070 2023-06-14 01:47:41.850137 conplex_dti-0.1.3/conplex_dti/__main__.py
+-rw-r--r--   0        0        0    23714 2023-06-14 01:47:41.852511 conplex_dti-0.1.3/conplex_dti/architectures.py
+-rw-r--r--   0        0        0      166 2023-06-14 01:47:41.854260 conplex_dti-0.1.3/conplex_dti/cli/__init__.py
+-rw-r--r--   0        0        0     3520 2023-06-14 01:49:08.121559 conplex_dti-0.1.3/conplex_dti/cli/download.py
+-rw-r--r--   0        0        0    19492 2023-06-14 01:53:03.395219 conplex_dti-0.1.3/conplex_dti/cli/train.py
+-rw-r--r--   0        0        0      171 2023-06-14 01:47:41.895917 conplex_dti-0.1.3/conplex_dti/dataset/__init__.py
+-rw-r--r--   0        0        0    24289 2023-06-14 01:59:20.076442 conplex_dti-0.1.3/conplex_dti/dataset/datamodules.py
+-rw-r--r--   0        0        0      421 2023-06-14 01:47:41.919180 conplex_dti-0.1.3/conplex_dti/featurizer/__init__.py
+-rw-r--r--   0        0        0     7731 2023-06-14 01:47:41.938695 conplex_dti-0.1.3/conplex_dti/featurizer/base.py
+-rw-r--r--   0        0        0    11422 2023-06-14 01:47:41.958730 conplex_dti-0.1.3/conplex_dti/featurizer/molecule.py
+-rw-r--r--   0        0        0    11493 2023-06-14 01:47:41.996784 conplex_dti-0.1.3/conplex_dti/featurizer/protein.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:47:41.997856 conplex_dti-0.1.3/conplex_dti/model/__init__.py
+-rw-r--r--   0        0        0    23789 2023-06-14 01:47:42.015759 conplex_dti-0.1.3/conplex_dti/model/architectures.py
+-rw-r--r--   0        0        0     2125 2023-06-14 01:47:42.044312 conplex_dti-0.1.3/conplex_dti/model/margin.py
+-rw-r--r--   0        0        0     4022 2023-06-14 01:47:42.059531 conplex_dti-0.1.3/conplex_dti/utils.py
+-rw-r--r--   0        0        0     4177 2023-06-14 01:53:47.956602 conplex_dti-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5325 1970-01-01 00:00:00.000000 conplex_dti-0.1.3/PKG-INFO
```

### Comparing `conplex_dti-0.1.2/LICENSE` & `conplex_dti-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.2/README.md` & `conplex_dti-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.2/conplex_dti/MAIN_OLD.txt` & `conplex_dti-0.1.3/conplex_dti/MAIN_OLD.txt`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.2/conplex_dti/__main__.py` & `conplex_dti-0.1.3/conplex_dti/__main__.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.2/conplex_dti/architectures.py` & `conplex_dti-0.1.3/conplex_dti/architectures.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.2/conplex_dti/cli/train.py` & `conplex_dti-0.1.3/conplex_dti/cli/train.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.2/conplex_dti/dataset/datamodules.py` & `conplex_dti-0.1.3/conplex_dti/dataset/datamodules.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     :param task_name: Name of benchmark
     :type task_name: str
     """
 
     database_root = Path(database_root).resolve()
 
     task_paths = {
-        "biosnap": database_root / "/BIOSNAP/full_data",
+        "biosnap": database_root / "BIOSNAP/full_data",
         "biosnap_prot": database_root / "BIOSNAP/unseen_protein",
         "biosnap_mol": database_root / "BIOSNAP/unseen_drug",
         "bindingdb": database_root / "BindingDB",
         "davis": database_root / "DAVIS",
         "dti_dg": database_root / "TDC",
         "dude": database_root / "DUDe",
         "halogenase": database_root / "EnzPred/halogenase_NaCl_binary",
```

### Comparing `conplex_dti-0.1.2/conplex_dti/featurizer/base.py` & `conplex_dti-0.1.3/conplex_dti/featurizer/base.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.2/conplex_dti/featurizer/molecule.py` & `conplex_dti-0.1.3/conplex_dti/featurizer/molecule.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.2/conplex_dti/featurizer/protein.py` & `conplex_dti-0.1.3/conplex_dti/featurizer/protein.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.2/conplex_dti/model/architectures.py` & `conplex_dti-0.1.3/conplex_dti/model/architectures.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.2/conplex_dti/model/margin.py` & `conplex_dti-0.1.3/conplex_dti/model/margin.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.2/conplex_dti/utils.py` & `conplex_dti-0.1.3/conplex_dti/utils.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.2/pyproject.toml` & `conplex_dti-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "conplex-dti"
-version = "0.1.2"
+version = "0.1.3"
 description = "Adapting protein language models and contrastive learning for DTI prediction."
 readme = "README.md"
 authors = ["samsledje <samsl@mit.edu>"]
 license = "MIT"
 repository = "https://github.com/samsledje/ConPLex"
 homepage = "https://github.com/samsledje/ConPLex"
```

### Comparing `conplex_dti-0.1.2/PKG-INFO` & `conplex_dti-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conplex-dti
-Version: 0.1.2
+Version: 0.1.3
 Summary: Adapting protein language models and contrastive learning for DTI prediction.
 Home-page: https://github.com/samsledje/ConPLex
 License: MIT
 Keywords: protein language models,contrastive learning,drug target interaction,DTI
 Author: samsledje
 Author-email: samsl@mit.edu
 Requires-Python: >=3.9,<4.0
```

