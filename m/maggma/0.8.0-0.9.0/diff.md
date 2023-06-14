# Comparing `tmp/maggma-0.8.0.tar.gz` & `tmp/maggma-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/maggma-0.8.0.tar", last modified: Wed Aug 22 22:13:14 2018, max compression
+gzip compressed data, was "dist/maggma-0.9.0.tar", last modified: Mon Oct  1 21:00:00 2018, max compression
```

## Comparing `maggma-0.8.0.tar` & `maggma-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 dwinston   (501) staff       (20)        0 2018-08-22 22:13:14.000000 maggma-0.8.0/
-drwxr-xr-x   0 dwinston   (501) staff       (20)        0 2018-08-22 22:13:14.000000 maggma-0.8.0/maggma/
--rw-r--r--   0 dwinston   (501) staff       (20)       38 2018-08-22 22:12:07.000000 maggma-0.8.0/maggma/__init__.py
--rw-r--r--   0 dwinston   (501) staff       (20)    18830 2018-06-28 00:04:47.000000 maggma-0.8.0/maggma/advanced_stores.py
--rw-r--r--   0 dwinston   (501) staff       (20)     3192 2018-06-28 00:04:47.000000 maggma-0.8.0/maggma/builder.py
-drwxr-xr-x   0 dwinston   (501) staff       (20)        0 2018-08-22 22:13:14.000000 maggma-0.8.0/maggma/cli/
--rw-r--r--   0 dwinston   (501) staff       (20)       15 2018-06-28 00:04:47.000000 maggma-0.8.0/maggma/cli/__init__.py
--rw-r--r--   0 dwinston   (501) staff       (20)     2049 2018-08-22 22:11:04.000000 maggma-0.8.0/maggma/cli/mrun.py
--rw-r--r--   0 dwinston   (501) staff       (20)     1385 2018-08-22 22:11:04.000000 maggma-0.8.0/maggma/cli/test_mrun.py
-drwxr-xr-x   0 dwinston   (501) staff       (20)        0 2018-08-22 22:13:14.000000 maggma-0.8.0/maggma/examples/
--rw-r--r--   0 dwinston   (501) staff       (20)        0 2018-08-22 22:11:04.000000 maggma-0.8.0/maggma/examples/__init__.py
--rw-r--r--   0 dwinston   (501) staff       (20)    10265 2018-08-22 22:11:04.000000 maggma-0.8.0/maggma/examples/builders.py
--rwxr-xr-x   0 dwinston   (501) staff       (20)     2886 2018-08-22 22:11:04.000000 maggma-0.8.0/maggma/examples/runner_sample.py
-drwxr-xr-x   0 dwinston   (501) staff       (20)        0 2018-08-22 22:13:14.000000 maggma-0.8.0/maggma/examples/tests/
--rw-r--r--   0 dwinston   (501) staff       (20)        0 2018-08-22 22:11:04.000000 maggma-0.8.0/maggma/examples/tests/__init__.py
--rw-r--r--   0 dwinston   (501) staff       (20)     4017 2018-08-22 22:11:04.000000 maggma-0.8.0/maggma/examples/tests/test_copybuilder.py
--rw-r--r--   0 dwinston   (501) staff       (20)     2307 2018-06-28 00:04:47.000000 maggma-0.8.0/maggma/helpers.py
--rw-r--r--   0 dwinston   (501) staff       (20)    17521 2018-08-22 22:11:04.000000 maggma-0.8.0/maggma/runner.py
--rw-r--r--   0 dwinston   (501) staff       (20)    26412 2018-08-22 22:11:04.000000 maggma-0.8.0/maggma/stores.py
-drwxr-xr-x   0 dwinston   (501) staff       (20)        0 2018-08-22 22:13:14.000000 maggma-0.8.0/maggma/tests/
--rw-r--r--   0 dwinston   (501) staff       (20)       15 2018-06-28 00:04:47.000000 maggma-0.8.0/maggma/tests/__init__.py
--rw-r--r--   0 dwinston   (501) staff       (20)     1386 2018-06-28 00:04:47.000000 maggma-0.8.0/maggma/tests/mpi_test.py
--rw-r--r--   0 dwinston   (501) staff       (20)    12275 2018-06-28 00:04:47.000000 maggma-0.8.0/maggma/tests/test_advanced_stores.py
--rw-r--r--   0 dwinston   (501) staff       (20)     7704 2018-08-22 22:11:04.000000 maggma-0.8.0/maggma/tests/test_runner.py
--rw-r--r--   0 dwinston   (501) staff       (20)     8693 2018-06-28 00:04:47.000000 maggma-0.8.0/maggma/tests/test_stores.py
--rw-r--r--   0 dwinston   (501) staff       (20)     1523 2018-06-28 00:04:47.000000 maggma-0.8.0/maggma/tests/test_utils.py
--rw-r--r--   0 dwinston   (501) staff       (20)     2070 2018-06-28 00:04:47.000000 maggma-0.8.0/maggma/tests/test_validator.py
--rw-r--r--   0 dwinston   (501) staff       (20)     7402 2018-08-22 22:11:04.000000 maggma-0.8.0/maggma/utils.py
--rw-r--r--   0 dwinston   (501) staff       (20)     3412 2018-06-28 00:04:47.000000 maggma-0.8.0/maggma/validator.py
-drwxr-xr-x   0 dwinston   (501) staff       (20)        0 2018-08-22 22:13:14.000000 maggma-0.8.0/maggma.egg-info/
--rw-r--r--   0 dwinston   (501) staff       (20)        1 2018-08-22 22:13:14.000000 maggma-0.8.0/maggma.egg-info/dependency_links.txt
--rw-r--r--   0 dwinston   (501) staff       (20)       47 2018-08-22 22:13:14.000000 maggma-0.8.0/maggma.egg-info/entry_points.txt
--rw-r--r--   0 dwinston   (501) staff       (20)        1 2018-07-13 18:07:22.000000 maggma-0.8.0/maggma.egg-info/not-zip-safe
--rw-r--r--   0 dwinston   (501) staff       (20)      860 2018-08-22 22:13:14.000000 maggma-0.8.0/maggma.egg-info/PKG-INFO
--rw-r--r--   0 dwinston   (501) staff       (20)      162 2018-08-22 22:13:14.000000 maggma-0.8.0/maggma.egg-info/requires.txt
--rw-r--r--   0 dwinston   (501) staff       (20)      812 2018-08-22 22:13:14.000000 maggma-0.8.0/maggma.egg-info/SOURCES.txt
--rw-r--r--   0 dwinston   (501) staff       (20)        7 2018-08-22 22:13:14.000000 maggma-0.8.0/maggma.egg-info/top_level.txt
--rw-r--r--   0 dwinston   (501) staff       (20)      860 2018-08-22 22:13:14.000000 maggma-0.8.0/PKG-INFO
--rw-r--r--   0 dwinston   (501) staff       (20)       58 2018-06-28 00:04:47.000000 maggma-0.8.0/README.md
--rw-r--r--   0 dwinston   (501) staff       (20)       38 2018-08-22 22:13:14.000000 maggma-0.8.0/setup.cfg
--rw-r--r--   0 dwinston   (501) staff       (20)     1753 2018-08-22 22:12:07.000000 maggma-0.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-01 21:00:00.000000 maggma-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       58 2018-10-01 20:58:46.000000 maggma-0.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1752 2018-10-01 20:58:46.000000 maggma-0.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-01 21:00:00.000000 maggma-0.9.0/maggma/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-01 21:00:00.000000 maggma-0.9.0/maggma/cli/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       15 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/cli/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/cli/mrun.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1385 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/cli/test_mrun.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26411 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/stores.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-01 21:00:00.000000 maggma-0.9.0/maggma/examples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10698 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/examples/builders.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/examples/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-01 21:00:00.000000 maggma-0.9.0/maggma/examples/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/examples/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4017 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/examples/tests/test_copybuilder.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2886 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/examples/runner_sample.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2307 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17842 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/runner.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-01 21:00:00.000000 maggma-0.9.0/maggma/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7704 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/tests/test_runner.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16277 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/tests/test_advanced_stores.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9099 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/tests/test_stores.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1815 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/tests/test_validator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       15 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1386 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/tests/mpi_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1523 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/tests/test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24350 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/advanced_stores.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7721 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3192 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/builder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3283 2018-10-01 20:58:46.000000 maggma-0.9.0/maggma/validator.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-01 21:00:00.000000 maggma-0.9.0/maggma.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2018-10-01 21:00:00.000000 maggma-0.9.0/maggma.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-10-01 21:00:00.000000 maggma-0.9.0/maggma.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      161 2018-10-01 21:00:00.000000 maggma-0.9.0/maggma.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      860 2018-10-01 21:00:00.000000 maggma-0.9.0/maggma.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-10-01 21:00:00.000000 maggma-0.9.0/maggma.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       47 2018-10-01 21:00:00.000000 maggma-0.9.0/maggma.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      812 2018-10-01 21:00:00.000000 maggma-0.9.0/maggma.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2018-10-01 21:00:00.000000 maggma-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      860 2018-10-01 21:00:00.000000 maggma-0.9.0/PKG-INFO
```

### Comparing `maggma-0.8.0/maggma/advanced_stores.py` & `maggma-0.9.0/maggma/advanced_stores.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # coding: utf-8
 """
 Advanced Stores for behavior outside normal access patterns
 """
 import os
 import hvac
 import json
