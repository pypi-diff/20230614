# Comparing `tmp/superspreader-0.2.2.tar.gz` & `tmp/superspreader-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superspreader-0.2.2.tar", last modified: Tue Jun 13 12:23:34 2023, max compression
+gzip compressed data, was "superspreader-0.2.3.tar", last modified: Wed Jun 14 08:25:17 2023, max compression
```

## Comparing `superspreader-0.2.2.tar` & `superspreader-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:23:34.474596 superspreader-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 12:23:24.000000 superspreader-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-13 12:23:34.474596 superspreader-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-13 12:23:24.000000 superspreader-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 12:23:24.000000 superspreader-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-13 12:23:34.474596 superspreader-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-13 12:23:24.000000 superspreader-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:23:34.470596 superspreader-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:23:34.470596 superspreader-0.2.2/src/superspreader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:23:24.000000 superspreader-0.2.2/src/superspreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-13 12:23:24.000000 superspreader-0.2.2/src/superspreader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-13 12:23:24.000000 superspreader-0.2.2/src/superspreader/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-13 12:23:24.000000 superspreader-0.2.2/src/superspreader/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-13 12:23:24.000000 superspreader-0.2.2/src/superspreader/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-06-13 12:23:24.000000 superspreader-0.2.2/src/superspreader/sheets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:23:34.474596 superspreader-0.2.2/src/superspreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-13 12:23:34.000000 superspreader-0.2.2/src/superspreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-13 12:23:34.000000 superspreader-0.2.2/src/superspreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:23:34.000000 superspreader-0.2.2/src/superspreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 12:23:34.000000 superspreader-0.2.2/src/superspreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 12:23:34.000000 superspreader-0.2.2/src/superspreader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:23:34.474596 superspreader-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-13 12:23:24.000000 superspreader-0.2.2/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-13 12:23:24.000000 superspreader-0.2.2/tests/test_full_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-13 12:23:24.000000 superspreader-0.2.2/tests/test_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:25:16.996271 superspreader-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 08:25:04.000000 superspreader-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-14 08:25:16.996271 superspreader-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-14 08:25:04.000000 superspreader-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 08:25:04.000000 superspreader-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-14 08:25:16.996271 superspreader-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-14 08:25:04.000000 superspreader-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:25:16.992271 superspreader-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:25:16.992271 superspreader-0.2.3/src/superspreader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 08:25:04.000000 superspreader-0.2.3/src/superspreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-14 08:25:04.000000 superspreader-0.2.3/src/superspreader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-14 08:25:04.000000 superspreader-0.2.3/src/superspreader/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-14 08:25:04.000000 superspreader-0.2.3/src/superspreader/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-14 08:25:04.000000 superspreader-0.2.3/src/superspreader/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-06-14 08:25:04.000000 superspreader-0.2.3/src/superspreader/sheets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:25:16.996271 superspreader-0.2.3/src/superspreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-14 08:25:16.000000 superspreader-0.2.3/src/superspreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-14 08:25:16.000000 superspreader-0.2.3/src/superspreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:25:16.000000 superspreader-0.2.3/src/superspreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 08:25:16.000000 superspreader-0.2.3/src/superspreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 08:25:16.000000 superspreader-0.2.3/src/superspreader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:25:16.996271 superspreader-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-14 08:25:04.000000 superspreader-0.2.3/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-14 08:25:04.000000 superspreader-0.2.3/tests/test_full_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-14 08:25:04.000000 superspreader-0.2.3/tests/test_sheet.py
```

### Comparing `superspreader-0.2.2/LICENSE.txt` & `superspreader-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.2/PKG-INFO` & `superspreader-0.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.2
+Version: 0.2.3
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Development Status :: 3 - Alpha
@@ -24,34 +24,34 @@
 
 # Superspreader 🦠
 
 Superspreader is a little helper library that simplifies working with spreadsheets.
 It is built on top of [openpyxl](https://openpyxl.readthedocs.io/en/stable/).
 OpenPyXL is its only dependency.
 
-Instead of looping over rows and columns manually, the structure of a spreadsheet 
+Instead of looping over rows and columns manually, the structure of a spreadsheet
 is described in a class:
 
 ```
 from superspreader import fields
 from superspreader.sheets import BaseSheet
 
 
 class AlbumSheet(BaseSheet):
     """
     This class describes a sheet in an Excel document
     """
-    
+
     sheet_name = "Albums" # The sheet is named “albums”
     header_rows = 3 # The sheet has three header rows
-    
+
     # The column labels are in the second row.
     # It is *not* zero based to match the Excel row number
     label_row = 2
-    
+
 
     # The columns
     artist = fields.CharField(source="Artist", required=True)
     album = fields.CharField(source="Album")
     release_date = fields.DateField(source="Release Date")
     average_review = fields.FloatField(source="Average Review")
     chart_position = fields.IntegerField(source="Chart Position")
@@ -60,37 +60,64 @@
 Ready? Let’s load an Excel spreadsheet!
 
 ```
 if __name__ == "__main__":
     sheet = AlbumSheet("albums.xlsx")
     # Load and parse data from the document
     sheet.load()
-    
+
     print(sheet.has_errors)
     # False
     print(sheet.errors)
     # []
     print(sheet.infos)
     # []
-    
+
     for row_dict in sheet:
         print(row_dict)
-        
+
 # {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5}
 # {'artist': 'The Wombats', 'album': 'Fix Yourself, Not The World', 'release_date': datetime.date(2022, 3, 7), 'average_review': 3.9, 'chart_position': 7}
-# {'artist': 'Kokoroko', 'album': 'Could We Be More', 'release_date': datetime.date(2022, 8, 1), 'average_review': 4.7, 'chart_position': 30}   
+# {'artist': 'Kokoroko', 'album': 'Could We Be More', 'release_date': datetime.date(2022, 8, 1), 'average_review': 4.7, 'chart_position': 30}
 ```
 
 In `tests/spreadsheets` is a sample spreadsheet that is used for testing. Feel free to fiddle around.
 
 There’s a lot more to say and I’ll update the documentation as I go.
 
+## Adding non-spreadsheet fields
+
+To provide additional fields, use `extra_data`. Fields from the spreadsheet take precedence over extra data.
+
+```
+extra_data = {
+    "status": "released"
+}
+sheet = AlbumSheet("albums.xlsx", extra_data=extra_data)
+sheet.load()
+# {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'status': 'released'}
+```
+
+Use a callable for dynamic extra data:
+
+```
+extra_data = {
+    "summary": lambda row: f"{row.get('album')} by {row.get('artist')}"
+}
+
+sheet = AlbumSheet("albums.xlsx", extra_data=extra_data)
+# {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'summary': 'Toy by David Bowie'}
+```
+
 ## Changelog
 
-### 0.1.4
+### 0.2.3
 
-* Adds basic documentation on how to use superspreader
+- Adds support for inheriting sheets (before that, fields from base classes weren’t recognized)
 
----
-The API is inspired by [Django’s model API](https://docs.djangoproject.com/en/dev/ref/models/) and [ElasticSearch DSL](https://elasticsearch-dsl.readthedocs.io/en/latest/persistence.html#document).
+### 0.2.2
 
+- Adds support for callables in `extra_data``
 
+---
+
+The API is inspired by [Django’s model API](https://docs.djangoproject.com/en/dev/ref/models/) and [ElasticSearch DSL](https://elasticsearch-dsl.readthedocs.io/en/latest/persistence.html#document).
```

### Comparing `superspreader-0.2.2/setup.py` & `superspreader-0.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="superspreader",
-    version="0.2.2",
+    version="0.2.3",
     description="Load data from spreadsheets easily",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/julianklotz/superspreader",
     author="Julian Klotz",
     author_email="post@julianklotz.de",
     classifiers=[
```

### Comparing `superspreader-0.2.2/src/superspreader/fields.py` & `superspreader-0.2.3/src/superspreader/fields.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.2/src/superspreader/i18n.py` & `superspreader-0.2.3/src/superspreader/i18n.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.2/src/superspreader/messages.py` & `superspreader-0.2.3/src/superspreader/messages.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.2/src/superspreader/sheets.py` & `superspreader-0.2.3/src/superspreader/sheets.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,17 +176,21 @@
 
     #
     # === Protected ===
     #
 
     def _build_fields(self) -> dict:
         fields = {}
-        for attr, field in self.__class__.__dict__.items():
-            if isinstance(field, BaseField):
-                fields[attr] = field
+
+        bases = self.__class__.mro()
+
+        for base in bases:
+            for attr, field in vars(base).items():
+                if isinstance(field, BaseField):
+                    fields[attr] = field
 
         return fields
 
     def _add_error(self, message, index=None) -> None:
         # Add to row index, if it’s related to a row.
         if isinstance(index, int):
             message = _(
```

### Comparing `superspreader-0.2.2/src/superspreader.egg-info/PKG-INFO` & `superspreader-0.2.3/src/superspreader.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.2
+Version: 0.2.3
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Development Status :: 3 - Alpha
@@ -24,34 +24,34 @@
 
 # Superspreader 🦠
 
 Superspreader is a little helper library that simplifies working with spreadsheets.
 It is built on top of [openpyxl](https://openpyxl.readthedocs.io/en/stable/).
 OpenPyXL is its only dependency.
 
-Instead of looping over rows and columns manually, the structure of a spreadsheet 
+Instead of looping over rows and columns manually, the structure of a spreadsheet
 is described in a class:
 
 ```
 from superspreader import fields
 from superspreader.sheets import BaseSheet
 
 
 class AlbumSheet(BaseSheet):
     """
     This class describes a sheet in an Excel document
     """
-    
+
     sheet_name = "Albums" # The sheet is named “albums”
     header_rows = 3 # The sheet has three header rows
-    
+
     # The column labels are in the second row.
     # It is *not* zero based to match the Excel row number
     label_row = 2
-    
+
 
     # The columns
     artist = fields.CharField(source="Artist", required=True)
     album = fields.CharField(source="Album")
     release_date = fields.DateField(source="Release Date")
     average_review = fields.FloatField(source="Average Review")
     chart_position = fields.IntegerField(source="Chart Position")
@@ -60,37 +60,64 @@
 Ready? Let’s load an Excel spreadsheet!
 
 ```
 if __name__ == "__main__":
     sheet = AlbumSheet("albums.xlsx")
     # Load and parse data from the document
     sheet.load()
-    
+
     print(sheet.has_errors)
     # False
     print(sheet.errors)
     # []
     print(sheet.infos)
     # []
-    
+
     for row_dict in sheet:
         print(row_dict)
-        
+
 # {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5}
 # {'artist': 'The Wombats', 'album': 'Fix Yourself, Not The World', 'release_date': datetime.date(2022, 3, 7), 'average_review': 3.9, 'chart_position': 7}
-# {'artist': 'Kokoroko', 'album': 'Could We Be More', 'release_date': datetime.date(2022, 8, 1), 'average_review': 4.7, 'chart_position': 30}   
+# {'artist': 'Kokoroko', 'album': 'Could We Be More', 'release_date': datetime.date(2022, 8, 1), 'average_review': 4.7, 'chart_position': 30}
 ```
 
 In `tests/spreadsheets` is a sample spreadsheet that is used for testing. Feel free to fiddle around.
 
 There’s a lot more to say and I’ll update the documentation as I go.
 
+## Adding non-spreadsheet fields
+
+To provide additional fields, use `extra_data`. Fields from the spreadsheet take precedence over extra data.
+
+```
+extra_data = {
+    "status": "released"
+}
+sheet = AlbumSheet("albums.xlsx", extra_data=extra_data)
+sheet.load()
+# {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'status': 'released'}
+```
+
+Use a callable for dynamic extra data:
+
+```
+extra_data = {
+    "summary": lambda row: f"{row.get('album')} by {row.get('artist')}"
+}
+
+sheet = AlbumSheet("albums.xlsx", extra_data=extra_data)
+# {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'summary': 'Toy by David Bowie'}
+```
+
 ## Changelog
 
-### 0.1.4
+### 0.2.3
 
-* Adds basic documentation on how to use superspreader
+- Adds support for inheriting sheets (before that, fields from base classes weren’t recognized)
 
----
-The API is inspired by [Django’s model API](https://docs.djangoproject.com/en/dev/ref/models/) and [ElasticSearch DSL](https://elasticsearch-dsl.readthedocs.io/en/latest/persistence.html#document).
+### 0.2.2
 
+- Adds support for callables in `extra_data``
 
+---
+
+The API is inspired by [Django’s model API](https://docs.djangoproject.com/en/dev/ref/models/) and [ElasticSearch DSL](https://elasticsearch-dsl.readthedocs.io/en/latest/persistence.html#document).
```

### Comparing `superspreader-0.2.2/tests/test_fields.py` & `superspreader-0.2.3/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.2/tests/test_full_import.py` & `superspreader-0.2.3/tests/test_full_import.py`

 * *Files identical despite different names*

