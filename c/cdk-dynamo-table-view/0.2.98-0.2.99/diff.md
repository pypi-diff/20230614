# Comparing `tmp/cdk-dynamo-table-view-0.2.98.tar.gz` & `tmp/cdk-dynamo-table-view-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-dynamo-table-view-0.2.98.tar", last modified: Sun Mar 13 00:27:25 2022, max compression
+gzip compressed data, was "cdk-dynamo-table-view-0.2.99.tar", last modified: Mon Mar 14 00:30:47 2022, max compression
```

## Comparing `cdk-dynamo-table-view-0.2.98.tar` & `cdk-dynamo-table-view-0.2.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-13 00:27:25.063787 cdk-dynamo-table-view-0.2.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-03-13 00:27:14.000000 cdk-dynamo-table-view-0.2.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-03-13 00:27:14.000000 cdk-dynamo-table-view-0.2.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2579 2022-03-13 00:27:25.063787 cdk-dynamo-table-view-0.2.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-03-13 00:27:14.000000 cdk-dynamo-table-view-0.2.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-03-13 00:27:14.000000 cdk-dynamo-table-view-0.2.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-13 00:27:25.063787 cdk-dynamo-table-view-0.2.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-03-13 00:27:14.000000 cdk-dynamo-table-view-0.2.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-13 00:27:25.063787 cdk-dynamo-table-view-0.2.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-13 00:27:25.063787 cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view/
--rw-r--r--   0 runner    (1001) docker     (121)     6696 2022-03-13 00:27:14.000000 cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-13 00:27:25.063787 cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-03-13 00:27:14.000000 cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19621 2022-03-13 00:27:14.000000 cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view/_jsii/cdk-dynamo-table-viewer@0.2.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-13 00:27:14.000000 cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-13 00:27:25.063787 cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2579 2022-03-13 00:27:24.000000 cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-03-13 00:27:24.000000 cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-13 00:27:24.000000 cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-03-13 00:27:24.000000 cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-13 00:27:24.000000 cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 00:30:47.116855 cdk-dynamo-table-view-0.2.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-03-14 00:30:33.000000 cdk-dynamo-table-view-0.2.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-03-14 00:30:33.000000 cdk-dynamo-table-view-0.2.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2579 2022-03-14 00:30:47.116855 cdk-dynamo-table-view-0.2.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-03-14 00:30:33.000000 cdk-dynamo-table-view-0.2.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-03-14 00:30:33.000000 cdk-dynamo-table-view-0.2.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-14 00:30:47.116855 cdk-dynamo-table-view-0.2.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-03-14 00:30:33.000000 cdk-dynamo-table-view-0.2.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 00:30:47.116855 cdk-dynamo-table-view-0.2.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 00:30:47.116855 cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view/
+-rw-r--r--   0 runner    (1001) docker     (121)     6696 2022-03-14 00:30:33.000000 cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 00:30:47.116855 cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-03-14 00:30:33.000000 cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19619 2022-03-14 00:30:33.000000 cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view/_jsii/cdk-dynamo-table-viewer@0.2.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-14 00:30:33.000000 cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 00:30:47.116855 cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2579 2022-03-14 00:30:47.000000 cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2022-03-14 00:30:47.000000 cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-14 00:30:47.000000 cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-03-14 00:30:47.000000 cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-14 00:30:47.000000 cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view.egg-info/top_level.txt
```

### Comparing `cdk-dynamo-table-view-0.2.98/LICENSE` & `cdk-dynamo-table-view-0.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-dynamo-table-view-0.2.98/PKG-INFO` & `cdk-dynamo-table-view-0.2.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-dynamo-table-view
-Version: 0.2.98
+Version: 0.2.99
 Summary: An AWS CDK construct which exposes an endpoint with the contents of a DynamoDB table
 Home-page: https://github.com/cdklabs/cdk-dynamo-table-viewer.git
 Author: Elad Ben-Israel<elad.benisrael@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-dynamo-table-viewer.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-dynamo-table-view-0.2.98/README.md` & `cdk-dynamo-table-view-0.2.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-dynamo-table-view-0.2.98/setup.py` & `cdk-dynamo-table-view-0.2.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-dynamo-table-view",
-    "version": "0.2.98",
+    "version": "0.2.99",
     "description": "An AWS CDK construct which exposes an endpoint with the contents of a DynamoDB table",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-dynamo-table-viewer.git",
     "long_description_content_type": "text/markdown",
     "author": "Elad Ben-Israel<elad.benisrael@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_dynamo_table_view",
         "cdk_dynamo_table_view._jsii"
     ],
     "package_data": {
         "cdk_dynamo_table_view._jsii": [
-            "cdk-dynamo-table-viewer@0.2.98.jsii.tgz"
+            "cdk-dynamo-table-viewer@0.2.99.jsii.tgz"
         ],
         "cdk_dynamo_table_view": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
```

### Comparing `cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view/__init__.py` & `cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-dynamo-table-view-0.2.98/src/cdk_dynamo_table_view.egg-info/PKG-INFO` & `cdk-dynamo-table-view-0.2.99/src/cdk_dynamo_table_view.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-dynamo-table-view
-Version: 0.2.98
+Version: 0.2.99
 Summary: An AWS CDK construct which exposes an endpoint with the contents of a DynamoDB table
 Home-page: https://github.com/cdklabs/cdk-dynamo-table-viewer.git
 Author: Elad Ben-Israel<elad.benisrael@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-dynamo-table-viewer.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