-import boto3
-import botocore
 import zlib
 from datetime import datetime
 
+from pydash import get, set_
 from maggma.stores import Store, MongoStore, StoreError, Mongolike
 from maggma.utils import lazy_substitute, substitute
 from mongogrant import Client
 from mongogrant.client import check
 from mongogrant.config import Config
 from monty.json import jsanitize
 from monty.functools import lru_cache
+from pymongo import MongoClient
+
+try:
+    import boto3
+    import botocore
+    boto_import = True
+except ImportError:
+    boto_import = False
 
 
 class MongograntStore(Mongolike, Store):
     """Initialize a Store with a mongogrant "<role>:<host>/<db>." spec.
 
     This class does not subclass MongoStore, though it aims to reproduce
     relevant functionality through method delegation, e.g. groupby.
@@ -63,17 +70,17 @@
                 client = Client()
             db = client.db(self.mongogrant_spec)
             self._collection = db[self.collection_name]
 
     def __hash__(self):
         return hash((self.mongogrant_spec, self.collection_name, self.lu_field))
 
-    def groupby(self, keys, properties=None, criteria=None, **kwargs):
+    def groupby(self, keys, criteria=None, properties=None, **kwargs):
         return MongoStore.groupby(
-            self, keys, properties=None, criteria=None, **kwargs)
+            self, keys, criteria=None, properties=None, **kwargs)
 
 
 class VaultStore(MongoStore):
     """
     Extends MongoStore to read credentials out of Vault server
     and uses these values to initialize MongoStore instance
     """
@@ -139,39 +146,39 @@
         # Given the internal key tells us what the external key is
         self.reverse_aliases = {v: k for k, v in aliases.items()}
         self.kwargs = kwargs
 
         kwargs.update({"lu_field": store.lu_field, "lu_type": store.lu_type})
         super(AliasingStore, self).__init__(**kwargs)
 
-    def query(self, properties=None, criteria=None, **kwargs):
+    def query(self, criteria=None, properties=None, **kwargs):
 
         if isinstance(properties, list):
             properties = {p: 1 for p in properties}
 
         criteria = criteria if criteria else {}
         substitute(properties, self.reverse_aliases)
         lazy_substitute(criteria, self.reverse_aliases)
-        for d in self.store.query(properties, criteria, **kwargs):
+        for d in self.store.query(properties=properties, criteria=criteria, **kwargs):
             substitute(d, self.aliases)
             yield d
 
-    def query_one(self, properties=None, criteria=None, **kwargs):
+    def query_one(self, criteria=None, properties=None, **kwargs):
 
         if isinstance(properties, list):
             properties = {p: 1 for p in properties}
 
         criteria = criteria if criteria else {}
         substitute(properties, self.reverse_aliases)
         lazy_substitute(criteria, self.reverse_aliases)
-        d = self.store.query_one(properties, criteria, **kwargs)
+        d = self.store.query_one(properties=properties, criteria=criteria, **kwargs)
         substitute(d, self.aliases)
         return d
 
-    def distinct(self, key, criteria=None, **kwargs):
+    def distinct(self, key, criteria=None, all_exist=True, **kwargs):
         if isinstance(key, list):
             criteria = criteria if criteria else {}
             # Update to ensure keys are there
             if all_exist:
                 criteria.update({k: {"$exists": True} for k in key if k not in criteria})
 
             results = []
@@ -181,15 +188,15 @@
 
         else:
             criteria = criteria if criteria else {}
             lazy_substitute(criteria, self.reverse_aliases)
             key = self.aliases[key] if key in self.aliases else key
             return self.collection.distinct(key, filter=criteria, **kwargs)
 
-    def groupby(self, keys, properties=None, criteria=None, **kwargs):
+    def groupby(self, keys, criteria=None, properties=None, **kwargs):
         # Convert to a list
         keys = keys if isinstance(keys, list) else [keys]
 
         # Make the aliasing transformations on keys
         keys = [self.aliases[k] if k in self.aliases else k for k in keys]
 
         # Update criteria and properties based on aliases
@@ -250,27 +257,27 @@
     def sbx_criteria(self):
         if self.exclusive:
             return {"sbxn": self.sandbox}
         else:
             return {"$or": [{"sbxn": {"$in": [self.sandbox]}},
                             {"sbxn": {"$exists": False}}]}
 
-    def query(self, properties=None, criteria=None, **kwargs):
+    def query(self, criteria=None, properties=None, **kwargs):
         criteria = dict(**criteria, **self.sbx_criteria) if criteria else self.sbx_criteria
         return self.store.query(properties=properties, criteria=criteria, **kwargs)
 
-    def query_one(self, properties=None, criteria=None, **kwargs):
+    def query_one(self, criteria=None, properties=None, **kwargs):
         criteria = dict(**criteria, **self.sbx_criteria) if criteria else self.sbx_criteria
         return self.store.query_one(properties=properties, criteria=criteria, **kwargs)
 
     def distinct(self, key, criteria=None, **kwargs):
         criteria = dict(**criteria, **self.sbx_criteria) if criteria else self.sbx_criteria
         return self.store.distinct(key=key, criteria=criteria, **kwargs)
 
-    def groupby(self, keys, properties=None, criteria=None, **kwargs):
+    def groupby(self, keys, criteria=None, properties=None, **kwargs):
         criteria = dict(**criteria, **self.sbx_criteria) if criteria else self.sbx_criteria
 
         return self.store.groupby(keys=keys, properties=properties, criteria=criteria, **kwargs)
 
     def update(self, docs, update_lu=True, key=None):
         for d in docs:
             if "sbxn" in d:
@@ -303,14 +310,17 @@
     def __init__(self, index, bucket, **kwargs):
         """
         Initializes an S3 Store
         Args:
             index (Store): a store to use to index the S3 Bucket
             bucket (str) : name of the bucket
         """
+        if not boto_import:
+            raise ValueError("boto not available, please install boto3 to "
+                             "use AmazonS3Store")
         self.index = index
         self.bucket = bucket
         self.s3 = None
         self.s3_bucket = None
         # Force the key to be the same as the index
         kwargs["key"] = index.key
         super(AmazonS3Store, self).__init__(**kwargs)
@@ -328,15 +338,15 @@
         self.index.close()
 
     @property
     def collection(self):
         # For now returns the index collection since that is what we would "search" on
         return self.index
 
-    def query(self, properties=None, criteria=None, **kwargs):
+    def query(self, criteria=None, properties=None, **kwargs):
         """
         Function that gets data from Amazon S3. This store ignores all
         property projections as its designed for whole document access
 
         Args:
             properties (list or dict): This will be ignored by the S3
                 Store
@@ -356,15 +366,15 @@
                     break
 
             if f.get("compression", "") is "zlib":
                 data = zlib.decompress(data)
 
             yield json.loads(data)
 
-    def query_one(self, properties=None, criteria=None, **kwargs):
+    def query_one(self, criteria=None, properties=None, **kwargs):
         """
         Function that gets a single document from Amazon S3. This store
         ignores all property projections as its designed for whole
         document access
 
         Args:
             properties (list or dict): This will be ignored by the S3
@@ -404,23 +414,23 @@
             all_exist (bool): whether to ensure all keys in list exist
                 in each document, defaults to False
             **kwargs (kwargs): kwargs corresponding to collection.distinct
         """
         # Index is a store so it should have its own distinct function
         return self.index.distinct(key, filter=criteria, **kwargs)
 
