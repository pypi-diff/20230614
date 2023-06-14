# Comparing `tmp/eotdl-2023.6.14.post4.tar.gz` & `tmp/eotdl-2023.6.14.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-2023.6.14.post4.tar", max compression
+gzip compressed data, was "eotdl-2023.6.14.post5.tar", max compression
```

## Comparing `eotdl-2023.6.14.post4.tar` & `eotdl-2023.6.14.post5.tar`

### file list

```diff
@@ -1,52 +1,54 @@
--rw-r--r--   0        0        0       47 2023-03-08 12:48:38.254243 eotdl-2023.6.14.post4/README.md
--rw-r--r--   0        0        0      936 2023-06-14 10:31:27.997185 eotdl-2023.6.14.post4/eotdl/__init__.py
--rw-r--r--   0        0        0      292 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post4/eotdl/access/__init__.py
--rw-r--r--   0        0        0      363 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post4/eotdl/access/parameters.py
--rw-r--r--   0        0        0      252 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post4/eotdl/access/sentinelhub/__init__.py
--rw-r--r--   0        0        0     7605 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post4/eotdl/access/sentinelhub/client.py
--rw-r--r--   0        0        0     6595 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post4/eotdl/access/sentinelhub/utils.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:15.563978 eotdl-2023.6.14.post4/eotdl/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-06-14 10:24:15.567978 eotdl-2023.6.14.post4/eotdl/commands/auth.py
--rw-r--r--   0        0        0     1618 2023-06-14 10:24:15.567978 eotdl-2023.6.14.post4/eotdl/commands/datasets.py
--rw-r--r--   0        0        0      270 2023-06-14 10:33:31.353776 eotdl-2023.6.14.post4/eotdl/curation/__init__.py
--rw-r--r--   0        0        0     2929 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post4/eotdl/curation/formatters.py
--rw-r--r--   0        0        0     1552 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post4/eotdl/curation/metadata.py
--rw-r--r--   0        0        0      201 2023-06-14 09:35:56.383873 eotdl-2023.6.14.post4/eotdl/curation/stac/__init__.py
--rw-r--r--   0        0        0     8495 2023-06-14 10:12:58.941969 eotdl-2023.6.14.post4/eotdl/curation/stac/dataframe.py
--rw-r--r--   0        0        0     5231 2023-06-14 09:10:22.117884 eotdl-2023.6.14.post4/eotdl/curation/stac/extensions.py
--rw-r--r--   0        0        0     1380 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post4/eotdl/curation/stac/parsers.py
--rw-r--r--   0        0        0    17796 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post4/eotdl/curation/stac/stac.py
--rw-r--r--   0        0        0     1855 2023-06-14 09:09:09.621596 eotdl-2023.6.14.post4/eotdl/curation/stac/utils.py
--rw-r--r--   0        0        0        0 2023-06-14 10:19:49.195213 eotdl-2023.6.14.post4/eotdl/datasets/__init__.py
--rw-r--r--   0        0        0       92 2023-06-14 10:23:43.387887 eotdl-2023.6.14.post4/eotdl/datasets/ingest.py
--rw-r--r--   0        0        0       74 2023-04-18 14:58:49.560135 eotdl-2023.6.14.post4/eotdl/hello.py
--rw-r--r--   0        0        0      367 2023-06-14 10:24:27.780013 eotdl-2023.6.14.post4/eotdl/main.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.807993 eotdl-2023.6.14.post4/eotdl/src/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post4/eotdl/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post4/eotdl/src/errors/auth.py
--rw-r--r--   0        0        0     9843 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post4/eotdl/src/repos/APIRepo.py
--rw-r--r--   0        0        0      955 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post4/eotdl/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post4/eotdl/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post4/eotdl/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post4/eotdl/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post4/eotdl/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post4/eotdl/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post4/eotdl/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      725 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post4/eotdl/src/usecases/auth/main.py
--rw-r--r--   0        0        0      763 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      932 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0     1403 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/IngestLargeDataset.py
--rw-r--r--   0        0        0     1595 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py
--rw-r--r--   0        0        0      421 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0      940 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/UpdateDataset.py
--rw-r--r--   0        0        0      168 2023-06-14 10:24:20.823993 eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0     2168 2023-06-14 10:24:20.823993 eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/main.py
--rw-r--r--   0        0        0      479 2023-06-14 10:24:20.823993 eotdl-2023.6.14.post4/eotdl/src/utils.py
--rw-r--r--   0        0        0      277 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post4/eotdl/tools/__init__.py
--rw-r--r--   0        0        0      215 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post4/eotdl/tools/sen12floods/__init__.py
--rw-r--r--   0        0        0     8124 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post4/eotdl/tools/sen12floods/tools.py
--rw-r--r--   0        0        0      636 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post4/eotdl/tools/stac.py
--rw-r--r--   0        0        0      622 2023-06-14 10:33:35.413794 eotdl-2023.6.14.post4/pyproject.toml
--rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 eotdl-2023.6.14.post4/setup.py
--rw-r--r--   0        0        0      737 1970-01-01 00:00:00.000000 eotdl-2023.6.14.post4/PKG-INFO
+-rw-r--r--   0        0        0       47 2023-03-08 12:48:38.254243 eotdl-2023.6.14.post5/README.md
+-rw-r--r--   0        0        0      936 2023-06-14 10:31:27.997185 eotdl-2023.6.14.post5/eotdl/__init__.py
+-rw-r--r--   0        0        0      292 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post5/eotdl/access/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post5/eotdl/access/parameters.py
+-rw-r--r--   0        0        0      252 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post5/eotdl/access/sentinelhub/__init__.py
+-rw-r--r--   0        0        0     7605 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post5/eotdl/access/sentinelhub/client.py
+-rw-r--r--   0        0        0     6595 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post5/eotdl/access/sentinelhub/utils.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:15.563978 eotdl-2023.6.14.post5/eotdl/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-06-14 10:24:15.567978 eotdl-2023.6.14.post5/eotdl/commands/auth.py
+-rw-r--r--   0        0        0     1607 2023-06-14 11:02:17.051684 eotdl-2023.6.14.post5/eotdl/commands/datasets.py
+-rw-r--r--   0        0        0      270 2023-06-14 10:33:31.353776 eotdl-2023.6.14.post5/eotdl/curation/__init__.py
+-rw-r--r--   0        0        0     2929 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post5/eotdl/curation/formatters.py
+-rw-r--r--   0        0        0     1552 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post5/eotdl/curation/metadata.py
+-rw-r--r--   0        0        0      201 2023-06-14 09:35:56.383873 eotdl-2023.6.14.post5/eotdl/curation/stac/__init__.py
+-rw-r--r--   0        0        0     8495 2023-06-14 10:12:58.941969 eotdl-2023.6.14.post5/eotdl/curation/stac/dataframe.py
+-rw-r--r--   0        0        0     5231 2023-06-14 09:10:22.117884 eotdl-2023.6.14.post5/eotdl/curation/stac/extensions.py
+-rw-r--r--   0        0        0     1380 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post5/eotdl/curation/stac/parsers.py
+-rw-r--r--   0        0        0    17796 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post5/eotdl/curation/stac/stac.py
+-rw-r--r--   0        0        0     1855 2023-06-14 09:09:09.621596 eotdl-2023.6.14.post5/eotdl/curation/stac/utils.py
+-rw-r--r--   0        0        0      211 2023-06-14 10:56:55.854708 eotdl-2023.6.14.post5/eotdl/datasets/__init__.py
+-rw-r--r--   0        0        0      525 2023-06-14 11:03:13.187853 eotdl-2023.6.14.post5/eotdl/datasets/download.py
+-rw-r--r--   0        0        0      818 2023-06-14 11:02:58.123808 eotdl-2023.6.14.post5/eotdl/datasets/ingest.py
+-rw-r--r--   0        0        0      542 2023-06-14 11:03:39.503932 eotdl-2023.6.14.post5/eotdl/datasets/retrieve.py
+-rw-r--r--   0        0        0      326 2023-06-14 11:03:47.951958 eotdl-2023.6.14.post5/eotdl/datasets/update.py
+-rw-r--r--   0        0        0       74 2023-04-18 14:58:49.560135 eotdl-2023.6.14.post5/eotdl/hello.py
+-rw-r--r--   0        0        0      359 2023-06-14 11:02:07.315654 eotdl-2023.6.14.post5/eotdl/main.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.807993 eotdl-2023.6.14.post5/eotdl/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post5/eotdl/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post5/eotdl/src/errors/auth.py
+-rw-r--r--   0        0        0     9843 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post5/eotdl/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      955 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post5/eotdl/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post5/eotdl/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post5/eotdl/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post5/eotdl/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post5/eotdl/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post5/eotdl/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post5/eotdl/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post5/eotdl/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      763 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post5/eotdl/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      932 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post5/eotdl/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0     1403 2023-06-14 11:03:29.391902 eotdl-2023.6.14.post5/eotdl/src/usecases/datasets/IngestLargeDataset.py
+-rw-r--r--   0        0        0     1595 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post5/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py
+-rw-r--r--   0        0        0      421 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post5/eotdl/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post5/eotdl/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0      940 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post5/eotdl/src/usecases/datasets/UpdateDataset.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:51:58.909786 eotdl-2023.6.14.post5/eotdl/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0      479 2023-06-14 10:24:20.823993 eotdl-2023.6.14.post5/eotdl/src/utils.py
+-rw-r--r--   0        0        0      277 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post5/eotdl/tools/__init__.py
+-rw-r--r--   0        0        0      215 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post5/eotdl/tools/sen12floods/__init__.py
+-rw-r--r--   0        0        0     8124 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post5/eotdl/tools/sen12floods/tools.py
+-rw-r--r--   0        0        0      636 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post5/eotdl/tools/stac.py
+-rw-r--r--   0        0        0      622 2023-06-14 11:03:59.351992 eotdl-2023.6.14.post5/pyproject.toml
+-rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 eotdl-2023.6.14.post5/setup.py
+-rw-r--r--   0        0        0      737 1970-01-01 00:00:00.000000 eotdl-2023.6.14.post5/PKG-INFO
```

### Comparing `eotdl-2023.6.14.post4/eotdl/__init__.py` & `eotdl-2023.6.14.post5/eotdl/__init__.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/access/sentinelhub/client.py` & `eotdl-2023.6.14.post5/eotdl/access/sentinelhub/client.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/access/sentinelhub/utils.py` & `eotdl-2023.6.14.post5/eotdl/access/sentinelhub/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/commands/auth.py` & `eotdl-2023.6.14.post5/eotdl/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/commands/datasets.py` & `eotdl-2023.6.14.post5/eotdl/commands/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typer
-from src.usecases.datasets import (
+from datasets import (
     retrieve_datasets,
     download_dataset,
     update_dataset,
     ingest_large_dataset,
-    ingest_large_dataset_parallel,
+    # ingest_large_dataset_parallel,
 )
 from src.usecases.auth import auth
 from typing import Optional
 
 app = typer.Typer()
```

### Comparing `eotdl-2023.6.14.post4/eotdl/curation/formatters.py` & `eotdl-2023.6.14.post5/eotdl/curation/formatters.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/curation/metadata.py` & `eotdl-2023.6.14.post5/eotdl/curation/metadata.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/curation/stac/dataframe.py` & `eotdl-2023.6.14.post5/eotdl/curation/stac/dataframe.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/curation/stac/extensions.py` & `eotdl-2023.6.14.post5/eotdl/curation/stac/extensions.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/curation/stac/parsers.py` & `eotdl-2023.6.14.post5/eotdl/curation/stac/parsers.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/curation/stac/stac.py` & `eotdl-2023.6.14.post5/eotdl/curation/stac/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/curation/stac/utils.py` & `eotdl-2023.6.14.post5/eotdl/curation/stac/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/src/repos/APIRepo.py` & `eotdl-2023.6.14.post5/eotdl/src/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/src/repos/AuthRepo.py` & `eotdl-2023.6.14.post5/eotdl/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/src/usecases/auth/Auth.py` & `eotdl-2023.6.14.post5/eotdl/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/src/usecases/auth/main.py` & `eotdl-2023.6.14.post5/eotdl/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/DownloadDataset.py` & `eotdl-2023.6.14.post5/eotdl/src/usecases/datasets/DownloadDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/IngestDataset.py` & `eotdl-2023.6.14.post5/eotdl/src/usecases/datasets/IngestDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/IngestLargeDataset.py` & `eotdl-2023.6.14.post5/eotdl/src/usecases/datasets/IngestLargeDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py` & `eotdl-2023.6.14.post5/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/src/usecases/datasets/UpdateDataset.py` & `eotdl-2023.6.14.post5/eotdl/src/usecases/datasets/UpdateDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/tools/sen12floods/tools.py` & `eotdl-2023.6.14.post5/eotdl/tools/sen12floods/tools.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/eotdl/tools/stac.py` & `eotdl-2023.6.14.post5/eotdl/tools/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post4/pyproject.toml` & `eotdl-2023.6.14.post5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl"
-version = "2023.06.14-4"
+version = "2023.06.14-5"
 description = "Earth Observation Training Data Lab"
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl-2023.6.14.post4/setup.py` & `eotdl-2023.6.14.post5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['eotdl = eotdl.main:app']}
 
 setup_kwargs = {
     'name': 'eotdl',
-    'version': '2023.6.14.post4',
+    'version': '2023.6.14.post5',
     'description': 'Earth Observation Training Data Lab',
     'long_description': '# eotdl \n\nThis is the main library for EOTDL.\n\n',
     'author': 'EarthPulse',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `eotdl-2023.6.14.post4/PKG-INFO` & `eotdl-2023.6.14.post5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl
-Version: 2023.6.14.post4
+Version: 2023.6.14.post5
 Summary: Earth Observation Training Data Lab
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

