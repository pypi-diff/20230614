# Comparing `tmp/superspreader-0.2.3.tar.gz` & `tmp/superspreader-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superspreader-0.2.3.tar", last modified: Wed Jun 14 08:25:17 2023, max compression
+gzip compressed data, was "superspreader-0.2.4.tar", last modified: Wed Jun 14 15:15:59 2023, max compression
```

## Comparing `superspreader-0.2.3.tar` & `superspreader-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:25:16.996271 superspreader-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 08:25:04.000000 superspreader-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-14 08:25:16.996271 superspreader-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-14 08:25:04.000000 superspreader-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 08:25:04.000000 superspreader-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-14 08:25:16.996271 superspreader-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-14 08:25:04.000000 superspreader-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:25:16.992271 superspreader-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:25:16.992271 superspreader-0.2.3/src/superspreader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 08:25:04.000000 superspreader-0.2.3/src/superspreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-14 08:25:04.000000 superspreader-0.2.3/src/superspreader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-14 08:25:04.000000 superspreader-0.2.3/src/superspreader/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-14 08:25:04.000000 superspreader-0.2.3/src/superspreader/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-14 08:25:04.000000 superspreader-0.2.3/src/superspreader/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-06-14 08:25:04.000000 superspreader-0.2.3/src/superspreader/sheets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:25:16.996271 superspreader-0.2.3/src/superspreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-14 08:25:16.000000 superspreader-0.2.3/src/superspreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-14 08:25:16.000000 superspreader-0.2.3/src/superspreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:25:16.000000 superspreader-0.2.3/src/superspreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 08:25:16.000000 superspreader-0.2.3/src/superspreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 08:25:16.000000 superspreader-0.2.3/src/superspreader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:25:16.996271 superspreader-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-14 08:25:04.000000 superspreader-0.2.3/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-14 08:25:04.000000 superspreader-0.2.3/tests/test_full_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-14 08:25:04.000000 superspreader-0.2.3/tests/test_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:15:59.955763 superspreader-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 15:15:50.000000 superspreader-0.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-14 15:15:59.955763 superspreader-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-14 15:15:50.000000 superspreader-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 15:15:50.000000 superspreader-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-14 15:15:59.959763 superspreader-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-14 15:15:50.000000 superspreader-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:15:59.955763 superspreader-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:15:59.955763 superspreader-0.2.4/src/superspreader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:15:50.000000 superspreader-0.2.4/src/superspreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-14 15:15:50.000000 superspreader-0.2.4/src/superspreader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-14 15:15:50.000000 superspreader-0.2.4/src/superspreader/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-14 15:15:50.000000 superspreader-0.2.4/src/superspreader/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-14 15:15:50.000000 superspreader-0.2.4/src/superspreader/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-14 15:15:50.000000 superspreader-0.2.4/src/superspreader/sheets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:15:59.955763 superspreader-0.2.4/src/superspreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-14 15:15:59.000000 superspreader-0.2.4/src/superspreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-14 15:15:59.000000 superspreader-0.2.4/src/superspreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:15:59.000000 superspreader-0.2.4/src/superspreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 15:15:59.000000 superspreader-0.2.4/src/superspreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 15:15:59.000000 superspreader-0.2.4/src/superspreader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:15:59.955763 superspreader-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-14 15:15:50.000000 superspreader-0.2.4/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-14 15:15:50.000000 superspreader-0.2.4/tests/test_full_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-14 15:15:50.000000 superspreader-0.2.4/tests/test_sheet.py
```

### Comparing `superspreader-0.2.3/LICENSE.txt` & `superspreader-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.3/PKG-INFO` & `superspreader-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.3
+Version: 0.2.4
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `superspreader-0.2.3/README.md` & `superspreader-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.3/setup.py` & `superspreader-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="superspreader",
-    version="0.2.3",
+    version="0.2.4",
     description="Load data from spreadsheets easily",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/julianklotz/superspreader",
     author="Julian Klotz",
     author_email="post@julianklotz.de",
     classifiers=[
```

### Comparing `superspreader-0.2.3/src/superspreader/fields.py` & `superspreader-0.2.4/src/superspreader/fields.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.3/src/superspreader/i18n.py` & `superspreader-0.2.4/src/superspreader/i18n.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.3/src/superspreader/messages.py` & `superspreader-0.2.4/src/superspreader/messages.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.3/src/superspreader/sheets.py` & `superspreader-0.2.4/src/superspreader/sheets.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,23 +110,24 @@
                             extra_context=extra_context,
                         )
                     except ValidationException as error:
                         row_dict[name] = None
                         error_cache.append((str(error), row_index))
                 except KeyError:
                     pass
-            # Use extra data as a basis
-            full_dict = self.get_extra_data(row_dict)
-            # And update with “real” data, which takes precedence
-            full_dict.update(row_dict)
 
-            if self.shall_skip(full_dict):
+            # Evaluate before adding extra data
+            if self.shall_skip(row_dict):
                 self._add_info("Skipped row", index=row_index)
                 continue
             else:
+                # Use extra data as a basis
+                full_dict = self.get_extra_data(row_dict)
+                # And update with “real” data, which takes precedence
+                full_dict.update(row_dict)
                 self._rows.append(full_dict)
                 self._add_errors(error_cache)
 
     def get_sheet_name(self):
         """
         Gets the sheet
         :return: str
```

### Comparing `superspreader-0.2.3/src/superspreader.egg-info/PKG-INFO` & `superspreader-0.2.4/src/superspreader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.3
+Version: 0.2.4
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `superspreader-0.2.3/tests/test_fields.py` & `superspreader-0.2.4/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.3/tests/test_full_import.py` & `superspreader-0.2.4/tests/test_full_import.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.3/tests/test_sheet.py` & `superspreader-0.2.4/tests/test_sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import unittest
 
 from superspreader.exceptions import ImproperlyConfigured
 from superspreader.sheets import BaseSheet
 from superspreader import fields
 
 
-
 class TestSheet(unittest.TestCase):
     def test_sheet_name(self):
         class AlbumSheet(BaseSheet):
             pass
 
         with self.assertRaises(ImproperlyConfigured):
             AlbumSheet(path="test")
@@ -40,10 +39,7 @@
         class BSheet(ASheet):
             pass
 
         sheet = BSheet(path="test")
         sheet_fields = sheet._build_fields()
 
         self.assertTrue('a_field' in sheet_fields)
-
-
-
```

