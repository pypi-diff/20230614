# Comparing `tmp/pepperize.cdk-ses-smtp-credentials-0.3.358.tar.gz` & `tmp/pepperize.cdk-ses-smtp-credentials-0.3.359.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperize.cdk-ses-smtp-credentials-0.3.358.tar", last modified: Mon Jun 12 23:09:59 2023, max compression
+gzip compressed data, was "pepperize.cdk-ses-smtp-credentials-0.3.359.tar", last modified: Mon Jun 12 23:16:10 2023, max compression
```

## Comparing `pepperize.cdk-ses-smtp-credentials-0.3.358.tar` & `pepperize.cdk-ses-smtp-credentials-0.3.359.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:09:59.918662 pepperize.cdk-ses-smtp-credentials-0.3.358/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-12 23:09:48.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 23:09:48.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-12 23:09:59.918662 pepperize.cdk-ses-smtp-credentials-0.3.358/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-06-12 23:09:48.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 23:09:48.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 23:09:59.922662 pepperize.cdk-ses-smtp-credentials-0.3.358/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-12 23:09:48.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:09:59.918662 pepperize.cdk-ses-smtp-credentials-0.3.358/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:09:59.918662 pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize.cdk_ses_smtp_credentials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-12 23:09:59.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize.cdk_ses_smtp_credentials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-12 23:09:59.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize.cdk_ses_smtp_credentials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 23:09:59.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize.cdk_ses_smtp_credentials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 23:09:59.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize.cdk_ses_smtp_credentials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 23:09:59.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize.cdk_ses_smtp_credentials.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:09:59.918662 pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize_cdk_ses_smtp_credentials/
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-06-12 23:09:48.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize_cdk_ses_smtp_credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:09:59.918662 pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize_cdk_ses_smtp_credentials/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-12 23:09:48.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize_cdk_ses_smtp_credentials/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31026 2023-06-12 23:09:48.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize_cdk_ses_smtp_credentials/_jsii/cdk-ses-smtp-credentials@0.3.358.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 23:09:48.000000 pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize_cdk_ses_smtp_credentials/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:16:10.127142 pepperize.cdk-ses-smtp-credentials-0.3.359/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-12 23:15:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 23:15:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-12 23:16:10.127142 pepperize.cdk-ses-smtp-credentials-0.3.359/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-06-12 23:15:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 23:15:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 23:16:10.127142 pepperize.cdk-ses-smtp-credentials-0.3.359/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-12 23:15:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:16:10.127142 pepperize.cdk-ses-smtp-credentials-0.3.359/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:16:10.127142 pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize.cdk_ses_smtp_credentials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-12 23:16:10.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize.cdk_ses_smtp_credentials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-12 23:16:10.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize.cdk_ses_smtp_credentials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 23:16:10.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize.cdk_ses_smtp_credentials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 23:16:10.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize.cdk_ses_smtp_credentials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 23:16:10.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize.cdk_ses_smtp_credentials.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:16:10.127142 pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize_cdk_ses_smtp_credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-06-12 23:15:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize_cdk_ses_smtp_credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:16:10.127142 pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize_cdk_ses_smtp_credentials/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-12 23:15:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize_cdk_ses_smtp_credentials/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31024 2023-06-12 23:15:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize_cdk_ses_smtp_credentials/_jsii/cdk-ses-smtp-credentials@0.3.359.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 23:15:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize_cdk_ses_smtp_credentials/py.typed
```

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.358/LICENSE` & `pepperize.cdk-ses-smtp-credentials-0.3.359/LICENSE`

 * *Files identical despite different names*

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.358/PKG-INFO` & `pepperize.cdk-ses-smtp-credentials-0.3.359/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepperize.cdk-ses-smtp-credentials
-Version: 0.3.358
+Version: 0.3.359
 Summary: Generate SES smtp credentials for a given user and store the credentials in a SecretsManager Secret.
 Home-page: https://github.com/pepperize/cdk-ses-smtp-credentials.git
 Author: Patrick Florek<patrick.florek@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/pepperize/cdk-ses-smtp-credentials.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.358/README.md` & `pepperize.cdk-ses-smtp-credentials-0.3.359/README.md`

 * *Files identical despite different names*

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.358/setup.py` & `pepperize.cdk-ses-smtp-credentials-0.3.359/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "pepperize.cdk-ses-smtp-credentials",
-    "version": "0.3.358",
+    "version": "0.3.359",
     "description": "Generate SES smtp credentials for a given user and store the credentials in a SecretsManager Secret.",
     "license": "MIT",
     "url": "https://github.com/pepperize/cdk-ses-smtp-credentials.git",
     "long_description_content_type": "text/markdown",
     "author": "Patrick Florek<patrick.florek@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "pepperize_cdk_ses_smtp_credentials",
         "pepperize_cdk_ses_smtp_credentials._jsii"
     ],
     "package_data": {
         "pepperize_cdk_ses_smtp_credentials._jsii": [
-            "cdk-ses-smtp-credentials@0.3.358.jsii.tgz"
+            "cdk-ses-smtp-credentials@0.3.359.jsii.tgz"
         ],
         "pepperize_cdk_ses_smtp_credentials": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize.cdk_ses_smtp_credentials.egg-info/PKG-INFO` & `pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize.cdk_ses_smtp_credentials.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepperize.cdk-ses-smtp-credentials
-Version: 0.3.358
+Version: 0.3.359
 Summary: Generate SES smtp credentials for a given user and store the credentials in a SecretsManager Secret.
 Home-page: https://github.com/pepperize/cdk-ses-smtp-credentials.git
 Author: Patrick Florek<patrick.florek@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/pepperize/cdk-ses-smtp-credentials.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize.cdk_ses_smtp_credentials.egg-info/SOURCES.txt` & `pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize.cdk_ses_smtp_credentials.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/pepperize.cdk_ses_smtp_credentials.egg-info/SOURCES.txt
 src/pepperize.cdk_ses_smtp_credentials.egg-info/dependency_links.txt
 src/pepperize.cdk_ses_smtp_credentials.egg-info/requires.txt
 src/pepperize.cdk_ses_smtp_credentials.egg-info/top_level.txt
 src/pepperize_cdk_ses_smtp_credentials/__init__.py
 src/pepperize_cdk_ses_smtp_credentials/py.typed
 src/pepperize_cdk_ses_smtp_credentials/_jsii/__init__.py
-src/pepperize_cdk_ses_smtp_credentials/_jsii/cdk-ses-smtp-credentials@0.3.358.jsii.tgz
+src/pepperize_cdk_ses_smtp_credentials/_jsii/cdk-ses-smtp-credentials@0.3.359.jsii.tgz
```

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.358/src/pepperize_cdk_ses_smtp_credentials/__init__.py` & `pepperize.cdk-ses-smtp-credentials-0.3.359/src/pepperize_cdk_ses_smtp_credentials/__init__.py`

 * *Files identical despite different names*

