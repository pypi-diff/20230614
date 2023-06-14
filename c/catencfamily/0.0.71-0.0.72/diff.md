# Comparing `tmp/catencfamily-0.0.71.tar.gz` & `tmp/catencfamily-0.0.72.tar.gz`

## Comparing `catencfamily-0.0.71.tar` & `catencfamily-0.0.72.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.71/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.71/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 catencfamily-0.0.71/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.71/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.71/README.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 catencfamily-0.0.71/pyproject.toml
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 catencfamily-0.0.71/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.72/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.72/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 catencfamily-0.0.72/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.72/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.72/README.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 catencfamily-0.0.72/pyproject.toml
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 catencfamily-0.0.72/PKG-INFO
```

### Comparing `catencfamily-0.0.71/src/catencfamily/encoders.py` & `catencfamily-0.0.72/src/catencfamily/encoders.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.71/src/catencfamily/utils.py` & `catencfamily-0.0.72/src/catencfamily/utils.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.71/LICENSE` & `catencfamily-0.0.72/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.71/README.md` & `catencfamily-0.0.72/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.71/pyproject.toml` & `catencfamily-0.0.72/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.71"
+version = "0.0.72"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -20,13 +20,12 @@
   "pandas",
   "numpy",
   "networkx",
   "cdlib",
   "matplotlib",
   "seaborn",
   "pathlib",
-  "itertools",
   "pickle",
   "scipy"
 ]
 [project.urls]
 "Homepage" = "https://github.com/harnalashok/CatEncodersFamily"
```

### Comparing `catencfamily-0.0.71/PKG-INFO` & `catencfamily-0.0.72/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.71
+Version: 0.0.72
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: cdlib
-Requires-Dist: itertools
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pathlib
 Requires-Dist: pickle
 Requires-Dist: scikit-learn
```

