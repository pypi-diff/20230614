# Comparing `tmp/cdk8s-valheim-0.0.85.tar.gz` & `tmp/cdk8s-valheim-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-valheim-0.0.85.tar", last modified: Wed Jun 14 00:19:26 2023, max compression
+gzip compressed data, was "cdk8s-valheim-0.0.9.tar", last modified: Wed Mar 29 00:19:55 2023, max compression
```

## Comparing `cdk8s-valheim-0.0.85.tar` & `cdk8s-valheim-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:19:26.440495 cdk8s-valheim-0.0.85/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-14 00:19:13.000000 cdk8s-valheim-0.0.85/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 00:19:13.000000 cdk8s-valheim-0.0.85/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-14 00:19:26.440495 cdk8s-valheim-0.0.85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-14 00:19:13.000000 cdk8s-valheim-0.0.85/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 00:19:13.000000 cdk8s-valheim-0.0.85/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 00:19:26.440495 cdk8s-valheim-0.0.85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-14 00:19:13.000000 cdk8s-valheim-0.0.85/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:19:26.436495 cdk8s-valheim-0.0.85/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:19:26.440495 cdk8s-valheim-0.0.85/src/cdk8s_valheim/
--rw-r--r--   0 runner    (1001) docker     (123)    74269 2023-06-14 00:19:13.000000 cdk8s-valheim-0.0.85/src/cdk8s_valheim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:19:26.440495 cdk8s-valheim-0.0.85/src/cdk8s_valheim/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-14 00:19:13.000000 cdk8s-valheim-0.0.85/src/cdk8s_valheim/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35323 2023-06-14 00:19:13.000000 cdk8s-valheim-0.0.85/src/cdk8s_valheim/_jsii/cdk8s-valheim@0.0.85.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:19:13.000000 cdk8s-valheim-0.0.85/src/cdk8s_valheim/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:19:26.440495 cdk8s-valheim-0.0.85/src/cdk8s_valheim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-14 00:19:26.000000 cdk8s-valheim-0.0.85/src/cdk8s_valheim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-14 00:19:26.000000 cdk8s-valheim-0.0.85/src/cdk8s_valheim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:19:26.000000 cdk8s-valheim-0.0.85/src/cdk8s_valheim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-14 00:19:26.000000 cdk8s-valheim-0.0.85/src/cdk8s_valheim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 00:19:26.000000 cdk8s-valheim-0.0.85/src/cdk8s_valheim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:19:55.046563 cdk8s-valheim-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-29 00:19:42.000000 cdk8s-valheim-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-29 00:19:42.000000 cdk8s-valheim-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-03-29 00:19:55.046563 cdk8s-valheim-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-03-29 00:19:42.000000 cdk8s-valheim-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-29 00:19:42.000000 cdk8s-valheim-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 00:19:55.046563 cdk8s-valheim-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-29 00:19:42.000000 cdk8s-valheim-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:19:55.042563 cdk8s-valheim-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:19:55.042563 cdk8s-valheim-0.0.9/src/cdk8s_valheim/
+-rw-r--r--   0 runner    (1001) docker     (123)    74269 2023-03-29 00:19:42.000000 cdk8s-valheim-0.0.9/src/cdk8s_valheim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:19:55.046563 cdk8s-valheim-0.0.9/src/cdk8s_valheim/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-29 00:19:42.000000 cdk8s-valheim-0.0.9/src/cdk8s_valheim/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34804 2023-03-29 00:19:42.000000 cdk8s-valheim-0.0.9/src/cdk8s_valheim/_jsii/cdk8s-valheim@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 00:19:42.000000 cdk8s-valheim-0.0.9/src/cdk8s_valheim/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:19:55.046563 cdk8s-valheim-0.0.9/src/cdk8s_valheim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-03-29 00:19:55.000000 cdk8s-valheim-0.0.9/src/cdk8s_valheim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-29 00:19:55.000000 cdk8s-valheim-0.0.9/src/cdk8s_valheim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 00:19:55.000000 cdk8s-valheim-0.0.9/src/cdk8s_valheim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-29 00:19:55.000000 cdk8s-valheim-0.0.9/src/cdk8s_valheim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-29 00:19:55.000000 cdk8s-valheim-0.0.9/src/cdk8s_valheim.egg-info/top_level.txt
```

### Comparing `cdk8s-valheim-0.0.85/LICENSE` & `cdk8s-valheim-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-valheim-0.0.85/PKG-INFO` & `cdk8s-valheim-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-valheim
-Version: 0.0.85
+Version: 0.0.9
 Summary: A package that vends a Valheim server chart.
 Home-page: https://github.com/awlsring/cdk8s-valheim.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdk8s-valheim.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-valheim-0.0.85/README.md` & `cdk8s-valheim-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-valheim-0.0.85/setup.py` & `cdk8s-valheim-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-valheim",
-    "version": "0.0.85",
+    "version": "0.0.9",
     "description": "A package that vends a Valheim server chart.",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdk8s-valheim.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "cdk8s_valheim",
         "cdk8s_valheim._jsii"
     ],
     "package_data": {
         "cdk8s_valheim._jsii": [
-            "cdk8s-valheim@0.0.85.jsii.tgz"
+            "cdk8s-valheim@0.0.9.jsii.tgz"
         ],
         "cdk8s_valheim": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdk8s-plus-26==2.2.2",
         "cdk8s>=2.7.36, <3.0.0",
         "constructs>=10.1.281, <11.0.0",
-        "jsii>=1.83.0, <2.0.0",
+        "jsii>=1.79.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk8s-valheim-0.0.85/src/cdk8s_valheim/__init__.py` & `cdk8s-valheim-0.0.9/src/cdk8s_valheim/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-valheim-0.0.85/src/cdk8s_valheim.egg-info/PKG-INFO` & `cdk8s-valheim-0.0.9/src/cdk8s_valheim.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-valheim
-Version: 0.0.85
+Version: 0.0.9
 Summary: A package that vends a Valheim server chart.
 Home-page: https://github.com/awlsring/cdk8s-valheim.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdk8s-valheim.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

