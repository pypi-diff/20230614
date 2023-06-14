# Comparing `tmp/casanova-1.8.0a2.tar.gz` & `tmp/casanova-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/casanova-1.8.0a2.tar", last modified: Wed Apr  5 09:51:48 2023, max compression
+gzip compressed data, was "dist/casanova-1.9.0.tar", last modified: Thu Apr 27 09:12:52 2023, max compression
```

## Comparing `casanova-1.8.0a2.tar` & `casanova-1.9.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-04-05 09:51:48.000000 casanova-1.8.0a2/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    36933 2023-04-05 09:51:48.000000 casanova-1.8.0a2/PKG-INFO
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    30111 2023-03-28 09:04:58.000000 casanova-1.8.0a2/README.md
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1211 2023-03-28 09:04:58.000000 casanova-1.8.0a2/casanova/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    12958 2023-04-05 09:22:51.000000 casanova-1.8.0a2/casanova/__main__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    14278 2023-04-05 09:27:15.000000 casanova-1.8.0a2/casanova/cli.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3298 2023-02-14 10:56:01.000000 casanova-1.8.0a2/casanova/contiguous_range_set.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2090 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/defaults.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     8020 2023-03-28 09:04:58.000000 casanova-1.8.0a2/casanova/enricher.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1652 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    16577 2023-03-28 09:04:58.000000 casanova-1.8.0a2/casanova/headers.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1227 2023-02-24 13:49:12.000000 casanova-1.8.0a2/casanova/http.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    10161 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/namedrecord.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      450 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/ndjson.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    14525 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/reader.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     7415 2023-02-24 12:30:01.000000 casanova-1.8.0a2/casanova/resumers.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3024 2023-02-17 09:45:23.000000 casanova-1.8.0a2/casanova/reverse_reader.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2874 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/serialization.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     7430 2023-03-31 13:21:46.000000 casanova-1.8.0a2/casanova/utils.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4168 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/writer.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    36933 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/PKG-INFO
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      675 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/SOURCES.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/dependency_links.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       83 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/entry_points.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      114 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/requires.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       17 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/top_level.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/zip-safe
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-04-05 09:51:48.000000 casanova-1.8.0a2/scripts/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-02-24 12:50:33.000000 casanova-1.8.0a2/scripts/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      198 2023-02-24 13:49:12.000000 casanova-1.8.0a2/scripts/http.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      189 2023-02-15 10:13:26.000000 casanova-1.8.0a2/scripts/null_byte_writer_error.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       38 2023-04-05 09:51:48.000000 casanova-1.8.0a2/setup.cfg
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1016 2023-04-05 09:51:28.000000 casanova-1.8.0a2/setup.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-04-27 09:12:52.000000 casanova-1.9.0/
+-rw-r--r--   0 Yomgui     (501) staff       (20)    36931 2023-04-27 09:12:52.000000 casanova-1.9.0/PKG-INFO
+-rw-r--r--   0 Yomgui     (501) staff       (20)    30111 2023-03-27 12:52:48.000000 casanova-1.9.0/README.md
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-04-27 09:12:52.000000 casanova-1.9.0/casanova/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1211 2023-03-27 12:42:01.000000 casanova-1.9.0/casanova/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    12958 2023-04-06 07:57:31.000000 casanova-1.9.0/casanova/__main__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    14278 2023-04-06 07:57:31.000000 casanova-1.9.0/casanova/cli.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3298 2023-02-15 19:50:58.000000 casanova-1.9.0/casanova/contiguous_range_set.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2090 2023-02-27 08:37:06.000000 casanova-1.9.0/casanova/defaults.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     8020 2023-03-24 15:04:16.000000 casanova-1.9.0/casanova/enricher.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1652 2023-02-27 12:19:46.000000 casanova-1.9.0/casanova/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    16577 2023-03-27 12:47:25.000000 casanova-1.9.0/casanova/headers.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1227 2023-02-24 20:55:02.000000 casanova-1.9.0/casanova/http.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    10708 2023-04-27 09:06:25.000000 casanova-1.9.0/casanova/namedrecord.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      450 2023-02-27 11:54:09.000000 casanova-1.9.0/casanova/ndjson.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    14525 2023-03-03 18:58:41.000000 casanova-1.9.0/casanova/reader.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     7415 2023-02-24 20:55:02.000000 casanova-1.9.0/casanova/resumers.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3024 2023-02-16 09:15:22.000000 casanova-1.9.0/casanova/reverse_reader.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3450 2023-04-27 08:48:48.000000 casanova-1.9.0/casanova/serialization.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     7430 2023-04-01 11:02:05.000000 casanova-1.9.0/casanova/utils.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4168 2023-03-11 16:53:03.000000 casanova-1.9.0/casanova/writer.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-04-27 09:12:52.000000 casanova-1.9.0/casanova.egg-info/
+-rw-r--r--   0 Yomgui     (501) staff       (20)    36931 2023-04-27 09:12:52.000000 casanova-1.9.0/casanova.egg-info/PKG-INFO
+-rw-r--r--   0 Yomgui     (501) staff       (20)      675 2023-04-27 09:12:52.000000 casanova-1.9.0/casanova.egg-info/SOURCES.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-04-27 09:12:52.000000 casanova-1.9.0/casanova.egg-info/dependency_links.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)       83 2023-04-27 09:12:52.000000 casanova-1.9.0/casanova.egg-info/entry_points.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)      114 2023-04-27 09:12:52.000000 casanova-1.9.0/casanova.egg-info/requires.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)       17 2023-04-27 09:12:52.000000 casanova-1.9.0/casanova.egg-info/top_level.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-04-27 09:12:52.000000 casanova-1.9.0/casanova.egg-info/zip-safe
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-04-27 09:12:52.000000 casanova-1.9.0/scripts/
+-rw-r--r--   0 Yomgui     (501) staff       (20)        0 2023-02-24 20:55:02.000000 casanova-1.9.0/scripts/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      198 2023-02-24 20:55:02.000000 casanova-1.9.0/scripts/http.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      189 2023-02-15 19:50:58.000000 casanova-1.9.0/scripts/null_byte_writer_error.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)       38 2023-04-27 09:12:52.000000 casanova-1.9.0/setup.cfg
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1013 2023-04-27 09:11:09.000000 casanova-1.9.0/setup.py
```

### Comparing `casanova-1.8.0a2/PKG-INFO` & `casanova-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casanova
-Version: 1.8.0a2
+Version: 1.9.0
 Summary: Specialized & performant CSV readers, writers and enrichers for python.
 Home-page: http://github.com/medialab/casanova
 Author: Guillaume Plique
 Author-email: kropotkinepiotr@gmail.com
 License: MIT
 Description: [![Build Status](https://github.com/medialab/casanova/workflows/Tests/badge.svg)](https://github.com/medialab/casanova/actions)
```

### Comparing `casanova-1.8.0a2/README.md` & `casanova-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/__init__.py` & `casanova-1.9.0/casanova/__init__.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/__main__.py` & `casanova-1.9.0/casanova/__main__.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/cli.py` & `casanova-1.9.0/casanova/cli.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/contiguous_range_set.py` & `casanova-1.9.0/casanova/contiguous_range_set.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/defaults.py` & `casanova-1.9.0/casanova/defaults.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/enricher.py` & `casanova-1.9.0/casanova/enricher.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/exceptions.py` & `casanova-1.9.0/casanova/exceptions.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/headers.py` & `casanova-1.9.0/casanova/headers.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/http.py` & `casanova-1.9.0/casanova/http.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/namedrecord.py` & `casanova-1.9.0/casanova/namedrecord.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Casanova Named Record Helper
 # =============================================================================
 #
 # CSV-aware improvement over python's namedtuple.
 #
 import sys
 import json
-from typing import Optional, Iterable, Union, List
+from typing import Optional, Iterable, Union, List, Callable, Any
 
 if sys.version_info[:2] >= (3, 10):
     from typing import get_origin, get_args
 else:
     from typing_extensions import get_origin, get_args
 
 from collections import OrderedDict, namedtuple
@@ -143,14 +143,15 @@
     *,
     plural_separator: Optional[str] = None,
     none_value: Optional[str] = None,
     true_value: Optional[str] = None,
     false_value: Optional[str] = None,
     stringify_everything: Optional[bool] = None,
     as_json: Optional[bool] = None,
+    serializer: Optional[Callable[[Any], str]] = None,
     **field_kwargs
 ):
     f = field(**field_kwargs)
 
     f_serialization_options = {}
 
     if plural_separator is not None:
@@ -167,14 +168,17 @@
 
     if stringify_everything is not None:
         f_serialization_options["stringify_everything"] = stringify_everything
 
     if as_json is not None and as_json:
         f_serialization_options["as_json"] = as_json
 
+    if serializer is not None:
+        f_serialization_options["serializer"] = serializer
+
     if f_serialization_options:
         TABULAR_FIELDS[f] = f_serialization_options
 
     return f
 
 
 NoneType = type(None)
@@ -322,17 +326,23 @@
 
         for f in _cached_fields(self):
             f_options = {**options, **TABULAR_FIELDS.get(f, {})}
 
             if is_tabular_record_class(f.type):
                 row.extend(getattr(self, f.name).as_csv_row())
             else:
-                row.append(
-                    TABULAR_RECORD_SERIALIZER(getattr(self, f.name), **f_options)
-                )
+                custom_serializer = f_options.get("serializer")
+                v = getattr(self, f.name)
+
+                if custom_serializer is not None:
+                    s = custom_serializer(v)
+                else:
+                    s = TABULAR_RECORD_SERIALIZER(v, **f_options)
+
+                row.append(s)
 
         return row
 
     def as_csv_dict_row(self):
         row = {}
 
         options = self._serializer_options
@@ -342,17 +352,23 @@
 
             if is_tabular_record_class(f.type):
                 data = getattr(self, f.name).as_csv_dict_row()
 
                 for n, v in data.items():
                     row[f.name + "_" + n] = v
             else:
-                row[f.name] = TABULAR_RECORD_SERIALIZER(
-                    getattr(self, f.name), **f_options
-                )
+                custom_serializer = f_options.get("serializer")
+                v = getattr(self, f.name)
+
+                if custom_serializer is not None:
+                    s = custom_serializer(v)
+                else:
+                    s = TABULAR_RECORD_SERIALIZER(v, **f_options)
+
+                row[f.name] = s
 
         return row
 
 
 def coerce_row(row, consume=False):
     as_csv_row = getattr(row, "as_csv_row", None)
```

### Comparing `casanova-1.8.0a2/casanova/reader.py` & `casanova-1.9.0/casanova/reader.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/resumers.py` & `casanova-1.9.0/casanova/resumers.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/reverse_reader.py` & `casanova-1.9.0/casanova/reverse_reader.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/serialization.py` & `casanova-1.9.0/casanova/serialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,66 @@
-from typing import Optional, Iterable, Mapping, Any
+from typing import Optional, Iterable, Mapping, Any, Dict, Callable, Type
 
 from json import dumps
 from datetime import date, datetime, time
 
 NUMBERS = (int, float)
 DATES = (date, datetime, time)
 LISTS = (list, set, frozenset, tuple)
 
+CustomTypes = Dict[Type, Callable[[Type], str]]
+
 
 class CSVSerializer(object):
     def __init__(
         self,
         plural_separator: Optional[str] = None,
         none_value: Optional[str] = None,
         true_value: Optional[str] = None,
         false_value: Optional[str] = None,
         stringify_everything: Optional[bool] = None,
+        custom_types: Optional[CustomTypes] = None,
     ):
         self.plural_separator = plural_separator or "|"
         self.none_value = none_value or ""
         self.true_value = true_value or "true"
         self.false_value = false_value or "false"
         self.stringify_everything = (
             stringify_everything if stringify_everything is not None else True
         )
+        self.custom_types = custom_types
 
     def __call__(
         self,
         value,
         plural_separator: Optional[str] = None,
         none_value: Optional[str] = None,
         true_value: Optional[str] = None,
         false_value: Optional[str] = None,
+        custom_types: Optional[CustomTypes] = None,
         stringify_everything: Optional[bool] = None,
         as_json: bool = False,
     ):
         if as_json:
             return dumps(value, ensure_ascii=False)
 
         stringify_everything = (
             stringify_everything
             if stringify_everything is not None
             else self.stringify_everything
         )
 
+        custom_types = custom_types if custom_types is not None else self.custom_types
+
+        if custom_types is not None:
+            custom_serializer = custom_types.get(type(value))
+
+            if custom_serializer is not None:
+                return custom_serializer(value)
+
         if value is None:
             none_value = none_value if none_value is not None else self.none_value
 
             if not none_value and not stringify_everything:
                 return None
 
             return none_value
@@ -74,14 +87,17 @@
                 else self.plural_separator
             )
             return plural_separator.join(str(i) for i in value)
 
         if isinstance(value, DATES):
             return value.isoformat()
 
