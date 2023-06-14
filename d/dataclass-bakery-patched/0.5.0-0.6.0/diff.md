# Comparing `tmp/dataclass_bakery_patched-0.5.0.tar.gz` & `tmp/dataclass_bakery_patched-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_bakery_patched-0.5.0.tar", max compression
+gzip compressed data, was "dataclass_bakery_patched-0.6.0.tar", max compression
```

## Comparing `dataclass_bakery_patched-0.5.0.tar` & `dataclass_bakery_patched-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0        0 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/__init__.py
--rw-r--r--   0        0        0      675 2023-06-13 11:26:46.274978 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/baker.py
--rw-r--r--   0        0        0        0 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/__init__.py
--rw-r--r--   0        0        0     2980 2023-06-13 11:23:25.696246 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/defaults.py
--rw-r--r--   0        0        0      145 2023-06-13 08:43:13.495241 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/generators_exceptions.py
--rw-r--r--   0        0        0      334 2023-06-13 11:23:34.985109 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_bool_generator.py
--rw-r--r--   0        0        0      892 2023-06-13 11:23:37.746882 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_complex_generator.py
--rw-r--r--   0        0        0     3080 2023-06-13 11:23:39.750171 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_data_class_generator.py
--rw-r--r--   0        0        0      812 2023-06-13 11:23:52.467563 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_decimal_generator.py
--rw-r--r--   0        0        0     1820 2023-06-13 11:23:54.182632 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_dict_generator.py
--rw-r--r--   0        0        0      724 2023-06-13 11:23:57.623576 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_float_generator.py
--rw-r--r--   0        0        0      178 2023-06-13 08:43:13.499432 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_generator.py
--rw-r--r--   0        0        0      587 2023-06-13 11:24:01.861372 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_int_generator.py
--rw-r--r--   0        0        0     1219 2023-06-13 11:24:04.043714 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_list_generator.py
--rw-r--r--   0        0        0      562 2023-06-13 11:24:06.361799 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_option_generator.py
--rw-r--r--   0        0        0      636 2023-06-13 11:24:08.697490 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_path_generator.py
--rw-r--r--   0        0        0      697 2023-06-13 11:24:10.611366 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_range_generator.py
--rw-r--r--   0        0        0      826 2023-06-13 11:24:12.802182 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_set_generator.py
--rw-r--r--   0        0        0      619 2023-06-13 11:24:35.759623 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_str_generator.py
--rw-r--r--   0        0        0     1234 2023-06-13 11:24:17.288064 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_tuple_generator.py
--rw-r--r--   0        0        0      285 2023-06-13 11:24:19.756139 dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_uuid_generator.py
--rw-r--r--   0        0        0    11558 2023-06-13 08:43:13.449996 dataclass_bakery_patched-0.5.0/LICENSE
--rw-r--r--   0        0        0      539 2023-06-13 11:26:58.234329 dataclass_bakery_patched-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1218 2023-06-13 08:43:13.451303 dataclass_bakery_patched-0.5.0/README.md
--rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 dataclass_bakery_patched-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/__init__.py
+-rw-r--r--   0        0        0      675 2023-06-13 11:26:46.274978 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/baker.py
+-rw-r--r--   0        0        0        0 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/__init__.py
+-rw-r--r--   0        0        0     3126 2023-06-14 07:19:46.953415 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/defaults.py
+-rw-r--r--   0        0        0      145 2023-06-13 08:43:13.495241 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/generators_exceptions.py
+-rw-r--r--   0        0        0      334 2023-06-13 11:23:34.985109 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_bool_generator.py
+-rw-r--r--   0        0        0      892 2023-06-13 11:23:37.746882 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_complex_generator.py
+-rw-r--r--   0        0        0     3080 2023-06-13 11:23:39.750171 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_data_class_generator.py
+-rw-r--r--   0        0        0      812 2023-06-13 11:23:52.467563 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_decimal_generator.py
+-rw-r--r--   0        0        0     1820 2023-06-13 11:23:54.182632 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_dict_generator.py
+-rw-r--r--   0        0        0      296 2023-06-14 07:18:13.147811 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_enum_generator.py
+-rw-r--r--   0        0        0      724 2023-06-13 11:23:57.623576 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_float_generator.py
+-rw-r--r--   0        0        0      178 2023-06-13 08:43:13.499432 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_generator.py
+-rw-r--r--   0        0        0      587 2023-06-13 11:24:01.861372 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_int_generator.py
+-rw-r--r--   0        0        0     1219 2023-06-13 11:24:04.043714 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_list_generator.py
+-rw-r--r--   0        0        0      562 2023-06-13 11:24:06.361799 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_option_generator.py
+-rw-r--r--   0        0        0      636 2023-06-13 11:24:08.697490 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_path_generator.py
+-rw-r--r--   0        0        0      697 2023-06-13 11:24:10.611366 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_range_generator.py
+-rw-r--r--   0        0        0      826 2023-06-13 11:24:12.802182 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_set_generator.py
+-rw-r--r--   0        0        0      619 2023-06-13 11:24:35.759623 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_str_generator.py
+-rw-r--r--   0        0        0     1234 2023-06-13 11:24:17.288064 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_tuple_generator.py
+-rw-r--r--   0        0        0      285 2023-06-13 11:24:19.756139 dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_uuid_generator.py
+-rw-r--r--   0        0        0    11558 2023-06-13 08:43:13.449996 dataclass_bakery_patched-0.6.0/LICENSE
+-rw-r--r--   0        0        0      539 2023-06-14 14:39:32.657750 dataclass_bakery_patched-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1218 2023-06-13 08:43:13.451303 dataclass_bakery_patched-0.6.0/README.md
+-rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 dataclass_bakery_patched-0.6.0/PKG-INFO
```

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/baker.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/baker.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/defaults.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from decimal import Decimal
 from pathlib import Path
 from typing import Literal
 from uuid import UUID
+from enum import Enum
 
 from dataclass_bakery_patched.generators.random_bool_generator import RandomBoolGenerator
 from dataclass_bakery_patched.generators.random_complex_generator import RandomComplexGenerator
 from dataclass_bakery_patched.generators.random_decimal_generator import RandomDecimalGenerator
 from dataclass_bakery_patched.generators.random_dict_generator import RandomDictGenerator
 from dataclass_bakery_patched.generators.random_float_generator import RandomFloatGenerator
 from dataclass_bakery_patched.generators.random_int_generator import RandomIntGenerator
@@ -13,14 +14,15 @@
 from dataclass_bakery_patched.generators.random_option_generator import RandomOptionGenerator
 from dataclass_bakery_patched.generators.random_path_generator import RandomPathGenerator
 from dataclass_bakery_patched.generators.random_range_generator import RandomRangeGenerator
 from dataclass_bakery_patched.generators.random_set_generator import RandomSetGenerator
 from dataclass_bakery_patched.generators.random_str_generator import RandomStrGenerator
 from dataclass_bakery_patched.generators.random_tuple_generator import RandomTupleGenerator
 from dataclass_bakery_patched.generators.random_uuid_generator import RandomUuidGenerator
+from dataclass_bakery_patched.generators.random_enum_generator import RandomEnumGenerator
 
 # Generators
 TYPING_GENERATORS = {
     str: RandomStrGenerator,
     int: RandomIntGenerator,
     float: RandomFloatGenerator,
     complex: RandomComplexGenerator,
@@ -30,14 +32,15 @@
     tuple: RandomTupleGenerator,
     set: RandomSetGenerator,
     range: RandomRangeGenerator,
     Decimal: RandomDecimalGenerator,
     Path: RandomPathGenerator,
     UUID: RandomUuidGenerator,
     Literal: RandomOptionGenerator,
+    Enum: RandomEnumGenerator,
 }
 
 # Generator Default Values
 NUMBER_MIN_LIMIT = 0
 NUMBER_MAX_LIMIT = 100
 
 DECIMALS = 2
```

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_complex_generator.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_complex_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_data_class_generator.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_data_class_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_decimal_generator.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_decimal_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_dict_generator.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_dict_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_float_generator.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_float_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_int_generator.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_int_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_list_generator.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_list_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_option_generator.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_option_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_path_generator.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_path_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_range_generator.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_range_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_set_generator.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_set_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_str_generator.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_str_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/dataclass_bakery_patched/generators/random_tuple_generator.py` & `dataclass_bakery_patched-0.6.0/dataclass_bakery_patched/generators/random_tuple_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/LICENSE` & `dataclass_bakery_patched-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/pyproject.toml` & `dataclass_bakery_patched-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-bakery-patched"
-version = "0.5.0"
+version = "0.6.0"
 description = "A fork from dataclass-bakery, with a tweak to consider inherited attributes when creating dataclasses."
 authors = ["Adam Ruman <469068@muni.cz>"]
 readme = "README.md"
 packages = [{include = "dataclass_bakery_patched"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dataclass_bakery_patched-0.5.0/README.md` & `dataclass_bakery_patched-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.5.0/PKG-INFO` & `dataclass_bakery_patched-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-bakery-patched
-Version: 0.5.0
+Version: 0.6.0
 Summary: A fork from dataclass-bakery, with a tweak to consider inherited attributes when creating dataclasses.
 Author: Adam Ruman
 Author-email: 469068@muni.cz
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

