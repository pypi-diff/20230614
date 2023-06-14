# Comparing `tmp/clevertable-3.0.3.tar.gz` & `tmp/clevertable-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevertable-3.0.3.tar", last modified: Sat Jun  3 10:24:27 2023, max compression
+gzip compressed data, was "clevertable-3.1.0.tar", last modified: Wed Jun 14 06:16:54 2023, max compression
```

## Comparing `clevertable-3.0.3.tar` & `clevertable-3.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 10:24:27.869383 clevertable-3.0.3/
--rw-rw-rw-   0        0        0     1086 2023-06-01 10:04:41.000000 clevertable-3.0.3/LICENSE
--rw-rw-rw-   0        0        0    36138 2023-06-03 10:24:27.868050 clevertable-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    34368 2023-06-01 10:06:41.000000 clevertable-3.0.3/README.md
--rw-rw-rw-   0        0        0     1301 2023-06-03 10:23:46.000000 clevertable-3.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-03 10:24:27.869383 clevertable-3.0.3/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-06-01 10:04:41.000000 clevertable-3.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 10:24:27.716666 clevertable-3.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 10:24:27.820853 clevertable-3.0.3/src/clevertable/
--rw-rw-rw-   0        0        0     3518 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Binary.py
--rw-rw-rw-   0        0        0      268 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Const.py
--rw-rw-rw-   0        0        0     3016 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/ConversionProfile.py
--rw-rw-rw-   0        0        0     3765 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Converter.py
--rw-rw-rw-   0        0        0     4367 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/DataFrameProfile.py
--rw-rw-rw-   0        0        0     1018 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Enumerate.py
--rw-rw-rw-   0        0        0      291 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Flatten.py
--rw-rw-rw-   0        0        0     3297 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Float.py
--rw-rw-rw-   0        0        0      896 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/ForEach.py
--rw-rw-rw-   0        0        0     4976 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Function.py
--rw-rw-rw-   0        0        0      213 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Id.py
--rw-rw-rw-   0        0        0      369 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Ignore.py
--rw-rw-rw-   0        0        0     3087 2023-06-03 10:16:43.000000 clevertable-3.0.3/src/clevertable/Infer.py
--rw-rw-rw-   0        0        0      398 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Label.py
--rw-rw-rw-   0        0        0     3302 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/List.py
--rw-rw-rw-   0        0        0     1566 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Map.py
--rw-rw-rw-   0        0        0     1558 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/OneHot.py
--rw-rw-rw-   0        0        0     1830 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Parallel.py
--rw-rw-rw-   0        0        0     2877 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Pipeline.py
--rw-rw-rw-   0        0        0     9272 2023-06-03 09:39:39.000000 clevertable-3.0.3/src/clevertable/RecordProfile.py
--rw-rw-rw-   0        0        0      843 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Split.py
--rw-rw-rw-   0        0        0     3576 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/StrictFunction.py
--rw-rw-rw-   0        0        0      991 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Strip.py
--rw-rw-rw-   0        0        0     1194 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Transpose.py
--rw-rw-rw-   0        0        0     2769 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Try.py
--rw-rw-rw-   0        0        0      716 2023-06-03 10:23:46.000000 clevertable-3.0.3/src/clevertable/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/__main__.py
--rw-rw-rw-   0        0        0     2501 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-03 10:24:27.852384 clevertable-3.0.3/src/clevertable.egg-info/
--rw-rw-rw-   0        0        0    36138 2023-06-03 10:24:27.000000 clevertable-3.0.3/src/clevertable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2023-06-03 10:24:27.000000 clevertable-3.0.3/src/clevertable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 10:24:27.000000 clevertable-3.0.3/src/clevertable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-03 10:24:27.000000 clevertable-3.0.3/src/clevertable.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-06-03 10:24:27.000000 clevertable-3.0.3/src/clevertable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-03 10:24:27.000000 clevertable-3.0.3/src/clevertable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 06:16:54.828343 clevertable-3.1.0/
+-rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0    36138 2023-06-14 06:16:54.828343 clevertable-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    34368 2023-06-01 10:04:43.000000 clevertable-3.1.0/README.md
+-rw-rw-rw-   0        0        0     1301 2023-06-14 06:15:51.000000 clevertable-3.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:16:54.828343 clevertable-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:16:54.746786 clevertable-3.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 06:16:54.806069 clevertable-3.1.0/src/clevertable/
+-rw-rw-rw-   0        0        0     3518 2023-05-29 17:24:28.000000 clevertable-3.1.0/src/clevertable/Binary.py
+-rw-rw-rw-   0        0        0      268 2023-05-29 17:07:53.000000 clevertable-3.1.0/src/clevertable/Const.py
+-rw-rw-rw-   0        0        0     3016 2023-05-29 17:07:53.000000 clevertable-3.1.0/src/clevertable/ConversionProfile.py
+-rw-rw-rw-   0        0        0     3765 2023-05-29 17:37:25.000000 clevertable-3.1.0/src/clevertable/Converter.py
+-rw-rw-rw-   0        0        0     4527 2023-06-14 06:06:10.000000 clevertable-3.1.0/src/clevertable/DataFrameProfile.py
+-rw-rw-rw-   0        0        0     1018 2023-05-29 18:08:53.000000 clevertable-3.1.0/src/clevertable/Enumerate.py
+-rw-rw-rw-   0        0        0      291 2023-05-29 17:07:53.000000 clevertable-3.1.0/src/clevertable/Flatten.py
+-rw-rw-rw-   0        0        0     3297 2023-05-30 06:09:36.000000 clevertable-3.1.0/src/clevertable/Float.py
+-rw-rw-rw-   0        0        0      896 2023-05-29 17:37:25.000000 clevertable-3.1.0/src/clevertable/ForEach.py
+-rw-rw-rw-   0        0        0     4976 2023-05-29 17:37:25.000000 clevertable-3.1.0/src/clevertable/Function.py
+-rw-rw-rw-   0        0        0      213 2023-05-29 17:07:53.000000 clevertable-3.1.0/src/clevertable/Id.py
+-rw-rw-rw-   0        0        0      369 2023-05-29 17:43:58.000000 clevertable-3.1.0/src/clevertable/Ignore.py
+-rw-rw-rw-   0        0        0     2998 2023-06-14 05:55:27.000000 clevertable-3.1.0/src/clevertable/Infer.py
+-rw-rw-rw-   0        0        0      398 2023-05-29 17:11:23.000000 clevertable-3.1.0/src/clevertable/Label.py
+-rw-rw-rw-   0        0        0     3302 2023-05-29 17:07:53.000000 clevertable-3.1.0/src/clevertable/List.py
+-rw-rw-rw-   0        0        0     1566 2023-05-29 18:13:39.000000 clevertable-3.1.0/src/clevertable/Map.py
+-rw-rw-rw-   0        0        0     1558 2023-05-29 17:59:47.000000 clevertable-3.1.0/src/clevertable/OneHot.py
+-rw-rw-rw-   0        0        0     1830 2023-05-29 17:43:58.000000 clevertable-3.1.0/src/clevertable/Parallel.py
+-rw-rw-rw-   0        0        0     2877 2023-05-29 17:07:53.000000 clevertable-3.1.0/src/clevertable/Pipeline.py
+-rw-rw-rw-   0        0        0     9198 2023-06-14 06:05:59.000000 clevertable-3.1.0/src/clevertable/RecordProfile.py
+-rw-rw-rw-   0        0        0      843 2023-05-29 17:51:55.000000 clevertable-3.1.0/src/clevertable/Split.py
+-rw-rw-rw-   0        0        0     3576 2023-05-29 17:18:36.000000 clevertable-3.1.0/src/clevertable/StrictFunction.py
+-rw-rw-rw-   0        0        0      991 2023-05-29 17:52:36.000000 clevertable-3.1.0/src/clevertable/Strip.py
+-rw-rw-rw-   0        0        0     1194 2023-05-29 17:18:36.000000 clevertable-3.1.0/src/clevertable/Transpose.py
+-rw-rw-rw-   0        0        0     2769 2023-05-29 17:07:53.000000 clevertable-3.1.0/src/clevertable/Try.py
+-rw-rw-rw-   0        0        0      716 2023-06-14 06:15:51.000000 clevertable-3.1.0/src/clevertable/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-05-29 17:07:53.000000 clevertable-3.1.0/src/clevertable/__main__.py
+-rw-rw-rw-   0        0        0     2501 2023-05-29 17:43:58.000000 clevertable-3.1.0/src/clevertable/_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:16:54.822177 clevertable-3.1.0/src/clevertable.egg-info/
+-rw-rw-rw-   0        0        0    36138 2023-06-14 06:16:54.000000 clevertable-3.1.0/src/clevertable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1044 2023-06-14 06:16:54.000000 clevertable-3.1.0/src/clevertable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:16:54.000000 clevertable-3.1.0/src/clevertable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-14 06:16:54.000000 clevertable-3.1.0/src/clevertable.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-06-14 06:16:54.000000 clevertable-3.1.0/src/clevertable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-14 06:16:54.000000 clevertable-3.1.0/src/clevertable.egg-info/top_level.txt
```

### Comparing `clevertable-3.0.3/LICENSE` & `clevertable-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/PKG-INFO` & `clevertable-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 3.0.3
+Version: 3.1.0
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `clevertable-3.0.3/README.md` & `clevertable-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/pyproject.toml` & `clevertable-3.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clevertable"
-version = "3.0.3"
+version = "3.1.0"
 description = "Low effort conversion of tabular data into numerical values."
 readme = "README.md"
 authors = [{ name = "Tom Mohr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -28,15 +28,15 @@
 [project.urls]
 Homepage = "https://github.com/tom-mohr/clevertable"
 
 [project.scripts]
 clevertable = "clevertable.__main__:main"
 
 [tool.bumpver]
-current_version = "3.0.3"
+current_version = "3.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `clevertable-3.0.3/src/clevertable/Binary.py` & `clevertable-3.1.0/src/clevertable/Binary.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/ConversionProfile.py` & `clevertable-3.1.0/src/clevertable/ConversionProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/Converter.py` & `clevertable-3.1.0/src/clevertable/Converter.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/DataFrameProfile.py` & `clevertable-3.1.0/src/clevertable/DataFrameProfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,9 +98,15 @@
 
     def __getitem__(self, item):
         return self._record_profile[item]
 
     def __setitem__(self, key, value):
         self._record_profile[key] = value
 
