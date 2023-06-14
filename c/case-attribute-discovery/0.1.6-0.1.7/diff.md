# Comparing `tmp/case_attribute_discovery-0.1.6.tar.gz` & `tmp/case_attribute_discovery-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "case_attribute_discovery-0.1.6.tar", max compression
+gzip compressed data, was "case_attribute_discovery-0.1.7.tar", max compression
```

## Comparing `case_attribute_discovery-0.1.6.tar` & `case_attribute_discovery-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-06-06 11:52:25.738977 case_attribute_discovery-0.1.6/LICENSE
--rw-r--r--   0        0        0     2049 2023-06-06 11:52:25.738977 case_attribute_discovery-0.1.6/README.md
--rw-r--r--   0        0        0      571 2023-06-06 11:52:25.738977 case_attribute_discovery-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 11:52:25.738977 case_attribute_discovery-0.1.6/src/case_attribute_discovery/__init__.py
--rw-r--r--   0        0        0      362 2023-06-06 11:52:25.738977 case_attribute_discovery-0.1.6/src/case_attribute_discovery/config.py
--rw-r--r--   0        0        0     4293 2023-06-06 11:52:25.738977 case_attribute_discovery-0.1.6/src/case_attribute_discovery/discovery.py
--rw-r--r--   0        0        0     2610 1970-01-01 00:00:00.000000 case_attribute_discovery-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-14 13:36:41.734031 case_attribute_discovery-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2049 2023-06-14 13:36:41.734031 case_attribute_discovery-0.1.7/README.md
+-rw-r--r--   0        0        0      571 2023-06-14 13:36:41.734031 case_attribute_discovery-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 13:36:41.734031 case_attribute_discovery-0.1.7/src/case_attribute_discovery/__init__.py
+-rw-r--r--   0        0        0      362 2023-06-14 13:36:41.734031 case_attribute_discovery-0.1.7/src/case_attribute_discovery/config.py
+-rw-r--r--   0        0        0     4293 2023-06-14 13:36:41.734031 case_attribute_discovery-0.1.7/src/case_attribute_discovery/discovery.py
+-rw-r--r--   0        0        0     2611 1970-01-01 00:00:00.000000 case_attribute_discovery-0.1.7/PKG-INFO
```

### Comparing `case_attribute_discovery-0.1.6/LICENSE` & `case_attribute_discovery-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `case_attribute_discovery-0.1.6/README.md` & `case_attribute_discovery-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `case_attribute_discovery-0.1.6/pyproject.toml` & `case_attribute_discovery-0.1.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "case-attribute-discovery"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "case_attribute_discovery", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 pandas = "^2.0.2"
 setuptools = "^67.8.0"
-pix-framework = "^0.8.8"
+pix-framework = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
 [tool.black]
 line-length = 120
```

### Comparing `case_attribute_discovery-0.1.6/src/case_attribute_discovery/discovery.py` & `case_attribute_discovery-0.1.7/src/case_attribute_discovery/discovery.py`

 * *Files identical despite different names*

### Comparing `case_attribute_discovery-0.1.6/PKG-INFO` & `case_attribute_discovery-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: case-attribute-discovery
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
-Requires-Dist: pix-framework (>=0.8.8,<0.9.0)
+Requires-Dist: pix-framework (>=0.9.0,<0.10.0)
 Requires-Dist: setuptools (>=67.8.0,<68.0.0)
 Description-Content-Type: text/markdown
 
 # Case Attribute Discovery
 
 ![case-attribute-discovery](https://github.com/AutomatedProcessImprovement/case-attribute-discovery/actions/workflows/build.yaml/badge.svg)
 ![version](https://img.shields.io/github/v/tag/AutomatedProcessImprovement/case-attribute-discovery)
```

