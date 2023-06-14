# Comparing `tmp/docbuild-0.1.111.tar.gz` & `tmp/docbuild-0.1.112.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docbuild-0.1.111.tar", last modified: Mon Jun 12 10:35:57 2023, max compression
+gzip compressed data, was "docbuild-0.1.112.tar", last modified: Wed Jun 14 12:23:17 2023, max compression
```

## Comparing `docbuild-0.1.111.tar` & `docbuild-0.1.112.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-12 10:35:57.781215 docbuild-0.1.111/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-12 10:35:57.780849 docbuild-0.1.111/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.111/README.md
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-12 10:35:57.770877 docbuild-0.1.111/docbuild/
--rw-r--r--   0 moran      (501) staff       (20)       63 2023-06-12 10:35:46.000000 docbuild-0.1.111/docbuild/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      438 2023-06-11 11:52:15.000000 docbuild-0.1.111/docbuild/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6297 2023-06-11 16:15:35.000000 docbuild-0.1.111/docbuild/graph.py
--rw-r--r--   0 moran      (501) staff       (20)     4479 2023-06-11 11:17:19.000000 docbuild-0.1.111/docbuild/hocr_parser.py
--rw-r--r--   0 moran      (501) staff       (20)     7417 2023-06-12 10:32:35.000000 docbuild-0.1.111/docbuild/page_creator.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-12 10:35:57.774225 docbuild-0.1.111/docbuild/paragraph_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.111/docbuild/paragraph_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.111/docbuild/paragraph_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6831 2023-06-08 11:20:02.000000 docbuild-0.1.111/docbuild/paragraph_detection/paragraph_extractor.py
--rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.111/docbuild/paragraph_detection/paragraph_sorter.py
--rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.111/docbuild/paragraph_detection/two_columns.py
--rw-r--r--   0 moran      (501) staff       (20)     6062 2023-06-11 11:17:19.000000 docbuild-0.1.111/docbuild/textract_parser.py
--rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.111/docbuild/utils.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-12 10:35:57.779859 docbuild-0.1.111/docbuild/visual_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.111/docbuild/visual_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)    16698 2023-06-11 16:15:54.000000 docbuild-0.1.111/docbuild/visual_detection/bordered_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)    23226 2023-06-11 16:15:35.000000 docbuild-0.1.111/docbuild/visual_detection/borderless_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)      257 2023-06-11 11:52:24.000000 docbuild-0.1.111/docbuild/visual_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)    16302 2023-06-11 16:15:35.000000 docbuild-0.1.111/docbuild/visual_detection/vis_line_detection.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-12 10:35:57.772315 docbuild-0.1.111/docbuild.egg-info/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-12 10:35:57.000000 docbuild-0.1.111/docbuild.egg-info/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)      798 2023-06-12 10:35:57.000000 docbuild-0.1.111/docbuild.egg-info/SOURCES.txt
--rw-r--r--   0 moran      (501) staff       (20)        1 2023-06-12 10:35:57.000000 docbuild-0.1.111/docbuild.egg-info/dependency_links.txt
--rw-r--r--   0 moran      (501) staff       (20)       97 2023-06-12 10:35:57.000000 docbuild-0.1.111/docbuild.egg-info/requires.txt
--rw-r--r--   0 moran      (501) staff       (20)        9 2023-06-12 10:35:57.000000 docbuild-0.1.111/docbuild.egg-info/top_level.txt
--rw-r--r--   0 moran      (501) staff       (20)       38 2023-06-12 10:35:57.781273 docbuild-0.1.111/setup.cfg
--rw-r--r--   0 moran      (501) staff       (20)      857 2023-06-12 10:35:51.000000 docbuild-0.1.111/setup.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-14 12:23:17.018692 docbuild-0.1.112/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-14 12:23:17.018545 docbuild-0.1.112/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.112/README.md
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-14 12:23:17.015060 docbuild-0.1.112/docbuild/
+-rw-r--r--   0 moran      (501) staff       (20)       63 2023-06-14 12:22:47.000000 docbuild-0.1.112/docbuild/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      438 2023-06-11 11:52:15.000000 docbuild-0.1.112/docbuild/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6297 2023-06-11 16:15:35.000000 docbuild-0.1.112/docbuild/graph.py
+-rw-r--r--   0 moran      (501) staff       (20)     4479 2023-06-11 11:17:19.000000 docbuild-0.1.112/docbuild/hocr_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)     7417 2023-06-14 12:20:13.000000 docbuild-0.1.112/docbuild/page_creator.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-14 12:23:17.016986 docbuild-0.1.112/docbuild/paragraph_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.112/docbuild/paragraph_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.112/docbuild/paragraph_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6831 2023-06-08 11:20:02.000000 docbuild-0.1.112/docbuild/paragraph_detection/paragraph_extractor.py
+-rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.112/docbuild/paragraph_detection/paragraph_sorter.py
+-rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.112/docbuild/paragraph_detection/two_columns.py
+-rw-r--r--   0 moran      (501) staff       (20)     6062 2023-06-11 11:17:19.000000 docbuild-0.1.112/docbuild/textract_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.112/docbuild/utils.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-14 12:23:17.018221 docbuild-0.1.112/docbuild/visual_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.112/docbuild/visual_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)    16698 2023-06-14 12:20:13.000000 docbuild-0.1.112/docbuild/visual_detection/bordered_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)    23404 2023-06-14 12:21:11.000000 docbuild-0.1.112/docbuild/visual_detection/borderless_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)      257 2023-06-11 11:52:24.000000 docbuild-0.1.112/docbuild/visual_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)    16302 2023-06-11 16:15:35.000000 docbuild-0.1.112/docbuild/visual_detection/vis_line_detection.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-14 12:23:17.016008 docbuild-0.1.112/docbuild.egg-info/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-14 12:23:16.000000 docbuild-0.1.112/docbuild.egg-info/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)      798 2023-06-14 12:23:16.000000 docbuild-0.1.112/docbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 moran      (501) staff       (20)        1 2023-06-14 12:23:16.000000 docbuild-0.1.112/docbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 moran      (501) staff       (20)       97 2023-06-14 12:23:16.000000 docbuild-0.1.112/docbuild.egg-info/requires.txt
+-rw-r--r--   0 moran      (501) staff       (20)        9 2023-06-14 12:23:16.000000 docbuild-0.1.112/docbuild.egg-info/top_level.txt
+-rw-r--r--   0 moran      (501) staff       (20)       38 2023-06-14 12:23:17.018730 docbuild-0.1.112/setup.cfg
+-rw-r--r--   0 moran      (501) staff       (20)      857 2023-06-14 12:23:11.000000 docbuild-0.1.112/setup.py
```

### Comparing `docbuild-0.1.111/PKG-INFO` & `docbuild-0.1.112/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.111
+Version: 0.1.112
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.111/docbuild/graph.py` & `docbuild-0.1.112/docbuild/graph.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.111/docbuild/hocr_parser.py` & `docbuild-0.1.112/docbuild/hocr_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.111/docbuild/page_creator.py` & `docbuild-0.1.112/docbuild/page_creator.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.111/docbuild/paragraph_detection/paragraph_extractor.py` & `docbuild-0.1.112/docbuild/paragraph_detection/paragraph_extractor.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.111/docbuild/paragraph_detection/paragraph_sorter.py` & `docbuild-0.1.112/docbuild/paragraph_detection/paragraph_sorter.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.111/docbuild/paragraph_detection/two_columns.py` & `docbuild-0.1.112/docbuild/paragraph_detection/two_columns.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.111/docbuild/textract_parser.py` & `docbuild-0.1.112/docbuild/textract_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.111/docbuild/utils.py` & `docbuild-0.1.112/docbuild/utils.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.111/docbuild/visual_detection/bordered_table_extraction.py` & `docbuild-0.1.112/docbuild/visual_detection/bordered_table_extraction.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.111/docbuild/visual_detection/borderless_table_extraction.py` & `docbuild-0.1.112/docbuild/visual_detection/borderless_table_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from docstruct.spatial_grid_indexing import SpatialGrid
 from ..visual_detection.constants import SPATIAL_GRID_SIZE
 from typing import Optional
 
 import numpy as np
 import string
