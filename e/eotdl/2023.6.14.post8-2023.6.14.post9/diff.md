# Comparing `tmp/eotdl-2023.6.14.post8.tar.gz` & `tmp/eotdl-2023.6.14.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-2023.6.14.post8.tar", max compression
+gzip compressed data, was "eotdl-2023.6.14.post9.tar", max compression
```

## Comparing `eotdl-2023.6.14.post8.tar` & `eotdl-2023.6.14.post9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0       55 2023-06-14 11:11:09.535553 eotdl-2023.6.14.post8/README.md
--rw-r--r--   0        0        0      936 2023-06-14 11:29:35.346126 eotdl-2023.6.14.post8/eotdl/__init__.py
--rw-r--r--   0        0        0      292 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post8/eotdl/access/__init__.py
--rw-r--r--   0        0        0      363 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post8/eotdl/access/parameters.py
--rw-r--r--   0        0        0      252 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post8/eotdl/access/sentinelhub/__init__.py
--rw-r--r--   0        0        0     7605 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post8/eotdl/access/sentinelhub/client.py
--rw-r--r--   0        0        0     6595 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post8/eotdl/access/sentinelhub/utils.py
--rw-r--r--   0        0        0       55 2023-06-14 11:05:23.616245 eotdl-2023.6.14.post8/eotdl/auth/__init__.py
--rw-r--r--   0        0        0      776 2023-06-14 12:12:34.337586 eotdl-2023.6.14.post8/eotdl/auth/main.py
--rw-r--r--   0        0        0      193 2023-06-14 12:17:22.982144 eotdl-2023.6.14.post8/eotdl/cli.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:15.563978 eotdl-2023.6.14.post8/eotdl/commands/__init__.py
--rw-r--r--   0        0        0      937 2023-06-14 12:12:41.917619 eotdl-2023.6.14.post8/eotdl/commands/auth.py
--rw-r--r--   0        0        0     1569 2023-06-14 12:14:04.769935 eotdl-2023.6.14.post8/eotdl/commands/datasets.py
--rw-r--r--   0        0        0      270 2023-06-14 10:33:31.353776 eotdl-2023.6.14.post8/eotdl/curation/__init__.py
--rw-r--r--   0        0        0     2929 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post8/eotdl/curation/formatters.py
--rw-r--r--   0        0        0     1552 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post8/eotdl/curation/metadata.py
--rw-r--r--   0        0        0      201 2023-06-14 09:35:56.383873 eotdl-2023.6.14.post8/eotdl/curation/stac/__init__.py
--rw-r--r--   0        0        0     8495 2023-06-14 10:12:58.941969 eotdl-2023.6.14.post8/eotdl/curation/stac/dataframe.py
--rw-r--r--   0        0        0     5231 2023-06-14 09:10:22.117884 eotdl-2023.6.14.post8/eotdl/curation/stac/extensions.py
--rw-r--r--   0        0        0     1380 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post8/eotdl/curation/stac/parsers.py
--rw-r--r--   0        0        0    17796 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post8/eotdl/curation/stac/stac.py
--rw-r--r--   0        0        0     1855 2023-06-14 09:09:09.621596 eotdl-2023.6.14.post8/eotdl/curation/stac/utils.py
--rw-r--r--   0        0        0      211 2023-06-14 12:14:03.597934 eotdl-2023.6.14.post8/eotdl/datasets/__init__.py
--rw-r--r--   0        0        0      529 2023-06-14 12:14:02.581934 eotdl-2023.6.14.post8/eotdl/datasets/download.py
--rw-r--r--   0        0        0      824 2023-06-14 12:14:01.877933 eotdl-2023.6.14.post8/eotdl/datasets/ingest.py
--rw-r--r--   0        0        0      548 2023-06-14 12:14:01.141933 eotdl-2023.6.14.post8/eotdl/datasets/retrieve.py
--rw-r--r--   0        0        0      330 2023-06-14 12:14:00.433933 eotdl-2023.6.14.post8/eotdl/datasets/update.py
--rw-r--r--   0        0        0       74 2023-04-18 14:58:49.560135 eotdl-2023.6.14.post8/eotdl/hello.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.807993 eotdl-2023.6.14.post8/eotdl/src/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post8/eotdl/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post8/eotdl/src/errors/auth.py
--rw-r--r--   0        0        0     9843 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post8/eotdl/src/repos/APIRepo.py
--rw-r--r--   0        0        0      955 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post8/eotdl/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post8/eotdl/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post8/eotdl/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post8/eotdl/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post8/eotdl/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post8/eotdl/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0        0 2023-06-14 11:04:47.532137 eotdl-2023.6.14.post8/eotdl/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      767 2023-06-14 12:13:58.693932 eotdl-2023.6.14.post8/eotdl/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      932 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post8/eotdl/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0     1407 2023-06-14 12:13:59.605932 eotdl-2023.6.14.post8/eotdl/src/usecases/datasets/IngestLargeDataset.py
--rw-r--r--   0        0        0     1595 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post8/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py
--rw-r--r--   0        0        0      421 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post8/eotdl/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post8/eotdl/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0      944 2023-06-14 12:13:57.889932 eotdl-2023.6.14.post8/eotdl/src/usecases/datasets/UpdateDataset.py
--rw-r--r--   0        0        0        0 2023-06-14 10:51:58.909786 eotdl-2023.6.14.post8/eotdl/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0      479 2023-06-14 10:24:20.823993 eotdl-2023.6.14.post8/eotdl/src/utils.py
--rw-r--r--   0        0        0      277 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post8/eotdl/tools/__init__.py
--rw-r--r--   0        0        0      215 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post8/eotdl/tools/sen12floods/__init__.py
--rw-r--r--   0        0        0     8124 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post8/eotdl/tools/sen12floods/tools.py
--rw-r--r--   0        0        0      636 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post8/eotdl/tools/stac.py
--rw-r--r--   0        0        0      621 2023-06-14 12:17:43.342177 eotdl-2023.6.14.post8/pyproject.toml
--rw-r--r--   0        0        0     1213 1970-01-01 00:00:00.000000 eotdl-2023.6.14.post8/setup.py
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 eotdl-2023.6.14.post8/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-06-14 11:11:09.535553 eotdl-2023.6.14.post9/README.md
+-rw-r--r--   0        0        0      936 2023-06-14 11:29:35.346126 eotdl-2023.6.14.post9/eotdl/__init__.py
+-rw-r--r--   0        0        0      292 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/access/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/access/parameters.py
+-rw-r--r--   0        0        0      252 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/access/sentinelhub/__init__.py
+-rw-r--r--   0        0        0     7605 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/access/sentinelhub/client.py
+-rw-r--r--   0        0        0     6595 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/access/sentinelhub/utils.py
+-rw-r--r--   0        0        0       66 2023-06-14 12:47:21.260036 eotdl-2023.6.14.post9/eotdl/auth/__init__.py
+-rw-r--r--   0        0        0      857 2023-06-14 12:49:25.712094 eotdl-2023.6.14.post9/eotdl/auth/main.py
+-rw-r--r--   0        0        0      193 2023-06-14 12:17:22.982144 eotdl-2023.6.14.post9/eotdl/cli.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:15.563978 eotdl-2023.6.14.post9/eotdl/commands/__init__.py
+-rw-r--r--   0        0        0      937 2023-06-14 13:05:32.317534 eotdl-2023.6.14.post9/eotdl/commands/auth.py
+-rw-r--r--   0        0        0     1491 2023-06-14 13:05:31.529532 eotdl-2023.6.14.post9/eotdl/commands/datasets.py
+-rw-r--r--   0        0        0      270 2023-06-14 10:33:31.353776 eotdl-2023.6.14.post9/eotdl/curation/__init__.py
+-rw-r--r--   0        0        0     2929 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/curation/formatters.py
+-rw-r--r--   0        0        0     1552 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/curation/metadata.py
+-rw-r--r--   0        0        0      201 2023-06-14 09:35:56.383873 eotdl-2023.6.14.post9/eotdl/curation/stac/__init__.py
+-rw-r--r--   0        0        0     8495 2023-06-14 10:12:58.941969 eotdl-2023.6.14.post9/eotdl/curation/stac/dataframe.py
+-rw-r--r--   0        0        0     5231 2023-06-14 09:10:22.117884 eotdl-2023.6.14.post9/eotdl/curation/stac/extensions.py
+-rw-r--r--   0        0        0     1380 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/curation/stac/parsers.py
+-rw-r--r--   0        0        0    17796 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/curation/stac/stac.py
+-rw-r--r--   0        0        0     1855 2023-06-14 09:09:09.621596 eotdl-2023.6.14.post9/eotdl/curation/stac/utils.py
+-rw-r--r--   0        0        0      226 2023-06-14 12:42:18.658877 eotdl-2023.6.14.post9/eotdl/datasets/__init__.py
+-rw-r--r--   0        0        0      568 2023-06-14 13:04:46.461411 eotdl-2023.6.14.post9/eotdl/datasets/download.py
+-rw-r--r--   0        0        0      846 2023-06-14 13:04:11.725320 eotdl-2023.6.14.post9/eotdl/datasets/ingest.py
+-rw-r--r--   0        0        0      534 2023-06-14 12:41:38.606725 eotdl-2023.6.14.post9/eotdl/datasets/retrieve.py
+-rw-r--r--   0        0        0      366 2023-06-14 13:05:23.913511 eotdl-2023.6.14.post9/eotdl/datasets/update.py
+-rw-r--r--   0        0        0       74 2023-04-18 14:58:49.560135 eotdl-2023.6.14.post9/eotdl/hello.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.807993 eotdl-2023.6.14.post9/eotdl/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post9/eotdl/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post9/eotdl/src/errors/auth.py
+-rw-r--r--   0        0        0     9935 2023-06-14 12:57:49.716461 eotdl-2023.6.14.post9/eotdl/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      987 2023-06-14 12:53:43.856124 eotdl-2023.6.14.post9/eotdl/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post9/eotdl/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post9/eotdl/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post9/eotdl/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post9/eotdl/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post9/eotdl/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       81 2023-06-14 12:28:54.159966 eotdl-2023.6.14.post9/eotdl/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      788 2023-06-14 13:04:43.661404 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      953 2023-06-14 12:59:21.144637 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0     1428 2023-06-14 12:59:27.016649 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/IngestLargeDataset.py
+-rw-r--r--   0        0        0     1595 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py
+-rw-r--r--   0        0        0      421 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0      965 2023-06-14 13:05:23.037509 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/UpdateDataset.py
+-rw-r--r--   0        0        0      270 2023-06-14 12:30:22.104262 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0      479 2023-06-14 10:24:20.823993 eotdl-2023.6.14.post9/eotdl/src/utils.py
+-rw-r--r--   0        0        0      277 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/tools/__init__.py
+-rw-r--r--   0        0        0      215 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/tools/sen12floods/__init__.py
+-rw-r--r--   0        0        0     8124 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/tools/sen12floods/tools.py
+-rw-r--r--   0        0        0      636 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/tools/stac.py
+-rw-r--r--   0        0        0      621 2023-06-14 13:05:58.245604 eotdl-2023.6.14.post9/pyproject.toml
+-rw-r--r--   0        0        0     1213 1970-01-01 00:00:00.000000 eotdl-2023.6.14.post9/setup.py
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 eotdl-2023.6.14.post9/PKG-INFO
```

### Comparing `eotdl-2023.6.14.post8/eotdl/__init__.py` & `eotdl-2023.6.14.post9/eotdl/__init__.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/access/sentinelhub/client.py` & `eotdl-2023.6.14.post9/eotdl/access/sentinelhub/client.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/access/sentinelhub/utils.py` & `eotdl-2023.6.14.post9/eotdl/access/sentinelhub/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/commands/auth.py` & `eotdl-2023.6.14.post9/eotdl/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/commands/datasets.py` & `eotdl-2023.6.14.post9/eotdl/commands/datasets.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     """
     Download a dataset
 
     name: Name of the dataset
     path: Path to download the dataset to
     """
     try:
