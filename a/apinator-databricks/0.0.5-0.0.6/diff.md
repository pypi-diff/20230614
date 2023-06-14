# Comparing `tmp/apinator-databricks-0.0.5.tar.gz` & `tmp/apinator_databricks-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apinator-databricks-0.0.5.tar", last modified: Fri Apr 28 19:33:03 2023, max compression
+gzip compressed data, was "apinator_databricks-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `apinator-databricks-0.0.5.tar` & `apinator_databricks-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      145 2023-04-28 19:31:54.469664 apinator-databricks-0.0.5/.bumpversion.cfg
--rw-r--r--   0        0        0      584 2023-04-20 17:19:38.874735 apinator-databricks-0.0.5/.github/workflows/dagger.yml
--rw-r--r--   0        0        0      423 2023-04-28 19:32:29.902026 apinator-databricks-0.0.5/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0     2162 2023-04-20 17:19:38.874735 apinator-databricks-0.0.5/.gitignore
--rw-r--r--   0        0        0      696 2023-04-20 17:19:38.875754 apinator-databricks-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1044 2023-04-20 17:19:38.875754 apinator-databricks-0.0.5/.ruff.toml
--rw-r--r--   0        0        0    11357 2023-04-20 17:19:38.876299 apinator-databricks-0.0.5/LICENSE
--rw-r--r--   0        0        0      655 2023-04-20 17:19:38.876299 apinator-databricks-0.0.5/README.md
--rw-r--r--   0        0        0       66 2023-04-28 19:31:54.469664 apinator-databricks-0.0.5/apinator_databricks/__init__.py
--rw-r--r--   0        0        0      871 2023-04-20 17:19:38.876299 apinator-databricks-0.0.5/apinator_databricks/_common/api.py
--rw-r--r--   0        0        0      301 2023-04-20 22:37:33.605665 apinator-databricks-0.0.5/apinator_databricks/_common/model.py
--rw-r--r--   0        0        0      198 2023-04-20 17:19:38.876299 apinator-databricks-0.0.5/apinator_databricks/common.py
--rw-r--r--   0        0        0      153 2023-04-20 17:19:38.877328 apinator-databricks-0.0.5/apinator_databricks/marketplace_provider/__init__.py
--rw-r--r--   0        0        0      651 2023-04-20 17:19:38.877328 apinator-databricks-0.0.5/apinator_databricks/marketplace_provider/api.py
--rw-r--r--   0        0        0     2252 2023-04-20 23:20:27.208660 apinator-databricks-0.0.5/apinator_databricks/marketplace_provider/model.py
--rw-r--r--   0        0        0      139 2023-04-20 17:19:38.877328 apinator-databricks-0.0.5/apinator_databricks/unity_catalog/__init__.py
--rw-r--r--   0        0        0     3391 2023-04-20 22:32:39.531667 apinator-databricks-0.0.5/apinator_databricks/unity_catalog/api.py
--rw-r--r--   0        0        0     4893 2023-04-20 22:50:59.150488 apinator-databricks-0.0.5/apinator_databricks/unity_catalog/model.py
--rw-r--r--   0        0        0      895 2023-04-20 17:19:38.878327 apinator-databricks-0.0.5/ci/main.py
--rw-r--r--   0        0        0      480 2023-04-20 17:19:38.878327 apinator-databricks-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      580 2023-04-28 19:31:54.469664 apinator-databricks-0.0.5/setup.cfg
--rw-r--r--   0        0        0        0 2023-04-20 17:19:38.878327 apinator-databricks-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     1564 2023-04-20 17:19:38.879326 apinator-databricks-0.0.5/tests/test_marketplace_provider.py
--rw-r--r--   0        0        0     1452 2023-04-20 17:19:38.879326 apinator-databricks-0.0.5/tests/test_unity_catalog.py
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 apinator-databricks-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      145 2023-06-14 19:01:27.813741 apinator_databricks-0.0.6/.bumpversion.cfg
+-rw-r--r--   0        0        0      584 2023-04-20 17:19:38.874735 apinator_databricks-0.0.6/.github/workflows/dagger.yml
+-rw-r--r--   0        0        0      423 2023-04-28 19:32:29.902026 apinator_databricks-0.0.6/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     2162 2023-04-20 17:19:38.874735 apinator_databricks-0.0.6/.gitignore
+-rw-r--r--   0        0        0      696 2023-04-20 17:19:38.875754 apinator_databricks-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1044 2023-04-20 17:19:38.875754 apinator_databricks-0.0.6/.ruff.toml
+-rw-r--r--   0        0        0    11357 2023-04-20 17:19:38.876299 apinator_databricks-0.0.6/LICENSE
+-rw-r--r--   0        0        0      655 2023-04-20 17:19:38.876299 apinator_databricks-0.0.6/README.md
+-rw-r--r--   0        0        0       66 2023-06-14 19:01:27.814735 apinator_databricks-0.0.6/apinator_databricks/__init__.py
+-rw-r--r--   0        0        0      871 2023-04-20 17:19:38.876299 apinator_databricks-0.0.6/apinator_databricks/_common/api.py
+-rw-r--r--   0        0        0      301 2023-04-20 22:37:33.605665 apinator_databricks-0.0.6/apinator_databricks/_common/model.py
+-rw-r--r--   0        0        0      198 2023-04-20 17:19:38.876299 apinator_databricks-0.0.6/apinator_databricks/common.py
+-rw-r--r--   0        0        0      153 2023-04-20 17:19:38.877328 apinator_databricks-0.0.6/apinator_databricks/marketplace_provider/__init__.py
+-rw-r--r--   0        0        0      651 2023-04-20 17:19:38.877328 apinator_databricks-0.0.6/apinator_databricks/marketplace_provider/api.py
+-rw-r--r--   0        0        0     2252 2023-04-20 23:20:27.208660 apinator_databricks-0.0.6/apinator_databricks/marketplace_provider/model.py
+-rw-r--r--   0        0        0      139 2023-04-20 17:19:38.877328 apinator_databricks-0.0.6/apinator_databricks/unity_catalog/__init__.py
+-rw-r--r--   0        0        0     3391 2023-04-20 22:32:39.531667 apinator_databricks-0.0.6/apinator_databricks/unity_catalog/api.py
+-rw-r--r--   0        0        0     4917 2023-06-14 19:01:27.814735 apinator_databricks-0.0.6/apinator_databricks/unity_catalog/model.py
+-rw-r--r--   0        0        0      895 2023-04-20 17:19:38.878327 apinator_databricks-0.0.6/ci/main.py
+-rw-r--r--   0        0        0      480 2023-04-20 17:19:38.878327 apinator_databricks-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      580 2023-06-14 19:01:27.816258 apinator_databricks-0.0.6/setup.cfg
+-rw-r--r--   0        0        0        0 2023-04-20 17:19:38.878327 apinator_databricks-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     1564 2023-04-20 17:19:38.879326 apinator_databricks-0.0.6/tests/test_marketplace_provider.py
+-rw-r--r--   0        0        0     1452 2023-06-14 18:23:03.932832 apinator_databricks-0.0.6/tests/test_unity_catalog.py
+-rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 apinator_databricks-0.0.6/PKG-INFO
```

### Comparing `apinator-databricks-0.0.5/.github/workflows/dagger.yml` & `apinator_databricks-0.0.6/.github/workflows/dagger.yml`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.5/.gitignore` & `apinator_databricks-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.5/.pre-commit-config.yaml` & `apinator_databricks-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.5/.ruff.toml` & `apinator_databricks-0.0.6/.ruff.toml`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.5/LICENSE` & `apinator_databricks-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.5/README.md` & `apinator_databricks-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.5/apinator_databricks/_common/api.py` & `apinator_databricks-0.0.6/apinator_databricks/_common/api.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.5/apinator_databricks/marketplace_provider/api.py` & `apinator_databricks-0.0.6/apinator_databricks/marketplace_provider/api.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.5/apinator_databricks/marketplace_provider/model.py` & `apinator_databricks-0.0.6/apinator_databricks/marketplace_provider/model.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.5/apinator_databricks/unity_catalog/api.py` & `apinator_databricks-0.0.6/apinator_databricks/unity_catalog/api.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.5/apinator_databricks/unity_catalog/model.py` & `apinator_databricks-0.0.6/apinator_databricks/unity_catalog/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     shared_as: str
     cdf_enabled: bool
     history_data_sharing_status: str
     status: str
 
 
 class SharePartial(SecurableDatabricksBase):
+    share_id: uuid.UUID
     name: str
     owner: str
     full_name: str
     comment: str = ""
 
 
 class Share(SharePartial):
```

### Comparing `apinator-databricks-0.0.5/ci/main.py` & `apinator_databricks-0.0.6/ci/main.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.5/setup.cfg` & `apinator_databricks-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.0.5
+version = 0.0.6
 name = apinator-databricks
 description = APInator binding to Databricks API
 author = Rearc Data
 author_email = data@rearc.io
 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `apinator-databricks-0.0.5/tests/test_marketplace_provider.py` & `apinator_databricks-0.0.6/tests/test_marketplace_provider.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.5/tests/test_unity_catalog.py` & `apinator_databricks-0.0.6/tests/test_unity_catalog.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.5/PKG-INFO` & `apinator_databricks-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apinator-databricks
-Version: 0.0.5
+Version: 0.0.6
 Summary: APInator bindings for Databricks API
 Author-email: Rearc Data <data@rearc.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: apinator~=0.0.2
 Requires-Dist: pytest ; extra == "tests"
 Requires-Dist: pytest-cov ; extra == "tests"
```

