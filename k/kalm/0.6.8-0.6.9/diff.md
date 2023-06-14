# Comparing `tmp/kalm-0.6.8.tar.gz` & `tmp/kalm-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.6.8.tar", max compression
+gzip compressed data, was "kalm-0.6.9.tar", max compression
```

## Comparing `kalm-0.6.8.tar` & `kalm-0.6.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.8/LICENSE.txt
--rw-r--r--   0        0        0     1943 2023-06-03 20:13:50.968023 kalm-0.6.8/pyproject.toml
--rw-r--r--   0        0        0    10461 2023-06-02 10:48:49.438130 kalm-0.6.8/src/kalm/__init__.py
--rw-r--r--   0        0        0       27 2023-06-03 20:11:44.187283 kalm-0.6.8/src/kalm/inabox.py
--rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.8/src/kalm/jenkins.py
--rw-r--r--   0        0        0    33198 2023-06-03 20:08:23.030101 kalm-0.6.8/src/kalm/kalm.py
--rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.8/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.8/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.8/src/kalm/toolbox.py
--rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 kalm-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.9/LICENSE.txt
+-rw-r--r--   0        0        0     1943 2023-06-03 20:16:14.860858 kalm-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0    10461 2023-06-02 10:48:49.438130 kalm-0.6.9/src/kalm/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.9/src/kalm/jenkins.py
+-rw-r--r--   0        0        0    33198 2023-06-03 20:08:23.030101 kalm-0.6.9/src/kalm/kalm.py
+-rw-r--r--   0        0        0       27 2023-06-03 20:16:14.860858 kalm-0.6.9/src/kalm/kalm_inabox.py
+-rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.9/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.9/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.9/src/kalm/toolbox.py
+-rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 kalm-0.6.9/PKG-INFO
```

### Comparing `kalm-0.6.8/LICENSE.txt` & `kalm-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.6.8/pyproject.toml` & `kalm-0.6.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalm"
-version = "0.6.8"
+version = "0.6.9"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
 [tool.poetry.scripts]
@@ -26,15 +26,15 @@
 python-jenkins = "^1.7.0"
 urllib3 = "^2.0.2"
 
 
 
 [project]
 name = "kalm"  
-version = "0.6.8" 
+version = "0.6.9" 
 description = "Knowit automation lifecycle management"
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["kalm", "awx", "ansible", "automation"]  
 authors = [
   {name = "Jakob Holst", email = "jho@miracle.dk" }
```

### Comparing `kalm-0.6.8/src/kalm/__init__.py` & `kalm-0.6.9/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.8/src/kalm/kalm.py` & `kalm-0.6.9/src/kalm/kalm.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.8/src/kalm/netbox.py` & `kalm-0.6.9/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.8/PKG-INFO` & `kalm-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.6.8
+Version: 0.6.9
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