-        user = auth()
         dst_path = download_dataset(name, path, user, typer.echo)
         typer.echo(f"Dataset {name} downloaded to {dst_path}")
     except Exception as e:
         typer.echo(e)
 
 
 @app.command()
@@ -45,18 +44,17 @@
     """
     Ingest a dataset
 
     path: Path to dataset to ingest
     n: Name of the dataset
     """
     try:
-        user = auth()
         # if p:
         #     ingest_large_dataset_parallel(name, path, user, p, typer.echo)
-        ingest_large_dataset(name, path, user, typer.echo)
+        ingest_large_dataset(name, path, typer.echo)
         typer.echo(f"Dataset {name} ingested")
     except Exception as e:
         typer.echo(e)
 
 
 @app.command()
 def update(
@@ -66,16 +64,15 @@
     """
     Update a dataset
 
     name: Name of the dataset
     path: Path to dataset to ingest
     """
     try:
-        user = auth()
-        update_dataset(name, path, user, typer.echo)
+        update_dataset(name, path, typer.echo)
         typer.echo(f"Dataset {name} updated")
     except Exception as e:
         typer.echo(e)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `eotdl-2023.6.14.post8/eotdl/curation/formatters.py` & `eotdl-2023.6.14.post9/eotdl/curation/formatters.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/curation/metadata.py` & `eotdl-2023.6.14.post9/eotdl/curation/metadata.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/curation/stac/dataframe.py` & `eotdl-2023.6.14.post9/eotdl/curation/stac/dataframe.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/curation/stac/extensions.py` & `eotdl-2023.6.14.post9/eotdl/curation/stac/extensions.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/curation/stac/parsers.py` & `eotdl-2023.6.14.post9/eotdl/curation/stac/parsers.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/curation/stac/stac.py` & `eotdl-2023.6.14.post9/eotdl/curation/stac/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/curation/stac/utils.py` & `eotdl-2023.6.14.post9/eotdl/curation/stac/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/datasets/ingest.py` & `eotdl-2023.6.14.post9/eotdl/datasets/ingest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from ..src.repos import APIRepo
-from ..src.usecases.datasets.IngestDataset import IngestDataset
-from ..src.usecases.datasets.IngestLargeDataset import IngestLargeDataset
+from ..src.usecases.datasets import IngestDataset, IngestLargeDataset
+from ..auth import with_auth
 
 
-def ingest_q0(dataset, file):
-    print("hola")
-    return
-
-
-def ingest_q1(dataset, stac_catalog):
-    print("hola")
-    return
-
-
-def ingest_dataset(name, description, path, user, logger):
+@with_auth
+def ingest_dataset(name, description, path, logger=None, user=None):
     api_repo = APIRepo()
     ingest = IngestDataset(
         api_repo,
     )
     inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
     outputs = ingest(inputs)
     return outputs.dataset
 
 
-def ingest_large_dataset(name, path, user, logger):
+@with_auth
+def ingest_large_dataset(name, path, logger=None, user=None):
     api_repo = APIRepo()
     ingest = IngestLargeDataset(api_repo, logger)
     inputs = ingest.Inputs(name=name, path=path, user=user)
     outputs = ingest(inputs)
     return outputs.dataset
+
+
+def ingest_q0(dataset, path):
+    return ingest_large_dataset(dataset, path)
+
+
+def ingest_q1(dataset, stac_catalog):
+    print("holas")
+    return
```

### Comparing `eotdl-2023.6.14.post8/eotdl/datasets/retrieve.py` & `eotdl-2023.6.14.post9/eotdl/datasets/retrieve.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from ..src.repos import APIRepo
-from ..src.usecases.datasets.RetrieveDatasets import RetrieveDatasets
-from ..src.usecases.datasets.RetrieveDataset import RetrieveDataset
+from ..src.usecases.datasets import RetrieveDatasets, RetrieveDataset
+
+
+def list_datasets():
+    return retrieve_datasets()
 
 
 def retrieve_datasets():
     api_repo = APIRepo()
     retrieve = RetrieveDatasets(api_repo)
     inputs = retrieve.Inputs()
     outputs = retrieve(inputs)
```

### Comparing `eotdl-2023.6.14.post8/eotdl/src/repos/APIRepo.py` & `eotdl-2023.6.14.post9/eotdl/src/repos/APIRepo.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,25 +31,27 @@
             return response.json(), None
         return None, response.json()["detail"]
 
     def download_dataset(self, dataset_id, id_token, path):
         url = self.url + "datasets/" + dataset_id + "/download"
         headers = {"Authorization": "Bearer " + id_token}
         if path is None:
-            path = str(Path.home()) + "/.etodl/datasets"
+            path = str(Path.home()) + "/.eotdl/datasets"
             os.makedirs(path, exist_ok=True)
         with requests.get(url, headers=headers, stream=True) as r:
             r.raise_for_status()
             total_size = int(r.headers.get("content-length", 0))
             block_size = 1024 * 1024 * 10
             progress_bar = tqdm(
                 total=total_size, unit="iB", unit_scale=True, unit_divisor=1024
             )
             filename = r.headers.get("content-disposition").split("filename=")[1][1:-1]
             path = f"{path}/{filename}"
+            if os.path.exists(path):
+                raise Exception("File already exists")
             with open(path, "wb") as f:
                 for chunk in r.iter_content(block_size):
                     progress_bar.update(len(chunk))
                     if chunk:
                         f.write(chunk)
             progress_bar.close()
             return path
```

### Comparing `eotdl-2023.6.14.post8/eotdl/src/repos/AuthRepo.py` & `eotdl-2023.6.14.post9/eotdl/src/repos/AuthRepo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from pathlib import Path
-import os 
-import json 
+import os
+import json
 import jwt
 
-class AuthRepo():
+
+class AuthRepo:
     def __init__(self):
-        self.algorithms = ['RS256']
+        self.algorithms = ["RS256"]
         self.home = str(Path.home())
-        self.creds_path = self.home + '/.etodl/creds.json'
+        self.creds_path = self.home + "/.eotdl/creds.json"
 
     def save_creds(self, data):
-        os.makedirs(self.home + '/.etodl', exist_ok=True)
-        with open(self.creds_path, 'w') as f:
+        os.makedirs(self.home + "/.eotdl", exist_ok=True)
+        with open(self.creds_path, "w") as f:
             json.dump(data, f)
         return self.creds_path
-    
+
     def load_creds(self):
         if os.path.exists(self.creds_path):
-            with open(self.creds_path, 'r') as f:
+            with open(self.creds_path, "r") as f:
                 creds = json.load(f)
             user = self.decode_token(creds)
-            user['id_token'] = creds['id_token']
+            user["id_token"] = creds["id_token"]
             return user
         return None
-    
+
     def decode_token(self, token_data):
-        return jwt.decode(token_data['id_token'], algorithms=self.algorithms, options={"verify_signature": False})
-    
+        return jwt.decode(
+            token_data["id_token"],
+            algorithms=self.algorithms,
+            options={"verify_signature": False},
+        )
+
     def logout(self):
         os.remove(self.creds_path)
```

### Comparing `eotdl-2023.6.14.post8/eotdl/src/usecases/auth/Auth.py` & `eotdl-2023.6.14.post9/eotdl/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/src/usecases/datasets/DownloadDataset.py` & `eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/DownloadDataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pydantic import BaseModel
 from ....src.utils import calculate_checksum
 
 
 class DownloadDataset:
     def __init__(self, repo, logger):
         self.repo = repo
-        self.logger = logger
+        self.logger = logger if logger else print
 
     class Inputs(BaseModel):
         dataset: str
         path: str = None
         user: dict
         checksum: str
```

### Comparing `eotdl-2023.6.14.post8/eotdl/src/usecases/datasets/IngestDataset.py` & `eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/IngestDataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pydantic import BaseModel
 
 
 class IngestDataset:
     def __init__(self, repo, logger):
         self.repo = repo
-        self.logger = logger
+        self.logger = logger if logger else print
 
     class Inputs(BaseModel):
         name: str
         description: str
         path: str = None
         user: dict
```

### Comparing `eotdl-2023.6.14.post8/eotdl/src/usecases/datasets/IngestLargeDataset.py` & `eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/IngestLargeDataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pydantic import BaseModel
 from ....src.utils import calculate_checksum
 
 
 class IngestLargeDataset:
     def __init__(self, repo, logger):
         self.repo = repo
-        self.logger = logger
+        self.logger = logger if logger else print
 
     class Inputs(BaseModel):
         name: str
         path: str = None
         user: dict
 
     class Outputs(BaseModel):
```

### Comparing `eotdl-2023.6.14.post8/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py` & `eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/src/usecases/datasets/UpdateDataset.py` & `eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/UpdateDataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pydantic import BaseModel
 from ....src.utils import calculate_checksum
 
 
 class UpdateDataset:
     def __init__(self, repo, logger):
         self.repo = repo
-        self.logger = logger
+        self.logger = logger if logger else print
 
     class Inputs(BaseModel):
         name: str
         path: str = None
         user: dict
 
     class Outputs(BaseModel):
```

### Comparing `eotdl-2023.6.14.post8/eotdl/tools/sen12floods/tools.py` & `eotdl-2023.6.14.post9/eotdl/tools/sen12floods/tools.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/eotdl/tools/stac.py` & `eotdl-2023.6.14.post9/eotdl/tools/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post8/pyproject.toml` & `eotdl-2023.6.14.post9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl"
-version = "2023.06.14-8"
+version = "2023.06.14-9"
 description = "Earth Observation Training Data Lab"
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl-2023.6.14.post8/setup.py` & `eotdl-2023.6.14.post9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['eotdl = eotdl.cli:app']}
 
 setup_kwargs = {
     'name': 'eotdl',
-    'version': '2023.6.14.post8',
+    'version': '2023.6.14.post9',
     'description': 'Earth Observation Training Data Lab',
     'long_description': '# eotdl \n\nThis is the main library and CLI for EOTDL.\n\n',
     'author': 'EarthPulse',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `eotdl-2023.6.14.post8/PKG-INFO` & `eotdl-2023.6.14.post9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl
-Version: 2023.6.14.post8
+Version: 2023.6.14.post9
 Summary: Earth Observation Training Data Lab
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

