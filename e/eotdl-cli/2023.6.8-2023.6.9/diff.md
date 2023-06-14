# Comparing `tmp/eotdl-cli-2023.6.8.tar.gz` & `tmp/eotdl-cli-2023.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-cli-2023.6.8.tar", max compression
+gzip compressed data, was "eotdl-cli-2023.6.9.tar", max compression
```

## Comparing `eotdl-cli-2023.6.8.tar` & `eotdl-cli-2023.6.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl-cli-2023.6.8/README.md
--rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl-cli-2023.6.8/eotdl_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.6.8/eotdl_cli/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-04-26 16:16:15.561454 eotdl-cli-2023.6.8/eotdl_cli/commands/auth.py
--rw-r--r--   0        0        0     1598 2023-05-23 12:10:19.220001 eotdl-cli-2023.6.8/eotdl_cli/commands/datasets.py
--rw-r--r--   0        0        0      367 2023-05-23 10:31:57.663189 eotdl-cli-2023.6.8/eotdl_cli/main.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.6.8/eotdl_cli/src/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.6.8/eotdl_cli/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl-cli-2023.6.8/eotdl_cli/src/errors/auth.py
--rw-r--r--   0        0        0     9594 2023-06-08 14:47:32.367190 eotdl-cli-2023.6.8/eotdl_cli/src/repos/APIRepo.py
--rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl-cli-2023.6.8/eotdl_cli/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.8/eotdl_cli/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/main.py
--rw-r--r--   0        0        0      763 2023-05-23 12:06:36.471211 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      932 2023-05-09 15:05:12.940722 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0     1375 2023-06-08 14:44:02.846956 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py
--rw-r--r--   0        0        0      927 2023-05-16 10:10:52.296818 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py
--rw-r--r--   0        0        0      421 2023-05-09 15:05:12.940722 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0      940 2023-05-23 11:36:06.764258 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/UpdateDataset.py
--rw-r--r--   0        0        0      168 2023-05-16 10:10:52.296818 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0     2168 2023-05-23 12:06:38.803219 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/main.py
--rw-r--r--   0        0        0      235 2023-05-23 11:05:01.073388 eotdl-cli-2023.6.8/eotdl_cli/src/utils.py
--rw-r--r--   0        0        0      601 2023-06-08 15:06:34.445545 eotdl-cli-2023.6.8/pyproject.toml
--rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 eotdl-cli-2023.6.8/setup.py
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 eotdl-cli-2023.6.8/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl-cli-2023.6.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl-cli-2023.6.9/eotdl_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.6.9/eotdl_cli/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-04-26 16:16:15.561454 eotdl-cli-2023.6.9/eotdl_cli/commands/auth.py
+-rw-r--r--   0        0        0     1598 2023-05-23 12:10:19.220001 eotdl-cli-2023.6.9/eotdl_cli/commands/datasets.py
+-rw-r--r--   0        0        0      367 2023-05-23 10:31:57.663189 eotdl-cli-2023.6.9/eotdl_cli/main.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.6.9/eotdl_cli/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.6.9/eotdl_cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl-cli-2023.6.9/eotdl_cli/src/errors/auth.py
+-rw-r--r--   0        0        0     9596 2023-06-09 06:38:04.673056 eotdl-cli-2023.6.9/eotdl_cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl-cli-2023.6.9/eotdl_cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.9/eotdl_cli/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      763 2023-05-23 12:06:36.471211 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      932 2023-05-09 15:05:12.940722 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0     1376 2023-06-09 06:39:04.149380 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py
+-rw-r--r--   0        0        0      927 2023-05-16 10:10:52.296818 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py
+-rw-r--r--   0        0        0      421 2023-05-09 15:05:12.940722 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0      940 2023-05-23 11:36:06.764258 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/UpdateDataset.py
+-rw-r--r--   0        0        0      168 2023-05-16 10:10:52.296818 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0     2168 2023-05-23 12:06:38.803219 eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/main.py
+-rw-r--r--   0        0        0      235 2023-05-23 11:05:01.073388 eotdl-cli-2023.6.9/eotdl_cli/src/utils.py
+-rw-r--r--   0        0        0      601 2023-06-09 06:39:18.857458 eotdl-cli-2023.6.9/pyproject.toml
+-rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 eotdl-cli-2023.6.9/setup.py
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 eotdl-cli-2023.6.9/PKG-INFO
```

### Comparing `eotdl-cli-2023.6.8/eotdl_cli/commands/auth.py` & `eotdl-cli-2023.6.9/eotdl_cli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.6.8/eotdl_cli/commands/datasets.py` & `eotdl-cli-2023.6.9/eotdl_cli/commands/datasets.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.6.8/eotdl_cli/src/repos/APIRepo.py` & `eotdl-cli-2023.6.9/eotdl_cli/src/repos/APIRepo.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             return None, response.json()["detail"]
         data = response.json()
         _, upload_id, parts = data["dataset_id"], data["upload_id"], data["parts"]
         # assert dataset_id is None
         content_path = os.path.abspath(path)
         content_size = os.stat(content_path).st_size
         url = self.url + "datasets/chunk"
-        chunk_size = 1024 * 1024 * 10  # 10 MiB
+        chunk_size = 1024 * 1024 * 100  # 100 MiB
         total_chunks = content_size // chunk_size
         headers = {
             "Authorization": "Bearer " + id_token,
             "Upload-Id": upload_id,
             "Dataset-Id": dataset_id,
         }
         # upload chunks sequentially
```

### Comparing `eotdl-cli-2023.6.8/eotdl_cli/src/repos/AuthRepo.py` & `eotdl-cli-2023.6.9/eotdl_cli/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/Auth.py` & `eotdl-cli-2023.6.9/eotdl_cli/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/main.py` & `eotdl-cli-2023.6.9/eotdl_cli/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/DownloadDataset.py` & `eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/DownloadDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/IngestDataset.py` & `eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/IngestDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py` & `eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.logger(checksum)
         self.logger("Ingesting dataset...")
         id_token = inputs.user["id_token"]
         dataset_id, upload_id, parts = self.repo.prepare_large_upload(
             inputs.name, id_token, checksum
         )
         self.repo.ingest_large_dataset(
-            inputs.path, 1024 * 1024 * 10, upload_id, dataset_id, id_token, parts
+            inputs.path, 1024 * 1024 * 100, upload_id, dataset_id, id_token, parts
         )
         data, error = self.repo.complete_upload(
             inputs.name, id_token, upload_id, dataset_id, checksum
         )
         if error:
             raise Exception(error)
         self.logger("Done")
```

### Comparing `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py` & `eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/UpdateDataset.py` & `eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/UpdateDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/main.py` & `eotdl-cli-2023.6.9/eotdl_cli/src/usecases/datasets/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.6.8/pyproject.toml` & `eotdl-cli-2023.6.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl-cli"
-version = "2023.06.08"
+version = "2023.06.09"
 description = ""
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl_cli"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl-cli-2023.6.8/setup.py` & `eotdl-cli-2023.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['eotdl-cli = eotdl_cli.main:app']}
 
 setup_kwargs = {
     'name': 'eotdl-cli',
-    'version': '2023.6.8',
+    'version': '2023.6.9',
     'description': '',
     'long_description': '# eotdl-cli\n\nThis is the CLI for EOTDL.\n\n',
     'author': 'EarthPulse',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `eotdl-cli-2023.6.8/PKG-INFO` & `eotdl-cli-2023.6.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl-cli
-Version: 2023.6.8
+Version: 2023.6.9
 Summary: 
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

