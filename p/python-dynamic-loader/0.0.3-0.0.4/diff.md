# Comparing `tmp/python-dynamic-loader-0.0.3.tar.gz` & `tmp/python-dynamic-loader-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dynamic-loader-0.0.3.tar", last modified: Wed Jun 14 19:09:42 2023, max compression
+gzip compressed data, was "python-dynamic-loader-0.0.4.tar", last modified: Wed Jun 14 21:09:12 2023, max compression
```

## Comparing `python-dynamic-loader-0.0.3.tar` & `python-dynamic-loader-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-14 19:09:42.591386 python-dynamic-loader-0.0.3/
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)    11357 2023-05-18 14:13:32.000000 python-dynamic-loader-0.0.3/LICENSE
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      576 2023-06-14 19:09:42.591386 python-dynamic-loader-0.0.3/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       24 2023-06-05 15:59:56.000000 python-dynamic-loader-0.0.3/README.md
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-14 19:09:42.591386 python-dynamic-loader-0.0.3/dynamic/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      874 2023-05-16 16:01:08.000000 python-dynamic-loader-0.0.3/dynamic/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4797 2023-06-14 19:03:19.000000 python-dynamic-loader-0.0.3/dynamic/dynamic_loader.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3582 2023-06-14 19:07:30.000000 python-dynamic-loader-0.0.3/dynamic/source_grabbers.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      732 2023-06-14 19:08:24.000000 python-dynamic-loader-0.0.3/pyproject.toml
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-14 19:09:42.591386 python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      576 2023-06-14 19:09:42.000000 python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      329 2023-06-14 19:09:42.000000 python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/SOURCES.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-14 19:09:42.000000 python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/dependency_links.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       63 2023-06-14 19:09:42.000000 python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/requires.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        8 2023-06-14 19:09:42.000000 python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/top_level.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-14 19:09:42.591386 python-dynamic-loader-0.0.3/setup.cfg
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-14 21:09:12.686746 python-dynamic-loader-0.0.4/
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)    11357 2023-05-18 14:13:32.000000 python-dynamic-loader-0.0.4/LICENSE
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      576 2023-06-14 21:09:12.686746 python-dynamic-loader-0.0.4/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       24 2023-06-05 15:59:56.000000 python-dynamic-loader-0.0.4/README.md
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-14 21:09:12.682746 python-dynamic-loader-0.0.4/dynamic/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      874 2023-05-16 16:01:08.000000 python-dynamic-loader-0.0.4/dynamic/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4825 2023-06-14 21:04:51.000000 python-dynamic-loader-0.0.4/dynamic/dynamic_loader.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3658 2023-06-14 21:05:47.000000 python-dynamic-loader-0.0.4/dynamic/source_grabbers.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      732 2023-06-14 21:08:53.000000 python-dynamic-loader-0.0.4/pyproject.toml
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-14 21:09:12.686746 python-dynamic-loader-0.0.4/python_dynamic_loader.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      576 2023-06-14 21:09:12.000000 python-dynamic-loader-0.0.4/python_dynamic_loader.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      329 2023-06-14 21:09:12.000000 python-dynamic-loader-0.0.4/python_dynamic_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-14 21:09:12.000000 python-dynamic-loader-0.0.4/python_dynamic_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       63 2023-06-14 21:09:12.000000 python-dynamic-loader-0.0.4/python_dynamic_loader.egg-info/requires.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        8 2023-06-14 21:09:12.000000 python-dynamic-loader-0.0.4/python_dynamic_loader.egg-info/top_level.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-14 21:09:12.686746 python-dynamic-loader-0.0.4/setup.cfg
```

### Comparing `python-dynamic-loader-0.0.3/LICENSE` & `python-dynamic-loader-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-dynamic-loader-0.0.3/PKG-INFO` & `python-dynamic-loader-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dynamic-loader
-Version: 0.0.3
+Version: 0.0.4
 Summary: API for dynamically loading Python classes from Google Cloud Storage or Secret Manager.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `python-dynamic-loader-0.0.3/dynamic/__init__.py` & `python-dynamic-loader-0.0.4/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dynamic-loader-0.0.3/dynamic/dynamic_loader.py` & `python-dynamic-loader-0.0.4/dynamic/dynamic_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,29 +103,30 @@
   In order to be loaded by the DynamicClass mechanism, all/any classes
   MUST extend this class and implement the 'run' method.
   """
   TDatastore = TypeVar('TDatastore', bound=SourceGrabber)
 
   def install(module_name: str,
               class_name: str = 'Class',
-              storage: Type[TDatastore] = CloudStorage) -> DynamicClass:
+              storage: Type[TDatastore] = CloudStorage,
+              **args) -> DynamicClass:
     """Inserts the finder into the import machinery.
 
     *** THIS METHOD SHOULD NOT BE OVERRIDDEN ***
 
     Args:
         module_name (str): the name of the module
         class_name (str, optional): the name of the loaded class.
                                     Defaults to 'Class'.
         storage (Type[TDatastore]): the StorageGrabber class to use
 
     Returns:
         DynamicClass: the new Class
     """
-    datastore = storage()
+    datastore = storage(**args)
     sys.meta_path.append(DynamicClassFinder(datastore))
     _module = f'classes.dynamic.{module_name}'
 
     if _module in sys.modules:
       module = sys.modules[_module]
       module = reload(module)
```

### Comparing `python-dynamic-loader-0.0.3/dynamic/source_grabbers.py` & `python-dynamic-loader-0.0.4/dynamic/source_grabbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
   def bucket(self) -> str:
     return self._bucket
 
   @bucket.setter
   def bucket(self, bucket: str=None) -> None:
     self._bucket = bucket
 
-  def __init__(self, bucket: str) -> CloudStorage:
+  def __init__(self, bucket: str, **unused) -> CloudStorage:
     self.bucket = f'{self.project}-{bucket or "dynamic-commands"}'
 
   def fetch_source(self, source: str, **unused: Any) -> str:
     """Fetches the source from the Google Cloud Storage.
 
     The cloud function's implicit credentials are used for this operation.
     Any args other than the two listed will be ignored.
@@ -85,14 +85,17 @@
 
     return content
 
 
 class SecretManager(SourceGrabber):
   """Secret Manager SourceGrabber"""
 
+  def __init__(self, **unused) -> SecretManager:
+    return self
+
   def fetch_source(self, source: str, **unused: Any) -> str:
     """Fetches the source from the Google Cloud Storage.
 
     The cloud function's implicit credentials are used for this operation.
     Any args other than the one listed will be ignored.
 
     Args:
```

### Comparing `python-dynamic-loader-0.0.3/pyproject.toml` & `python-dynamic-loader-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "python-dynamic-loader"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="David Harcombe", email="david.harcombe@gmail.com" },
 ]
 description = "API for dynamically loading Python classes from Google Cloud Storage or Secret Manager."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/PKG-INFO` & `python-dynamic-loader-0.0.4/python_dynamic_loader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dynamic-loader
-Version: 0.0.3
+Version: 0.0.4
 Summary: API for dynamically loading Python classes from Google Cloud Storage or Secret Manager.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

