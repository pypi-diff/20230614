# Comparing `tmp/cmaclp-0.0.8-py3-none-any.whl.zip` & `tmp/cmaclp-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 11697 bytes, number of entries: 8
--rw-r--r--  2.0 unx    20942 b- defN 23-Jun-14 09:16 cmaclp/SVM_prediction.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-14 09:16 cmaclp/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-14 09:19 cmaclp-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      755 b- defN 23-Jun-14 09:19 cmaclp-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 09:19 cmaclp-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx      164 b- defN 23-Jun-14 09:19 cmaclp-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-14 09:19 cmaclp-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      629 b- defN 23-Jun-14 09:19 cmaclp-0.0.8.dist-info/RECORD
-8 files, 33946 bytes uncompressed, 10597 bytes compressed:  68.8%
+Zip file size: 11913 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    21604 b- defN 23-Jun-14 16:22 cmaclp/SVM_prediction.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-14 16:22 cmaclp/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-14 16:25 cmaclp-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      755 b- defN 23-Jun-14 16:25 cmaclp-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 16:25 cmaclp-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-14 16:25 cmaclp-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-14 16:25 cmaclp-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      629 b- defN 23-Jun-14 16:25 cmaclp-0.0.9.dist-info/RECORD
+8 files, 34608 bytes uncompressed, 10813 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: cmaclp/SVM_prediction.py
 Comment: 
 
 Filename: cmaclp/__init__.py
 Comment: 
 
-Filename: cmaclp-0.0.8.dist-info/LICENSE
+Filename: cmaclp-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: cmaclp-0.0.8.dist-info/METADATA
+Filename: cmaclp-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: cmaclp-0.0.8.dist-info/WHEEL
+Filename: cmaclp-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: cmaclp-0.0.8.dist-info/entry_points.txt
+Filename: cmaclp-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: cmaclp-0.0.8.dist-info/top_level.txt
+Filename: cmaclp-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: cmaclp-0.0.8.dist-info/RECORD
+Filename: cmaclp-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmaclp/SVM_prediction.py

