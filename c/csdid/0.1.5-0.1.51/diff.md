# Comparing `tmp/csdid-0.1.5.tar.gz` & `tmp/csdid-0.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.5.tar", last modified: Tue Jun 13 22:07:27 2023, max compression
+gzip compressed data, was "csdid-0.1.51.tar", last modified: Tue Jun 13 22:10:50 2023, max compression
```

## Comparing `csdid-0.1.5.tar` & `csdid-0.1.51.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 22:07:27.693867 csdid-0.1.5/
--rw-rw-rw-   0        0        0     1126 2023-06-13 21:34:25.000000 csdid-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      533 2023-06-13 22:07:27.693867 csdid-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 22:07:27.674863 csdid-0.1.5/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:53:11.000000 csdid-0.1.5/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:07:27.684865 csdid-0.1.5/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:50:26.000000 csdid-0.1.5/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4700 2023-06-13 21:47:11.000000 csdid-0.1.5/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-13 21:47:35.000000 csdid-0.1.5/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-13 21:50:11.000000 csdid-0.1.5/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     3842 2023-06-13 21:46:48.000000 csdid-0.1.5/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:07:27.685865 csdid-0.1.5/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:48:55.000000 csdid-0.1.5/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-13 21:47:23.000000 csdid-0.1.5/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-13 21:47:19.000000 csdid-0.1.5/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:07:27.692868 csdid-0.1.5/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:48:44.000000 csdid-0.1.5/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-13 19:21:02.000000 csdid-0.1.5/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-13 22:07:15.000000 csdid-0.1.5/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:07:27.681864 csdid-0.1.5/csdid.egg-info/
--rw-rw-rw-   0        0        0      533 2023-06-13 22:07:27.000000 csdid-0.1.5/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-06-13 22:07:27.000000 csdid-0.1.5/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 22:07:27.000000 csdid-0.1.5/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 22:07:27.000000 csdid-0.1.5/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 22:07:27.694868 csdid-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      628 2023-06-13 22:07:20.000000 csdid-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:10:50.358677 csdid-0.1.51/
+-rw-rw-rw-   0        0        0     1126 2023-06-13 21:34:25.000000 csdid-0.1.51/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-13 22:10:50.358677 csdid-0.1.51/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 22:10:50.344673 csdid-0.1.51/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:53:11.000000 csdid-0.1.51/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:10:50.353675 csdid-0.1.51/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:50:26.000000 csdid-0.1.51/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4700 2023-06-13 21:47:11.000000 csdid-0.1.51/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-13 21:47:35.000000 csdid-0.1.51/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-13 21:50:11.000000 csdid-0.1.51/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     3890 2023-06-13 22:10:35.000000 csdid-0.1.51/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:10:50.355675 csdid-0.1.51/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:48:55.000000 csdid-0.1.51/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-13 21:47:23.000000 csdid-0.1.51/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-13 21:47:19.000000 csdid-0.1.51/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:10:50.357677 csdid-0.1.51/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:48:44.000000 csdid-0.1.51/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-13 19:21:02.000000 csdid-0.1.51/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-13 22:07:15.000000 csdid-0.1.51/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:10:50.351675 csdid-0.1.51/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-13 22:10:50.000000 csdid-0.1.51/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-06-13 22:10:50.000000 csdid-0.1.51/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 22:10:50.000000 csdid-0.1.51/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 22:10:50.000000 csdid-0.1.51/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 22:10:50.358677 csdid-0.1.51/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-06-13 22:10:46.000000 csdid-0.1.51/setup.py
```

### Comparing `csdid-0.1.5/LICENSE` & `csdid-0.1.51/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.5/PKG-INFO` & `csdid-0.1.51/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.5
+Version: 0.1.51
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.5/csdid/aggte_fnc/aggte.py` & `csdid-0.1.51/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.5/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.51/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.5/csdid/aggte_fnc/utils.py` & `csdid-0.1.51/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.5/csdid/att_gt.py` & `csdid-0.1.51/csdid/att_gt.py`

 * *Files 7% similar despite different names*

```diff
@@ -99,44 +99,44 @@
       biters=biters, cband=cband, alp=alp, clustervars=clustervars
     )
     return self
     
   
 
 
-import yaml, pandas as pd
+# import yaml, pandas as pd
 
-with open('configs/data.yml') as f:
-  dt = yaml.safe_load(f)
+# with open('configs/data.yml') as f:
+#   dt = yaml.safe_load(f)
 
-data = pd.read_csv(dt['mpdata'])
+# data = pd.read_csv(dt['mpdata'])
 
 
-yname = "lemp"
-gname = "first.treat"
-idname = "countyreal"
-tname = "year"
-xformla = f"lemp~1"
-# data = mpdta
-# print(data)
-# print(tname)
-b = ATTgt(yname, tname, idname, gname, data = data, xformla=xformla).fit()
-c = b.summ_attgt().summary2
-b.aggte(balance_e=1)
-# print(c)
-
-# print(aggte(b.MP, typec='dynamic'))
-# data = pd.read_csv(dt['simdata'])
-
-# yname = "Y"
-# tname = "period"
-# idname = "id"
-# gname = "G"
-# data = data
-# xformla = "Y~1"
+# yname = "lemp"
+# gname = "first.treat"
+# idname = "countyreal"
+# tname = "year"
+# xformla = f"lemp~1"
+# # data = mpdta
+# # print(data)
+# # print(tname)
+# b = ATTgt(yname, tname, idname, gname, data = data, xformla=xformla).fit()
+# c = b.summ_attgt().summary2
+# b.aggte(balance_e=1)
+# # print(c)
+
+# # print(aggte(b.MP, typec='dynamic'))
+# # data = pd.read_csv(dt['simdata'])
+
+# # yname = "Y"
+# # tname = "period"
+# # idname = "id"
+# # gname = "G"
+# # data = data
+# # xformla = "Y~1"
 
 
 # a = ATTgt(yname, idname, gname, data, xformla=xformla).fit().summ_attgt()
 # mp = a.MP
 
 
 # b = aggte(mp, typec='simple')
```

### Comparing `csdid-0.1.5/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.51/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.5/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.51/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.5/csdid/utils/bmisc.py` & `csdid-0.1.51/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.5/csdid/utils/mboot.py` & `csdid-0.1.51/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.5/csdid.egg-info/PKG-INFO` & `csdid-0.1.51/csdid.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.5
+Version: 0.1.51
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.5/setup.py` & `csdid-0.1.51/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'csdid',
-  version='0.1.5',
+  version='0.1.51',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
```