+        if isinstance(value, BaseException):
+            return repr(value)
+
         raise NotImplementedError(
             "CSVSerializer does not support this kind of value: {}".format(
                 value.__class__.__name__
             )
         )
 
     def serialize_row(self, row: Iterable, **kwargs):
```

### Comparing `casanova-1.8.0a2/casanova/utils.py` & `casanova-1.9.0/casanova/utils.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova/writer.py` & `casanova-1.9.0/casanova/writer.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/casanova.egg-info/PKG-INFO` & `casanova-1.9.0/casanova.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casanova
-Version: 1.8.0a2
+Version: 1.9.0
 Summary: Specialized & performant CSV readers, writers and enrichers for python.
 Home-page: http://github.com/medialab/casanova
 Author: Guillaume Plique
 Author-email: kropotkinepiotr@gmail.com
 License: MIT
 Description: [![Build Status](https://github.com/medialab/casanova/workflows/Tests/badge.svg)](https://github.com/medialab/casanova/actions)
```

### Comparing `casanova-1.8.0a2/casanova.egg-info/SOURCES.txt` & `casanova-1.9.0/casanova.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a2/setup.py` & `casanova-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="casanova",
-    version="1.8.0-a2",
+    version="1.9.0",
     description="Specialized & performant CSV readers, writers and enrichers for python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/medialab/casanova",
     license="MIT",
     author="Guillaume Plique",
     author_email="kropotkinepiotr@gmail.com",
```

