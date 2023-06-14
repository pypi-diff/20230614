# Comparing `tmp/cdk-backup-plan-0.0.6.tar.gz` & `tmp/cdk-backup-plan-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-backup-plan-0.0.6.tar", last modified: Wed May 24 15:56:53 2023, max compression
+gzip compressed data, was "cdk-backup-plan-0.0.7.tar", last modified: Wed Jun 14 13:55:35 2023, max compression
```

## Comparing `cdk-backup-plan-0.0.6.tar` & `cdk-backup-plan-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:56:53.249343 cdk-backup-plan-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-24 15:56:38.000000 cdk-backup-plan-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 15:56:38.000000 cdk-backup-plan-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-24 15:56:53.249343 cdk-backup-plan-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-24 15:56:38.000000 cdk-backup-plan-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-24 15:56:38.000000 cdk-backup-plan-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:56:53.249343 cdk-backup-plan-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-24 15:56:38.000000 cdk-backup-plan-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:56:53.245343 cdk-backup-plan-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:56:53.249343 cdk-backup-plan-0.0.6/src/cdk_backup_plan/
--rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-05-24 15:56:38.000000 cdk-backup-plan-0.0.6/src/cdk_backup_plan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:56:53.249343 cdk-backup-plan-0.0.6/src/cdk_backup_plan/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-24 15:56:38.000000 cdk-backup-plan-0.0.6/src/cdk_backup_plan/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-05-24 15:56:38.000000 cdk-backup-plan-0.0.6/src/cdk_backup_plan/_jsii/cdk-backup-plan@0.0.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:56:38.000000 cdk-backup-plan-0.0.6/src/cdk_backup_plan/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:56:53.249343 cdk-backup-plan-0.0.6/src/cdk_backup_plan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-24 15:56:53.000000 cdk-backup-plan-0.0.6/src/cdk_backup_plan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-24 15:56:53.000000 cdk-backup-plan-0.0.6/src/cdk_backup_plan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:56:53.000000 cdk-backup-plan-0.0.6/src/cdk_backup_plan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-24 15:56:53.000000 cdk-backup-plan-0.0.6/src/cdk_backup_plan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 15:56:53.000000 cdk-backup-plan-0.0.6/src/cdk_backup_plan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:55:35.439926 cdk-backup-plan-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-14 13:55:23.000000 cdk-backup-plan-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 13:55:23.000000 cdk-backup-plan-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-14 13:55:35.439926 cdk-backup-plan-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-14 13:55:23.000000 cdk-backup-plan-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 13:55:23.000000 cdk-backup-plan-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 13:55:35.439926 cdk-backup-plan-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-14 13:55:23.000000 cdk-backup-plan-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:55:35.435926 cdk-backup-plan-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:55:35.435926 cdk-backup-plan-0.0.7/src/cdk_backup_plan/
+-rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-06-14 13:55:23.000000 cdk-backup-plan-0.0.7/src/cdk_backup_plan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:55:35.439926 cdk-backup-plan-0.0.7/src/cdk_backup_plan/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-14 13:55:23.000000 cdk-backup-plan-0.0.7/src/cdk_backup_plan/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-06-14 13:55:23.000000 cdk-backup-plan-0.0.7/src/cdk_backup_plan/_jsii/cdk-backup-plan@0.0.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:55:23.000000 cdk-backup-plan-0.0.7/src/cdk_backup_plan/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:55:35.439926 cdk-backup-plan-0.0.7/src/cdk_backup_plan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-14 13:55:35.000000 cdk-backup-plan-0.0.7/src/cdk_backup_plan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-14 13:55:35.000000 cdk-backup-plan-0.0.7/src/cdk_backup_plan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:55:35.000000 cdk-backup-plan-0.0.7/src/cdk_backup_plan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-14 13:55:35.000000 cdk-backup-plan-0.0.7/src/cdk_backup_plan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 13:55:35.000000 cdk-backup-plan-0.0.7/src/cdk_backup_plan.egg-info/top_level.txt
```

### Comparing `cdk-backup-plan-0.0.6/LICENSE` & `cdk-backup-plan-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-backup-plan-0.0.6/PKG-INFO` & `cdk-backup-plan-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-backup-plan
-Version: 0.0.6
+Version: 0.0.7
 Summary: CDK construct to create AWS Backup Plans
 Home-page: https://github.com/aws-samples/cdk-backup-plan.git
 Author: Mauricio Villaescusa<maurovc@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/cdk-backup-plan.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-backup-plan-0.0.6/README.md` & `cdk-backup-plan-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cdk-backup-plan-0.0.6/setup.py` & `cdk-backup-plan-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-backup-plan",
-    "version": "0.0.6",
+    "version": "0.0.7",
     "description": "CDK construct to create AWS Backup Plans",
     "license": "MIT-0",
     "url": "https://github.com/aws-samples/cdk-backup-plan.git",
     "long_description_content_type": "text/markdown",
     "author": "Mauricio Villaescusa<maurovc@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_backup_plan",
         "cdk_backup_plan._jsii"
     ],
     "package_data": {
         "cdk_backup_plan._jsii": [
-            "cdk-backup-plan@0.0.6.jsii.tgz"
+            "cdk-backup-plan@0.0.7.jsii.tgz"
         ],
         "cdk_backup_plan": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.49.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.82.0, <2.0.0",
+        "jsii>=1.83.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-backup-plan-0.0.6/src/cdk_backup_plan/__init__.py` & `cdk-backup-plan-0.0.7/src/cdk_backup_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-backup-plan-0.0.6/src/cdk_backup_plan.egg-info/PKG-INFO` & `cdk-backup-plan-0.0.7/src/cdk_backup_plan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-backup-plan
-Version: 0.0.6
+Version: 0.0.7
 Summary: CDK construct to create AWS Backup Plans
 Home-page: https://github.com/aws-samples/cdk-backup-plan.git
 Author: Mauricio Villaescusa<maurovc@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/cdk-backup-plan.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

