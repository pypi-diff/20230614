# Comparing `tmp/eotdl-2023.6.14.tar.gz` & `tmp/eotdl-2023.6.14.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-2023.6.14.tar", max compression
+gzip compressed data, was "eotdl-2023.6.14.post2.tar", max compression
```

## Comparing `eotdl-2023.6.14.tar` & `eotdl-2023.6.14.post2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0       47 2023-03-08 12:48:38.254243 eotdl-2023.6.14/README.md
--rw-r--r--   0        0        0      934 2023-06-14 09:35:09.859839 eotdl-2023.6.14/eotdl/__init__.py
--rw-r--r--   0        0        0      292 2023-06-14 08:30:42.023737 eotdl-2023.6.14/eotdl/access/__init__.py
--rw-r--r--   0        0        0      362 2023-06-14 09:01:13.971570 eotdl-2023.6.14/eotdl/access/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      747 2023-06-14 09:01:14.123571 eotdl-2023.6.14/eotdl/access/__pycache__/parameters.cpython-38.pyc
--rw-r--r--   0        0        0      363 2023-06-14 08:30:42.023737 eotdl-2023.6.14/eotdl/access/parameters.py
--rw-r--r--   0        0        0      252 2023-06-14 08:30:42.023737 eotdl-2023.6.14/eotdl/access/sentinelhub/__init__.py
--rw-r--r--   0        0        0      388 2023-06-14 09:01:13.975570 eotdl-2023.6.14/eotdl/access/sentinelhub/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5973 2023-06-14 09:01:13.975570 eotdl-2023.6.14/eotdl/access/sentinelhub/__pycache__/client.cpython-38.pyc
--rw-r--r--   0        0        0     5935 2023-06-14 09:01:14.119570 eotdl-2023.6.14/eotdl/access/sentinelhub/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     7605 2023-06-14 08:30:42.023737 eotdl-2023.6.14/eotdl/access/sentinelhub/client.py
--rw-r--r--   0        0        0     6595 2023-06-14 08:30:42.023737 eotdl-2023.6.14/eotdl/access/sentinelhub/utils.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:15.563978 eotdl-2023.6.14/eotdl/commands/__init__.py
--rw-r--r--   0        0        0      148 2023-06-14 10:27:36.340542 eotdl-2023.6.14/eotdl/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1165 2023-06-14 10:27:36.340542 eotdl-2023.6.14/eotdl/commands/__pycache__/auth.cpython-38.pyc
--rw-r--r--   0        0        0     1863 2023-06-14 10:27:36.412543 eotdl-2023.6.14/eotdl/commands/__pycache__/datasets.cpython-38.pyc
--rw-r--r--   0        0        0      920 2023-06-14 10:24:15.567978 eotdl-2023.6.14/eotdl/commands/auth.py
--rw-r--r--   0        0        0     1618 2023-06-14 10:24:15.567978 eotdl-2023.6.14/eotdl/commands/datasets.py
--rw-r--r--   0        0        0      268 2023-06-14 09:43:15.012446 eotdl-2023.6.14/eotdl/curation/__init__.py
--rw-r--r--   0        0        0      179 2023-06-14 09:43:21.640457 eotdl-2023.6.14/eotdl/curation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      200 2023-06-14 09:07:38.637229 eotdl-2023.6.14/eotdl/curation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2402 2023-06-14 09:01:14.263571 eotdl-2023.6.14/eotdl/curation/__pycache__/formatters.cpython-38.pyc
--rw-r--r--   0        0        0     1378 2023-06-14 09:01:14.363572 eotdl-2023.6.14/eotdl/curation/__pycache__/metadata.cpython-38.pyc
--rw-r--r--   0        0        0     2929 2023-06-14 08:30:42.023737 eotdl-2023.6.14/eotdl/curation/formatters.py
--rw-r--r--   0        0        0     1552 2023-06-14 08:30:42.023737 eotdl-2023.6.14/eotdl/curation/metadata.py
--rw-r--r--   0        0        0      201 2023-06-14 09:35:56.383873 eotdl-2023.6.14/eotdl/curation/stac/__init__.py
--rw-r--r--   0        0        0      132 2023-06-14 09:36:01.251877 eotdl-2023.6.14/eotdl/curation/stac/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      417 2023-06-14 09:07:38.637229 eotdl-2023.6.14/eotdl/curation/stac/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6141 2023-06-14 10:19:16.183116 eotdl-2023.6.14/eotdl/curation/stac/__pycache__/dataframe.cpython-310.pyc
--rw-r--r--   0        0        0     5841 2023-06-14 09:10:41.613961 eotdl-2023.6.14/eotdl/curation/stac/__pycache__/dataframe.cpython-38.pyc
--rw-r--r--   0        0        0     4146 2023-06-14 09:29:29.599856 eotdl-2023.6.14/eotdl/curation/stac/__pycache__/extensions.cpython-310.pyc
--rw-r--r--   0        0        0     4319 2023-06-14 09:10:41.613961 eotdl-2023.6.14/eotdl/curation/stac/__pycache__/extensions.cpython-38.pyc
--rw-r--r--   0        0        0     2206 2023-06-14 09:29:29.599856 eotdl-2023.6.14/eotdl/curation/stac/__pycache__/parsers.cpython-310.pyc
--rw-r--r--   0        0        0     2290 2023-06-14 09:08:03.765331 eotdl-2023.6.14/eotdl/curation/stac/__pycache__/parsers.cpython-38.pyc
--rw-r--r--   0        0        0    12691 2023-06-14 09:27:19.432035 eotdl-2023.6.14/eotdl/curation/stac/__pycache__/stac.cpython-310.pyc
--rw-r--r--   0        0        0    12654 2023-06-14 09:07:38.641229 eotdl-2023.6.14/eotdl/curation/stac/__pycache__/stac.cpython-38.pyc
--rw-r--r--   0        0        0     1893 2023-06-14 09:29:29.599856 eotdl-2023.6.14/eotdl/curation/stac/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     1918 2023-06-14 09:09:16.441624 eotdl-2023.6.14/eotdl/curation/stac/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     8495 2023-06-14 10:12:58.941969 eotdl-2023.6.14/eotdl/curation/stac/dataframe.py
--rw-r--r--   0        0        0     5231 2023-06-14 09:10:22.117884 eotdl-2023.6.14/eotdl/curation/stac/extensions.py
--rw-r--r--   0        0        0     1380 2023-06-14 08:30:42.023737 eotdl-2023.6.14/eotdl/curation/stac/parsers.py
--rw-r--r--   0        0        0    17796 2023-06-14 08:30:42.023737 eotdl-2023.6.14/eotdl/curation/stac/stac.py
--rw-r--r--   0        0        0     1855 2023-06-14 09:09:09.621596 eotdl-2023.6.14/eotdl/curation/stac/utils.py
--rw-r--r--   0        0        0        0 2023-06-14 10:19:49.195213 eotdl-2023.6.14/eotdl/datasets/__init__.py
--rw-r--r--   0        0        0       92 2023-06-14 10:23:43.387887 eotdl-2023.6.14/eotdl/datasets/ingest.py
--rw-r--r--   0        0        0       74 2023-04-18 14:58:49.560135 eotdl-2023.6.14/eotdl/hello.py
--rw-r--r--   0        0        0      367 2023-06-14 10:24:27.780013 eotdl-2023.6.14/eotdl/main.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.807993 eotdl-2023.6.14/eotdl/src/__init__.py
--rw-r--r--   0        0        0      143 2023-06-14 10:27:36.340542 eotdl-2023.6.14/eotdl/src/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2457 2023-06-14 10:24:20.811993 eotdl-2023.6.14/eotdl/src/__pycache__/auth.cpython-38.pyc
--rw-r--r--   0        0        0      551 2023-06-14 10:27:36.416543 eotdl-2023.6.14/eotdl/src/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.811993 eotdl-2023.6.14/eotdl/src/errors/__init__.py
--rw-r--r--   0        0        0      150 2023-06-14 10:27:36.412543 eotdl-2023.6.14/eotdl/src/errors/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      829 2023-06-14 10:27:36.412543 eotdl-2023.6.14/eotdl/src/errors/__pycache__/auth.cpython-38.pyc
--rw-r--r--   0        0        0      306 2023-06-14 10:24:20.811993 eotdl-2023.6.14/eotdl/src/errors/auth.py
--rw-r--r--   0        0        0     9843 2023-06-14 10:24:20.811993 eotdl-2023.6.14/eotdl/src/repos/APIRepo.py
--rw-r--r--   0        0        0      955 2023-06-14 10:24:20.811993 eotdl-2023.6.14/eotdl/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-06-14 10:24:20.815993 eotdl-2023.6.14/eotdl/src/repos/__init__.py
--rw-r--r--   0        0        0     7183 2023-06-14 10:27:36.364543 eotdl-2023.6.14/eotdl/src/repos/__pycache__/APIRepo.cpython-38.pyc
--rw-r--r--   0        0        0     1503 2023-06-14 10:27:36.344542 eotdl-2023.6.14/eotdl/src/repos/__pycache__/AuthRepo.cpython-38.pyc
--rw-r--r--   0        0        0      210 2023-06-14 10:27:36.344542 eotdl-2023.6.14/eotdl/src/repos/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.815993 eotdl-2023.6.14/eotdl/src/usecases/__init__.py
--rw-r--r--   0        0        0      152 2023-06-14 10:27:36.340542 eotdl-2023.6.14/eotdl/src/usecases/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1851 2023-06-14 10:24:20.815993 eotdl-2023.6.14/eotdl/src/usecases/__pycache__/auth.cpython-38.pyc
--rw-r--r--   0        0        0     1587 2023-06-14 10:24:20.815993 eotdl-2023.6.14/eotdl/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-06-14 10:24:20.815993 eotdl-2023.6.14/eotdl/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-06-14 10:24:20.815993 eotdl-2023.6.14/eotdl/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-06-14 10:24:20.815993 eotdl-2023.6.14/eotdl/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0     1790 2023-06-14 10:27:36.412543 eotdl-2023.6.14/eotdl/src/usecases/auth/__pycache__/Auth.cpython-38.pyc
--rw-r--r--   0        0        0     1034 2023-06-14 10:27:36.396543 eotdl-2023.6.14/eotdl/src/usecases/auth/__pycache__/IsLogged.cpython-38.pyc
--rw-r--r--   0        0        0     1059 2023-06-14 10:27:36.412543 eotdl-2023.6.14/eotdl/src/usecases/auth/__pycache__/Logout.cpython-38.pyc
--rw-r--r--   0        0        0      240 2023-06-14 10:27:36.344542 eotdl-2023.6.14/eotdl/src/usecases/auth/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      951 2023-06-14 10:27:36.344542 eotdl-2023.6.14/eotdl/src/usecases/auth/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0      725 2023-06-14 10:24:20.819993 eotdl-2023.6.14/eotdl/src/usecases/auth/main.py
--rw-r--r--   0        0        0      763 2023-06-14 10:24:20.819993 eotdl-2023.6.14/eotdl/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      932 2023-06-14 10:24:20.819993 eotdl-2023.6.14/eotdl/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0     1403 2023-06-14 10:24:20.819993 eotdl-2023.6.14/eotdl/src/usecases/datasets/IngestLargeDataset.py
--rw-r--r--   0        0        0     1595 2023-06-14 10:24:20.819993 eotdl-2023.6.14/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py
--rw-r--r--   0        0        0      421 2023-06-14 10:24:20.819993 eotdl-2023.6.14/eotdl/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-06-14 10:24:20.819993 eotdl-2023.6.14/eotdl/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0      940 2023-06-14 10:24:20.819993 eotdl-2023.6.14/eotdl/src/usecases/datasets/UpdateDataset.py
--rw-r--r--   0        0        0      168 2023-06-14 10:24:20.823993 eotdl-2023.6.14/eotdl/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0     1406 2023-06-14 10:27:36.416543 eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/DownloadDataset.cpython-38.pyc
--rw-r--r--   0        0        0     1406 2023-06-14 10:27:36.416543 eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/IngestDataset.cpython-38.pyc
--rw-r--r--   0        0        0     1803 2023-06-14 10:27:36.416543 eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/IngestLargeDataset.cpython-38.pyc
--rw-r--r--   0        0        0     1913 2023-06-14 10:27:36.420543 eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/IngestLargeDatasetParallel.cpython-38.pyc
--rw-r--r--   0        0        0     1154 2023-06-14 10:27:36.416543 eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/RetrieveDataset.cpython-38.pyc
--rw-r--r--   0        0        0     1312 2023-06-14 10:27:36.416543 eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/RetrieveDatasets.cpython-38.pyc
--rw-r--r--   0        0        0     1501 2023-06-14 10:27:36.420543 eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/UpdateDataset.cpython-38.pyc
--rw-r--r--   0        0        0      355 2023-06-14 10:27:36.412543 eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2156 2023-06-14 10:27:36.416543 eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0     2168 2023-06-14 10:24:20.823993 eotdl-2023.6.14/eotdl/src/usecases/datasets/main.py
--rw-r--r--   0        0        0      479 2023-06-14 10:24:20.823993 eotdl-2023.6.14/eotdl/src/utils.py
--rw-r--r--   0        0        0      277 2023-06-14 08:30:42.023737 eotdl-2023.6.14/eotdl/tools/__init__.py
--rw-r--r--   0        0        0      391 2023-06-14 09:01:14.123571 eotdl-2023.6.14/eotdl/tools/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      874 2023-06-14 09:01:14.123571 eotdl-2023.6.14/eotdl/tools/__pycache__/stac.cpython-38.pyc
--rw-r--r--   0        0        0      215 2023-06-14 08:30:42.023737 eotdl-2023.6.14/eotdl/tools/sen12floods/__init__.py
--rw-r--r--   0        0        0      351 2023-06-14 09:01:14.259571 eotdl-2023.6.14/eotdl/tools/sen12floods/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6462 2023-06-14 09:01:14.263571 eotdl-2023.6.14/eotdl/tools/sen12floods/__pycache__/tools.cpython-38.pyc
--rw-r--r--   0        0        0     8124 2023-06-14 08:30:42.023737 eotdl-2023.6.14/eotdl/tools/sen12floods/tools.py
--rw-r--r--   0        0        0      636 2023-06-14 08:30:42.023737 eotdl-2023.6.14/eotdl/tools/stac.py
--rw-r--r--   0        0        0      621 2023-06-14 10:26:12.688308 eotdl-2023.6.14/pyproject.toml
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 eotdl-2023.6.14/setup.py
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 eotdl-2023.6.14/PKG-INFO
+-rw-r--r--   0        0        0       47 2023-03-08 12:48:38.254243 eotdl-2023.6.14.post2/README.md
+-rw-r--r--   0        0        0      936 2023-06-14 10:31:27.997185 eotdl-2023.6.14.post2/eotdl/__init__.py
+-rw-r--r--   0        0        0      292 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post2/eotdl/access/__init__.py
+-rw-r--r--   0        0        0      362 2023-06-14 09:01:13.971570 eotdl-2023.6.14.post2/eotdl/access/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      747 2023-06-14 09:01:14.123571 eotdl-2023.6.14.post2/eotdl/access/__pycache__/parameters.cpython-38.pyc
+-rw-r--r--   0        0        0      363 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post2/eotdl/access/parameters.py
+-rw-r--r--   0        0        0      252 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post2/eotdl/access/sentinelhub/__init__.py
+-rw-r--r--   0        0        0      388 2023-06-14 09:01:13.975570 eotdl-2023.6.14.post2/eotdl/access/sentinelhub/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5973 2023-06-14 09:01:13.975570 eotdl-2023.6.14.post2/eotdl/access/sentinelhub/__pycache__/client.cpython-38.pyc
+-rw-r--r--   0        0        0     5935 2023-06-14 09:01:14.119570 eotdl-2023.6.14.post2/eotdl/access/sentinelhub/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     7605 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post2/eotdl/access/sentinelhub/client.py
+-rw-r--r--   0        0        0     6595 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post2/eotdl/access/sentinelhub/utils.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:15.563978 eotdl-2023.6.14.post2/eotdl/commands/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-14 10:27:36.340542 eotdl-2023.6.14.post2/eotdl/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1165 2023-06-14 10:27:36.340542 eotdl-2023.6.14.post2/eotdl/commands/__pycache__/auth.cpython-38.pyc
+-rw-r--r--   0        0        0     1863 2023-06-14 10:27:36.412543 eotdl-2023.6.14.post2/eotdl/commands/__pycache__/datasets.cpython-38.pyc
+-rw-r--r--   0        0        0      920 2023-06-14 10:24:15.567978 eotdl-2023.6.14.post2/eotdl/commands/auth.py
+-rw-r--r--   0        0        0     1618 2023-06-14 10:24:15.567978 eotdl-2023.6.14.post2/eotdl/commands/datasets.py
+-rw-r--r--   0        0        0      268 2023-06-14 09:43:15.012446 eotdl-2023.6.14.post2/eotdl/curation/__init__.py
+-rw-r--r--   0        0        0      179 2023-06-14 09:43:21.640457 eotdl-2023.6.14.post2/eotdl/curation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      200 2023-06-14 09:07:38.637229 eotdl-2023.6.14.post2/eotdl/curation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2402 2023-06-14 09:01:14.263571 eotdl-2023.6.14.post2/eotdl/curation/__pycache__/formatters.cpython-38.pyc
+-rw-r--r--   0        0        0     1378 2023-06-14 09:01:14.363572 eotdl-2023.6.14.post2/eotdl/curation/__pycache__/metadata.cpython-38.pyc
+-rw-r--r--   0        0        0     2929 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post2/eotdl/curation/formatters.py
+-rw-r--r--   0        0        0     1552 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post2/eotdl/curation/metadata.py
+-rw-r--r--   0        0        0      201 2023-06-14 09:35:56.383873 eotdl-2023.6.14.post2/eotdl/curation/stac/__init__.py
+-rw-r--r--   0        0        0      132 2023-06-14 09:36:01.251877 eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      417 2023-06-14 09:07:38.637229 eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6141 2023-06-14 10:19:16.183116 eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/dataframe.cpython-310.pyc
+-rw-r--r--   0        0        0     5841 2023-06-14 09:10:41.613961 eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/dataframe.cpython-38.pyc
+-rw-r--r--   0        0        0     4146 2023-06-14 09:29:29.599856 eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/extensions.cpython-310.pyc
+-rw-r--r--   0        0        0     4319 2023-06-14 09:10:41.613961 eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/extensions.cpython-38.pyc
+-rw-r--r--   0        0        0     2206 2023-06-14 09:29:29.599856 eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/parsers.cpython-310.pyc
+-rw-r--r--   0        0        0     2290 2023-06-14 09:08:03.765331 eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/parsers.cpython-38.pyc
+-rw-r--r--   0        0        0    12691 2023-06-14 09:27:19.432035 eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/stac.cpython-310.pyc
+-rw-r--r--   0        0        0    12654 2023-06-14 09:07:38.641229 eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/stac.cpython-38.pyc
+-rw-r--r--   0        0        0     1893 2023-06-14 09:29:29.599856 eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1918 2023-06-14 09:09:16.441624 eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     8495 2023-06-14 10:12:58.941969 eotdl-2023.6.14.post2/eotdl/curation/stac/dataframe.py
+-rw-r--r--   0        0        0     5231 2023-06-14 09:10:22.117884 eotdl-2023.6.14.post2/eotdl/curation/stac/extensions.py
+-rw-r--r--   0        0        0     1380 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post2/eotdl/curation/stac/parsers.py
+-rw-r--r--   0        0        0    17796 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post2/eotdl/curation/stac/stac.py
+-rw-r--r--   0        0        0     1855 2023-06-14 09:09:09.621596 eotdl-2023.6.14.post2/eotdl/curation/stac/utils.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:19:49.195213 eotdl-2023.6.14.post2/eotdl/datasets/__init__.py
+-rw-r--r--   0        0        0       92 2023-06-14 10:23:43.387887 eotdl-2023.6.14.post2/eotdl/datasets/ingest.py
+-rw-r--r--   0        0        0       74 2023-04-18 14:58:49.560135 eotdl-2023.6.14.post2/eotdl/hello.py
+-rw-r--r--   0        0        0      367 2023-06-14 10:24:27.780013 eotdl-2023.6.14.post2/eotdl/main.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.807993 eotdl-2023.6.14.post2/eotdl/src/__init__.py
+-rw-r--r--   0        0        0      143 2023-06-14 10:27:36.340542 eotdl-2023.6.14.post2/eotdl/src/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2457 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post2/eotdl/src/__pycache__/auth.cpython-38.pyc
+-rw-r--r--   0        0        0      551 2023-06-14 10:27:36.416543 eotdl-2023.6.14.post2/eotdl/src/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post2/eotdl/src/errors/__init__.py
+-rw-r--r--   0        0        0      150 2023-06-14 10:27:36.412543 eotdl-2023.6.14.post2/eotdl/src/errors/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      829 2023-06-14 10:27:36.412543 eotdl-2023.6.14.post2/eotdl/src/errors/__pycache__/auth.cpython-38.pyc
+-rw-r--r--   0        0        0      306 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post2/eotdl/src/errors/auth.py
+-rw-r--r--   0        0        0     9843 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post2/eotdl/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      955 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post2/eotdl/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post2/eotdl/src/repos/__init__.py
+-rw-r--r--   0        0        0     7183 2023-06-14 10:27:36.364543 eotdl-2023.6.14.post2/eotdl/src/repos/__pycache__/APIRepo.cpython-38.pyc
+-rw-r--r--   0        0        0     1503 2023-06-14 10:27:36.344542 eotdl-2023.6.14.post2/eotdl/src/repos/__pycache__/AuthRepo.cpython-38.pyc
+-rw-r--r--   0        0        0      210 2023-06-14 10:27:36.344542 eotdl-2023.6.14.post2/eotdl/src/repos/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post2/eotdl/src/usecases/__init__.py
+-rw-r--r--   0        0        0      152 2023-06-14 10:27:36.340542 eotdl-2023.6.14.post2/eotdl/src/usecases/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1851 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post2/eotdl/src/usecases/__pycache__/auth.cpython-38.pyc
+-rw-r--r--   0        0        0     1587 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post2/eotdl/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post2/eotdl/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post2/eotdl/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post2/eotdl/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0     1790 2023-06-14 10:27:36.412543 eotdl-2023.6.14.post2/eotdl/src/usecases/auth/__pycache__/Auth.cpython-38.pyc
+-rw-r--r--   0        0        0     1034 2023-06-14 10:27:36.396543 eotdl-2023.6.14.post2/eotdl/src/usecases/auth/__pycache__/IsLogged.cpython-38.pyc
+-rw-r--r--   0        0        0     1059 2023-06-14 10:27:36.412543 eotdl-2023.6.14.post2/eotdl/src/usecases/auth/__pycache__/Logout.cpython-38.pyc
+-rw-r--r--   0        0        0      240 2023-06-14 10:27:36.344542 eotdl-2023.6.14.post2/eotdl/src/usecases/auth/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      951 2023-06-14 10:27:36.344542 eotdl-2023.6.14.post2/eotdl/src/usecases/auth/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0        0        0      725 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post2/eotdl/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      763 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      932 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0     1403 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/IngestLargeDataset.py
+-rw-r--r--   0        0        0     1595 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py
+-rw-r--r--   0        0        0      421 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0      940 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/UpdateDataset.py
+-rw-r--r--   0        0        0      168 2023-06-14 10:24:20.823993 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0     1406 2023-06-14 10:27:36.416543 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/DownloadDataset.cpython-38.pyc
+-rw-r--r--   0        0        0     1406 2023-06-14 10:27:36.416543 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/IngestDataset.cpython-38.pyc
+-rw-r--r--   0        0        0     1803 2023-06-14 10:27:36.416543 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/IngestLargeDataset.cpython-38.pyc
+-rw-r--r--   0        0        0     1913 2023-06-14 10:27:36.420543 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/IngestLargeDatasetParallel.cpython-38.pyc
+-rw-r--r--   0        0        0     1154 2023-06-14 10:27:36.416543 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/RetrieveDataset.cpython-38.pyc
+-rw-r--r--   0        0        0     1312 2023-06-14 10:27:36.416543 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/RetrieveDatasets.cpython-38.pyc
+-rw-r--r--   0        0        0     1501 2023-06-14 10:27:36.420543 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/UpdateDataset.cpython-38.pyc
+-rw-r--r--   0        0        0      355 2023-06-14 10:27:36.412543 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2156 2023-06-14 10:27:36.416543 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0        0        0     2168 2023-06-14 10:24:20.823993 eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/main.py
+-rw-r--r--   0        0        0      479 2023-06-14 10:24:20.823993 eotdl-2023.6.14.post2/eotdl/src/utils.py
+-rw-r--r--   0        0        0      277 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post2/eotdl/tools/__init__.py
+-rw-r--r--   0        0        0      391 2023-06-14 09:01:14.123571 eotdl-2023.6.14.post2/eotdl/tools/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      874 2023-06-14 09:01:14.123571 eotdl-2023.6.14.post2/eotdl/tools/__pycache__/stac.cpython-38.pyc
+-rw-r--r--   0        0        0      215 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post2/eotdl/tools/sen12floods/__init__.py
+-rw-r--r--   0        0        0      351 2023-06-14 09:01:14.259571 eotdl-2023.6.14.post2/eotdl/tools/sen12floods/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6462 2023-06-14 09:01:14.263571 eotdl-2023.6.14.post2/eotdl/tools/sen12floods/__pycache__/tools.cpython-38.pyc
+-rw-r--r--   0        0        0     8124 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post2/eotdl/tools/sen12floods/tools.py
+-rw-r--r--   0        0        0      636 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post2/eotdl/tools/stac.py
+-rw-r--r--   0        0        0      622 2023-06-14 10:31:39.945245 eotdl-2023.6.14.post2/pyproject.toml
+-rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 eotdl-2023.6.14.post2/setup.py
+-rw-r--r--   0        0        0      737 1970-01-01 00:00:00.000000 eotdl-2023.6.14.post2/PKG-INFO
```

### Comparing `eotdl-2023.6.14/eotdl/__init__.py` & `eotdl-2023.6.14.post2/eotdl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .curation import *
+# from .curation import *
 
 # from .curation import (SHFolderFormatter,
 #                        STACGenerator,
 #                        format_time_acquired,
 #                        STACIdParser,
 #                        StructuredParser,
 #                        UnestructuredParser,