-    def groupby(self, keys, properties=None, criteria=None, **kwargs):
+    def groupby(self, keys, criteria=None, properties=None, **kwargs):
         """
         Simple grouping function that will group documents
         by keys. Only searches the index collection
 
         Args:
             keys (list or string): fields to group documents
-            properties (list): properties to return in grouped documents
             criteria (dict): filter for documents to group
+            properties (list): properties to return in grouped documents
             allow_disk_use (bool): whether to allow disk use in aggregation
 
         Returns:
             command cursor corresponding to grouped documents
 
             elements of the command cursor have the structure:
             {'_id': {"KEY_1": value_1, "KEY_2": value_2 ...,
@@ -505,7 +515,147 @@
         """
         index_docs = []
         for file in self.s3_bucket.objects.all():
             # TODO: Transform the data back from strings and remove AWS S3 specific keys
             index_docs.append(file.metadata)
 
         self.index.update(index_docs)
+
+
+class JointStore(Store):
+    """Store corresponding to multiple collections, uses lookup to join"""
+    def __init__(self, database, collection_names, host="localhost",
+                 port=27017, username="", password="", master=None, **kwargs):
+        self.database = database
+        self.collection_names = collection_names
+        self.host = host
+        self.port = port
+        self.username = username
+        self.password = password
+        self._collection = None
+        self.master = master or collection_names[0]
+        self.kwargs = kwargs
+        super(JointStore, self).__init__(**kwargs)
+
+    def connect(self, force_reset=False):
+        conn = MongoClient(self.host, self.port)
+        db = conn[self.database]
+        if self.username is not "":
+            db.authenticate(self.username, self.password)
+        self._collection = db[self.master]
+
+    def close(self):
+        self.collection.database.client.close()
+
+    @property
+    def collection(self):
+        return self._collection
+
+    @property
+    def nonmaster_names(self):
+        return list(set(self.collection_names) - {self.master})
+
+    def query(self, criteria=None, properties=None, **kwargs):
+        pipeline = self._get_pipeline(criteria=criteria, properties=properties)
+        return self.collection.aggregate(pipeline, **kwargs)
+
+    @property
+    def last_updated(self):
+        lus = []
+        for cname in self.collection_names:
+            lu = MongoStore.from_collection(
+                self.collection.database[cname],
+                lu_field=self.lu_field).last_updated
+            lus.append(lu)
+        return max(lus)
+
+    # TODO: implement update?
+    def update(self, docs, update_lu=True, key=None, **kwargs):
+        raise NotImplementedError("No update method for JointStore")
+
+    def _get_store_by_name(self, name):
+        return MongoStore.from_collection(self.collection.database[name])
+
+    def distinct(self, key, criteria=None, all_exist=True, **kwargs):
+        g_key = key if isinstance(key, list) else [key]
+        if all_exist:
+            criteria = criteria or {}
+            criteria.update({k: {"$exists": True} for k in g_key
+                             if k not in criteria})
+        cursor = self.groupby(g_key, criteria=criteria, **kwargs)
+        if isinstance(key, list):
+            return [d['_id'] for d in cursor]
+        else:
+            return [get(d['_id'], key) for d in cursor]
+
+    def ensure_index(self, key, unique=False, **kwargs):
+        raise NotImplementedError("No ensure_index method for JointStore")
+
+    def _get_pipeline(self, criteria=None, properties=None):
+        """
+        Gets the aggregation pipeline for query and query_one
+
+        Args:
+            properties: properties to be returned
+            criteria: criteria to filter by
+
+        Returns:
+            list of aggregation operators
+        """
+        pipeline = []
+        for cname in self.collection_names:
+            if cname is not self.master:
+                pipeline.append({
+                    "$lookup": {"from": cname, "localField": self.key,
+                                "foreignField": self.key, "as": cname}})
+                pipeline.append({
+                    "$unwind": {"path": "${}".format(cname),
+                                "preserveNullAndEmptyArrays": True}})
+
+        # Do projection for max last_updated
+        lu_max_fields = ["${}".format(self.lu_field)]
+        lu_max_fields.extend(["${}.{}".format(cname, self.lu_field)
+                              for cname in self.collection_names])
+        lu_proj = {self.lu_field: {"$max": lu_max_fields}}
+        pipeline.append({"$addFields": lu_proj})
+
+        if criteria:
+            pipeline.append({"$match": criteria})
+        if isinstance(properties, list):
+            properties = {k: 1 for k in properties}
+        if properties:
+            pipeline.append({"$project": properties})
+        return pipeline
+
+    def groupby(self, keys, criteria=None, properties=None, **kwargs):
+        pipeline = self._get_pipeline(criteria=criteria, properties=properties)
+        if not isinstance(keys, list):
+            keys = [keys]
+        group_id = {}
+        for key in keys:
+            set_(group_id, key, "${}".format(key))
+        pipeline.append({"$group": {"_id": group_id,
+                                    "docs": {"$push": "$$ROOT"}}})
+
+        return self.collection.aggregate(pipeline, **kwargs)
+
+    def query_one(self, criteria=None, properties=None, **kwargs):
+        """
+        Get one document
+
+        Args:
+            properties([str] or {}): properties to return in query
+            criteria ({}): filter for matching
+            **kwargs: kwargs for collection.aggregate
+
+        Returns:
+            single document
+        """
+        # TODO: maybe adding explicit limit in agg pipeline is better as below?
+        # pipeline = self._get_pipeline(properties, criteria)
+        # pipeline.append({"$limit": 1})
+        query = self.query(criteria=criteria, properties=properties, **kwargs)
+        try:
+            doc = query.next()
+            return doc
+        except StopIteration:
+            return None
```

### Comparing `maggma-0.8.0/maggma/builder.py` & `maggma-0.9.0/maggma/builder.py`

 * *Files identical despite different names*

### Comparing `maggma-0.8.0/maggma/cli/mrun.py` & `maggma-0.9.0/maggma/cli/mrun.py`

 * *Files identical despite different names*

### Comparing `maggma-0.8.0/maggma/cli/test_mrun.py` & `maggma-0.9.0/maggma/cli/test_mrun.py`

 * *Files identical despite different names*

### Comparing `maggma-0.8.0/maggma/examples/builders.py` & `maggma-0.9.0/maggma/examples/builders.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,19 +18,17 @@
 
     Called should ensure [(lu_field, -1),(key, 1)] compound index on both source
     and target.
 
     """
     keys_updated = set()  # Handle non-unique keys, e.g. for GroupBuilder.
     cursor_source = source.query(
-        properties=[source.key, source.lu_field],
-        sort=[(source.lu_field, -1), (source.key, 1)])
+        properties=[source.key, source.lu_field], sort=[(source.lu_field, -1), (source.key, 1)])
     cursor_target = target.query(
-        properties=[target.key, target.lu_field],
-        sort=[(target.lu_field, -1), (target.key, 1)])
+        properties=[target.key, target.lu_field], sort=[(target.lu_field, -1), (target.key, 1)])
     tdoc = next(cursor_target, None)
     for sdoc in cursor_source:
         if tdoc is None:
             keys_updated.add(sdoc[source.key])
             continue
 
         if tdoc[target.key] == sdoc[source.key]:
@@ -46,24 +44,21 @@
     """Return criteria to pass to `source.query` to get items."""
     index_checks = [confirm_field_index(target, target.key)]
     if incremental:
         # Ensure [(lu_field, -1), (key, 1)] index on both source and target
         for store in (source, target):
             info = store.collection.index_information().values()
             index_checks.append(
-                any(spec == [(store.lu_field, -1), (store.key, 1)]
-                    for spec in (index['key'] for index in info)))
+                any(spec == [(store.lu_field, -1), (store.key, 1)] for spec in (index['key'] for index in info)))
     if not all(index_checks):
-        index_warning = (
-            "Missing one or more important indices on stores. "
-            "Performance for large stores may be severely degraded. "
-            "Ensure indices on target.key and "
-            "[(store.lu_field, -1), (store.key, 1)] "
-            "for each of source and target."
-        )
+        index_warning = ("Missing one or more important indices on stores. "
+                         "Performance for large stores may be severely degraded. "
+                         "Ensure indices on target.key and "
+                         "[(store.lu_field, -1), (store.key, 1)] "
+                         "for each of source and target.")
         if logger:
             logger.warning(index_warning)
 
     criteria = {}
     if query:
         criteria.update(query)
     if incremental:
@@ -72,93 +67,97 @@
         keys_updated = source_keys_updated(source, target)
         # Merge existing criteria and {source.key: {"$in": keys_updated}}.
         if "$and" in criteria:
             criteria["$and"].append({source.key: {"$in": keys_updated}})
         elif source.key in criteria:
             # XXX could go deeper and check for $in, but this is fine.
             criteria["$and"] = [
-                {source.key: criteria[source.key].copy()},
-                {source.key: {"$in": keys_updated}},
+                {
+                    source.key: criteria[source.key].copy()
+                },
+                {
+                    source.key: {
+                        "$in": keys_updated
+                    }
+                },
             ]
             del criteria[source.key]
         else:
             criteria.update({source.key: {"$in": keys_updated}})
     # Check ratio of criteria size to 16 MB MongoDB document size limit.
     # Overestimates ratio via 1000 * 1000 instead of 1024 * 1024.
     # If criteria is > 16MB, even cursor.count() will fail with a
     # "DocumentTooLarge: "command document too large" error.
     if (total_size(criteria) / (16 * 1000 * 1000)) >= 1:
-        raise RuntimeError(
-            "`get_items` query criteria too large. This can happen if "
-            "trying to run incremental=True for the initial build of a "
-            "very large source store, or if `query` is too large. You "
-            "can use maggma.utils.total_size to ensure `query` is smaller "
-            "than 16,000,000 bytes.")
+        raise RuntimeError("`get_items` query criteria too large. This can happen if "
+                           "trying to run incremental=True for the initial build of a "
+                           "very large source store, or if `query` is too large. You "
+                           "can use maggma.utils.total_size to ensure `query` is smaller "
+                           "than 16,000,000 bytes.")
     return criteria
 
 
 class MapBuilder(Builder, metaclass=ABCMeta):
     """
     Apply a unary function to yield a target document for each source document.
 
     Supports incremental building, where a source document gets built only if it
     has newer (by lu_field) data than the corresponding (by key) target
     document.
 
     """
-    def __init__(self, source, target, query=None, incremental=True, **kwargs):
+
+    def __init__(self, source, target, ufn, query=None, incremental=True, projection=None, **kwargs):
         """
         Apply a unary function to each source document.
 
         Args:
             source (Store): source store
             target (Store): target store
