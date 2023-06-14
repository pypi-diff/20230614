# Comparing `tmp/grai_schemas-0.1.8.tar.gz` & `tmp/grai_schemas-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_schemas-0.1.8.tar", max compression
+gzip compressed data, was "grai_schemas-0.1.9.tar", max compression
```

## Comparing `grai_schemas-0.1.8.tar` & `grai_schemas-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3793 2023-01-10 22:34:25.293196 grai_schemas-0.1.8/LICENSE
--rw-r--r--   0        0        0        0 2023-01-10 22:34:25.293226 grai_schemas-0.1.8/README.md
--rw-r--r--   0        0        0      558 2023-01-30 22:55:51.598057 grai_schemas-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      180 2023-01-27 01:14:06.497464 grai_schemas-0.1.8/src/grai_schemas/__init__.py
--rw-r--r--   0        0        0      345 2023-01-27 01:14:06.497536 grai_schemas-0.1.8/src/grai_schemas/base.py
--rw-r--r--   0        0        0     2798 2023-01-29 22:48:26.179628 grai_schemas-0.1.8/src/grai_schemas/generics.py
--rw-r--r--   0        0        0      162 2023-01-29 22:48:26.179850 grai_schemas-0.1.8/src/grai_schemas/package_definitions.py
--rw-r--r--   0        0        0        0 2023-01-18 14:35:11.049253 grai_schemas-0.1.8/src/grai_schemas/py.typed
--rw-r--r--   0        0        0      500 2023-01-29 22:48:26.180085 grai_schemas-0.1.8/src/grai_schemas/schema.py
--rw-r--r--   0        0        0      795 2023-01-30 22:09:59.327833 grai_schemas-0.1.8/src/grai_schemas/utilities.py
--rw-r--r--   0        0        0      139 2023-01-27 01:14:06.497746 grai_schemas-0.1.8/src/grai_schemas/v1/__init__.py
--rw-r--r--   0        0        0     1277 2023-01-30 22:47:36.259803 grai_schemas-0.1.8/src/grai_schemas/v1/edge.py
--rw-r--r--   0        0        0      790 2023-01-30 22:44:06.657171 grai_schemas-0.1.8/src/grai_schemas/v1/generics.py
--rw-r--r--   0        0        0      269 2023-01-27 01:14:06.497906 grai_schemas-0.1.8/src/grai_schemas/v1/metadata/__init__.py
--rw-r--r--   0        0        0     1001 2023-01-27 01:14:06.497953 grai_schemas-0.1.8/src/grai_schemas/v1/metadata/edges.py
--rw-r--r--   0        0        0      289 2023-01-27 01:14:06.497998 grai_schemas-0.1.8/src/grai_schemas/v1/metadata/metadata.py
--rw-r--r--   0        0        0     1086 2023-01-27 01:14:06.498045 grai_schemas-0.1.8/src/grai_schemas/v1/metadata/nodes.py
--rw-r--r--   0        0        0     1096 2023-01-29 22:48:26.180432 grai_schemas-0.1.8/src/grai_schemas/v1/node.py
--rw-r--r--   0        0        0        0 2023-01-27 01:14:06.498108 grai_schemas-0.1.8/src/grai_schemas/v1/workspace.py
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 grai_schemas-0.1.8/setup.py
--rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 grai_schemas-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3793 2023-01-10 22:34:25.293196 grai_schemas-0.1.9/LICENSE
+-rw-r--r--   0        0        0        0 2023-01-10 22:34:25.293226 grai_schemas-0.1.9/README.md
+-rw-r--r--   0        0        0      558 2023-02-01 16:25:14.091601 grai_schemas-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      180 2023-01-27 01:14:06.497464 grai_schemas-0.1.9/src/grai_schemas/__init__.py
+-rw-r--r--   0        0        0      345 2023-01-27 01:14:06.497536 grai_schemas-0.1.9/src/grai_schemas/base.py
+-rw-r--r--   0        0        0     2798 2023-01-29 22:48:26.179628 grai_schemas-0.1.9/src/grai_schemas/generics.py
+-rw-r--r--   0        0        0      162 2023-01-29 22:48:26.179850 grai_schemas-0.1.9/src/grai_schemas/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-01-18 14:35:11.049253 grai_schemas-0.1.9/src/grai_schemas/py.typed
+-rw-r--r--   0        0        0      500 2023-01-29 22:48:26.180085 grai_schemas-0.1.9/src/grai_schemas/schema.py
+-rw-r--r--   0        0        0      795 2023-01-31 02:14:01.658847 grai_schemas-0.1.9/src/grai_schemas/utilities.py
+-rw-r--r--   0        0        0      139 2023-01-27 01:14:06.497746 grai_schemas-0.1.9/src/grai_schemas/v1/__init__.py
+-rw-r--r--   0        0        0     1277 2023-01-31 02:14:01.659066 grai_schemas-0.1.9/src/grai_schemas/v1/edge.py
+-rw-r--r--   0        0        0      790 2023-01-31 02:14:01.659316 grai_schemas-0.1.9/src/grai_schemas/v1/generics.py
+-rw-r--r--   0        0        0      269 2023-01-27 01:14:06.497906 grai_schemas-0.1.9/src/grai_schemas/v1/metadata/__init__.py
+-rw-r--r--   0        0        0     1251 2023-02-01 16:24:41.545223 grai_schemas-0.1.9/src/grai_schemas/v1/metadata/edges.py
+-rw-r--r--   0        0        0      289 2023-01-27 01:14:06.497998 grai_schemas-0.1.9/src/grai_schemas/v1/metadata/metadata.py
+-rw-r--r--   0        0        0     1086 2023-01-27 01:14:06.498045 grai_schemas-0.1.9/src/grai_schemas/v1/metadata/nodes.py
+-rw-r--r--   0        0        0     1096 2023-01-29 22:48:26.180432 grai_schemas-0.1.9/src/grai_schemas/v1/node.py
+-rw-r--r--   0        0        0        0 2023-01-27 01:14:06.498108 grai_schemas-0.1.9/src/grai_schemas/v1/workspace.py
+-rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 grai_schemas-0.1.9/setup.py
+-rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 grai_schemas-0.1.9/PKG-INFO
```

### Comparing `grai_schemas-0.1.8/LICENSE` & `grai_schemas-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.1.8/pyproject.toml` & `grai_schemas-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_schemas"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 readme = "README.md"
 license = "Elastic-2.0"
 packages = [{ include = "grai_schemas", from = "src" },]
 
 [tool.poetry.dependencies]
