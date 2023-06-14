# Comparing `tmp/catencfamily-0.0.72.tar.gz` & `tmp/catencfamily-0.0.73.tar.gz`

## Comparing `catencfamily-0.0.72.tar` & `catencfamily-0.0.73.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.72/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.72/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 catencfamily-0.0.72/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.72/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.72/README.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 catencfamily-0.0.72/pyproject.toml
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 catencfamily-0.0.72/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.73/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.73/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 catencfamily-0.0.73/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.73/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.73/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 catencfamily-0.0.73/pyproject.toml
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.73/PKG-INFO
```

### Comparing `catencfamily-0.0.72/src/catencfamily/encoders.py` & `catencfamily-0.0.73/src/catencfamily/encoders.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.72/src/catencfamily/utils.py` & `catencfamily-0.0.73/src/catencfamily/utils.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.72/LICENSE` & `catencfamily-0.0.73/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.72/README.md` & `catencfamily-0.0.73/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.72/pyproject.toml` & `catencfamily-0.0.73/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.72"
+version = "0.0.73"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -20,12 +20,11 @@
   "pandas",
   "numpy",
   "networkx",
   "cdlib",
   "matplotlib",
   "seaborn",
   "pathlib",
-  "pickle",
   "scipy"
 ]
 [project.urls]
 "Homepage" = "https://github.com/harnalashok/CatEncodersFamily"
```

### Comparing `catencfamily-0.0.72/PKG-INFO` & `catencfamily-0.0.73/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.72
+Version: 0.0.73
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: cdlib
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pathlib
-Requires-Dist: pickle
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: seaborn
 Description-Content-Type: text/markdown
 
 # catencfamily
```