+            ufn (function): Unary function to process item
+                            You do not need to provide values for
+                            source.key and source.lu_field in the output.
+                            Any uncaught exceptions will be caught by 
+                            process_item and logged to the "error" field 
+                            in the target document.
             query (dict): optional query to filter source store
             incremental (bool): whether to use lu_field of source and target
                 to get only new/updated documents.
+            projection (list): list of keys to project from the source for processing.
+                This can be used to limit the data to improve efficiency
         """
         self.source = source
         self.target = target
         self.incremental = incremental
         self.query = query
+        self.ufn = ufn
+        self.projection = projection if projection else []
         super().__init__(sources=[source], targets=[target], **kwargs)
         self.kwargs = kwargs.copy()
         self.kwargs.update(query=query, incremental=incremental)
 
-    @staticmethod
-    @abstractmethod
-    def ufn(item):
-        """
-        Unary function to process item. You do not need to provide values for
-        source.key and source.lu_field in the output. Any uncaught exceptions
-        will be caught by process_item and logged to the "error" field in the
-        target document.
-
-        Args:
-            item: item to process
-
-        Returns:
-            dict: a dict that will extend a dict pre-populated with
-                {self.source.key, self.course.lu_field} fields.
-        """
-
     def get_items(self):
         criteria = get_criteria(
-            self.source, self.target, query=self.query,
-            incremental=self.incremental, logger=self.logger)
-        return self.source.query(criteria=criteria)
+            self.source, self.target, query=self.query, incremental=self.incremental, logger=self.logger)
+        if self.projection:
+            projection = list(set(self.projection + [self.source.key, self.source.lu_field]))
+        else:
+            projection = None
+
+        return self.source.query(criteria=criteria, properties=projection)
 
     def process_item(self, item):
         try:
             processed = self.ufn.__call__(item)
         except Exception as e:
             self.logger.error(traceback.format_exc())
             processed = {"error": str(e)}
         key, lu_field = self.source.key, self.source.lu_field
-        out = {key: item[key], lu_field: item[lu_field]}
+        out = {self.target.key: item[key]}
+        out[self.target.lu_field] =  self.source.lu_func[0](item[self.source.lu_field])
         out.update(processed)
         return out
 
     def update_targets(self, items):
         source, target = self.source, self.target
         for item in items:
             # Use source last-updated value, ensuring `datetime` type.
@@ -174,14 +173,15 @@
 class GroupBuilder(MapBuilder, metaclass=ABCMeta):
     """
     Group source docs and produce one target doc from each group.
 
     Supports incremental building, where a source group gets (re)built only if
     it has a newer (by lu_field) doc than the corresponding (by key) target doc.
     """
+
     def __init__(self, source, target, query=None, incremental=True, **kwargs):
         """
 
         Given criteria, get docs with needed grouping properties. With these
         minimal docs, yield groups. For each group, fetch all needed data for
         item processing, and yield one or more items (i.e. subgroups as
         appropriate).
@@ -189,31 +189,27 @@
         Args:
             source (Store): source store
             target (Store): target store
             query (dict): optional query to filter source store
             incremental (bool): whether to use lu_field of source and target
                 to get only new/updated documents.
         """
-        super().__init__(
-            source, target, query=query, incremental=incremental, **kwargs)
+        super().__init__(source, target, query=query, incremental=incremental, **kwargs)
         self.total = None
 
     def get_items(self):
         criteria = get_criteria(
-            self.source, self.target, query=self.query,
-            incremental=self.incremental, logger=self.logger)
+            self.source, self.target, query=self.query, incremental=self.incremental, logger=self.logger)
         if all(isinstance(entry, str) for entry in self.grouping_properties()):
             properties = {entry: 1 for entry in self.grouping_properties()}
             if "_id" not in properties:
                 properties.update({"_id": 0})
         else:
-            properties = {entry: include
-                          for entry, include in self.grouping_properties()}
-        groups = self.docs_to_groups(
-            self.source.query(criteria=criteria, properties=properties))
+            properties = {entry: include for entry, include in self.grouping_properties()}
+        groups = self.docs_to_groups(self.source.query(criteria=criteria, properties=properties))
         self.total = len(groups)
         if hasattr(self, "n_items_per_group"):
             n = self.n_items_per_group
             if isinstance(n, int) and n >= 1:
                 self.total *= n
         for group in groups:
             for item in self.group_to_items(group):
@@ -262,13 +258,10 @@
         Returns:
             iterable: one or more items per group for process_item.
         """
 
 
 class CopyBuilder(MapBuilder):
     """Sync a source store with a target store."""
-    def __init__(self, source, target, **kwargs):
-        super().__init__(source=source, target=target, **kwargs)
 
-    @staticmethod
-    def ufn(item):
-        return item
+    def __init__(self, source, target, **kwargs):
+        super().__init__(source=source, target=target, ufn=lambda x: x, **kwargs)
```

### Comparing `maggma-0.8.0/maggma/examples/runner_sample.py` & `maggma-0.9.0/maggma/examples/runner_sample.py`

 * *Files identical despite different names*

### Comparing `maggma-0.8.0/maggma/examples/tests/test_copybuilder.py` & `maggma-0.9.0/maggma/examples/tests/test_copybuilder.py`

 * *Files identical despite different names*

### Comparing `maggma-0.8.0/maggma/helpers.py` & `maggma-0.9.0/maggma/helpers.py`

 * *Files identical despite different names*

### Comparing `maggma-0.8.0/maggma/runner.py` & `maggma-0.9.0/maggma/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,24 @@
 import multiprocessing
 import types
 from collections import defaultdict, deque
 from threading import Thread, Condition, BoundedSemaphore
 from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
 from monty.json import MSONable
 from maggma.utils import get_mpi, grouper, primed
-from tqdm import tqdm
 