```

### Comparing `eotdl-2023.6.14/eotdl/access/__pycache__/parameters.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/access/__pycache__/parameters.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/access/sentinelhub/__pycache__/client.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/access/sentinelhub/__pycache__/client.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/access/sentinelhub/__pycache__/utils.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/access/sentinelhub/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/access/sentinelhub/client.py` & `eotdl-2023.6.14.post2/eotdl/access/sentinelhub/client.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/access/sentinelhub/utils.py` & `eotdl-2023.6.14.post2/eotdl/access/sentinelhub/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/commands/__pycache__/auth.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/commands/__pycache__/auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/commands/__pycache__/datasets.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/commands/__pycache__/datasets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/commands/auth.py` & `eotdl-2023.6.14.post2/eotdl/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/commands/datasets.py` & `eotdl-2023.6.14.post2/eotdl/commands/datasets.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/__pycache__/formatters.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/curation/__pycache__/formatters.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/__pycache__/metadata.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/curation/__pycache__/metadata.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/formatters.py` & `eotdl-2023.6.14.post2/eotdl/curation/formatters.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/metadata.py` & `eotdl-2023.6.14.post2/eotdl/curation/metadata.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/__pycache__/dataframe.cpython-310.pyc` & `eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/dataframe.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/__pycache__/dataframe.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/dataframe.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/__pycache__/extensions.cpython-310.pyc` & `eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/extensions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/__pycache__/extensions.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/extensions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/__pycache__/parsers.cpython-310.pyc` & `eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/parsers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/__pycache__/parsers.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/parsers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/__pycache__/stac.cpython-310.pyc` & `eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/stac.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/__pycache__/stac.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/stac.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/__pycache__/utils.cpython-310.pyc` & `eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/__pycache__/utils.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/curation/stac/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/dataframe.py` & `eotdl-2023.6.14.post2/eotdl/curation/stac/dataframe.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/extensions.py` & `eotdl-2023.6.14.post2/eotdl/curation/stac/extensions.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/parsers.py` & `eotdl-2023.6.14.post2/eotdl/curation/stac/parsers.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/stac.py` & `eotdl-2023.6.14.post2/eotdl/curation/stac/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/curation/stac/utils.py` & `eotdl-2023.6.14.post2/eotdl/curation/stac/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/__pycache__/auth.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/__pycache__/auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/__pycache__/utils.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/errors/__pycache__/auth.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/errors/__pycache__/auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/repos/APIRepo.py` & `eotdl-2023.6.14.post2/eotdl/src/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/repos/AuthRepo.py` & `eotdl-2023.6.14.post2/eotdl/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/repos/__pycache__/APIRepo.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/repos/__pycache__/APIRepo.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/repos/__pycache__/AuthRepo.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/repos/__pycache__/AuthRepo.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/__pycache__/auth.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/usecases/__pycache__/auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/auth/Auth.py` & `eotdl-2023.6.14.post2/eotdl/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/auth/__pycache__/Auth.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/usecases/auth/__pycache__/Auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/auth/__pycache__/IsLogged.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/usecases/auth/__pycache__/IsLogged.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/auth/__pycache__/Logout.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/usecases/auth/__pycache__/Logout.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/auth/__pycache__/main.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/usecases/auth/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/auth/main.py` & `eotdl-2023.6.14.post2/eotdl/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/DownloadDataset.py` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/DownloadDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/IngestDataset.py` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/IngestDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/IngestLargeDataset.py` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/IngestLargeDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/UpdateDataset.py` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/UpdateDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/DownloadDataset.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/DownloadDataset.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/IngestDataset.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/IngestDataset.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/IngestLargeDataset.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/IngestLargeDataset.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/IngestLargeDatasetParallel.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/IngestLargeDatasetParallel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/RetrieveDataset.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/RetrieveDataset.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/RetrieveDatasets.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/RetrieveDatasets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/UpdateDataset.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/UpdateDataset.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/__pycache__/main.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/src/usecases/datasets/main.py` & `eotdl-2023.6.14.post2/eotdl/src/usecases/datasets/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/tools/__pycache__/stac.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/tools/__pycache__/stac.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/tools/sen12floods/__pycache__/tools.cpython-38.pyc` & `eotdl-2023.6.14.post2/eotdl/tools/sen12floods/__pycache__/tools.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/tools/sen12floods/tools.py` & `eotdl-2023.6.14.post2/eotdl/tools/sen12floods/tools.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/eotdl/tools/stac.py` & `eotdl-2023.6.14.post2/eotdl/tools/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14/pyproject.toml` & `eotdl-2023.6.14.post2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl"
-version = "2023.06.14"
+version = "2023.06.14-2"
 description = "Earth Observation Training Data Lab"
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl"}]
 
 [tool.poetry.scripts]
@@ -14,15 +14,14 @@
 python = "^3.8"
 typer = {extras = ["all"], version = "^0.7.0"}
 requests = "^2.28.2"
 pydantic = "^1.10.6"
 tqdm = "^4.65.0"
 pyjwt = "^2.6.0"
 
-
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-watch = "^4.2.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `eotdl-2023.6.14/setup.py` & `eotdl-2023.6.14.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['eotdl = eotdl.main:app']}
 
 setup_kwargs = {
     'name': 'eotdl',
-    'version': '2023.6.14',
+    'version': '2023.6.14.post2',
     'description': 'Earth Observation Training Data Lab',
     'long_description': '# eotdl \n\nThis is the main library for EOTDL.\n\n',
     'author': 'EarthPulse',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `eotdl-2023.6.14/PKG-INFO` & `eotdl-2023.6.14.post2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl
-Version: 2023.6.14
+Version: 2023.6.14.post2
 Summary: Earth Observation Training Data Lab
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

