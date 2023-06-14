# Comparing `tmp/cdktf-cdk8s-0.5.8.tar.gz` & `tmp/cdktf-cdk8s-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdk8s-0.5.8.tar", last modified: Tue May 23 08:27:09 2023, max compression
+gzip compressed data, was "cdktf-cdk8s-0.5.9.tar", last modified: Tue May 23 16:12:03 2023, max compression
```

## Comparing `cdktf-cdk8s-0.5.8.tar` & `cdktf-cdk8s-0.5.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:27:09.637307 cdktf-cdk8s-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-23 08:26:57.000000 cdktf-cdk8s-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 08:26:57.000000 cdktf-cdk8s-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-23 08:27:09.637307 cdktf-cdk8s-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-23 08:26:57.000000 cdktf-cdk8s-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-23 08:26:57.000000 cdktf-cdk8s-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 08:27:09.637307 cdktf-cdk8s-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-23 08:26:57.000000 cdktf-cdk8s-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:27:09.633307 cdktf-cdk8s-0.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:27:09.637307 cdktf-cdk8s-0.5.8/src/cdktf_cdk8s/
--rw-r--r--   0 runner    (1001) docker     (123)    34263 2023-05-23 08:26:57.000000 cdktf-cdk8s-0.5.8/src/cdktf_cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:27:09.637307 cdktf-cdk8s-0.5.8/src/cdktf_cdk8s/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-23 08:26:57.000000 cdktf-cdk8s-0.5.8/src/cdktf_cdk8s/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   360064 2023-05-23 08:26:57.000000 cdktf-cdk8s-0.5.8/src/cdktf_cdk8s/_jsii/cdktf-cdk8s@0.5.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:26:57.000000 cdktf-cdk8s-0.5.8/src/cdktf_cdk8s/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:27:09.637307 cdktf-cdk8s-0.5.8/src/cdktf_cdk8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-23 08:27:09.000000 cdktf-cdk8s-0.5.8/src/cdktf_cdk8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-23 08:27:09.000000 cdktf-cdk8s-0.5.8/src/cdktf_cdk8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:27:09.000000 cdktf-cdk8s-0.5.8/src/cdktf_cdk8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-23 08:27:09.000000 cdktf-cdk8s-0.5.8/src/cdktf_cdk8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 08:27:09.000000 cdktf-cdk8s-0.5.8/src/cdktf_cdk8s.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:12:03.423100 cdktf-cdk8s-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-23 16:11:50.000000 cdktf-cdk8s-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 16:11:50.000000 cdktf-cdk8s-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-23 16:12:03.423100 cdktf-cdk8s-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-23 16:11:50.000000 cdktf-cdk8s-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-23 16:11:50.000000 cdktf-cdk8s-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 16:12:03.423100 cdktf-cdk8s-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-23 16:11:50.000000 cdktf-cdk8s-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:12:03.419100 cdktf-cdk8s-0.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:12:03.419100 cdktf-cdk8s-0.5.9/src/cdktf_cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (123)    34263 2023-05-23 16:11:50.000000 cdktf-cdk8s-0.5.9/src/cdktf_cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:12:03.423100 cdktf-cdk8s-0.5.9/src/cdktf_cdk8s/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-23 16:11:50.000000 cdktf-cdk8s-0.5.9/src/cdktf_cdk8s/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   360063 2023-05-23 16:11:50.000000 cdktf-cdk8s-0.5.9/src/cdktf_cdk8s/_jsii/cdktf-cdk8s@0.5.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:11:50.000000 cdktf-cdk8s-0.5.9/src/cdktf_cdk8s/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:12:03.423100 cdktf-cdk8s-0.5.9/src/cdktf_cdk8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-23 16:12:03.000000 cdktf-cdk8s-0.5.9/src/cdktf_cdk8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-23 16:12:03.000000 cdktf-cdk8s-0.5.9/src/cdktf_cdk8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:12:03.000000 cdktf-cdk8s-0.5.9/src/cdktf_cdk8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-23 16:12:03.000000 cdktf-cdk8s-0.5.9/src/cdktf_cdk8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 16:12:03.000000 cdktf-cdk8s-0.5.9/src/cdktf_cdk8s.egg-info/top_level.txt
```

### Comparing `cdktf-cdk8s-0.5.8/LICENSE` & `cdktf-cdk8s-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdk8s-0.5.8/PKG-INFO` & `cdktf-cdk8s-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdk8s
-Version: 0.5.8
+Version: 0.5.9
 Summary: A compatibility layer for using cdk8s constructs within Terraform CDK.
 Home-page: https://github.com/cdktf/cdktf-cdk8s.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-cdk8s.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdk8s-0.5.8/README.md` & `cdktf-cdk8s-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdk8s-0.5.8/setup.py` & `cdktf-cdk8s-0.5.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdk8s",
-    "version": "0.5.8",
+    "version": "0.5.9",
     "description": "A compatibility layer for using cdk8s constructs within Terraform CDK.",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-cdk8s.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -22,27 +22,27 @@
     },
     "packages": [
         "cdktf_cdk8s",
         "cdktf_cdk8s._jsii"
     ],
     "package_data": {
         "cdktf_cdk8s._jsii": [
-            "cdktf-cdk8s@0.5.8.jsii.tgz"
+            "cdktf-cdk8s@0.5.9.jsii.tgz"
         ],
         "cdktf_cdk8s": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdk8s>=2.1.6",
         "cdktf-cdktf-provider-kubernetes>=6.0.0",
         "cdktf>=0.16.0",
         "constructs>=10.0.25, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdk8s-0.5.8/src/cdktf_cdk8s/__init__.py` & `cdktf-cdk8s-0.5.9/src/cdktf_cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdk8s-0.5.8/src/cdktf_cdk8s.egg-info/PKG-INFO` & `cdktf-cdk8s-0.5.9/src/cdktf_cdk8s.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdk8s
-Version: 0.5.8
+Version: 0.5.9
 Summary: A compatibility layer for using cdk8s constructs within Terraform CDK.
 Home-page: https://github.com/cdktf/cdktf-cdk8s.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-cdk8s.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

