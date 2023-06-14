# Comparing `tmp/lxtractor-0.1.dev5.tar.gz` & `tmp/lxtractor-0.1.dev6.tar.gz`

## Comparing `lxtractor-0.1.dev5.tar` & `lxtractor-0.1.dev6.tar`

### file list

```diff
@@ -1,50 +1,47 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/.DS_Store
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/__init__.py
--rw-r--r--   0        0        0    18511 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/protocols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/py.typed
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/__init__.py
--rw-r--r--   0        0        0    15016 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/alignment.py
--rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/base.py
--rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/config.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/exceptions.py
--rw-r--r--   0        0        0    26168 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/segment.py
--rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/structure.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/chain/__init__.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/chain/base.py
--rw-r--r--   0        0        0    19660 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/chain/chain.py
--rw-r--r--   0        0        0    15733 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/chain/initializer.py
--rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/chain/io.py
--rw-r--r--   0        0        0    18956 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/chain/list.py
--rw-r--r--   0        0        0    33430 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/chain/sequence.py
--rw-r--r--   0        0        0    21023 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/chain/structure.py
--rw-r--r--   0        0        0     9846 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/core/chain/tree.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/ext/.DS_Store
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/ext/__init__.py
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/ext/alphafold.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/ext/base.py
--rw-r--r--   0        0        0    10285 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/ext/hmm.py
--rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/ext/pdb_.py
--rw-r--r--   0        0        0    16091 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/ext/sifts.py
--rw-r--r--   0        0        0    16171 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/ext/uniprot.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/ext/resources/.DS_Store
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/ext/resources/PFP.csv
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/ext/resources/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/util/__init__.py
--rw-r--r--   0        0        0    16174 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/util/io.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/util/misc.py
--rw-r--r--   0        0        0    16266 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/util/seq.py
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/util/structure.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/util/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/variables/__init__.py
--rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/variables/base.py
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/variables/calculator.py
--rw-r--r--   0        0        0    17743 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/variables/manager.py
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/variables/parser.py
--rw-r--r--   0        0        0     8762 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/variables/sequential.py
--rw-r--r--   0        0        0    13138 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/lXtractor/variables/structural.py
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/LICENSE
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/README.rst
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/pyproject.toml
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 lxtractor-0.1.dev5/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/__init__.py
+-rw-r--r--   0        0        0    18511 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/protocols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/py.typed
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/__init__.py
+-rw-r--r--   0        0        0    15016 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/alignment.py
+-rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/base.py
+-rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/config.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/exceptions.py
+-rw-r--r--   0        0        0    26168 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/segment.py
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/structure.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/chain/__init__.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/chain/base.py
+-rw-r--r--   0        0        0    19660 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/chain/chain.py
+-rw-r--r--   0        0        0    15733 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/chain/initializer.py
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/chain/io.py
+-rw-r--r--   0        0        0    18956 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/chain/list.py
+-rw-r--r--   0        0        0    33430 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/chain/sequence.py
+-rw-r--r--   0        0        0    21023 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/chain/structure.py
+-rw-r--r--   0        0        0     9846 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/core/chain/tree.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/ext/__init__.py
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/ext/alphafold.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/ext/base.py
+-rw-r--r--   0        0        0    10285 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/ext/hmm.py
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/ext/pdb_.py
+-rw-r--r--   0        0        0    16091 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/ext/sifts.py
+-rw-r--r--   0        0        0    16171 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/ext/uniprot.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/ext/resources/PFP.csv
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/ext/resources/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/util/__init__.py
+-rw-r--r--   0        0        0    16174 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/util/io.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/util/misc.py
+-rw-r--r--   0        0        0    16266 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/util/seq.py
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/util/structure.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/util/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/variables/__init__.py
+-rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/variables/base.py
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/variables/calculator.py
+-rw-r--r--   0        0        0    17743 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/variables/manager.py
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/variables/parser.py
+-rw-r--r--   0        0        0     8762 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/variables/sequential.py
+-rw-r--r--   0        0        0    13138 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/lXtractor/variables/structural.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/LICENSE
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/README.rst
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 lxtractor-0.1.dev6/PKG-INFO
```

