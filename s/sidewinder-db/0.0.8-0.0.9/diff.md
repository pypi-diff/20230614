# Comparing `tmp/sidewinder-db-0.0.8.tar.gz` & `tmp/sidewinder-db-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidewinder-db-0.0.8.tar", last modified: Fri Feb 17 22:14:52 2023, max compression
+gzip compressed data, was "sidewinder-db-0.0.9.tar", last modified: Wed Mar  1 15:57:41 2023, max compression
```

## Comparing `sidewinder-db-0.0.8.tar` & `sidewinder-db-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:14:52.731318 sidewinder-db-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-17 22:14:41.000000 sidewinder-db-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-02-17 22:14:52.731318 sidewinder-db-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-02-17 22:14:41.000000 sidewinder-db-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-17 22:14:41.000000 sidewinder-db-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 22:14:52.731318 sidewinder-db-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:14:52.731318 sidewinder-db-0.0.8/sidewinder/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-17 22:14:41.000000 sidewinder-db-0.0.8/sidewinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-02-17 22:14:41.000000 sidewinder-db-0.0.8/sidewinder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-17 22:14:41.000000 sidewinder-db-0.0.8/sidewinder/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-17 22:14:41.000000 sidewinder-db-0.0.8/sidewinder/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:14:52.731318 sidewinder-db-0.0.8/sidewinder/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 22:14:41.000000 sidewinder-db-0.0.8/sidewinder/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-02-17 22:14:41.000000 sidewinder-db-0.0.8/sidewinder/parser/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    22295 2023-02-17 22:14:41.000000 sidewinder-db-0.0.8/sidewinder/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-02-17 22:14:41.000000 sidewinder-db-0.0.8/sidewinder/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-02-17 22:14:41.000000 sidewinder-db-0.0.8/sidewinder/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:14:52.731318 sidewinder-db-0.0.8/sidewinder_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-02-17 22:14:52.000000 sidewinder-db-0.0.8/sidewinder_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-17 22:14:52.000000 sidewinder-db-0.0.8/sidewinder_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 22:14:52.000000 sidewinder-db-0.0.8/sidewinder_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-17 22:14:52.000000 sidewinder-db-0.0.8/sidewinder_db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-17 22:14:52.000000 sidewinder-db-0.0.8/sidewinder_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-17 22:14:52.000000 sidewinder-db-0.0.8/sidewinder_db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:57:41.943916 sidewinder-db-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-01 15:57:31.000000 sidewinder-db-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-03-01 15:57:41.943916 sidewinder-db-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-03-01 15:57:31.000000 sidewinder-db-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-01 15:57:31.000000 sidewinder-db-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 15:57:41.943916 sidewinder-db-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:57:41.943916 sidewinder-db-0.0.9/sidewinder/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-01 15:57:31.000000 sidewinder-db-0.0.9/sidewinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-03-01 15:57:31.000000 sidewinder-db-0.0.9/sidewinder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-01 15:57:31.000000 sidewinder-db-0.0.9/sidewinder/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-01 15:57:31.000000 sidewinder-db-0.0.9/sidewinder/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:57:41.943916 sidewinder-db-0.0.9/sidewinder/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:57:31.000000 sidewinder-db-0.0.9/sidewinder/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-03-01 15:57:31.000000 sidewinder-db-0.0.9/sidewinder/parser/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22295 2023-03-01 15:57:31.000000 sidewinder-db-0.0.9/sidewinder/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-03-01 15:57:31.000000 sidewinder-db-0.0.9/sidewinder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-03-01 15:57:31.000000 sidewinder-db-0.0.9/sidewinder/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:57:41.943916 sidewinder-db-0.0.9/sidewinder_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-03-01 15:57:41.000000 sidewinder-db-0.0.9/sidewinder_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-01 15:57:41.000000 sidewinder-db-0.0.9/sidewinder_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 15:57:41.000000 sidewinder-db-0.0.9/sidewinder_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-01 15:57:41.000000 sidewinder-db-0.0.9/sidewinder_db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-01 15:57:41.000000 sidewinder-db-0.0.9/sidewinder_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-01 15:57:41.000000 sidewinder-db-0.0.9/sidewinder_db.egg-info/top_level.txt
```

### Comparing `sidewinder-db-0.0.8/LICENSE` & `sidewinder-db-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sidewinder-db-0.0.8/PKG-INFO` & `sidewinder-db-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidewinder-db
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python-based Distributed Database
 Author-email: Philip Moore <prmoore77@hotmail.com>
 License: MIT License
         
         Copyright (c) 2022 prmoore77
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -79,20 +79,20 @@
 
 #### Alternative installation from PyPi
 ```shell
 pip install sidewinder-db
 ```
 
 ### DuckDB CLI
