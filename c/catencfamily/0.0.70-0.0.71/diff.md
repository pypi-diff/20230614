# Comparing `tmp/catencfamily-0.0.70.tar.gz` & `tmp/catencfamily-0.0.71.tar.gz`

## Comparing `catencfamily-0.0.70.tar` & `catencfamily-0.0.71.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.70/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.70/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    30887 2020-02-02 00:00:00.000000 catencfamily-0.0.70/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.70/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.70/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.70/pyproject.toml
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.70/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.71/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.71/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 catencfamily-0.0.71/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.71/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.71/README.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 catencfamily-0.0.71/pyproject.toml
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 catencfamily-0.0.71/PKG-INFO
```

### Comparing `catencfamily-0.0.70/src/catencfamily/encoders.py` & `catencfamily-0.0.71/src/catencfamily/encoders.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.70/src/catencfamily/utils.py` & `catencfamily-0.0.71/src/catencfamily/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-# 11th June, 2023
+# 14th June, 2023
 
 ## Utility functions
 
 
 import pandas as pd
 import numpy as np
 from scipy.stats import kurtosis
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import StandardScaler
 from sklearn.datasets import make_classification
 from sklearn.feature_selection import  mutual_info_classif
 import networkx as nx
+import itertools
 import pickle
 import pathlib
 import string
 import matplotlib.pyplot as plt
 import seaborn as sns
+from pathlib import Path
 
 
 
 def xgImptFeatures(model, df_columns, filename = None, master=None):
     """
     Given an xgboost classifier model & data col
     names, the function returns two lists of cols,
@@ -258,14 +260,15 @@
     X_data = np.array(X)
     y_data = np.array(y)
     
     orig_train, orig_test,train_binned,test_binned = transformFeatures(X_data,y_data, test_size, bins, genColName)
     return orig_train, orig_test, train_binned, test_binned    
 
 
+
  
 def transformFeatures(X_data,y_data, test_size = 0.25, bins= 20,  colnames = None, genColName = True):
     
     """
     Called by: transformToCatFeatures() , generateClassificationData
     Calls: None
     
@@ -955,12 +958,123 @@
     nx.draw_networkx_edges(G, pos, width = edgewidth, ax =ax);
     nx.draw_networkx_nodes(G, pos, node_color=dict(color_map_b).values(), ax =ax);
     if withLabels:
       nx.draw_networkx_labels(G, pos, font_size = font_size, font_weight = 'bold',ax =ax)
     plt.axis("off");
     plt.title(title)
     #plt.show();    