+# import tqdm Jupyter widget if running inside Jupyter
+try:
+    # noinspection PyUnresolvedReferences
+    if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
+        from tqdm import tqdm_notebook as tqdm
+    else: # likely 'TerminalInteractiveShell'
+        from tqdm import tqdm
+except NameError:
+    from tqdm import tqdm
 
 class BaseProcessor(MSONable, metaclass=abc.ABCMeta):
     """
     Base processor class for multiprocessing paradigms
     """
 
     def __init__(self, builders):
@@ -254,15 +262,15 @@
                 self.update_data_condition.wait_for(
                     lambda: not self.run_update_targets or len(self.data) > self.builder.chunk_size)
                 try:
                     self.builder.update_targets(self.data)
                     self.update_pbar.update(len(self.data))
                     self.data.clear()
                 except Exception as e:
-                    self.logger.debug("Problem in updating targets in builder run: {}".format(e))
+                    self.logger.exception("Problem in updating targets in builder run: {}".format(e))
 
 
 class MultiprocProcessor(BaseProcessor):
     """
     Processor to run builders using python multiprocessing
     """
 
@@ -388,15 +396,15 @@
                 try:
                     if self.data is not None:
                         self.update_pbar.unpause()
                         self.builder.update_targets(self.data)
                         self.update_pbar.update(len(self.data))
                         self.data.clear()
                 except Exception as e:
-                    self.logger.debug("Problem in updating targets in builder run: {}".format(e))
+                    self.logger.exception("Problem in updating targets in builder run: {}".format(e))
 
 
 class Runner(MSONable):
     def __init__(self, builders, max_workers=1, mpi=False):
         """
         Initialize with a list of builders
```

### Comparing `maggma-0.8.0/maggma/stores.py` & `maggma-0.9.0/maggma/stores.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import zlib
 
 import mongomock
 import pymongo
 import gridfs
 from itertools import groupby
 from operator import itemgetter
-from pymongo import MongoClient, DESCENDING
-from pydash import identity
+from pymongo import MongoClient
+from pydash import identity, set_
 
 from pymongo import ReplaceOne
 
 from monty.json import MSONable, jsanitize, MontyDecoder
 from monty.io import zopen
 from monty.serialization import loadfn
 from maggma.utils import LU_KEY_ISOFORMAT, confirm_field_index
@@ -65,22 +65,22 @@
     def close(self):
         """
         Closes any connections
         """
         pass
 
     @abstractmethod
-    def query(self, properties=None, criteria=None, **kwargs):
+    def query(self, criteria=None, properties=None, **kwargs):
         """
         Queries the Store for a set of properties
         """
         pass
 
     @abstractmethod
-    def query_one(self, properties=None, criteria=None, **kwargs):
+    def query_one(self, criteria=None, properties=None, **kwargs):
         """
         Get one property from the store
         """
         pass
 
     @abstractmethod
     def distinct(self, key, criteria=None, **kwargs):
@@ -106,23 +106,23 @@
 
         Returns:
             bool indicating if the index exists/was created
         """
         pass
 
     @abstractmethod
-    def groupby(self, keys, properties=None, criteria=None, **kwargs):
+    def groupby(self, keys, criteria=None, properties=None, **kwargs):
         """
         Simple grouping function that will group documents
         by keys.
 
         Args:
             keys (list or string): fields to group documents
-            properties (list): properties to return in grouped documents
             criteria (dict): filter for documents to group
+            properties (list): properties to return in grouped documents
 
         Returns:
             command cursor corresponding to grouped documents
 
             elements of the command cursor have the structure:
             {'_id': {"KEY_1": value_1, "KEY_2": value_2 ...,
              'docs': [list_of_documents corresponding to key values]}
@@ -183,43 +183,45 @@
 class Mongolike(object):
     """
     Mixin class that allows for basic mongo functionality
     """
 
     @property
     def collection(self):
+        if self._collection is None:
+            raise Exception("Must connect Mongo-like store before attemping to use it")
         return self._collection
 
-    def query(self, properties=None, criteria=None, **kwargs):
+    def query(self, criteria=None, properties=None, **kwargs):
         """
         Function that gets data from MongoStore with property focus.
 
         Args:
+            criteria (dict): filter for query, matches documents
+                against key-value pairs
             properties (list or dict): list of properties to return
                 or dictionary with {"property": 1} type structure
                 from standard mongo Collection.find syntax
-            criteria (dict): filter for query, matches documents
-                against key-value pairs
             **kwargs (kwargs): further kwargs to Collection.find
         """
         if isinstance(properties, list):
             properties = {p: 1 for p in properties}
         return self.collection.find(filter=criteria, projection=properties, **kwargs)
 
-    def query_one(self, properties=None, criteria=None, **kwargs):
+    def query_one(self, criteria=None, properties=None, **kwargs):
         """
         Function that gets a single from MongoStore with property focus.
         Returns None if nothing matches
 
         Args:
+            criteria (dict): filter for query, matches documents
+                against key-value pairs
             properties (list or dict): list of properties to return
                 or dictionary with {"property": 1} type structure
                 from standard mongo Collection.find syntax
-            criteria (dict): filter for query, matches documents
-                against key-value pairs
             **kwargs (kwargs): further kwargs to Collection.find_one
         """
         if isinstance(properties, list):
             properties = {p: 1 for p in properties}
         return self.collection.find_one(filter=criteria, projection=properties, **kwargs)
 
     def ensure_index(self, key, unique=False, **kwargs):
@@ -253,31 +255,28 @@
             d = jsanitize(d, allow_bson=True)
 
             # document-level validation is optional
             validates = True
             if self.validator:
                 validates = self.validator.is_valid(d)
                 if not validates:
-                    if self.validator.strict:
-                        raise ValueError('Document failed to validate: {}'.format(d))
-                    else:
-                        self.logger.error('Document failed to validate: {}'.format(d))
+                    self.logger.error('Document failed to validate:\n{}'.format(d))
 
             if validates:
                 key = key if key else self.key
                 if isinstance(key, list):
                     search_doc = {k: d[k] for k in key}
                 else:
                     search_doc = {key: d[key]}
                 if update_lu:
                     d[self.lu_field] = datetime.utcnow()
 
-                requests.append(ReplaceOne(search_doc,d,upsert=True))
+                requests.append(ReplaceOne(search_doc, d, upsert=True))
 
-        self.collection.bulk_write(requests,ordered=ordered)
+        self.collection.bulk_write(requests, ordered=ordered)
 
     def distinct(self, key, criteria=None, all_exist=False, **kwargs):
         """
         Function get to get all distinct values of a certain key in
         a mongolike store.  May take a single key or a list of keys
 
         Args:
@@ -350,23 +349,23 @@
         kwargs = loadfn(filename)
         if "collection" in kwargs:
             kwargs["collection_name"] = kwargs.pop("collection")
         # Get rid of aliases from traditional query engine db docs
         kwargs.pop("aliases", None)
         return cls(**kwargs)
 
-    def groupby(self, keys, properties=None, criteria=None, allow_disk_use=True, **kwargs):
+    def groupby(self, keys, criteria=None, properties=None, allow_disk_use=True, **kwargs):
         """
         Simple grouping function that will group documents
         by keys.
 
         Args:
             keys (list or string): fields to group documents
-            properties (list): properties to return in grouped documents
             criteria (dict): filter for documents to group
+            properties (list): properties to return in grouped documents
             allow_disk_use (bool): whether to allow disk use in aggregation
 
         Returns:
             command cursor corresponding to grouped documents
 
             elements of the command cursor have the structure:
             {'_id': {"KEY_1": value_1, "KEY_2": value_2 ...,
@@ -379,15 +378,17 @@
 
         if properties is not None:
             pipeline.append({"$project": {p: 1 for p in properties}})
 
         if isinstance(keys, str):
             keys = [keys]
 
-        group_id = {key: "${}".format(key) for key in keys}
+        group_id = {}
+        for key in keys:
+            set_(group_id, key, "${}".format(key))
         pipeline.append({"$group": {"_id": group_id, "docs": {"$push": "$$ROOT"}}})
 
         return self.collection.aggregate(pipeline, allowDiskUse=allow_disk_use)
 
     @classmethod
     def from_collection(cls, collection, **kwargs):
         """
@@ -419,23 +420,23 @@
     def connect(self, force_reset=False):
         if not self._collection or force_reset:
             self._collection = mongomock.MongoClient().db[self.name]
 
     def __hash__(self):
         return hash((self.name, self.lu_field))
 
