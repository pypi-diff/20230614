# Comparing `tmp/metaschema-0.0.2.tar.gz` & `tmp/metaschema-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaschema-0.0.2.tar", max compression
+gzip compressed data, was "metaschema-0.0.3.tar", max compression
```

## Comparing `metaschema-0.0.2.tar` & `metaschema-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1075 2023-02-21 06:35:15.938858 metaschema-0.0.2/LICENSE
--rw-r--r--   0        0        0     1115 2023-05-27 20:50:26.950675 metaschema-0.0.2/README.md
--rw-r--r--   0        0        0      639 2023-06-14 01:17:48.242391 metaschema-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-14 01:17:48.246786 metaschema-0.0.2/src/metaschema/__init__.py
--rw-r--r--   0        0        0     9836 2023-05-27 21:25:33.959152 metaschema-0.0.2/src/metaschema/doc.py
--rw-r--r--   0        0        0     2376 2023-02-21 09:06:26.479087 metaschema-0.0.2/src/metaschema/indicators.py
--rw-r--r--   0        0        0    23342 2023-02-21 09:16:26.541485 metaschema-0.0.2/src/metaschema/indicators2.py
--rw-r--r--   0        0        0     1731 1970-01-01 00:00:00.000000 metaschema-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-02-21 06:35:15.938858 metaschema-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1115 2023-05-27 20:50:26.950675 metaschema-0.0.3/README.md
+-rw-r--r--   0        0        0      639 2023-06-14 04:28:42.426228 metaschema-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-14 04:28:42.430570 metaschema-0.0.3/src/metaschema/__init__.py
+-rw-r--r--   0        0        0     9899 2023-06-14 04:28:15.624915 metaschema-0.0.3/src/metaschema/doc.py
+-rw-r--r--   0        0        0     2376 2023-02-21 09:06:26.479087 metaschema-0.0.3/src/metaschema/indicators.py
+-rw-r--r--   0        0        0    23342 2023-02-21 09:16:26.541485 metaschema-0.0.3/src/metaschema/indicators2.py
+-rw-r--r--   0        0        0     1731 1970-01-01 00:00:00.000000 metaschema-0.0.3/PKG-INFO
```

### Comparing `metaschema-0.0.2/LICENSE` & `metaschema-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metaschema-0.0.2/README.md` & `metaschema-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `metaschema-0.0.2/pyproject.toml` & `metaschema-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metaschema"
-version = "0.0.2"
+version = "0.0.3"
 description = "Repository of Pydantic models for metadata schema."
 license = "MIT License"
 authors = ["Aivin V. Solatorio <avsolatorio@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `metaschema-0.0.2/src/metaschema/doc.py` & `metaschema-0.0.3/src/metaschema/doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,17 +297,17 @@
     id: str
     description: str
     date: str
     vector: None
 
 
 class Model(BaseModel):
-    repositoryid: str
-    published: int
-    overwrite: str
-    metadata_information: MetadataInformation
+    repositoryid: str = None
+    published: int = None
+    overwrite: str = None
+    metadata_information: MetadataInformation = None
     document_description: DocumentDescription
-    provenance: List[ProvenanceItem]
-    tags: List[Tag]
-    lda_topics: List[LdaTopic]
-    embeddings: List[Embedding]
-    additional: Dict[str, Any]
+    provenance: List[ProvenanceItem] = None
+    tags: List[Tag] = None
+    lda_topics: List[LdaTopic] = None
+    embeddings: List[Embedding] = None
+    additional: Dict[str, Any] = None
```

### Comparing `metaschema-0.0.2/src/metaschema/indicators.py` & `metaschema-0.0.3/src/metaschema/indicators.py`

 * *Files identical despite different names*

### Comparing `metaschema-0.0.2/src/metaschema/indicators2.py` & `metaschema-0.0.3/src/metaschema/indicators2.py`

 * *Files identical despite different names*

### Comparing `metaschema-0.0.2/PKG-INFO` & `metaschema-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaschema
-Version: 0.0.2
+Version: 0.0.3
 Summary: Repository of Pydantic models for metadata schema.
 License: MIT
 Author: Aivin V. Solatorio
 Author-email: avsolatorio@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

