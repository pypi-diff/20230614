# Comparing `tmp/TicTacToeAI-0.0.2.tar.gz` & `tmp/TicTacToeAI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TicTacToeAI-0.0.2.tar", last modified: Wed Jun 14 07:50:26 2023, max compression
+gzip compressed data, was "TicTacToeAI-0.0.3.tar", last modified: Wed Jun 14 07:53:43 2023, max compression
```

## Comparing `TicTacToeAI-0.0.2.tar` & `TicTacToeAI-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-14 07:50:26.142329 TicTacToeAI-0.0.2/
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1073 2023-06-07 01:00:16.000000 TicTacToeAI-0.0.2/LICENSE
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1425 2023-06-14 07:50:26.141853 TicTacToeAI-0.0.2/PKG-INFO
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      956 2023-06-14 07:43:13.000000 TicTacToeAI-0.0.2/README.md
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       38 2023-06-14 07:50:26.142553 TicTacToeAI-0.0.2/setup.cfg
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      784 2023-06-14 07:50:20.000000 TicTacToeAI-0.0.2/setup.py
-drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-14 07:50:26.137767 TicTacToeAI-0.0.2/src/
-drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-14 07:50:26.140962 TicTacToeAI-0.0.2/src/TicTacToeAI.egg-info/
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1425 2023-06-14 07:50:25.000000 TicTacToeAI-0.0.2/src/TicTacToeAI.egg-info/PKG-INFO
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      239 2023-06-14 07:50:26.000000 TicTacToeAI-0.0.2/src/TicTacToeAI.egg-info/SOURCES.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        1 2023-06-14 07:50:25.000000 TicTacToeAI-0.0.2/src/TicTacToeAI.egg-info/dependency_links.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        6 2023-06-14 07:50:26.000000 TicTacToeAI-0.0.2/src/TicTacToeAI.egg-info/requires.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       12 2023-06-14 07:50:26.000000 TicTacToeAI-0.0.2/src/TicTacToeAI.egg-info/top_level.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     3446 2023-06-14 07:33:27.000000 TicTacToeAI-0.0.2/src/TicTacToeAI.py
+drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-14 07:53:43.505732 TicTacToeAI-0.0.3/
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1073 2023-06-07 01:00:16.000000 TicTacToeAI-0.0.3/LICENSE
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1425 2023-06-14 07:53:43.505042 TicTacToeAI-0.0.3/PKG-INFO
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      956 2023-06-14 07:43:13.000000 TicTacToeAI-0.0.3/README.md
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       38 2023-06-14 07:53:43.506024 TicTacToeAI-0.0.3/setup.cfg
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      784 2023-06-14 07:52:39.000000 TicTacToeAI-0.0.3/setup.py
+drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-14 07:53:43.500378 TicTacToeAI-0.0.3/src/
+drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-14 07:53:43.503482 TicTacToeAI-0.0.3/src/TicTacToeAI.egg-info/
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1425 2023-06-14 07:53:43.000000 TicTacToeAI-0.0.3/src/TicTacToeAI.egg-info/PKG-INFO
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      239 2023-06-14 07:53:43.000000 TicTacToeAI-0.0.3/src/TicTacToeAI.egg-info/SOURCES.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        1 2023-06-14 07:53:43.000000 TicTacToeAI-0.0.3/src/TicTacToeAI.egg-info/dependency_links.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        6 2023-06-14 07:53:43.000000 TicTacToeAI-0.0.3/src/TicTacToeAI.egg-info/requires.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       12 2023-06-14 07:53:43.000000 TicTacToeAI-0.0.3/src/TicTacToeAI.egg-info/top_level.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     3446 2023-06-14 07:33:27.000000 TicTacToeAI-0.0.3/src/TicTacToeAI.py
```

### Comparing `TicTacToeAI-0.0.2/LICENSE` & `TicTacToeAI-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TicTacToeAI-0.0.2/PKG-INFO` & `TicTacToeAI-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TicTacToeAI
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tic Tac Toe with AI.
 Home-page: https://github.com/ujjwalredd/Tic-Tac-Toe-with-AI
 Author: Ujjwal Reddy K S
 License: UNKNOWN
 Keywords: MinMax,Diffcult,AI
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TicTacToeAI-0.0.2/README.md` & `TicTacToeAI-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `TicTacToeAI-0.0.2/setup.py` & `TicTacToeAI-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='TicTacToeAI',
-    version='0.0.2',
+    version='0.0.3',
     description='Tic Tac Toe with AI.',
     author= 'Ujjwal Reddy K S',
     url = 'https://github.com/ujjwalredd/Tic-Tac-Toe-with-AI',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     keywords=['MinMax', 'Diffcult', 'AI'],
```

### Comparing `TicTacToeAI-0.0.2/src/TicTacToeAI.egg-info/PKG-INFO` & `TicTacToeAI-0.0.3/src/TicTacToeAI.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TicTacToeAI
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tic Tac Toe with AI.
 Home-page: https://github.com/ujjwalredd/Tic-Tac-Toe-with-AI
 Author: Ujjwal Reddy K S
 License: UNKNOWN
 Keywords: MinMax,Diffcult,AI
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TicTacToeAI-0.0.2/src/TicTacToeAI.py` & `TicTacToeAI-0.0.3/src/TicTacToeAI.py`

 * *Files identical despite different names*