+    def __delitem__(self, key):
+        del self._record_profile[key]
+    
+    def __contains__(self, item):
+        return item in self._record_profile
+
     def __repr__(self):
         return repr(self._record_profile)
```

### Comparing `clevertable-3.0.3/src/clevertable/Enumerate.py` & `clevertable-3.1.0/src/clevertable/Enumerate.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/Float.py` & `clevertable-3.1.0/src/clevertable/Float.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/ForEach.py` & `clevertable-3.1.0/src/clevertable/ForEach.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/Function.py` & `clevertable-3.1.0/src/clevertable/Function.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/Infer.py` & `clevertable-3.1.0/src/clevertable/Pipeline.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,89 +1,81 @@
 from __future__ import annotations
 
-import re
-
+from .Infer import Infer
 from .Converter import Converter
-from .Ignore import Ignore
-
+from .Id import Id
+from ._utils import _parse_converter
 
-class Infer(Converter):
 
-    def __init__(self, ignore_uninferrable: bool = False):
-        self.ignore_uninferrable = ignore_uninferrable
-        self.inferred = None
+class _Pipeline(Converter):
 
-    def __repr__(self):
-        return repr(self.inferred)
-
-    def __getitem__(self, item):
-        return self.inferred[item]
+    def __init__(self, first: any, second: any):
+        self.first = _parse_converter(first)
+        self.second = _parse_converter(second)
 
     def fit(self, rows: list[tuple]):
