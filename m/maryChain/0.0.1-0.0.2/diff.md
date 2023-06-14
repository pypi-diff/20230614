# Comparing `tmp/maryChain-0.0.1.tar.gz` & `tmp/maryChain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maryChain-0.0.1.tar", last modified: Wed Jun 14 12:59:58 2023, max compression
+gzip compressed data, was "maryChain-0.0.2.tar", last modified: Wed Jun 14 14:39:01 2023, max compression
```

## Comparing `maryChain-0.0.1.tar` & `maryChain-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-06-14 12:59:58.121913 maryChain-0.0.1/
--rw-r--r--   0 alessioricco   (501) staff       (20)     1070 2023-06-14 11:53:05.000000 maryChain-0.0.1/LICENSE
--rw-r--r--   0 alessioricco   (501) staff       (20)     7451 2023-06-14 12:59:58.121736 maryChain-0.0.1/PKG-INFO
--rw-r--r--   0 alessioricco   (501) staff       (20)     6601 2023-06-14 12:25:32.000000 maryChain-0.0.1/README.md
-drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-06-14 12:59:58.121448 maryChain-0.0.1/maryChain.egg-info/
--rw-r--r--   0 alessioricco   (501) staff       (20)     7451 2023-06-14 12:59:58.000000 maryChain-0.0.1/maryChain.egg-info/PKG-INFO
--rw-r--r--   0 alessioricco   (501) staff       (20)      190 2023-06-14 12:59:58.000000 maryChain-0.0.1/maryChain.egg-info/SOURCES.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)        1 2023-06-14 12:59:58.000000 maryChain-0.0.1/maryChain.egg-info/dependency_links.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)        4 2023-06-14 12:59:58.000000 maryChain-0.0.1/maryChain.egg-info/requires.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)        1 2023-06-14 12:59:58.000000 maryChain-0.0.1/maryChain.egg-info/top_level.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)       38 2023-06-14 12:59:58.121964 maryChain-0.0.1/setup.cfg
--rw-r--r--   0 alessioricco   (501) staff       (20)     1663 2023-06-14 12:59:48.000000 maryChain-0.0.1/setup.py
+drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-06-14 14:39:01.258734 maryChain-0.0.2/
+-rw-r--r--   0 alessioricco   (501) staff       (20)     1070 2023-06-14 11:53:05.000000 maryChain-0.0.2/LICENSE
+-rw-r--r--   0 alessioricco   (501) staff       (20)     7430 2023-06-14 14:39:01.258469 maryChain-0.0.2/PKG-INFO
+-rw-r--r--   0 alessioricco   (501) staff       (20)     6601 2023-06-14 12:25:32.000000 maryChain-0.0.2/README.md
+drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-06-14 14:39:01.255822 maryChain-0.0.2/maryChain/
+-rw-r--r--   0 alessioricco   (501) staff       (20)        0 2023-06-11 22:34:10.000000 maryChain-0.0.2/maryChain/__init__.py
+-rw-r--r--   0 alessioricco   (501) staff       (20)    25622 2023-06-14 14:37:37.000000 maryChain-0.0.2/maryChain/maryChain.py
+-rw-r--r--   0 alessioricco   (501) staff       (20)    32183 2023-06-13 19:41:24.000000 maryChain-0.0.2/maryChain/maryChainAST.py
+-rw-r--r--   0 alessioricco   (501) staff       (20)    13166 2023-06-14 12:17:08.000000 maryChain-0.0.2/maryChain/parsetab.py
+drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-06-14 14:39:01.258152 maryChain-0.0.2/maryChain.egg-info/
+-rw-r--r--   0 alessioricco   (501) staff       (20)     7430 2023-06-14 14:39:01.000000 maryChain-0.0.2/maryChain.egg-info/PKG-INFO
+-rw-r--r--   0 alessioricco   (501) staff       (20)      283 2023-06-14 14:39:01.000000 maryChain-0.0.2/maryChain.egg-info/SOURCES.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)        1 2023-06-14 14:39:01.000000 maryChain-0.0.2/maryChain.egg-info/dependency_links.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)        4 2023-06-14 14:39:01.000000 maryChain-0.0.2/maryChain.egg-info/requires.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)       10 2023-06-14 14:39:01.000000 maryChain-0.0.2/maryChain.egg-info/top_level.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)       38 2023-06-14 14:39:01.258809 maryChain-0.0.2/setup.cfg
+-rw-r--r--   0 alessioricco   (501) staff       (20)     1642 2023-06-14 14:33:58.000000 maryChain-0.0.2/setup.py
```

### Comparing `maryChain-0.0.1/LICENSE` & `maryChain-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maryChain-0.0.1/PKG-INFO` & `maryChain-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: maryChain
-Version: 0.0.1
+Version: 0.0.2
 Summary: maryChain - lightweight programming functional language for LLM
 Home-page: https://github.com/alessioricco/maryChain
-Download-URL: https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.6
+Download-URL: https://github.com/alessioricco/maryChain
 Author: Alessio Ricco
 Author-email: alessio.ricco@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/alessioricco/maryChain/issues
 Keywords: pypi,maryChain,programming language,functional,ai,llm
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `maryChain-0.0.1/README.md` & `maryChain-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `maryChain-0.0.1/maryChain.egg-info/PKG-INFO` & `maryChain-0.0.2/maryChain.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: maryChain
-Version: 0.0.1
+Version: 0.0.2
 Summary: maryChain - lightweight programming functional language for LLM
 Home-page: https://github.com/alessioricco/maryChain
-Download-URL: https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.6
+Download-URL: https://github.com/alessioricco/maryChain
 Author: Alessio Ricco
 Author-email: alessio.ricco@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/alessioricco/maryChain/issues
 Keywords: pypi,maryChain,programming language,functional,ai,llm
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `maryChain-0.0.1/setup.py` & `maryChain-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='maryChain',                           # should match the package folder
-    version='0.0.1',                                # important for updates
+    version='0.0.2',                                # important for updates
     license='MIT',                                  # should match your chosen license
     description='maryChain - lightweight programming functional language for LLM',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='Alessio Ricco',
     author_email='alessio.ricco@gmail.com',
     url='https://github.com/alessioricco/maryChain', 
@@ -27,9 +27,9 @@
         'Programming Language :: Python :: 3',
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
         "ply",
     ],   
-    download_url="https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.6",
+    download_url="https://github.com/alessioricco/maryChain",
 )
```

