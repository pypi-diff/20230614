# Comparing `tmp/mobio-notify-sdk-test-1.0.8.tar.gz` & `tmp/mobio-notify-sdk-test-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-notify-sdk-test-1.0.8.tar", last modified: Wed Aug 24 01:51:48 2022, max compression
+gzip compressed data, was "mobio-notify-sdk-test-1.0.9.tar", last modified: Fri Aug 26 08:15:52 2022, max compression
```

## Comparing `mobio-notify-sdk-test-1.0.8.tar` & `mobio-notify-sdk-test-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-24 01:51:48.405974 mobio-notify-sdk-test-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    14316 2022-08-24 01:51:48.404974 mobio-notify-sdk-test-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11588 2022-08-24 01:50:40.000000 mobio-notify-sdk-test-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-24 01:51:48.393973 mobio-notify-sdk-test-1.0.8/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-24 01:51:48.393973 mobio-notify-sdk-test-1.0.8/mobio/sdks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-24 01:51:48.399974 mobio-notify-sdk-test-1.0.8/mobio/sdks/notify/
--rw-r--r--   0 root         (0) root         (0)    14184 2022-08-24 01:50:40.000000 mobio-notify-sdk-test-1.0.8/mobio/sdks/notify/__init__.py
--rw-r--r--   0 root         (0) root         (0)      273 2022-08-24 01:50:40.000000 mobio-notify-sdk-test-1.0.8/mobio/sdks/notify/config.py
--rw-r--r--   0 root         (0) root         (0)      471 2022-08-24 01:50:40.000000 mobio-notify-sdk-test-1.0.8/mobio/sdks/notify/constant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-24 01:51:48.403974 mobio-notify-sdk-test-1.0.8/mobio_notify_sdk_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14316 2022-08-24 01:51:48.000000 mobio-notify-sdk-test-1.0.8/mobio_notify_sdk_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      399 2022-08-24 01:51:48.000000 mobio-notify-sdk-test-1.0.8/mobio_notify_sdk_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-24 01:51:48.000000 mobio-notify-sdk-test-1.0.8/mobio_notify_sdk_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-08-24 01:51:48.000000 mobio-notify-sdk-test-1.0.8/mobio_notify_sdk_test.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       35 2022-08-24 01:51:48.000000 mobio-notify-sdk-test-1.0.8/mobio_notify_sdk_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-08-24 01:51:48.000000 mobio-notify-sdk-test-1.0.8/mobio_notify_sdk_test.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      104 2022-08-24 01:50:40.000000 mobio-notify-sdk-test-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-24 01:51:48.405974 mobio-notify-sdk-test-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8850 2022-08-24 01:51:47.000000 mobio-notify-sdk-test-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 08:15:52.803497 mobio-notify-sdk-test-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    14316 2022-08-26 08:15:52.802497 mobio-notify-sdk-test-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11588 2022-08-24 01:50:40.000000 mobio-notify-sdk-test-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 08:15:52.792497 mobio-notify-sdk-test-1.0.9/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 08:15:52.792497 mobio-notify-sdk-test-1.0.9/mobio/sdks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 08:15:52.797497 mobio-notify-sdk-test-1.0.9/mobio/sdks/notify/
+-rw-r--r--   0 root         (0) root         (0)    14184 2022-08-24 01:50:40.000000 mobio-notify-sdk-test-1.0.9/mobio/sdks/notify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      273 2022-08-24 01:50:40.000000 mobio-notify-sdk-test-1.0.9/mobio/sdks/notify/config.py
+-rw-r--r--   0 root         (0) root         (0)      471 2022-08-24 01:50:40.000000 mobio-notify-sdk-test-1.0.9/mobio/sdks/notify/constant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 08:15:52.801497 mobio-notify-sdk-test-1.0.9/mobio_notify_sdk_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14316 2022-08-26 08:15:52.000000 mobio-notify-sdk-test-1.0.9/mobio_notify_sdk_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      399 2022-08-26 08:15:52.000000 mobio-notify-sdk-test-1.0.9/mobio_notify_sdk_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 08:15:52.000000 mobio-notify-sdk-test-1.0.9/mobio_notify_sdk_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2022-08-26 08:15:52.000000 mobio-notify-sdk-test-1.0.9/mobio_notify_sdk_test.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-08-26 08:15:52.000000 mobio-notify-sdk-test-1.0.9/mobio_notify_sdk_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2022-08-26 08:15:52.000000 mobio-notify-sdk-test-1.0.9/mobio_notify_sdk_test.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2022-08-24 01:50:40.000000 mobio-notify-sdk-test-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-26 08:15:52.803497 mobio-notify-sdk-test-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8824 2022-08-26 08:15:52.000000 mobio-notify-sdk-test-1.0.9/setup.py
```

### Comparing `mobio-notify-sdk-test-1.0.8/PKG-INFO` & `mobio-notify-sdk-test-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-notify-sdk-test
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mobio Notify SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: ## Cài đặt thư viện SDK Notify
```

### Comparing `mobio-notify-sdk-test-1.0.8/README.md` & `mobio-notify-sdk-test-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mobio-notify-sdk-test-1.0.8/mobio/sdks/notify/__init__.py` & `mobio-notify-sdk-test-1.0.9/mobio/sdks/notify/__init__.py`

 * *Files identical despite different names*

### Comparing `mobio-notify-sdk-test-1.0.8/mobio_notify_sdk_test.egg-info/PKG-INFO` & `mobio-notify-sdk-test-1.0.9/mobio_notify_sdk_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-notify-sdk-test
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mobio Notify SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: ## Cài đặt thư viện SDK Notify
```

### Comparing `mobio-notify-sdk-test-1.0.8/setup.py` & `mobio-notify-sdk-test-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 
     @staticmethod
     def get():
         """Retrieve all dependencies for this project
         :param filename:
         :return:
         """
-        requirements = ["m-singleton", "confluent_kafka==1.5.0"]
+        requirements = ["m-singleton"]
         return requirements
 
-version_dev='1.0.8'
-version_prod='1.0.6'
+version_dev='1.0.9'
+version_prod='1.0.7'
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -47,15 +47,15 @@
     name="mobio-notify-sdk" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.8',  # Required
+    version='1.0.9',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio Notify SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