-        """
-        Tries to infer this converter from the given data.
-        If a converter could be inferred, it is fitted with the data and stored in self.inferred.
-        :raises ValueError: if no converter can be inferred and ignore_uninferrable is False
-        """
-        try:
-            self.inferred = _infer_converter_from_data(rows)
-        except ValueError as e:
-            if self.ignore_uninferrable:
-                self.inferred = Ignore()
-                return
-            raise e
-        self.inferred.fit(rows)
+        self.first.fit(rows)
+        self.second.fit([self.first.transform(row) for row in rows])
+
+        # replace Infer() converters with the nested inferred converter
+        if isinstance(self.first, Infer):
+            assert self.first.inferred is not None, \
+                f"Infer() converter for did not infer a converter during fit()"
+            self.first = self.first.inferred
+        if isinstance(self.second, Infer):
+            assert self.second.inferred is not None, \
+                f"Infer() converter for did not infer a converter during fit()"
+            self.second = self.second.inferred
 
     def labels(self, labels: tuple) -> tuple:
-        return self.inferred.labels(labels)
+        return self.second.labels(self.first.labels(labels))
 
     def transform(self, row: tuple) -> tuple:
-        return self.inferred.transform(row)
+        return self.second.transform(self.first.transform(row))
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}({repr(self.first)}, {repr(self.second)})"
 
 
-def _infer_converter_from_data(rows: list[tuple]) -> Converter:
-    """Tries to infer the best converter from the given data.
-    If no converter can be inferred, a ValueError is raised."""
-    # dynamic imports in order to break circular dependency
-    from .Binary import Binary
-    from .Enumerate import Enumerate
-    from .Float import Float
-    from .List import List, ListAndOr
-    from .OneHot import OneHot
-
-    # if only contains 1-element rows:
-    if all(len(row) == 1 for row in rows):
-
-        values = [row[0] for row in rows]  # unpack 1-element rows
-
-        def _is_parseable_float(val: any) -> bool:
-            try:
-                float(val)
-            except (ValueError, TypeError, OverflowError):
-                return False
-            return True
-
-        if all(map(_is_parseable_float, values)):
-            return Float()
-
-        # since numerical approach failed,
-        # we now try categorical approaches
-        string_values = [val for val in values if isinstance(val, str)]
-
-        # check if it can be split according to List()
-        regex_list = re.compile(List._DEFAULT_DELIMITER)
-        if any(map(regex_list.search, string_values)):
-            # check if there are also "and" or "or" in the values
-            regex_list_and_or = re.compile("|".join(ListAndOr._DEFAULT_DELIMITER_AND_OR))
-            if any(map(regex_list_and_or.search, string_values)):
-                return ListAndOr()
-            return List()
-
-        num_unique_entries = len(set(values))
-        if num_unique_entries <= 2:
-            return Binary()
-        elif num_unique_entries <= 10:
-            return OneHot()
-        elif num_unique_entries <= 100 or num_unique_entries < 0.1 * len(values):
-            return Enumerate()
+class Pipeline(_Pipeline):
 