-    def groupby(self, keys, properties=None, criteria=None, **kwargs):
+    def groupby(self, keys, criteria=None, properties=None, **kwargs):
         """
         Simple grouping function that will group documents
         by keys.
 
         Args:
             keys (list or string): fields to group documents
-            properties (list): properties to return in grouped documents
             criteria (dict): filter for documents to group
+            properties (list): properties to return in grouped documents
             allow_disk_use (bool): whether to allow disk use in aggregation
 
         Returns:
             command cursor corresponding to grouped documents
 
             elements of the command cursor have the structure:
             {'_id': {"KEY_1": value_1, "KEY_2": value_2 ...,
@@ -593,24 +594,24 @@
         """
         for field in criteria:
             if (field not in cls.files_collection_fields
                     and not field.startswith('metadata.')):
                 criteria['metadata.' + field] = copy.copy(criteria[field])
                 del criteria[field]
 
-    def query(self, properties=None, criteria=None, **kwargs):
+    def query(self, criteria=None, properties=None, **kwargs):
         """
         Function that gets data from GridFS. This store ignores all
         property projections as its designed for whole document access
 
         Args:
-            properties (list or dict): This will be ignored by the GridFS
-                Store
             criteria (dict): filter for query, matches documents
                 against key-value pairs
+            properties (list or dict): This will be ignored by the GridFS
+                Store
             **kwargs (kwargs): further kwargs to Collection.find
         """
         if isinstance(criteria, dict):
             self.transform_criteria(criteria)
         for f in self.collection.find(filter=criteria, **kwargs):
             data = f.read()
 
@@ -620,25 +621,25 @@
 
             try:
                 data = json.loads(data)
             except:
                 pass
             yield data
 
-    def query_one(self, properties=None, criteria=None, **kwargs):
+    def query_one(self, criteria=None, properties=None, **kwargs):
         """
         Function that gets a single document from GridFS. This store
         ignores all property projections as its designed for whole
         document access
 
         Args:
-            properties (list or dict): This will be ignored by the GridFS
-                Store
             criteria (dict): filter for query, matches documents
                 against key-value pairs
+            properties (list or dict): This will be ignored by the GridFS
+                Store
             **kwargs (kwargs): further kwargs to Collection.find
         """
         return next(self.query(criteria=criteria, **kwargs), None)
 
     def distinct(self, key, criteria=None, all_exist=False, **kwargs):
         """
         Function get to get all distinct values of a certain key in
@@ -668,23 +669,23 @@
                 self.transform_criteria(criteria)
             # Transfor to metadata subfield if not supposed to be in gridfs main fields
             if key not in self.files_collection_fields:
                 key = "metadata.{}".format(key)
 
             return self._files_collection.distinct(key, filter=criteria, **kwargs)
 
-    def groupby(self, keys, properties=None, criteria=None, allow_disk_use=True, **kwargs):
+    def groupby(self, keys, criteria=None, properties=None, allow_disk_use=True, **kwargs):
         """
         Simple grouping function that will group documents
         by keys.
 
         Args:
             keys (list or string): fields to group documents
-            properties (list): properties to return in grouped documents
             criteria (dict): filter for documents to group
