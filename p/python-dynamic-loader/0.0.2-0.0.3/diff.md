# Comparing `tmp/python-dynamic-loader-0.0.2.tar.gz` & `tmp/python-dynamic-loader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dynamic-loader-0.0.2.tar", last modified: Wed Jun 14 18:49:56 2023, max compression
+gzip compressed data, was "python-dynamic-loader-0.0.3.tar", last modified: Wed Jun 14 19:09:42 2023, max compression
```

## Comparing `python-dynamic-loader-0.0.2.tar` & `python-dynamic-loader-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-14 18:49:56.217576 python-dynamic-loader-0.0.2/
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)    11357 2023-05-18 14:13:32.000000 python-dynamic-loader-0.0.2/LICENSE
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      576 2023-06-14 18:49:56.217576 python-dynamic-loader-0.0.2/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       24 2023-06-05 15:59:56.000000 python-dynamic-loader-0.0.2/README.md
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-14 18:49:56.217576 python-dynamic-loader-0.0.2/dynamic/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      874 2023-05-16 16:01:08.000000 python-dynamic-loader-0.0.2/dynamic/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4949 2023-06-05 15:56:25.000000 python-dynamic-loader-0.0.2/dynamic/dynamic_loader.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3299 2023-05-18 14:10:46.000000 python-dynamic-loader-0.0.2/dynamic/source_grabbers.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      732 2023-06-14 18:48:44.000000 python-dynamic-loader-0.0.2/pyproject.toml
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-14 18:49:56.217576 python-dynamic-loader-0.0.2/python_dynamic_loader.egg-info/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      576 2023-06-14 18:49:56.000000 python-dynamic-loader-0.0.2/python_dynamic_loader.egg-info/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      329 2023-06-14 18:49:56.000000 python-dynamic-loader-0.0.2/python_dynamic_loader.egg-info/SOURCES.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-14 18:49:56.000000 python-dynamic-loader-0.0.2/python_dynamic_loader.egg-info/dependency_links.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       63 2023-06-14 18:49:56.000000 python-dynamic-loader-0.0.2/python_dynamic_loader.egg-info/requires.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        8 2023-06-14 18:49:56.000000 python-dynamic-loader-0.0.2/python_dynamic_loader.egg-info/top_level.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-14 18:49:56.217576 python-dynamic-loader-0.0.2/setup.cfg
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-14 19:09:42.591386 python-dynamic-loader-0.0.3/
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)    11357 2023-05-18 14:13:32.000000 python-dynamic-loader-0.0.3/LICENSE
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      576 2023-06-14 19:09:42.591386 python-dynamic-loader-0.0.3/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       24 2023-06-05 15:59:56.000000 python-dynamic-loader-0.0.3/README.md
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-14 19:09:42.591386 python-dynamic-loader-0.0.3/dynamic/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      874 2023-05-16 16:01:08.000000 python-dynamic-loader-0.0.3/dynamic/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4797 2023-06-14 19:03:19.000000 python-dynamic-loader-0.0.3/dynamic/dynamic_loader.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3582 2023-06-14 19:07:30.000000 python-dynamic-loader-0.0.3/dynamic/source_grabbers.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      732 2023-06-14 19:08:24.000000 python-dynamic-loader-0.0.3/pyproject.toml
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-14 19:09:42.591386 python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      576 2023-06-14 19:09:42.000000 python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      329 2023-06-14 19:09:42.000000 python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-14 19:09:42.000000 python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       63 2023-06-14 19:09:42.000000 python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/requires.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        8 2023-06-14 19:09:42.000000 python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/top_level.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-14 19:09:42.591386 python-dynamic-loader-0.0.3/setup.cfg
```

### Comparing `python-dynamic-loader-0.0.2/LICENSE` & `python-dynamic-loader-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-dynamic-loader-0.0.2/PKG-INFO` & `python-dynamic-loader-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dynamic-loader
-Version: 0.0.2
+Version: 0.0.3
 Summary: API for dynamically loading Python classes from Google Cloud Storage or Secret Manager.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `python-dynamic-loader-0.0.2/dynamic/__init__.py` & `python-dynamic-loader-0.0.3/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dynamic-loader-0.0.2/dynamic/dynamic_loader.py` & `python-dynamic-loader-0.0.3/dynamic/dynamic_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 class DynamicClassLoader(abc.Loader):
   """Load a DynamicClass
 
   Load an arbitrary DynamicClass subclass into the Python class library
   dynamically. The location to check is hardwired here for security
   reasons.
   """
+  storage: SourceGrabber = None
 
   def __init__(self, storage: SourceGrabber) -> None:
     self.storage = storage
 
   def exec_module(self, module: types.ModuleType):
     """Read the code from GCS and execute (load) it.
 
@@ -83,19 +84,16 @@
       # of the fully qualified name.
       filename = module.__name__.split('.')[-1]
 
       # Fetch the code here as string.
       # GCS? BQ? Firestore? Secret Manager? All good options - but for this
       # purpose we're hardcoding a specific GCS bucket. More, we're not passing
       # any credentials so it will be accessed as the service account.
-      bucket = f'{os.environ.get("GOOGLE_CLOUD_PROJECT")}-dynamic-commands'
       source = f'{filename}.py'
-      code = self.storage.fetch_source(bucket=bucket,
-                                       file=source,
-                                       secret=filename)
+      code = self.storage.fetch_source(source=source)
 
       exec(code, vars(module))
 
     except:
       raise ModuleNotFoundError()
```