-    raise ValueError(f"Cannot infer converter from values: {rows[:5]} ...")
+    def __init__(self, *converters: any):
+        if len(converters) == 0:
+            super().__init__(Id(), Id())
+        elif len(converters) == 1:
+            super().__init__(converters[0], Id())
+        elif len(converters) == 2:
+            super().__init__(converters[0], converters[1])
+        else:
+            super().__init__(converters[0], Pipeline(*converters[1:]))
+
+    def __getitem__(self, index):
+        return self.converters[index]
+
+    @property
+    def converters(self) -> list[Converter]:
+        convs = []
+        if isinstance(self.first, Pipeline):
+            convs.extend(self.first.converters)
+        else:
+            convs.append(self.first)
+        if isinstance(self.second, Pipeline):
+            convs.extend(self.second.converters)
+        else:
+            convs.append(self.second)
+        return convs
+
+    def __repr__(self):
+        converters_without_id = list(filter(lambda conv:
+                                            not type(conv) is Id,  # this will not filter out subclasses of Id!
+                                            self.converters))
+        if len(converters_without_id) <= 1:
+            # in one line
+            return f"[{', '.join(repr(conv) for conv in converters_without_id)}]"
+
+        # in multiple lines
+        s = "[\n"
+        for conv in converters_without_id:
+            s += "\t" + "\n\t".join(repr(conv).split("\n"))
+            s += ",\n"
+        s += "]"
+        return s
```

### Comparing `clevertable-3.0.3/src/clevertable/List.py` & `clevertable-3.1.0/src/clevertable/List.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/Map.py` & `clevertable-3.1.0/src/clevertable/Map.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/OneHot.py` & `clevertable-3.1.0/src/clevertable/OneHot.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/Parallel.py` & `clevertable-3.1.0/src/clevertable/Parallel.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/RecordProfile.py` & `clevertable-3.1.0/src/clevertable/RecordProfile.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,210 +1,216 @@
-from __future__ import annotations
-
-from textwrap import indent
-from typing import Callable
-
-from .Converter import Converter
-from .Ignore import Ignore
-from .Infer import Infer
-from ._utils import _parse_converter, _flatten_tuples, _index_duplicates
-
-
-def _check_and_unpack(row: tuple) -> dict:
-    # unpack a 1-element tuple with a dict
-    assert len(row) == 1, "Expects a 1-element tuple with a dict"
-    val = row[0]  # unpack 1-element tuple
-    assert isinstance(val, dict), "Expects a 1-element tuple with a dict"
-    return val
-
-
-def _getitem_nested(key: any, getitem_func: Callable[[any], any]) -> any:
-    """Key can be an atomic key or a tuple of keys.
-    If present, the nested key structure is preserved in the output.
-    Example::
-        >>> d = {'a': 1, 'b': 2, 'c': 3}
-        >>> _getitem_nested('a', d.get)
-        1
-        >>> _getitem_nested(('a', 'b'), d.get)
-        (1, 2)
-        >>> _getitem_nested(('a', ('b', 'c'), 'a'), d.get)
-        (1, (2, 3), 1)
-        >>> _getitem_nested(('a', 'a', 'a'), d.get)
-        (1, 1, 1)
-        >>> _getitem_nested(('a',), d.get)
-        (1,)
-
-    :param key: The key to lookup. May be an atomic key or a tuple of keys.
-    :param getitem_func: The lookup function. Takes an atomic key and returns the value.
-    """
-    if isinstance(key, tuple):
-        return tuple(_getitem_nested(k, getitem_func) for k in key)
-    return getitem_func(key)
-
-
-def _contains_nested(key: any, contains_func: Callable[[any], any]) -> any:
-    if isinstance(key, tuple):
-        return all(_contains_nested(k, contains_func) for k in key)
-    return contains_func(key)
-
-
-class RecordProfile(Converter):
-    def __init__(self, profile: dict[any, any] = None,
-                 ignore_undefined: bool = False,
-                 ignore_uninferrable: bool = False):
-        """
-        Works on records (dicts).
-        Takes a record, applies a different converter for each key (according to the given profile)
-        and outputs a record with transformed keys and values.
-        The new keys are computed using the label() function of the respective converter.
-        Their cardinality must match the cardinality of the output of the converter.
-
-        For keys that are not present in the profile but appear during fit(), the Infer() converter is used.
-
-        Keys that are not present in the profile and weren't present during fit() are simply ignored.
-
-        :param profile: Maps keys to converters.
-        :param ignore_undefined: If ``False``, all columns without a converter will be assigned a converter
-               automatically. If ``True``, these columns will be ignored instead, i.e. not produce any output columns.
-        :param ignore_uninferrable: If ``True``, keys which are not present in the profile and for which the converter
-               cannot be inferred during ``fit()`` are ignored during transform().
-        """
-        self._profile: dict[any, Converter] = {}
-        if profile:
-            self.update(profile)  # parses converters
-
-        self.keys: dict[any, tuple] = {}  # cache for the output keys computed during fit()
-
-        self.ignore_undefined = ignore_undefined
-        self.ignore_uninferrable = ignore_uninferrable
-
-    def fit(self, rows: list[tuple]):
-        # unpack each row and check the type
-        dicts = [_check_and_unpack(row) for row in rows]
-
-        all_keys = {key for d in dicts for key in d.keys()}  # collect all possible keys present in the dicts
-
-        # replace missing converters with Infer() or Ignore()
-        for key in all_keys:
-            if key not in self._profile:
-                if self.ignore_undefined:
-                    self._profile[key] = Ignore()
-                else:
-                    self._profile[key] = Infer(ignore_uninferrable=self.ignore_uninferrable)
-
-        # now actual fit
-        for key, conv in self._profile.items():
-            if isinstance(key, tuple):
-                rows = [
-                    _getitem_nested(key, d.__getitem__)
-                    for d in dicts
-                    if _contains_nested(key, d.__contains__)
-                ]
-            else:
-                rows = [
-                    (d[key],)  # wrap single element (row needs to be a tuple)
-                    for d in dicts
-                    if key in d
-                ]
-            if not rows:
-                raise ValueError(f"Not a single value for key {repr(key)} present during fit()!"
-                                 f" You must at least provide one value to fit() for this key.")
-                pass
-
-            try:
-                conv.fit(rows)
-            except Exception as e:
-                # add helpful context to error message
-                raise ValueError(f"at key {repr(key)}:\n"
-                                 f"{e.__class__.__name__} during {conv.__class__.__name__}.fit():\n"
-                                 f"{indent(str(e), ' ' * 4)}") from e
-
-        # replace all Infer() converters with the nested inferred converter
-        for key, conv in self._profile.items():
-            if isinstance(conv, Infer):
-                assert conv.inferred is not None, \
-                    f"Infer() converter for key {repr(key)} did not infer a converter during fit()"
-                self._profile[key] = conv.inferred
-
-        # save the output keys
-        for key, conv in self._profile.items():
-            try:
-                if isinstance(key, tuple):
-                    input_labels = key
-                else:
-                    input_labels = (key,)
-                output_labels = conv.labels(input_labels)
-                self.keys[key] = output_labels
-            except Exception as e:
-                # add helpful context to error message
-                raise ValueError(f"at key {repr(key)}:\n"
-                                 f"{e.__class__.__name__} during {conv.__class__.__name__}.labels():\n"
-                                 f"{indent(str(e), ' ' * 4)}") from e
-
-        # handle duplicate output keys
-        input_keys = list(self.keys.keys())
-        output_keys_flat = _flatten_tuples(tuple(self.keys[k]  # not using self.keys.values() because of order
-                                                 for k in self.keys))
-        output_keys_flat = _index_duplicates(output_keys_flat, lambda s, i: f"{s}_{i}")
-        # "unflatten" the output keys and write them back
-        for input_key in input_keys:
-            n = len(self.keys[input_key])  # number of output keys for this input key
-            self.keys[input_key] = output_keys_flat[:n]  # take n first
-            output_keys_flat = output_keys_flat[n:]  # remove n first
-
-    def labels(self, labels: tuple) -> (dict[any, tuple],):
-        """
-        :param labels: Will be ignored, as labels have been inferred from the given records during fit() already.
-        """
-        return (self.keys,)
-
-    def transform(self, row: tuple) -> tuple:
-        """
-        Transforms each value in the given dict with the respective converter.
-        The returned dict has the same keys as the input dict.
-
-        :param row: Must be a 1-element tuple with a dict
-        :return:
-        """
-        input_record = _check_and_unpack(row)
-        output_record = {}
-        for key, converter in self._profile.items():
-            input_values = _getitem_nested(key, input_record.__getitem__)
-            if not isinstance(key, tuple):
-                input_values = (input_values,)
-            try:
-                output_values = converter.transform(input_values)
-            except Exception as e:
-                # add helpful context to error message
-                raise ValueError(f"at key {repr(key)}:\n"
-                                 f"{e.__class__.__name__} during {converter.__class__.__name__}.transform():\n"
-                                 f"{indent(str(e), ' ' * 4)}") from e
-            output_keys = self.keys[key]
-            assert len(output_values) == len(output_keys), \
-                f"at {repr(key)}: Output length of {converter.__class__.__name__} converter" \
-                f" mismatches number of labels: {len(output_values)}!={len(output_keys)}." \
-                f"\n\tInput:\t{[input_record[key]]}" \
-                f"\n\tOutput (length {len(output_values)}):\t{output_values}" \
-                f"\n\tOutput Labels (length {len(output_keys)}):\t{output_keys}"
-            for out_val, out_key in zip(output_values, output_keys):
-                output_record[out_key] = out_val
-        return (output_record,)
-
-    def update(self, profile: dict[str, any]):
-        for key, value in profile.items():
-            self[key] = value
-
-    def __getitem__(self, item):
-        return self._profile[item]
-
-    def __setitem__(self, key, value):
-        self._profile[key] = _parse_converter(value)
-
-    def __repr__(self):
-        s = "{\n"
-        for key, conv in self._profile.items():
-            s += "\t"
-            s += f"{repr(key)}: "
-            s += "\n\t".join(repr(conv).split("\n"))
-            s += ",\n"
-        s += "}"
-        return s
+from __future__ import annotations
+
+from textwrap import indent
+from typing import Callable
+
+from .Converter import Converter
+from .Ignore import Ignore
+from .Infer import Infer
+from ._utils import _parse_converter, _flatten_tuples, _index_duplicates
+
+
+def _check_and_unpack(row: tuple) -> dict:
+    # unpack a 1-element tuple with a dict
+    assert len(row) == 1, "Expects a 1-element tuple with a dict"
+    val = row[0]  # unpack 1-element tuple
+    assert isinstance(val, dict), "Expects a 1-element tuple with a dict"
+    return val
+
+
+def _getitem_nested(key: any, getitem_func: Callable[[any], any]) -> any:
+    """Key can be an atomic key or a tuple of keys.
+    If present, the nested key structure is preserved in the output.
+    Example::
+        >>> d = {'a': 1, 'b': 2, 'c': 3}
+        >>> _getitem_nested('a', d.get)
+        1
+        >>> _getitem_nested(('a', 'b'), d.get)
+        (1, 2)
+        >>> _getitem_nested(('a', ('b', 'c'), 'a'), d.get)
+        (1, (2, 3), 1)
+        >>> _getitem_nested(('a', 'a', 'a'), d.get)
+        (1, 1, 1)
+        >>> _getitem_nested(('a',), d.get)
+        (1,)
+
+    :param key: The key to lookup. May be an atomic key or a tuple of keys.
+    :param getitem_func: The lookup function. Takes an atomic key and returns the value.
+    """
+    if isinstance(key, tuple):
+        return tuple(_getitem_nested(k, getitem_func) for k in key)
+    return getitem_func(key)
+
+
+def _contains_nested(key: any, contains_func: Callable[[any], any]) -> any:
+    if isinstance(key, tuple):
+        return all(_contains_nested(k, contains_func) for k in key)
+    return contains_func(key)
+
+
+class RecordProfile(Converter):
+    def __init__(self, profile: dict[any, any] = None,
+                 ignore_undefined: bool = False,
+                 ignore_uninferrable: bool = False):
+        """
+        Works on records (dicts).
+        Takes a record, applies a different converter for each key (according to the given profile)
+        and outputs a record with transformed keys and values.
+        The new keys are computed using the label() function of the respective converter.
+        Their cardinality must match the cardinality of the output of the converter.
+
+        For keys that are not present in the profile but appear during fit(), the Infer() converter is used.
+
+        Keys that are not present in the profile and weren't present during fit() are simply ignored.
+
+        :param profile: Maps keys to converters.
+        :param ignore_undefined: If ``False``, all columns without a converter will be assigned a converter
+               automatically. If ``True``, these columns will be ignored instead, i.e. not produce any output columns.
+        :param ignore_uninferrable: If ``True``, keys which are not present in the profile and for which the converter
+               cannot be inferred during ``fit()`` are ignored during transform().
+        """
+        self._profile: dict[any, Converter] = {}
+        if profile:
+            self.update(profile)  # parses converters
+
+        self.keys: dict[any, tuple] = {}  # cache for the output keys computed during fit()
+
+        self.ignore_undefined = ignore_undefined
+        self.ignore_uninferrable = ignore_uninferrable
+
+    def fit(self, rows: list[tuple]):
+        # unpack each row and check the type
+        dicts = [_check_and_unpack(row) for row in rows]
+
+        all_keys = {key for d in dicts for key in d.keys()}  # collect all possible keys present in the dicts
+
+        # replace missing converters with Infer() or Ignore()
+        for key in all_keys:
+            if key not in self._profile:
+                if self.ignore_undefined:
+                    self._profile[key] = Ignore()
+                else:
+                    self._profile[key] = Infer(ignore_uninferrable=self.ignore_uninferrable)
+
+        # now actual fit
+        for key, conv in self._profile.items():
+            if isinstance(key, tuple):
+                rows = [
+                    _getitem_nested(key, d.__getitem__)
+                    for d in dicts
+                    if _contains_nested(key, d.__contains__)
+                ]
+            else:
+                rows = [
+                    (d[key],)  # wrap single element (row needs to be a tuple)
+                    for d in dicts
+                    if key in d
+                ]
+            if not rows:
+                raise ValueError(f"Not a single value for key {repr(key)} present during fit()!"
+                                 f" You must at least provide one value to fit() for this key.")
+                pass
+
+            try:
+                conv.fit(rows)
+            except Exception as e:
+                # add helpful context to error message
+                raise ValueError(f"at key {repr(key)}:\n"
+                                 f"{e.__class__.__name__} during {conv.__class__.__name__}.fit():\n"
+                                 f"{indent(str(e), ' ' * 4)}") from e
+
+        # replace all Infer() converters with the nested inferred converter
+        for key, conv in self._profile.items():
+            if isinstance(conv, Infer):
+                assert conv.inferred is not None, \
+                    f"Infer() converter for key {repr(key)} did not infer a converter during fit()"
+                self._profile[key] = conv.inferred
+
+        # save the output keys
+        for key, conv in self._profile.items():
+            try:
+                if isinstance(key, tuple):
+                    input_labels = key
+                else:
+                    input_labels = (key,)
+                output_labels = conv.labels(input_labels)
+                self.keys[key] = output_labels
+            except Exception as e:
+                # add helpful context to error message
+                raise ValueError(f"at key {repr(key)}:\n"
+                                 f"{e.__class__.__name__} during {conv.__class__.__name__}.labels():\n"
+                                 f"{indent(str(e), ' ' * 4)}") from e
+
+        # handle duplicate output keys
+        input_keys = list(self.keys.keys())
+        output_keys_flat = _flatten_tuples(tuple(self.keys[k]  # not using self.keys.values() because of order
+                                                 for k in self.keys))
+        output_keys_flat = _index_duplicates(output_keys_flat, lambda s, i: f"{s}_{i}")
+        # "unflatten" the output keys and write them back
+        for input_key in input_keys:
+            n = len(self.keys[input_key])  # number of output keys for this input key
+            self.keys[input_key] = output_keys_flat[:n]  # take n first
+            output_keys_flat = output_keys_flat[n:]  # remove n first
+
+    def labels(self, labels: tuple) -> (dict[any, tuple],):
+        """
+        :param labels: Will be ignored, as labels have been inferred from the given records during fit() already.
+        """
+        return (self.keys,)
+
+    def transform(self, row: tuple) -> tuple:
+        """
+        Transforms each value in the given dict with the respective converter.
+        The returned dict has the same keys as the input dict.
+
+        :param row: Must be a 1-element tuple with a dict
+        :return:
+        """
+        input_record = _check_and_unpack(row)
+        output_record = {}
+        for key, converter in self._profile.items():
+            input_values = _getitem_nested(key, input_record.__getitem__)
+            if not isinstance(key, tuple):
+                input_values = (input_values,)
+            try:
+                output_values = converter.transform(input_values)
+            except Exception as e:
+                # add helpful context to error message
+                raise ValueError(f"at key {repr(key)}:\n"
+                                 f"{e.__class__.__name__} during {converter.__class__.__name__}.transform():\n"
+                                 f"{indent(str(e), ' ' * 4)}") from e
+            output_keys = self.keys[key]
+            assert len(output_values) == len(output_keys), \
+                f"at {repr(key)}: Output length of {converter.__class__.__name__} converter" \
+                f" mismatches number of labels: {len(output_values)}!={len(output_keys)}." \
+                f"\n\tInput:\t{[input_record[key]]}" \
+                f"\n\tOutput (length {len(output_values)}):\t{output_values}" \
+                f"\n\tOutput Labels (length {len(output_keys)}):\t{output_keys}"
+            for out_val, out_key in zip(output_values, output_keys):
+                output_record[out_key] = out_val
+        return (output_record,)
+
+    def update(self, profile: dict[str, any]):
+        for key, value in profile.items():
+            self[key] = value
+
+    def __getitem__(self, item):
+        return self._profile[item]
+
+    def __setitem__(self, key, value):
+        self._profile[key] = _parse_converter(value)
+
+    def __delitem__(self, key):
+        del self._profile[key]
+
+    def __contains__(self, item):
+        return item in self._profile
+
+    def __repr__(self):
+        s = "{\n"
+        for key, conv in self._profile.items():
+            s += "\t"
+            s += f"{repr(key)}: "
+            s += "\n\t".join(repr(conv).split("\n"))
+            s += ",\n"
+        s += "}"
+        return s
```

### Comparing `clevertable-3.0.3/src/clevertable/Split.py` & `clevertable-3.1.0/src/clevertable/Split.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/StrictFunction.py` & `clevertable-3.1.0/src/clevertable/StrictFunction.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/Strip.py` & `clevertable-3.1.0/src/clevertable/Strip.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/Transpose.py` & `clevertable-3.1.0/src/clevertable/Transpose.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/Try.py` & `clevertable-3.1.0/src/clevertable/Try.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/__init__.py` & `clevertable-3.1.0/src/clevertable/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.0.3"
+__version__ = "3.1.0"
 
 from .Binary import Binary
 from .Const import Const
 from .ConversionProfile import ConversionProfile
 from .Converter import Converter
 from .Enumerate import Enumerate
 from .Flatten import Flatten
```

### Comparing `clevertable-3.0.3/src/clevertable/__main__.py` & `clevertable-3.1.0/src/clevertable/__main__.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable/_utils.py` & `clevertable-3.1.0/src/clevertable/_utils.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.3/src/clevertable.egg-info/PKG-INFO` & `clevertable-3.1.0/src/clevertable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 3.0.3
+Version: 3.1.0
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `clevertable-3.0.3/src/clevertable.egg-info/SOURCES.txt` & `clevertable-3.1.0/src/clevertable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