+
+
+def transformBinnedDF2Communities(columnNames,pathToGraphFolder, train_binned, algo):
+    """
+    Desc
+    -----
+    Replace every column in the binned the Dataframe as per network community
+    Example binned/discrete dataframe:
+            'a'     'b
+            --      ---
+            434     709
+            435     789
+            23      710
+            78      756
+
+    Replace col 'a' as per communities discovered in network 'a_projected_b.gml':
+    434 & 435 belong to one community and 23 & 78 to other.    
+
+            'a'     'b'
+            ---     ---
+             0      709
+             0      789
+             1      710
+             1      756
+
+    Similarly, replace col 'b' as per communities in 'b_projected_a.gml':
+
+            'a'     'b'
+            ---     ---
+             0      1
+             0      0
+             1      0
+             1      1
+             
+    Parameters
+    -----------     
+    columnNames: list of cat cols
+    pathToGraphFolder: str: Folder that has graph files     
+    train_binned: DataFrame with binned/discrete columns  
+    algo: function object: networkx algorithm to be used to 
+          discover communities.
+          Example: nx.community.greedy_modularity_communities  
+          
+    Returns
+    -------
+    map_list: list of dictionaries. Each dictionary maps
+              levels in a column to a community 
+    df: DataFrame: Transformed train_binned DataFrame.
+        If train_binned had columns other than columnNames,
+        df would not contain those columns          
+
+
+    """
+
+    # 1. From col-names names, create graph filenames:
+    # Example: col-names: ['a','b','c']
+    # First permute col-names in pairs of two:
+    #  p = ('a','b'),('b','a'), ('a','c'),('c','a')...
+    p = list(itertools.permutations(columnNames,2))
+    # Prepare list of graph files:
+    # ('a_projected_b.gml', 'b_projected_a.gml'...)
+    filelist = [] 
+    for i in p:
+      filelist.append(i[0] + "_projected_" + i[1] + ".gml")
+
+    # 2. For every file in the filelist
+    map_list = []  # Start with a blank list of dictionaries
+    # df will store dataframe train_binned after each bin-col is mapped
+    #  
+    df = pd.DataFrame()
+    for file in filelist:
+      # 2.1 Load network
+      # Get full filename that includes filepath
+      filepath = Path(pathToGraphFolder) / file
+      # Read the file as a network
+      G = nx.read_gml(filepath)
+
+      # 2.2 Calculate community classes using algo
+      #    cm_mod contains as many frozensets of nodes
+      #    as there are communities:
+      cm_mod = algo(G)
+
+      # 3.0 We now create dict corresponding to
+      #     all communities in cm_mod
+      #    Example:
+      #                 frozenset1         frozenset2
+      #   cm_mod:      {'434', '435' },    {'23' , '78'}
+      #   fset_dict  {'434': 0, '435' :0, '23' : 1, '78': 1}
+
+      counter = 0  # Assigns values in dict
+      fset_dict = {}  # Start with blank dict
+      # For every frozenset
+      for i in cm_mod:
+        # For every item in this frozenset
+        for g in i:
+          # Set class to the value of counter
+          fset_dict[g] = counter
+
+        # Increment counter for next class
+        counter  +=1
+      # Now that map dict for the modularity
+      # classes are ready, append it to map_list
+      map_list.append(fset_dict)
+
+      # Extract column name from file:
+      colToProject = file.split('_')[0]
+      # Map train_binned column using the dict
+      df[file] = train_binned[colToProject].map(fset_dict)
+      # Continue for loop for the next filelist
+    return map_list,df
+
     
 ################### That's all folks #######################
```

### Comparing `catencfamily-0.0.70/LICENSE` & `catencfamily-0.0.71/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.70/README.md` & `catencfamily-0.0.71/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.70/pyproject.toml` & `catencfamily-0.0.71/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.70"
+version = "0.0.71"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,11 +18,15 @@
 dependencies = [
   "scikit-learn",
   "pandas",
   "numpy",
   "networkx",
   "cdlib",
   "matplotlib",
+  "seaborn",
   "pathlib",
+  "itertools",
+  "pickle",
+  "scipy"
 ]
 [project.urls]
 "Homepage" = "https://github.com/harnalashok/CatEncodersFamily"
```

### Comparing `catencfamily-0.0.70/PKG-INFO` & `catencfamily-0.0.71/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.70
+Version: 0.0.71
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: cdlib
+Requires-Dist: itertools
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pathlib
+Requires-Dist: pickle
 Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: seaborn
 Description-Content-Type: text/markdown
 
 # catencfamily
 
 The module provides a way to encode categorical features in multiple but related ways using network analysis. Together, the family of multiple encodings serve as a numerical vector for every level of a categorical feature. The class transforms a group of categorical features into corresponding numerical features which can then be used either in unsupervised learning or in predictive analytics. To assist in unsupervised learning, it has methods to save a categorical feature as network graphs and plot them. The class has methods to extract unit vectors for every level of a categorical feature to help, for example, in understanding relationshsips between various levels. Extracted numerical vectors can directly be used in plotting, for example, in tensorflow's Embedding Projector. Class provides methods to get categories encoded for large datasets; one can, for example, take a sample of data at a time, have categories encoded, then take another sample and have categories similarly encoded. After a number of iterations, take either a mean or median to get final category-wise vectors. As the encodings are calculated using a group of network analysis operations, the family of encodings is extensible. The class provides one way, but a limited one to extend it.
 
 ## Installation
```

