# Comparing `tmp/catencfamily-0.0.73.tar.gz` & `tmp/catencfamily-0.0.74.tar.gz`

## Comparing `catencfamily-0.0.73.tar` & `catencfamily-0.0.74.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.73/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.73/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 catencfamily-0.0.73/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.73/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.73/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 catencfamily-0.0.73/pyproject.toml
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.73/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.74/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.74/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    34919 2020-02-02 00:00:00.000000 catencfamily-0.0.74/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.74/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.74/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 catencfamily-0.0.74/pyproject.toml
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.74/PKG-INFO
```

### Comparing `catencfamily-0.0.73/src/catencfamily/encoders.py` & `catencfamily-0.0.74/src/catencfamily/encoders.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.73/src/catencfamily/utils.py` & `catencfamily-0.0.74/src/catencfamily/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1022,14 +1022,23 @@
     #  p = ('a','b'),('b','a'), ('a','c'),('c','a')...
     p = list(itertools.permutations(columnNames,2))
     # Prepare list of graph files:
     # ('a_projected_b.gml', 'b_projected_a.gml'...)
     filelist = [] 
     for i in p:
       filelist.append(i[0] + "_projected_" + i[1] + ".gml")
+    
+    # Check if all files in filelist exist. Or which files exist?      
+    filesexist = []
+    for i in filelist:
+        myfile = Path(pathToGraphFolder) / i
+        if myfile.exists():
+            filesexist.append(i) 
+            
+    filelist = filesexist        
 
     # 2. For every file in the filelist
     map_list = []  # Start with a blank list of dictionaries
     # df will store dataframe train_binned after each bin-col is mapped
     #  
     df = pd.DataFrame()
     for file in filelist:
```

### Comparing `catencfamily-0.0.73/LICENSE` & `catencfamily-0.0.74/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.73/README.md` & `catencfamily-0.0.74/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.73/pyproject.toml` & `catencfamily-0.0.74/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.73"
+version = "0.0.74"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.73/PKG-INFO` & `catencfamily-0.0.74/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.73
+Version: 0.0.74
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