-Install DuckDB CLI version [0.6.1](https://github.com/duckdb/duckdb/releases/tag/v0.6.1) - and make sure the executable is on your PATH.
+Install DuckDB CLI version [0.7.1](https://github.com/duckdb/duckdb/releases/tag/v0.7.1) - and make sure the executable is on your PATH.
 
 Platform Downloads:   
-[Linux x86-64](https://github.com/duckdb/duckdb/releases/download/v0.6.1/duckdb_cli-linux-amd64.zip)   
-[Linux arm64 (aarch64)](https://github.com/duckdb/duckdb/releases/download/v0.6.1/duckdb_cli-linux-aarch64.zip)   
-[MacOS Universal](https://github.com/duckdb/duckdb/releases/download/v0.6.1/duckdb_cli-osx-universal.zip)   
+[Linux x86-64](https://github.com/duckdb/duckdb/releases/download/v0.7.1/duckdb_cli-linux-amd64.zip)   
+[Linux arm64 (aarch64)](https://github.com/duckdb/duckdb/releases/download/v0.7.1/duckdb_cli-linux-aarch64.zip)   
+[MacOS Universal](https://github.com/duckdb/duckdb/releases/download/v0.7.1/duckdb_cli-osx-universal.zip)   
 
 ## Generate source sample TPC-H (Scale Factor 1) data (only possible from repo currently, not PyPi package)
 Note: If running on MacOS - you'll need to have [homebrew](https://brew.sh) installed, then install coreutils with:  
 ```brew install coreutils```
 
 After that - you can create sample TPC-H source data for Scale Factor 1 (in parquet format) - run:
 ```
```

### Comparing `sidewinder-db-0.0.8/README.md` & `sidewinder-db-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,20 +42,20 @@
 
 #### Alternative installation from PyPi
 ```shell
 pip install sidewinder-db
 ```
 
 ### DuckDB CLI
-Install DuckDB CLI version [0.6.1](https://github.com/duckdb/duckdb/releases/tag/v0.6.1) - and make sure the executable is on your PATH.
+Install DuckDB CLI version [0.7.1](https://github.com/duckdb/duckdb/releases/tag/v0.7.1) - and make sure the executable is on your PATH.
 
 Platform Downloads:   
-[Linux x86-64](https://github.com/duckdb/duckdb/releases/download/v0.6.1/duckdb_cli-linux-amd64.zip)   
-[Linux arm64 (aarch64)](https://github.com/duckdb/duckdb/releases/download/v0.6.1/duckdb_cli-linux-aarch64.zip)   
-[MacOS Universal](https://github.com/duckdb/duckdb/releases/download/v0.6.1/duckdb_cli-osx-universal.zip)   
+[Linux x86-64](https://github.com/duckdb/duckdb/releases/download/v0.7.1/duckdb_cli-linux-amd64.zip)   
+[Linux arm64 (aarch64)](https://github.com/duckdb/duckdb/releases/download/v0.7.1/duckdb_cli-linux-aarch64.zip)   
+[MacOS Universal](https://github.com/duckdb/duckdb/releases/download/v0.7.1/duckdb_cli-osx-universal.zip)   
 
 ## Generate source sample TPC-H (Scale Factor 1) data (only possible from repo currently, not PyPi package)
 Note: If running on MacOS - you'll need to have [homebrew](https://brew.sh) installed, then install coreutils with:  
 ```brew install coreutils```
 
 After that - you can create sample TPC-H source data for Scale Factor 1 (in parquet format) - run:
 ```
```

### Comparing `sidewinder-db-0.0.8/pyproject.toml` & `sidewinder-db-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]  # list of folders that contain the packages (["."] by default)
 include = ["sidewinder*"]  # package names should match these glob patterns (["*"] by default)
 
 [project]
 name = "sidewinder-db"
-version = "0.0.8"
+version = "0.0.9"
 description = "A Python-based Distributed Database"
 readme = "README.md"
 authors = [{ name = "Philip Moore", email = "prmoore77@hotmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -20,15 +20,15 @@
 ]
 keywords = ["sidwinder", "sidewinder-db", "database", "distributed", "shard"]
 dependencies = [
     "boto3==1.26.*",
     "botocore==1.29.*",
     "click==8.1.3",
     "codetiming==1.4.*",
-    "duckdb==0.7.0",
+    "duckdb==0.7.1",
     "duckdb-engine==0.6.*",
     "jmespath==1.0.*",
     "mgzip==0.2.*",
     "munch==2.5.*",
     "numpy==1.23.*",
     "pandas==1.5.*",
     "pglast==3.*",
@@ -55,15 +55,15 @@
 
 [project.scripts]
 sidewinder-server = "sidewinder.server:main"
 sidewinder-worker = "sidewinder.worker:main"
 sidewinder-client = "sidewinder.client:main"
 
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

### Comparing `sidewinder-db-0.0.8/sidewinder/client.py` & `sidewinder-db-0.0.9/sidewinder/client.py`

 * *Files identical despite different names*

### Comparing `sidewinder-db-0.0.8/sidewinder/parser/query.py` & `sidewinder-db-0.0.9/sidewinder/parser/query.py`

 * *Files identical despite different names*

### Comparing `sidewinder-db-0.0.8/sidewinder/server.py` & `sidewinder-db-0.0.9/sidewinder/server.py`

 * *Files identical despite different names*

### Comparing `sidewinder-db-0.0.8/sidewinder/utils.py` & `sidewinder-db-0.0.9/sidewinder/utils.py`

 * *Files identical despite different names*

### Comparing `sidewinder-db-0.0.8/sidewinder/worker.py` & `sidewinder-db-0.0.9/sidewinder/worker.py`

 * *Files identical despite different names*

### Comparing `sidewinder-db-0.0.8/sidewinder_db.egg-info/PKG-INFO` & `sidewinder-db-0.0.9/sidewinder_db.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidewinder-db
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python-based Distributed Database
 Author-email: Philip Moore <prmoore77@hotmail.com>
 License: MIT License
         
         Copyright (c) 2022 prmoore77
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -79,20 +79,20 @@
 
 #### Alternative installation from PyPi
 ```shell
 pip install sidewinder-db
 ```
 
 ### DuckDB CLI
-Install DuckDB CLI version [0.6.1](https://github.com/duckdb/duckdb/releases/tag/v0.6.1) - and make sure the executable is on your PATH.
+Install DuckDB CLI version [0.7.1](https://github.com/duckdb/duckdb/releases/tag/v0.7.1) - and make sure the executable is on your PATH.
 
 Platform Downloads:   
-[Linux x86-64](https://github.com/duckdb/duckdb/releases/download/v0.6.1/duckdb_cli-linux-amd64.zip)   
-[Linux arm64 (aarch64)](https://github.com/duckdb/duckdb/releases/download/v0.6.1/duckdb_cli-linux-aarch64.zip)   
-[MacOS Universal](https://github.com/duckdb/duckdb/releases/download/v0.6.1/duckdb_cli-osx-universal.zip)   
+[Linux x86-64](https://github.com/duckdb/duckdb/releases/download/v0.7.1/duckdb_cli-linux-amd64.zip)   
+[Linux arm64 (aarch64)](https://github.com/duckdb/duckdb/releases/download/v0.7.1/duckdb_cli-linux-aarch64.zip)   
+[MacOS Universal](https://github.com/duckdb/duckdb/releases/download/v0.7.1/duckdb_cli-osx-universal.zip)   
 
 ## Generate source sample TPC-H (Scale Factor 1) data (only possible from repo currently, not PyPi package)
 Note: If running on MacOS - you'll need to have [homebrew](https://brew.sh) installed, then install coreutils with:  
 ```brew install coreutils```
 
 After that - you can create sample TPC-H source data for Scale Factor 1 (in parquet format) - run:
 ```
```