```

### Comparing `grai_schemas-0.1.8/src/grai_schemas/generics.py` & `grai_schemas-0.1.9/src/grai_schemas/generics.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.1.8/src/grai_schemas/utilities.py` & `grai_schemas-0.1.9/src/grai_schemas/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.1.8/src/grai_schemas/v1/edge.py` & `grai_schemas-0.1.9/src/grai_schemas/v1/edge.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.1.8/src/grai_schemas/v1/generics.py` & `grai_schemas-0.1.9/src/grai_schemas/v1/generics.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.1.8/src/grai_schemas/v1/metadata/edges.py` & `grai_schemas-0.1.9/src/grai_schemas/v1/metadata/edges.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from grai_schemas.v1.generics import V1Mixin
 
 
 class EdgeTypeLabels(Enum):
     generic = "Edge"
     table_to_column = "TableToColumn"
     column_to_column = "ColumnToColumn"
+    table_to_table = "TableToTable"
 
 
 class GenericEdgeMetadataV1(V1Mixin):
     edge_type: Literal["Edge"]
     edge_attributes: dict = {}
 
 
@@ -20,14 +21,23 @@
 
 
 class TableToColumnMetadata(GenericEdgeMetadataV1):
     edge_type: Literal["TableToColumn"]
     edge_attributes: TableToColumnAttributes = TableToColumnAttributes()
 
 
+class TableToTableAttributes(V1Mixin):
+    pass
+
+
+class TableToTableMetadata(GenericEdgeMetadataV1):
+    edge_type: Literal["TableToTable"]
+    edge_attributes: TableToColumnAttributes = TableToTableAttributes()
+
+
 class ColumnToColumnAttributes(V1Mixin):
     preserves_data_type: Optional[bool] = None
     preserves_nullable: Optional[bool] = None
     preserves_unique: Optional[bool] = None
 
 
 class ColumnToColumnMetadata(GenericEdgeMetadataV1):
```

### Comparing `grai_schemas-0.1.8/src/grai_schemas/v1/metadata/nodes.py` & `grai_schemas-0.1.9/src/grai_schemas/v1/metadata/nodes.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.1.8/src/grai_schemas/v1/node.py` & `grai_schemas-0.1.9/src/grai_schemas/v1/node.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.1.8/setup.py` & `grai_schemas-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'grai-schemas',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_schemas-0.1.8/PKG-INFO` & `grai_schemas-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-schemas
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