### Comparing `lxtractor-0.1.dev5/lXtractor/protocols.py` & `lxtractor-0.1.dev6/lXtractor/protocols.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/alignment.py` & `lxtractor-0.1.dev6/lXtractor/core/alignment.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/base.py` & `lxtractor-0.1.dev6/lXtractor/core/base.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/config.py` & `lxtractor-0.1.dev6/lXtractor/core/config.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/exceptions.py` & `lxtractor-0.1.dev6/lXtractor/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/segment.py` & `lxtractor-0.1.dev6/lXtractor/core/segment.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/structure.py` & `lxtractor-0.1.dev6/lXtractor/core/structure.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/chain/base.py` & `lxtractor-0.1.dev6/lXtractor/core/chain/base.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/chain/chain.py` & `lxtractor-0.1.dev6/lXtractor/core/chain/chain.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/chain/initializer.py` & `lxtractor-0.1.dev6/lXtractor/core/chain/initializer.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/chain/io.py` & `lxtractor-0.1.dev6/lXtractor/core/chain/io.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/chain/list.py` & `lxtractor-0.1.dev6/lXtractor/core/chain/list.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/chain/sequence.py` & `lxtractor-0.1.dev6/lXtractor/core/chain/sequence.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/chain/structure.py` & `lxtractor-0.1.dev6/lXtractor/core/chain/structure.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/core/chain/tree.py` & `lxtractor-0.1.dev6/lXtractor/core/chain/tree.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/ext/alphafold.py` & `lxtractor-0.1.dev6/lXtractor/ext/alphafold.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/ext/base.py` & `lxtractor-0.1.dev6/lXtractor/ext/base.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/ext/hmm.py` & `lxtractor-0.1.dev6/lXtractor/ext/hmm.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/ext/pdb_.py` & `lxtractor-0.1.dev6/lXtractor/ext/pdb_.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/ext/sifts.py` & `lxtractor-0.1.dev6/lXtractor/ext/sifts.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/ext/uniprot.py` & `lxtractor-0.1.dev6/lXtractor/ext/uniprot.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/ext/resources/PFP.csv` & `lxtractor-0.1.dev6/lXtractor/ext/resources/PFP.csv`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/util/io.py` & `lxtractor-0.1.dev6/lXtractor/util/io.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/util/misc.py` & `lxtractor-0.1.dev6/lXtractor/util/misc.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/util/seq.py` & `lxtractor-0.1.dev6/lXtractor/util/seq.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/util/structure.py` & `lxtractor-0.1.dev6/lXtractor/util/structure.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/util/typing.py` & `lxtractor-0.1.dev6/lXtractor/util/typing.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/variables/base.py` & `lxtractor-0.1.dev6/lXtractor/variables/base.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/variables/calculator.py` & `lxtractor-0.1.dev6/lXtractor/variables/calculator.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/variables/manager.py` & `lxtractor-0.1.dev6/lXtractor/variables/manager.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/variables/parser.py` & `lxtractor-0.1.dev6/lXtractor/variables/parser.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/variables/sequential.py` & `lxtractor-0.1.dev6/lXtractor/variables/sequential.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/lXtractor/variables/structural.py` & `lxtractor-0.1.dev6/lXtractor/variables/structural.py`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/.gitignore` & `lxtractor-0.1.dev6/.gitignore`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/LICENSE` & `lxtractor-0.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `lxtractor-0.1.dev5/pyproject.toml` & `lxtractor-0.1.dev6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Documentation :: Sphinx",
 ]
 authors = [
     { name = "Ivan Reveguk", email = "ivan.reveguk@gmail.com" }
 ]
 maintainers = [
@@ -48,37 +49,20 @@
 
 [tool.hatch]
 version.path = "lXtractor/__about__.py"
 
 [tool.hatch.build]
 ignore-vcs = true
 packages = ["lXtractor"]
-include = [
-    "/resources"
-]
 exclude = [
     "*.gz"
 ]
 
-#[tool.hatch.build.targets.wheel]
-#only-include = ['lXtractor']
-
-[tool.hatch.envs.test]
-dependencies = [
-    "pytest",
-    "pytest-cov",
-    "pytest-sugar",
-]
-
-[tool.hatch.envs.test.scripts]
-cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=tkp_finder --cov=tests {args}"
-no-cov = "cov --no-cov {args}"
-
-[[tool.hatch.envs.test.matrix]]
-python = ["310", "311"]
+[tool.hatch.build.targets.wheel]
+only-include = ['lXtractor']
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
     "lXtractor/__about__.py",
 ]
```

### Comparing `lxtractor-0.1.dev5/PKG-INFO` & `lxtractor-0.1.dev6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: lXtractor
-Version: 0.1.dev5
+Version: 0.1.dev6
 Summary: Feature extraction library for sequences and structures
 Project-URL: Source code, https://github.com/edikedik/lXtractor
 Project-URL: Bug Tracker, https://github.com//edikedik/lXtractor/issues
 Author-email: Ivan Reveguk <ivan.reveguk@gmail.com>
 Maintainer-email: Ivan Reveguk <ivan.reveguk@gmail.com>
 License-File: LICENSE
 Keywords: Bioinformatics,Computational biology,Data Mining,Datasets,Feature extracton,Protein sequence,Protein structure
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Requires-Dist: biotite>=0.35.0
 Requires-Dist: more-itertools>=9.0
 Requires-Dist: networkx>=2.8.6
 Requires-Dist: numpy>=1.23
@@ -45,39 +46,8 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/lXtractor.svg
     :target: https://pypi.org/project/lXtractor
     :alt: Python version
 
 .. image:: https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg
    :alt: Hatch project
-   :target: https://github.com/pypa/hatch
-
-Installation
-============
-
-First, create a fresh conda environment::
-
-    conda create -n lxt python=3.10 -y
-
-Currently, `lXtractor` uses `mafft <https://mafft.cbrc.jp/alignment/software/>`_
-to handle mappings between a sequence and MSA columns. Consequently, it expects
-mafft to be available in ``$PATH$``. You can either install mafft system-wide
-or use conda::
-
-    conda install -c conda-forge mafft -y
-    conda activate lXt
-
-Using pip
----------
-
-..code :: python
-    pip install lXtractor
-
-Using conda
------------
-
-TBD
-
-
-From source
------------
-
+   :target: https://github.com/pypa/hatch
```