+import logging
 
 
 class BorderLessTableExtractor:
     def __init__(self):
         pass
 
 
@@ -540,21 +541,25 @@
             docstruct_cols.append(TableColumn(
                 children=docstruct_cells
             ))
         docstruct_table = Table(children=docstruct_cols, table_type=TableType.BORDERLESS_TABLE)
         return docstruct_table
 
     def extract_tables(self) -> list[Table]:
-        # Look for columns
-        column_extractor = ColumnExtractor(self.lines)
-        columns = column_extractor.extract_columns()
-        # Aggregate columns
-        aggregate_columns = self.aggregate_aligned_columns(columns)
-        # Look for missing lines
-        bb_tables = self.cluster_lines_to_tables(aggregate_columns)
-        # Look for potential headers
-        forced_headers = [self.force_headers(table) for table in bb_tables]
-        for t,f in zip(bb_tables, forced_headers):
-            self.decide_which_headers(t, f)
-        bb_tables = self.unite_tables(bb_tables)
-        tables = [self.convert_bounding_box_table_to_table(table) for table in bb_tables]
-        return tables
+        try:
+            # Look for columns
+            column_extractor = ColumnExtractor(self.lines)
+            columns = column_extractor.extract_columns()
+            # Aggregate columns
+            aggregate_columns = self.aggregate_aligned_columns(columns)
+            # Look for missing lines
+            bb_tables = self.cluster_lines_to_tables(aggregate_columns)
+            # Look for potential headers
+            forced_headers = [self.force_headers(table) for table in bb_tables]
+            for t,f in zip(bb_tables, forced_headers):
+                self.decide_which_headers(t, f)
+            bb_tables = self.unite_tables(bb_tables)
+            tables = [self.convert_bounding_box_table_to_table(table) for table in bb_tables]
+            return tables
+        except Exception as e:
+            logging.error(f"Error: {e}")
+            return []
```

### Comparing `docbuild-0.1.111/docbuild/visual_detection/vis_line_detection.py` & `docbuild-0.1.112/docbuild/visual_detection/vis_line_detection.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.111/docbuild.egg-info/PKG-INFO` & `docbuild-0.1.112/docbuild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.111
+Version: 0.1.112
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.111/docbuild.egg-info/SOURCES.txt` & `docbuild-0.1.112/docbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.111/setup.py` & `docbuild-0.1.112/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="docbuild",
-    version="0.1.111",
+    version="0.1.112",
     description="A package for building a document from a textract response, for more information see the docstruct package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Moran Nechushtan, Serah Tapia, Shlomo Agishtein",
     author_email="moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com",
     url="https://github.com/smrt-co/docbuild",
     packages=setuptools.find_packages(),
```

