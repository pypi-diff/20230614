# Comparing `tmp/propertysync-0.5.0.tar.gz` & `tmp/propertysync-0.6.0.tar.gz`

## Comparing `propertysync-0.5.0.tar` & `propertysync-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 propertysync-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 propertysync-0.5.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 propertysync-0.5.0/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.5.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propertysync-0.5.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.5.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/__about__.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/__init__.py
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/api.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/batch.py
--rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/document.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/search.py
--rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/titlesearch_batch.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 propertysync-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 propertysync-0.5.0/tests/test_batch.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 propertysync-0.5.0/tests/test_document.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 propertysync-0.5.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.5.0/LICENSE
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.5.0/README.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 propertysync-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 propertysync-0.6.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 propertysync-0.6.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 propertysync-0.6.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propertysync-0.6.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.6.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/__about__.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/__init__.py
+-rw-r--r--   0        0        0    16209 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/api.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/batch.py
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/document.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/search.py
+-rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/titlesearch_batch.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 propertysync-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 propertysync-0.6.0/tests/test_batch.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 propertysync-0.6.0/tests/test_document.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 propertysync-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.6.0/README.md
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.6.0/PKG-INFO
```

### Comparing `propertysync-0.5.0/CHANGELOG.md` & `propertysync-0.6.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [Unreleased]
-
-### Added
-### Fixed
-### Changed
-### Removed
+Generated by [`auto-changelog`](https://github.com/CookPete/auto-changelog).
 
+<!-- auto-changelog-above -->
 
 ## [0.5.0] - 2023-05-10
 
 ### Added
 - Lots of work to Batch and Document classes to support find and replace
 - Tests added for Batch and Document classes
 - New API method (get_document_pdf) to retrieve document PDFs
```

### Comparing `propertysync-0.5.0/propertysync/api.py` & `propertysync-0.6.0/propertysync/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import requests, os, time
+import requests, os, time, tempfile
 
 """
 This is a helper for interacting with the PropertySync API
 """
 
 # TODO: Follow styleguide: https://google.github.io/styleguide/pyguide.html#316-naming
 
@@ -306,16 +306,16 @@
         # find the PDF asset
         if "pdf" not in assets:
             raise Exception("No PDF found for document ID "+document_id)
         
         # get the PDF asset
         pdf_asset = self.get_document_asset(document_id, assets["pdf"]["id"])
 
-        # create a temp file name for the pdf using the document_id
-        temp_file_name = "/tmp/"+document_id+".pdf"
+        # create a temp file name for the pdf on this os
+        temp_file_name = tempfile.NamedTemporaryFile(suffix=".pdf").name
 
         # download the PDF to the temp file
         with open(temp_file_name, 'wb') as f:
             f.write(pdf_asset)
 
         # return the temp file name
         return temp_file_name
@@ -356,14 +356,23 @@
         url = f"{self.search_url}/reports/{report_id}/run"
         return self.api_call("GET", url, params=params)
     
     # run a search
     def run_search(self, search_query):
         url = f"{self.search_url}/document-groups/{self.document_group_id}/searches"
         return self.api_call("POST", url, body=search_query)
+    
+    # run a document action on a batch
+    def run_document_action(self, batch_id, action_id):
+        url = f"{self.indexing_url}/document-groups/{self.document_group_id}/document-actions/{action_id}/execute"
+        params = {
+            "batchId":batch_id
+        }
+        return self.api_call("POST", url, params=params)
+
 
     # run a search, then create a batch and wait for the batch to fully hydrate, then retrieve the batch and optionally delete it
     def run_search_and_create_batch(self, search_query, minimum_results=1,wait_time=2,batch_name='python-api-client temp batch', delete_batch=True):
         search = self.run_search(search_query)
         search_id = search["id"]
 
         # if we don't have enough results in the search, throw an exception
```

### Comparing `propertysync-0.5.0/propertysync/batch.py` & `propertysync-0.6.0/propertysync/batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.5.0/propertysync/document.py` & `propertysync-0.6.0/propertysync/document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.5.0/propertysync/search.py` & `propertysync-0.6.0/propertysync/search.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.5.0/propertysync/titlesearch_batch.py` & `propertysync-0.6.0/propertysync/titlesearch_batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.5.0/tests/test_batch.py` & `propertysync-0.6.0/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.5.0/tests/test_document.py` & `propertysync-0.6.0/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.5.0/LICENSE` & `propertysync-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propertysync-0.5.0/README.md` & `propertysync-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `propertysync-0.5.0/pyproject.toml` & `propertysync-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propertysync-0.5.0/PKG-INFO` & `propertysync-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertysync
-Version: 0.5.0
+Version: 0.6.0
 Summary: A package for interacting with the PropertySync API.
 Project-URL: Documentation, https://developer.propertysync.com/python/index.html
 Author-email: Rob Martinson <rob@limelyte.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