### Comparing `python-dynamic-loader-0.0.2/dynamic/source_grabbers.py` & `python-dynamic-loader-0.0.3/dynamic/source_grabbers.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,31 +32,41 @@
        environment.
 
     Returns:
         str: GCP name
     """
     return os.environ.get('GOOGLE_CLOUD_PROJECT') or os.environ.get('GCP_PROJECT')
 
-  def fetch_source(self, **kwargs: Mapping[str, Any]) -> str:
+  def fetch_source(self, source: str, **kwargs: Mapping[str, Any]) -> str:
     """Fetches the source from the datastore.
 
     All source should be returned as a string. It is required that the grabber
     perform this conversion as the remainder of the dynamic process will expect
     source in the form of a string, not bytes.
 
     Returns:
         str: the source as a string.
     """
     pass
 
 
 class CloudStorage(SourceGrabber):
   """Cloud Storage SourceGrabber"""
+  @property
+  def bucket(self) -> str:
+    return self._bucket
+
+  @bucket.setter
+  def bucket(self, bucket: str=None) -> None:
+    self._bucket = bucket
 
-  def fetch_source(self, bucket: str, file: str, **unused: Any) -> str:
+  def __init__(self, bucket: str) -> CloudStorage:
+    self.bucket = f'{self.project}-{bucket or "dynamic-commands"}'
+
+  def fetch_source(self, source: str, **unused: Any) -> str:
     """Fetches the source from the Google Cloud Storage.
 
     The cloud function's implicit credentials are used for this operation.
     Any args other than the two listed will be ignored.
 
     Args:
         bucket (str): the bucket containing the dynamic source
@@ -64,26 +74,26 @@
 
     Returns:
         str: the source
     """
     client = storage.Client()
 
     try:
-      content = client.get_bucket(bucket).blob(file).download_as_text()
+      content = client.get_bucket(self.bucket).blob(source).download_as_text()
     except Exception as ex:
       content = None
-      logging.error('Error fetching file %s\n%s', file, ex)
+      logging.error('Error fetching file %s\n%s', source, ex)
 
     return content
 
 
 class SecretManager(SourceGrabber):
   """Secret Manager SourceGrabber"""
 
-  def fetch_source(self, secret: str, **unused: Any) -> str:
+  def fetch_source(self, source: str, **unused: Any) -> str:
     """Fetches the source from the Google Cloud Storage.
 
     The cloud function's implicit credentials are used for this operation.
     Any args other than the one listed will be ignored.
 
     Args:
         secret (str): the name of the secret to fetch
@@ -91,17 +101,17 @@
     Returns:
         str: the source
     """
     client = secretmanager.SecretManagerServiceClient()
 
     try:
       secret_name = client.secret_version_path(project=self.project,
-                                               secret=secret,
+                                               secret=source,
                                                secret_version='latest')
       request = secretmanager_v1.AccessSecretVersionRequest(name=secret_name)
       response = client.access_secret_version(request=request)
       content = response.payload.data.decode(encoding='utf-8')
     except Exception as e:
       content = None
-      logging.error('Error fetching secret %s\n%s', secret, e)
+      logging.error('Error fetching secret %s\n%s', source, e)
 
     return content
```

### Comparing `python-dynamic-loader-0.0.2/pyproject.toml` & `python-dynamic-loader-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "python-dynamic-loader"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="David Harcombe", email="david.harcombe@gmail.com" },
 ]
 description = "API for dynamically loading Python classes from Google Cloud Storage or Secret Manager."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python-dynamic-loader-0.0.2/python_dynamic_loader.egg-info/PKG-INFO` & `python-dynamic-loader-0.0.3/python_dynamic_loader.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dynamic-loader
-Version: 0.0.2
+Version: 0.0.3
 Summary: API for dynamically loading Python classes from Google Cloud Storage or Secret Manager.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