+            properties (list): properties to return in grouped documents
             allow_disk_use (bool): whether to allow disk use in aggregation
 
         Returns:
             command cursor corresponding to grouped documents
 
             elements of the command cursor have the structure:
             {'_id': {"KEY_1": value_1, "KEY_2": value_2 ...,
```

### Comparing `maggma-0.8.0/maggma/tests/mpi_test.py` & `maggma-0.9.0/maggma/tests/mpi_test.py`

 * *Files identical despite different names*

### Comparing `maggma-0.8.0/maggma/tests/test_advanced_stores.py` & `maggma-0.9.0/maggma/tests/test_advanced_stores.py`

 * *Files 23% similar despite different names*

```diff
@@ -259,15 +259,17 @@
 class TestSandboxStore(unittest.TestCase):
 
     def setUp(self):
         self.store = MemoryStore()
         self.sandboxstore = SandboxStore(self.store, sandbox="test")
 
     def test_connect(self):
-        self.assertEqual(self.sandboxstore.collection, None)
+        with self.assertRaises(Exception):
+            self.sandboxstore.collection
+            
         self.sandboxstore.connect()
         self.assertIsInstance(self.sandboxstore.collection, mongomock.collection.Collection)
 
     def test_query(self):
         self.sandboxstore.connect()
         self.sandboxstore.collection.insert_one({"a": 1, "b": 2, "c": 3})
         self.assertEqual(self.sandboxstore.query_one(properties=["a"])['a'], 1)
@@ -297,13 +299,96 @@
         self.assertEqual(self.sandboxstore.query(criteria={"d": {"$exists": 1}}, properties=["d"])[0]["d"], 4)
         self.assertEqual(self.sandboxstore.collection.find_one({"e": 6})["sbxn"], ["test"])
         self.sandboxstore.update([{"e": 7, "sbxn": ["core"]}], key="e")
         self.assertEqual(set(self.sandboxstore.query_one(
             criteria={"e": 7})["sbxn"]), {"test", "core"})
 
     def tearDown(self):
-        if self.sandboxstore.collection:
+        try:
             self.sandboxstore.collection.drop()
+        except:
+            pass
+
+
+class JointStoreTest(unittest.TestCase):
+    def setUp(self):
+        self.jointstore = JointStore("maggma_test", ["test1", "test2"])
+        self.jointstore.connect()
+        self.jointstore.collection.drop()
+        self.jointstore.collection.insert_many(
+            [{"task_id": k, "my_prop": k+1, "last_updated": datetime.utcnow(),
+              "category": k // 5} for k in range(10)])
+        self.jointstore.collection.database["test2"].drop()
+        self.jointstore.collection.database["test2"].insert_many(
+            [{"task_id": 2*k, "your_prop": k+3, "last_updated": datetime.utcnow(),
+              "category2": k // 3} for k in range(5)])
+        self.test1 = MongoStore("maggma_test", "test1")
+        self.test1.connect()
+        self.test2 = MongoStore("maggma_test", "test2")
+        self.test2.connect()
+
+    def test_query(self):
+        # Test query all
+        docs = list(self.jointstore.query())
+        self.assertEqual(len(docs), 10)
+        docs_w_field = [d for d in docs if d.get("test2")]
+        self.assertEqual(len(docs_w_field), 5)
+        docs_w_field = sorted(docs_w_field, key=lambda x: x['task_id'])
+        self.assertEqual(docs_w_field[0]['test2']['your_prop'], 3)
+        self.assertEqual(docs_w_field[0]['task_id'], 0)
+        self.assertEqual(docs_w_field[0]['my_prop'], 1)
+
+    def test_query_one(self):
+        doc = self.jointstore.query_one()
+        self.assertEqual(doc['my_prop'], doc['task_id'] + 1)
+        # Test limit properties
+        doc = self.jointstore.query_one(properties=['test2', 'task_id'])
+        self.assertEqual(doc['test2']['your_prop'], doc['task_id'] + 3)
+        self.assertIsNone(doc.get("my_prop"))
+        # Test criteria
+        doc = self.jointstore.query_one(criteria={"task_id": {"$gte": 10}})
+        self.assertIsNone(doc)
+        doc = self.jointstore.query_one(criteria={"test2.your_prop": {"$gt": 6}})
+        self.assertEqual(doc['task_id'], 8)
+
+    def test_distinct(self):
+        dyour_prop = self.jointstore.distinct("test2.your_prop")
+        self.assertEqual(set(dyour_prop), {k + 3 for k in range(5)})
+        dmy_prop = self.jointstore.distinct("my_prop")
+        self.assertEqual(set(dmy_prop), {k + 1 for k in range(10)})
+        dmy_prop_cond = self.jointstore.distinct("my_prop", {"test2.your_prop": {"$gte": 5}})
+        self.assertEqual(set(dmy_prop_cond), {5, 7, 9})
+
+    def test_last_updated(self):
+        doc = self.jointstore.query_one({"task_id": 0})
+        test1doc = self.test1.query_one({"task_id": 0})
+        test2doc = self.test2.query_one({"task_id": 0})
+        self.assertEqual(test2doc['last_updated'], doc['last_updated'])
+        self.assertNotEqual(test1doc['last_updated'], doc['last_updated'])
+        # Swap the two
+        test2date = test2doc['last_updated']
+        test2doc['last_updated'] = test1doc['last_updated']
+        test1doc['last_updated'] = test2date
+        self.test1.update([test1doc], update_lu=False)
+        self.test2.update([test2doc], update_lu=False)
+        doc = self.jointstore.query_one({"task_id": 0})
+        test1doc = self.test1.query_one({"task_id": 0})
+        test2doc = self.test2.query_one({"task_id": 0})
+        self.assertEqual(test1doc['last_updated'], doc['last_updated'])
+        self.assertNotEqual(test2doc['last_updated'], doc['last_updated'])
+        # Check also that still has a field if no task2 doc
+        doc = self.jointstore.query_one({"task_id": 1})
+        self.assertIsNotNone(doc['last_updated'])
+
+    def test_groupby(self):
+        docs = list(self.jointstore.groupby("category"))
+        self.assertEqual(len(docs[0]['docs']), 5)
+        self.assertEqual(len(docs[1]['docs']), 5)
+        docs = list(self.jointstore.groupby("test2.category2"))
+        docs_by_id = {get(d, '_id.test2.category2'): d['docs'] for d in docs}
+        self.assertEqual(len(docs_by_id[None]), 5)
+        self.assertEqual(len(docs_by_id[0]), 3)
+        self.assertEqual(len(docs_by_id[1]), 2)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `maggma-0.8.0/maggma/tests/test_runner.py` & `maggma-0.9.0/maggma/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `maggma-0.8.0/maggma/tests/test_stores.py` & `maggma-0.9.0/maggma/tests/test_stores.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # coding: utf-8
 """
 Tests for the base Stores
 """
 import os
-import glob
 import unittest
 import numpy as np
 import mongomock.collection
 import pymongo.collection
 import numpy.testing.utils as nptu
 from maggma.stores import *
 
@@ -20,43 +19,51 @@
 
     def setUp(self):
         self.mongostore = MongoStore("maggma_test", "test")
         self.mongostore.connect()
 
     def test_connect(self):
         mongostore = MongoStore("maggma_test", "test")
-        self.assertEqual(mongostore.collection, None)
+        with self.assertRaises(Exception):
+            mongostore.collection
         mongostore.connect()
         self.assertIsInstance(mongostore.collection, pymongo.collection.Collection)
 
     def test_query(self):
         self.mongostore.collection.insert({"a": 1, "b": 2, "c": 3})
         self.assertEqual(self.mongostore.query_one(properties=["a"])["a"], 1)
         self.assertEqual(self.mongostore.query_one(properties=["a"])['a'], 1)
         self.assertEqual(self.mongostore.query_one(properties=["b"])['b'], 2)
         self.assertEqual(self.mongostore.query_one(properties=["c"])['c'], 3)
 
     def test_distinct(self):
         self.mongostore.collection.insert({"a": 1, "b": 2, "c": 3})
-        self.mongostore.collection.insert({"a": 4, "d": 5, "e": 6})
+        self.mongostore.collection.insert({"a": 4, "d": 5, "e": 6, "g": {"h": 1}})
         self.assertEqual(self.mongostore.distinct("a"), [1, 4])
 
         # Test list distinct functionality
         self.mongostore.collection.insert({"a": 4, "d": 6, "e": 7})
-        self.mongostore.collection.insert({"a": 4, "d": 6})
+        self.mongostore.collection.insert({"a": 4, "d": 6, "g": {"h": 2}})
         ad_distinct = self.mongostore.distinct(["a", "d"])
         self.assertTrue(len(ad_distinct), 3)
         self.assertTrue({"a": 4, "d": 6} in ad_distinct)
         self.assertTrue({"a": 1} in ad_distinct)
         self.assertEqual(len(self.mongostore.distinct(["d", "e"], {"a": 4})), 3)
         all_exist = self.mongostore.distinct(["a", "b"], all_exist=True)
         self.assertEqual(len(all_exist), 1)
         all_exist2 = self.mongostore.distinct(["a", "e"], all_exist=True, criteria={"d": 6})
         self.assertEqual(len(all_exist2), 1)
 
+        # Test distinct subdocument functionality
+        ghs = self.mongostore.distinct("g.h")
+        self.assertEqual(set(ghs), {1, 2})
+        ghs_ds = self.mongostore.distinct(["d", "g.h"], all_exist=True)
+        self.assertEqual({s['g']['h'] for s in ghs_ds}, {1, 2})
+        self.assertEqual({s['d'] for s in ghs_ds}, {5, 6})
+
     def test_update(self):
         self.mongostore.update([{"e": 6, "d": 4}], key="e")
         self.assertEqual(self.mongostore.query(criteria={"d": {"$exists": 1}}, properties=["d"])[0]["d"], 4)
 
         self.mongostore.update([{"e": 7, "d": 8, "f": 9}], key=["d", "f"])
         self.assertEqual(self.mongostore.query_one(criteria={"d": 8, "f": 9}, properties=["e"])["e"], 7)
         self.mongostore.update([{"e": 11, "d": 8, "f": 9}], key=["d", "f"])
@@ -112,25 +119,28 @@
         with self.assertRaises(StoreError) as cm:
             self.mongostore.last_updated
         self.assertIn(self.mongostore.lu_field, str(cm.exception))
         self.mongostore.update([{self.mongostore.key: 1, "a": 1}])
         self.assertGreaterEqual(self.mongostore.last_updated, tic)
 
     def tearDown(self):
-        if self.mongostore.collection:
+        try:
             self.mongostore.collection.drop()
+        except:
+            pass
 
 
 class TestMemoryStore(unittest.TestCase):
 
     def setUp(self):
         self.memstore = MemoryStore()
 
     def test(self):
-        self.assertEqual(self.memstore.collection, None)
+        with self.assertRaises(Exception):
+            self.memstore.collection
         self.memstore.connect()
         self.assertIsInstance(self.memstore.collection, mongomock.collection.Collection)
 
     def test_groupby(self):
         self.memstore.connect()
         self.memstore.update(
             [{
```

### Comparing `maggma-0.8.0/maggma/tests/test_utils.py` & `maggma-0.9.0/maggma/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `maggma-0.8.0/maggma/tests/test_validator.py` & `maggma-0.9.0/maggma/tests/test_validator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,44 @@
 # coding: utf-8
 """
 Tests the validators
 """
 import unittest
-from maggma.validator import StandardValidator
+from maggma.validator import JSONSchemaValidator, msonable_schema
 from monty.json import MSONable
 
 class ValidatorTests(unittest.TestCase):
     """
     Tests for Validators.
     """
 
-    def test_standardvalidator(self):
+    def test_jsonschemevalidator(self):
         """
-        Test the StandardValidator class.
+        Test the JSONSchemaValidator class.
         """
 
         class LatticeMock(MSONable):
             """
             A sample MSONable object, just for testing.
             """
             def __init__(self, a):
                 self.a = a
 
-        class SampleValidator(StandardValidator):
-            """
-            A sample validator, just for testing.
-            """
-
-            @property
-            def schema(self):
-                return {
-                    "type": "object",
-                    "properties":
-                        {
-                            "task_id": {"type": "string"},
-                            "successful": {"type": "boolean"}
-                        },
-                    "required": ["task_id", "successful"]
-                }
-
-            @property
-            def msonable_keypaths(self):
-                return {"lattice": LatticeMock}
+        test_schema = {
+            "type": "object",
+            "properties":
+                {
+                    "task_id": {"type": "string"},
+                    "successful": {"type": "boolean"},
+                    "lattice": msonable_schema(LatticeMock)
+                },
+            "required": ["task_id", "successful"]
+        }
 
-        validator = SampleValidator()
+        validator = JSONSchemaValidator(schema=test_schema)
 
         lattice = LatticeMock(5)
 
         valid_doc = {
             'task_id': 'mp-test',
             'successful': True,
             'lattice': lattice.as_dict()
@@ -70,8 +60,8 @@
             'successful': 'true',
             'lattice': lattice.as_dict()
         }
 
         self.assertTrue(validator.is_valid(valid_doc))
         self.assertFalse(validator.is_valid(invalid_doc_msonable))
         self.assertFalse(validator.is_valid(invalid_doc_missing_key))
-        self.assertFalse(validator.is_valid(invalid_doc_wrong_type))
+        self.assertFalse(validator.is_valid(invalid_doc_wrong_type))
```

### Comparing `maggma-0.8.0/maggma/utils.py` & `maggma-0.9.0/maggma/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,24 @@
 from datetime import datetime, timedelta
 from sys import getsizeof, stderr
 
 from pydash.utilities import to_path
 from pydash.objects import set_, get, has
 from pydash.objects import unset as _unset
 import logging
-import tqdm
 
+# import tqdm Jupyter widget if running inside Jupyter
+try:
+    # noinspection PyUnresolvedReferences
+    if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
+        from tqdm import tqdm_notebook as tqdm
+    else: # likely 'TerminalInteractiveShell'
+        from tqdm import tqdm
+except NameError:
+    from tqdm import tqdm
 
 def primed(iterable):
     """Preprimes an iterator so the first value is calculated immediately
        but not returned until the first iteration
     """
     itr = iter(iterable)
     try:
@@ -33,15 +41,15 @@
 
     def __init__(self, level=logging.NOTSET):
         super().__init__(level)
 
     def emit(self, record):
         try:
             msg = self.format(record)
-            tqdm.tqdm.write(msg)
+            tqdm.write(msg)
             self.flush()
         except (KeyboardInterrupt, SystemExit):
             raise
         except:
             self.handleError(record)
 
 
@@ -262,8 +270,8 @@
 
         for typ, handler in all_handlers.items():
             if isinstance(o, typ):
                 s += sum(map(sizeof, handler(o)))
                 break
         return s
 
-    return sizeof(o)
+    return sizeof(o)
```

### Comparing `maggma-0.8.0/maggma/validator.py` & `maggma-0.9.0/maggma/validator.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,107 +5,104 @@
 that Store.
 """
 
 from abc import ABC, abstractmethod
 from jsonschema import validate, ValidationError
 import pydash
 
+
 class Validator(ABC):
     """
     A generic class to perform document-level validation on Stores.
     Attach a Validator to a Store during initialization, any all documents
     added to the Store will call .validate_doc() before being added.
     """
 
-    def init(self, strict=False):
-        """
-        Args:
-            strict (bool): Informs Store how to treat Validator: if
-            True, will cause build to fail if invalid document
-            is found and raise a ValueError, if False will continue
-            build but log an error message. In both cases, invalid
-            documents will not be stored.
-        """
-        self.strict = strict
-
     @abstractmethod
     def is_valid(self, doc):
         """
         Returns (bool): True if document valid, False if document
         invalid
         """
         return NotImplementedError
 
 
-class StandardValidator(Validator):
+class JSONSchemaValidator(Validator):
     """
-    A standard Validator, which allows document validation against a
-    provided JSON schema, and also can check that specified keys, if present,
-    are MSONable (that is, a Python object can be reconstructed).
+    A validator that allows document validation against a
+    provided JSON schema.
 
-    To use, subclass StandardSchema and with your own `schema`
-    and `msonable_keypaths` keys.
+    For convenience, the helper method in this module
+    `msonable_schema` can be used to create a schema for a
+    specific MSONable object, which can be embedded in your
+    JSON schema. See the tests for an example of this.
     """
 
+    def __init__(self, schema, strict=False):
+        """
+        Args:
+            strict (bool): Informs Store how to treat Validator: if
+            True, will cause build to fail if invalid document
+            is found and raise a ValueError, if False will continue
+            build but log an error message. In both cases, invalid
+            documents will not be stored.
+            schema (dict): A Python dict representation of a JSON
+        """
+        self._schema = schema
+        self._strict = strict
+
+    @property
+    def strict(self):
+        """
+        Whether is_valid() should raise a ValidationError or
+        simply return False if a document fails validation.
+        :return (bool):
+        """
+        return self._strict
+
     @property
-    @abstractmethod
     def schema(self):
         """
         Defines a JSON schema for your document,
         which is used by the default `validate_doc()` method.
 
         This is a standard, with many validators existing, including
         MongoDB's own JSON schema validator (3.6+). Implementing this
         property allows both the document to be validated by a Builder,
         and also makes it possible to enable document-level validation
         inside MongoDB for Mongo-backed Stores.
 
         Returns (dict): a JSON schema as a Python dict
         """
-        return {}
+        return self._schema
 
-    @property
-    @abstractmethod
-    def msonable_keypaths(self):
+    def is_valid(self, doc):
         """
-        Optional. Used by the default `validate_doc()` method. Define a
-        list of keypaths
+        Returns True or False if validator initialized with
+        strict=False, or returns True or raises ValidationError
+        if strict=True.
 
-        Returns (dict): keys should be the keypath to the relevant value
-        in your document, and values should be the relevant class
+        :param doc (dict): a single document
+        :return: True, False or ValidationError
         """
-        return {}
-
-    def is_valid(self, doc):
-
-        # JSON validation
         try:
             validate(doc, schema=self.schema)
-            valid_schema = True
-        except ValidationError:
-            valid_schema = False
-
-        # MSONable validation
-        def _validate_doc_msonable(doc):
-            """
-            For every keypath, will return True if either
-            keypath does not exist, or keypath does exist
-            and a Python object can be reconstructed.
-            Otherwise will return False.
-            """
-
-            for keypath, obj in self.msonable_keypaths.items():
-
-                dict_to_check = pydash.get(doc, keypath, None)
-
-                if dict_to_check:
-                    try:
-                        obj.from_dict(dict_to_check)
-                    except:
-                        return False
-
             return True
+        except ValidationError:
+            if self.strict:
+                raise
+            else:
+                return False
 
-        valid_msonable = _validate_doc_msonable(doc)
-
-        return valid_schema and valid_msonable
 
+def msonable_schema(cls):
+    """
+    Convenience function to return a JSON Schema for any MSONable class.
+    """
+    return {
+        "type": "object",
+        "required": ["@class", "@module"],
+        "properties": {
+            "@class": {"const": cls.__name__},
+            "@module": {"const": cls.__module__}
+        }
+    }
```

### Comparing `maggma-0.8.0/maggma.egg-info/PKG-INFO` & `maggma-0.9.0/maggma.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maggma
-Version: 0.8.0
+Version: 0.9.0
 Summary: MongoDB aggregation machine
 Home-page: https://github.com/materialsproject/maggma
 Author: MP Team
 Author-email: matproj-develop@googlegroups.com
 License: modified BSD
 Description: # maggma
         Workflow tools for MongoDB aggregation in Python
```

### Comparing `maggma-0.8.0/maggma.egg-info/SOURCES.txt` & `maggma-0.9.0/maggma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maggma-0.8.0/PKG-INFO` & `maggma-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maggma
-Version: 0.8.0
+Version: 0.9.0
 Summary: MongoDB aggregation machine
 Home-page: https://github.com/materialsproject/maggma
 Author: MP Team
 Author-email: matproj-develop@googlegroups.com
 License: modified BSD
 Description: # maggma
         Workflow tools for MongoDB aggregation in Python
```

### Comparing `maggma-0.8.0/setup.py` & `maggma-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from setuptools import setup, find_packages
 
 module_dir = os.path.dirname(os.path.abspath(__file__))
 
 if __name__ == "__main__":
     setup(
         name="maggma",
-        version="0.8.0",
+        version="0.9.0",
         description="MongoDB aggregation machine",
         long_description=open(os.path.join(module_dir, "README.md")).read(),
         url="https://github.com/materialsproject/maggma",
         author="MP Team",
         author_email="matproj-develop@googlegroups.com",
         license="modified BSD",
         packages=find_packages(),
         package_data={},
         zip_safe=False,
         install_requires=[
             "pymongo>=3.6", "mongomock>=3.10.0", "monty>=1.0.2",
             "smoqe>=0.1.3", "PyYAML>=3.12", "pydash>=4.1.0", "tqdm>=4.19.6",
-            "mongogrant>=0.1.10", "hvac>=0.3.0", "boto3>=1.6.9",
+            "mongogrant>=0.2.2", "hvac>=0.3.0", "boto3>=1.6.9",
         ],
         extras_require={"mpi": ["mpi4py>=2.0.0"]},
         classifiers=["Programming Language :: Python :: 3",
                      "Programming Language :: Python :: 3.6",
                      "Development Status :: 2 - Pre-Alpha",
                      "Intended Audience :: Science/Research",
                      "Intended Audience :: System Administrators",
```