```diff
@@ -2,14 +2,15 @@
 import os
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import time as tm
 import seaborn as sns
 import rpy2.robjects as robjects
+import matplotlib
 import matplotlib.pyplot as plt
 from sklearn.svm import LinearSVC
 from sklearn.calibration import CalibratedClassifierCV
 from sklearn.metrics import confusion_matrix
 from sklearn.model_selection import KFold
 from sklearn.preprocessing import LabelEncoder
 from sklearn.metrics import f1_score
@@ -146,33 +147,14 @@
     meta_atlas:
     show_umap:
     show_bar:
     '''
     print("Reading query data")
     adata=read_h5ad(query_H5AD)
     SVM_key=f"{SVM_type}_predicted"
-    
-    # Set category colors:
-    if meta_atlas is True:
-        category_colors = {"LSC": "#66CD00",
-                    "LESC": "#76EE00",
-                    "LE": "#66CDAA",
-                    "Cj": "#191970",
-                    "CE": "#1874CD",
-                    "qSK": "#FFB90F",
-                    "SK": "#EEAD0E",
-                    "TSK": "#FF7F00",
-                    "CF": "#CD6600",
-                    "EC": "#87CEFA",
-                    "Ves": "#8B2323",
-                    "Mel": "#FFFF00",
-                    "IC": "#00CED1",
-                    "nm-cSC": "#FF0000",
-                    "MC": "#CD3700",
-                    "Unknown": "#808080"}
 
     # Load in the object and add the predicted labels
     print("Adding predictions to query data")
     for file in os.listdir(OutputDir):
         if file.endswith('.csv'):
             if 'rej' not in file:
                 filedir= OutputDir+file
@@ -192,14 +174,47 @@
                 filedir= OutputDir+file
                 #print(filedir)
                 influence_data= pd.read_csv(filedir,sep=',',index_col=0)
                 #print(influence_data)
                 influence_data=influence_data.index.tolist()
                 adata.obs["SVMrej_predicted_prob"]=influence_data
 
+    # Set category colors:
+    if meta_atlas is True:
+        category_colors = {"LSC": "#66CD00",
+                    "LESC": "#76EE00",
+                    "LE": "#66CDAA",
+                    "Cj": "#191970",
+                    "CE": "#1874CD",
+                    "qSK": "#FFB90F",
+                    "SK": "#EEAD0E",
+                    "TSK": "#FF7F00",
+                    "CF": "#CD6600",
+                    "EC": "#87CEFA",
+                    "Ves": "#8B2323",
+                    "Mel": "#FFFF00",
+                    "IC": "#00CED1",
+                    "nm-cSC": "#FF0000",
+                    "MC": "#CD3700",
+                    "Unknown": "#808080"}
+                    
+    if meta_atlas is False:
+    
+      # Load a large color palette
+      palette_name = "tab20"
+      cmap = plt.get_cmap(palette_name)
+      palette=[matplotlib.colors.rgb2hex(c) for c in cmap.colors] 
+      
+      # Extract the list of colors
+      colors = palette
+      key_cats = adata.obs[SVM_key].astype("category")
+      key_list = key_cats.cat.categories.to_list()
+            
+      category_colors = dict(zip(key_list, colors[:len(key_list)]))
+      
     # Plot UMAP if selected
     print("Plotting UMAP")
     sc.set_figure_params(figsize=(5, 5))
     if show_umap is True:
         if meta_atlas is True:
             category_order_list = ["LSC", "LESC","LE","Cj","CE","qSK","SK","TSK","CF","EC","Ves","Mel","IC","nm-cSC","MC","Unknown"]
             adata.obs[SVM_key] = adata.obs[SVM_key].astype("category")
@@ -236,35 +251,42 @@
 
         df = pd.DataFrame.from_dict(obs2_to_obs1,orient = 'index').reset_index()
         df = df.set_index(["index"])
         df.columns=obs1_clusters
         df.index.names = ['Replicate']
 
         if meta_atlas is True:
-            ordered_list=["LSC", "LESC","LE","Cj","CE","qSK","SK","TSK","CF","EC","Ves","Mel","IC","nm-cSC","MC","Unknown"]
             palette=category_colors
-            lstval = [palette[key] for key in ordered_list]
-            sorter=ordered_list
-            df = df[sorter]
+            if SVM_type == 'SVM':
+              ordered_list=["LSC", "LESC","LE","Cj","CE","qSK","SK","TSK","CF","EC","Ves","Mel","IC","nm-cSC","MC"]
+            if SVM_type == 'SVMrej':
+              ordered_list=["LSC", "LESC","LE","Cj","CE","qSK","SK","TSK","CF","EC","Ves","Mel","IC","nm-cSC","MC","Unknown"]
+            
+            # Sorts the df on the longer ordered list
+            sorter=sorted(df.columns, key=ordered_list.index)
+            
+            # Retrieve the color codes from the sorted list
+            lstval = [palette[key] for key in sorter]
+            
+            try:
+              df=df[sorter]
+            except KeyError:
+              df=df
+        else:
+            lstval=list(category_colors.values())
 
         stacked_data = df.apply(lambda x: x*100/sum(x), axis=1)
         stacked_data=stacked_data.iloc[:, ::-1]
 
         fig, ax =plt.subplots(1,2)
-        if meta_atlas is True:
-            df.plot(kind="bar", stacked=True, ax=ax[0], legend = False,color=lstval, rot=45, title='Absolute number of cells')
-        else:
-            df.plot(kind="bar", stacked=True, ax=ax[0], legend = False, rot=45, title='Absolute number of cells')
+        df.plot(kind="bar", stacked=True, ax=ax[0], legend = False,color=lstval, rot=45, title='Absolute number of cells')
 
         fig.legend(loc=7,title="Cell state")
 
-        if meta_atlas is True:
-            stacked_data.plot(kind="bar", stacked=True, legend = False, ax=ax[1],color=lstval[::-1], rot=45, title='Percentage of cells')
-        else:
-            stacked_data.plot(kind="bar", stacked=True, legend = False, ax=ax[1], rot=45, title='Percentage of cells')
+        stacked_data.plot(kind="bar", stacked=True, legend = False, ax=ax[1],color=lstval[::-1], rot=45, title='Percentage of cells')
 
         fig.tight_layout()
         fig.subplots_adjust(right=0.9)
         fig.savefig(f"figures/{SVM_key}_bar.pdf", bbox_inches='tight')
         plt.close(fig)
     else:
         None
```

## Comparing `cmaclp-0.0.8.dist-info/LICENSE` & `cmaclp-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cmaclp-0.0.8.dist-info/METADATA` & `cmaclp-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmaclp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Corneal meta-atlas command line predictor
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools (<=57.5.0)
 Requires-Dist: wheel
 Requires-Dist: python-build
 Requires-Dist: pytest-cov
```

