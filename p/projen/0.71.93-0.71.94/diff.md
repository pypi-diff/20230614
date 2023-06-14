# Comparing `tmp/projen-0.71.93.tar.gz` & `tmp/projen-0.71.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.71.93.tar", last modified: Tue Jun 13 11:28:54 2023, max compression
+gzip compressed data, was "projen-0.71.94.tar", last modified: Tue Jun 13 12:31:19 2023, max compression
```

## Comparing `projen-0.71.93.tar` & `projen-0.71.94.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.145880 projen-0.71.93/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-13 11:28:40.000000 projen-0.71.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 11:28:40.000000 projen-0.71.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    55404 2023-06-13 11:28:54.145880 projen-0.71.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    54524 2023-06-13 11:28:40.000000 projen-0.71.93/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-13 11:28:40.000000 projen-0.71.93/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 11:28:54.145880 projen-0.71.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-13 11:28:40.000000 projen-0.71.93/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.129879 projen-0.71.93/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.129879 projen-0.71.93/src/projen/
--rw-r--r--   0 runner    (1001) docker     (123)   593914 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.133879 projen-0.71.93/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.137880 projen-0.71.93/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (123)  2715365 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/_jsii/projen@0.71.93.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.137880 projen-0.71.93/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (123)  1036394 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.137880 projen-0.71.93/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (123)    39873 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.137880 projen-0.71.93/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (123)   478039 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.137880 projen-0.71.93/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (123)   572593 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.137880 projen-0.71.93/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (123)   211860 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.137880 projen-0.71.93/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (123)    75837 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.141880 projen-0.71.93/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (123)   275214 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.141880 projen-0.71.93/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)   235582 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.141880 projen-0.71.93/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)   196190 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.141880 projen-0.71.93/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (123)   175246 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.141880 projen-0.71.93/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)   604594 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.141880 projen-0.71.93/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (123)   190514 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.141880 projen-0.71.93/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (123)   246151 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.141880 projen-0.71.93/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (123)   427088 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.145880 projen-0.71.93/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.145880 projen-0.71.93/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (123)   750808 2023-06-13 11:28:40.000000 projen-0.71.93/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.133879 projen-0.71.93/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    55404 2023-06-13 11:28:54.000000 projen-0.71.93/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-13 11:28:54.000000 projen-0.71.93/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:28:54.000000 projen-0.71.93/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 11:28:54.000000 projen-0.71.93/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 11:28:54.000000 projen-0.71.93/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.259092 projen-0.71.94/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-13 12:31:08.000000 projen-0.71.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 12:31:08.000000 projen-0.71.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    55404 2023-06-13 12:31:19.259092 projen-0.71.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    54524 2023-06-13 12:31:08.000000 projen-0.71.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-13 12:31:08.000000 projen-0.71.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 12:31:19.259092 projen-0.71.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-13 12:31:08.000000 projen-0.71.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.243092 projen-0.71.94/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.247092 projen-0.71.94/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (123)   593914 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.247092 projen-0.71.94/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.251092 projen-0.71.94/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (123)  2731571 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/_jsii/projen@0.71.94.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.251092 projen-0.71.94/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (123)  1036394 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.251092 projen-0.71.94/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    39873 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.251092 projen-0.71.94/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)   478039 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.251092 projen-0.71.94/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (123)   572593 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.251092 projen-0.71.94/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (123)   211860 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.251092 projen-0.71.94/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)    75837 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.251092 projen-0.71.94/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (123)   275214 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.255092 projen-0.71.94/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)   235582 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.255092 projen-0.71.94/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)   196190 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.255092 projen-0.71.94/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (123)   175246 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.255092 projen-0.71.94/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)   604594 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.255092 projen-0.71.94/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (123)   190514 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.255092 projen-0.71.94/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (123)   246151 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.255092 projen-0.71.94/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (123)   427088 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.255092 projen-0.71.94/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.255092 projen-0.71.94/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (123)   750808 2023-06-13 12:31:08.000000 projen-0.71.94/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:31:19.247092 projen-0.71.94/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    55404 2023-06-13 12:31:19.000000 projen-0.71.94/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-13 12:31:19.000000 projen-0.71.94/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:31:19.000000 projen-0.71.94/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 12:31:19.000000 projen-0.71.94/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 12:31:19.000000 projen-0.71.94/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.71.93/LICENSE` & `projen-0.71.94/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/PKG-INFO` & `projen-0.71.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.71.93
+Version: 0.71.94
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.71.93/README.md` & `projen-0.71.94/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/setup.py` & `projen-0.71.94/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.71.93",
+    "version": "0.71.94",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,15 +38,15 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.71.93.jsii.tgz"
+            "projen@0.71.94.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `projen-0.71.93/src/projen/__init__.py` & `projen-0.71.94/src/projen/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/awscdk/__init__.py` & `projen-0.71.94/src/projen/awscdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/build/__init__.py` & `projen-0.71.94/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/cdk/__init__.py` & `projen-0.71.94/src/projen/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/cdk8s/__init__.py` & `projen-0.71.94/src/projen/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/cdktf/__init__.py` & `projen-0.71.94/src/projen/cdktf/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/circleci/__init__.py` & `projen-0.71.94/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/github/__init__.py` & `projen-0.71.94/src/projen/github/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/github/workflows/__init__.py` & `projen-0.71.94/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/gitlab/__init__.py` & `projen-0.71.94/src/projen/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/java/__init__.py` & `projen-0.71.94/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/javascript/__init__.py` & `projen-0.71.94/src/projen/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/python/__init__.py` & `projen-0.71.94/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/release/__init__.py` & `projen-0.71.94/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/typescript/__init__.py` & `projen-0.71.94/src/projen/typescript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/vscode/__init__.py` & `projen-0.71.94/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen/web/__init__.py` & `projen-0.71.94/src/projen/web/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.93/src/projen.egg-info/PKG-INFO` & `projen-0.71.94/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.71.93
+Version: 0.71.94
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.71.93/src/projen.egg-info/SOURCES.txt` & `projen-0.71.94/src/projen.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.71.93.jsii.tgz
+src/projen/_jsii/projen@0.71.94.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```

