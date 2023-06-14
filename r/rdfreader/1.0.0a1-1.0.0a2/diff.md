# Comparing `tmp/rdfreader-1.0.0a1.tar.gz` & `tmp/rdfreader-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfreader-1.0.0a1.tar", max compression
+gzip compressed data, was "rdfreader-1.0.0a2.tar", max compression
```

## Comparing `rdfreader-1.0.0a1.tar` & `rdfreader-1.0.0a2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      738 2023-06-14 12:57:20.407486 rdfreader-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0       49 2023-05-04 09:39:42.731680 rdfreader-1.0.0a1/rdfreader/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 09:39:42.731680 rdfreader-1.0.0a1/rdfreader/chem/__init__.py
--rw-r--r--   0        0        0     4977 2023-05-09 16:08:15.935278 rdfreader-1.0.0a1/rdfreader/chem/mol.py
--rw-r--r--   0        0        0     4775 2023-05-09 16:08:15.935278 rdfreader-1.0.0a1/rdfreader/chem/reaction.py
--rw-r--r--   0        0        0      881 2023-05-09 16:08:15.935278 rdfreader-1.0.0a1/rdfreader/chem/utils.py
--rw-r--r--   0        0        0      246 2023-05-09 16:08:15.935278 rdfreader-1.0.0a1/rdfreader/exceptions.py
--rw-r--r--   0        0        0     2758 2023-05-09 16:08:15.935278 rdfreader-1.0.0a1/rdfreader/parse/molblock.py
--rw-r--r--   0        0        0     8105 2023-06-14 12:39:56.244379 rdfreader-1.0.0a1/rdfreader/parse/rxnblock.py
--rw-r--r--   0        0        0    10226 2023-05-09 16:08:15.935278 rdfreader-1.0.0a1/rdfreader/parse/utils.py
--rw-r--r--   0        0        0     4951 2023-05-09 16:08:15.935278 rdfreader-1.0.0a1/rdfreader/rdf.py
--rw-r--r--   0        0        0      985 2023-05-09 16:08:15.935278 rdfreader-1.0.0a1/rdfreader/write.py
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 rdfreader-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0      738 2023-06-14 12:59:15.823827 rdfreader-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-05-04 09:39:42.731680 rdfreader-1.0.0a2/rdfreader/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 09:39:42.731680 rdfreader-1.0.0a2/rdfreader/chem/__init__.py
+-rw-r--r--   0        0        0     4977 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/chem/mol.py
+-rw-r--r--   0        0        0     4775 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/chem/reaction.py
+-rw-r--r--   0        0        0      881 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/chem/utils.py
+-rw-r--r--   0        0        0      246 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/exceptions.py
+-rw-r--r--   0        0        0     2758 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/parse/molblock.py
+-rw-r--r--   0        0        0     8105 2023-06-14 12:39:56.244379 rdfreader-1.0.0a2/rdfreader/parse/rxnblock.py
+-rw-r--r--   0        0        0    10226 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/parse/utils.py
+-rw-r--r--   0        0        0     4951 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/rdf.py
+-rw-r--r--   0        0        0      985 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/write.py
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 rdfreader-1.0.0a2/PKG-INFO
```

### Comparing `rdfreader-1.0.0a1/pyproject.toml` & `rdfreader-1.0.0a2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "rdfreader"
 # The version is currently managed by the github release workflow (see README), don't use.
-version = "1.0.0a1"  
+version = "1.0.0a2"  
 description = "Read the full contents of CTAB .rdf files in python. Captures RXN and MOL record using RDKit and reads additional data fields (including solvents/catalysts/agents)."
 authors = ["deepmatter <enquiries@deepmatter.io>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rdkit = "^2022.9.3"
```

### Comparing `rdfreader-1.0.0a1/rdfreader/chem/mol.py` & `rdfreader-1.0.0a2/rdfreader/chem/mol.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a1/rdfreader/chem/reaction.py` & `rdfreader-1.0.0a2/rdfreader/chem/reaction.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a1/rdfreader/chem/utils.py` & `rdfreader-1.0.0a2/rdfreader/chem/utils.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a1/rdfreader/parse/molblock.py` & `rdfreader-1.0.0a2/rdfreader/parse/molblock.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a1/rdfreader/parse/rxnblock.py` & `rdfreader-1.0.0a2/rdfreader/parse/rxnblock.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a1/rdfreader/parse/utils.py` & `rdfreader-1.0.0a2/rdfreader/parse/utils.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a1/rdfreader/rdf.py` & `rdfreader-1.0.0a2/rdfreader/rdf.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a1/rdfreader/write.py` & `rdfreader-1.0.0a2/rdfreader/write.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a1/PKG-INFO` & `rdfreader-1.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfreader
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Read the full contents of CTAB .rdf files in python. Captures RXN and MOL record using RDKit and reads additional data fields (including solvents/catalysts/agents).
 Author: deepmatter
 Author-email: enquiries@deepmatter.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

