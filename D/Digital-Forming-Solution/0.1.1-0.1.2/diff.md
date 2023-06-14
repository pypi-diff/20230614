# Comparing `tmp/Digital_Forming_Solution-0.1.1.tar.gz` & `tmp/Digital_Forming_Solution-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digital_Forming_Solution-0.1.1.tar", last modified: Tue Jun 13 15:04:44 2023, max compression
+gzip compressed data, was "Digital_Forming_Solution-0.1.2.tar", last modified: Wed Jun 14 10:30:53 2023, max compression
```

## Comparing `Digital_Forming_Solution-0.1.1.tar` & `Digital_Forming_Solution-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 15:04:44.562517 Digital_Forming_Solution-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-13 15:04:44.506567 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution/
--rw-rw-rw-   0        0        0      923 2023-06-13 15:03:46.000000 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution/Select_Operations.py
--rw-rw-rw-   0        0        0        0 2023-06-13 09:25:58.000000 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:04:44.546420 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution.egg-info/
--rw-rw-rw-   0        0        0      386 2023-06-13 15:04:43.000000 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-13 15:04:44.000000 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 15:04:43.000000 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 15:04:43.000000 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      386 2023-06-13 15:04:44.552381 Digital_Forming_Solution-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-13 15:04:44.563511 Digital_Forming_Solution-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      514 2023-06-13 15:04:02.000000 Digital_Forming_Solution-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 10:30:53.040635 Digital_Forming_Solution-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-06-14 10:30:52.979660 Digital_Forming_Solution-0.1.2/Digital_Forming_Solution/
+-rw-rw-rw-   0        0        0      910 2023-06-14 10:14:01.000000 Digital_Forming_Solution-0.1.2/Digital_Forming_Solution/Select_Operations.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 09:25:58.000000 Digital_Forming_Solution-0.1.2/Digital_Forming_Solution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 10:30:53.027590 Digital_Forming_Solution-0.1.2/Digital_Forming_Solution.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-06-14 10:30:52.000000 Digital_Forming_Solution-0.1.2/Digital_Forming_Solution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-14 10:30:52.000000 Digital_Forming_Solution-0.1.2/Digital_Forming_Solution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 10:30:52.000000 Digital_Forming_Solution-0.1.2/Digital_Forming_Solution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-14 10:30:52.000000 Digital_Forming_Solution-0.1.2/Digital_Forming_Solution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      386 2023-06-14 10:30:53.033513 Digital_Forming_Solution-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-14 10:30:53.043226 Digital_Forming_Solution-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      514 2023-06-14 10:30:36.000000 Digital_Forming_Solution-0.1.2/setup.py
```

### Comparing `Digital_Forming_Solution-0.1.1/Digital_Forming_Solution/Select_Operations.py` & `Digital_Forming_Solution-0.1.2/Digital_Forming_Solution/Select_Operations.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import numpy as np
 
 def Yield_Binning(datframe,column):
     
-    # Droping the Null Values
-    datframe = datframe.dropna(column)
-
-    # Copying the Dataframe
-    data =  datframe.copy()
+    # Filling the Missing Values   
+    datframe[column] = datframe[column].fillna(datframe[column].mean())
     
     # Calculating the yield quantiles
-    col_values = list(data[column])
+    col_values = list(datframe[column])
     Q_25 = np.percentile (col_values, 25) 
     Q_50 = np.percentile (col_values, 50)
     Q_75 = np.percentile (col_values, 75)
 
     # Creating the new column with the condtion
     for index,row in datframe.iterrows():
 
@@ -24,8 +21,9 @@
             datframe.at[index,'Category'] = 'Medium Low'
 
         elif (row[column]>Q_50 and row[column]<=Q_75):
             datframe.at[index,'Category'] = 'Medium High'
             
         else:
             datframe.at[index,'Category'] = 'High'
-    return datframe
+    return datframe
+
```

### Comparing `Digital_Forming_Solution-0.1.1/setup.py` & `Digital_Forming_Solution-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Digital_Forming_Solution",
-    version="0.1.1",
+    version="0.1.2",
     author="Bharatesha N S",
     author_email="bharatesha.ns.ext@bayer.com",
     description="DFS Projects Some of the Packages it help to perform task easily",
     packages=["Digital_Forming_Solution"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

