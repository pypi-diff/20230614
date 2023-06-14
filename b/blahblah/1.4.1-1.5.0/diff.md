# Comparing `tmp/blahblah-1.4.1.tar.gz` & `tmp/blahblah-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blahblah-1.4.1.tar", last modified: Mon Jan 24 17:15:35 2022, max compression
+gzip compressed data, was "blahblah-1.5.0.tar", last modified: Tue Feb  1 15:14:55 2022, max compression
```

## Comparing `blahblah-1.4.1.tar` & `blahblah-1.5.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.544527 blahblah-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-01-24 17:15:25.000000 blahblah-1.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8533 2022-01-24 17:15:35.544527 blahblah-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7804 2022-01-24 17:15:25.000000 blahblah-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.540527 blahblah-1.4.1/blahblah/
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-01-24 17:15:25.000000 blahblah-1.4.1/blahblah/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-01-24 17:15:25.000000 blahblah-1.4.1/blahblah/_consts.py
--rw-r--r--   0 runner    (1001) docker     (121)     5564 2022-01-24 17:15:25.000000 blahblah-1.4.1/blahblah/_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-01-24 17:15:25.000000 blahblah-1.4.1/blahblah/_random.py
--rw-r--r--   0 runner    (1001) docker     (121)     4861 2022-01-24 17:15:25.000000 blahblah-1.4.1/blahblah/_regex_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-24 17:15:25.000000 blahblah-1.4.1/blahblah/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:25.000000 blahblah-1.4.1/blahblah/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.540527 blahblah-1.4.1/blahblah.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8533 2022-01-24 17:15:35.000000 blahblah-1.4.1/blahblah.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-01-24 17:15:35.000000 blahblah-1.4.1/blahblah.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-24 17:15:35.000000 blahblah-1.4.1/blahblah.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-01-24 17:15:35.000000 blahblah-1.4.1/blahblah.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-24 17:15:35.000000 blahblah-1.4.1/blahblah.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-01-24 17:15:35.548528 blahblah-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-01-24 17:15:25.000000 blahblah-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.536527 blahblah-1.4.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.540527 blahblah-1.4.1/tests/any/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/any/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/any/test_any_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.544527 blahblah-1.4.1/tests/bool/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/bool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/bool/test_bool_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.544527 blahblah-1.4.1/tests/bytes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/bytes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/bytes/test_bytes_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.544527 blahblah-1.4.1/tests/const/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/const/test_const_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.544527 blahblah-1.4.1/tests/dict/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2510 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/dict/test_dict_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.544527 blahblah-1.4.1/tests/float/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/float/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/float/test_float_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.544527 blahblah-1.4.1/tests/int/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/int/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/int/test_int_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.544527 blahblah-1.4.1/tests/list/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6283 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/list/test_list_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.544527 blahblah-1.4.1/tests/none/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/none/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/none/test_none_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:35.544527 blahblah-1.4.1/tests/str/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/str/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7130 2022-01-24 17:15:25.000000 blahblah-1.4.1/tests/str/test_str_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-02-01 15:14:44.000000 blahblah-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8403 2022-02-01 15:14:55.490021 blahblah-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7804 2022-02-01 15:14:44.000000 blahblah-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/blahblah/
+-rw-r--r--   0 runner    (1001) docker     (121)      597 2022-02-01 15:14:44.000000 blahblah-1.5.0/blahblah/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-02-01 15:14:44.000000 blahblah-1.5.0/blahblah/_consts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5808 2022-02-01 15:14:44.000000 blahblah-1.5.0/blahblah/_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-02-01 15:14:44.000000 blahblah-1.5.0/blahblah/_random.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4861 2022-02-01 15:14:44.000000 blahblah-1.5.0/blahblah/_regex_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-01 15:14:44.000000 blahblah-1.5.0/blahblah/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:44.000000 blahblah-1.5.0/blahblah/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/blahblah.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8403 2022-02-01 15:14:55.000000 blahblah-1.5.0/blahblah.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2022-02-01 15:14:55.000000 blahblah-1.5.0/blahblah.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-01 15:14:55.000000 blahblah-1.5.0/blahblah.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-02-01 15:14:55.000000 blahblah-1.5.0/blahblah.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-02-01 15:14:55.000000 blahblah-1.5.0/blahblah.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      758 2022-02-01 15:14:55.494021 blahblah-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-02-01 15:14:44.000000 blahblah-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.486021 blahblah-1.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/tests/alias/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/alias/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/alias/test_alias_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/tests/any/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/any/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/any/test_any_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/tests/bool/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/bool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      665 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/bool/test_bool_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/tests/bytes/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/bytes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      956 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/bytes/test_bytes_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/tests/const/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/const/test_const_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/tests/dict/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2510 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/dict/test_dict_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/tests/float/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/float/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/float/test_float_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/tests/int/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/int/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/int/test_int_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/tests/list/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6283 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/list/test_list_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/tests/none/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/none/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/none/test_none_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:55.490021 blahblah-1.5.0/tests/str/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/str/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7130 2022-02-01 15:14:44.000000 blahblah-1.5.0/tests/str/test_str_generation.py
```

### Comparing `blahblah-1.4.1/LICENSE.txt` & `blahblah-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blahblah-1.4.1/PKG-INFO` & `blahblah-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: blahblah
-Version: 1.4.1
+Version: 1.5.0
 Summary: Fake data generator for district42 schema
 Home-page: https://github.com/nikitanovosibirsk/blahblah
 Author: Nikita Tsvetkov
 Author-email: nikitanovosibirsk@yandex.com
 License: Apache-2.0
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # blahblah
```

### Comparing `blahblah-1.4.1/README.md` & `blahblah-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `blahblah-1.4.1/blahblah/__init__.py` & `blahblah-1.5.0/blahblah/__init__.py`

 * *Files identical despite different names*

### Comparing `blahblah-1.4.1/blahblah/_generator.py` & `blahblah-1.5.0/blahblah/_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from district42.types import (
     AnySchema,
     BoolSchema,
     BytesSchema,
     ConstSchema,
     DictSchema,
     FloatSchema,
+    GenericTypeAliasSchema,
     IntSchema,
     ListSchema,
     NoneSchema,
     StrSchema,
+    TypeAliasPropsType,
 )
 from district42.utils import is_ellipsis
 from niltype import Nil
 
 from ._consts import (
     BYTES_LEN_MAX,
     BYTES_LEN_MIN,
@@ -152,7 +154,11 @@
 
     def visit_bytes(self, schema: BytesSchema, **kwargs: Any) -> bytes:
         if schema.props.value is not Nil:
             return schema.props.value
         length = self._random.random_int(BYTES_LEN_MIN, BYTES_LEN_MAX)
         alphabet = STR_ALPHABET
         return self._random.random_str(length, alphabet).encode()
+
+    def visit_type_alias(self, schema: GenericTypeAliasSchema[TypeAliasPropsType],
+                         **kwargs: Any) -> Any:
+        return schema.props.type.__accept__(self, **kwargs)
```

### Comparing `blahblah-1.4.1/blahblah/_random.py` & `blahblah-1.5.0/blahblah/_random.py`

 * *Files identical despite different names*

### Comparing `blahblah-1.4.1/blahblah/_regex_generator.py` & `blahblah-1.5.0/blahblah/_regex_generator.py`

 * *Files identical despite different names*

### Comparing `blahblah-1.4.1/blahblah.egg-info/PKG-INFO` & `blahblah-1.5.0/blahblah.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: blahblah
-Version: 1.4.1
+Version: 1.5.0
 Summary: Fake data generator for district42 schema
 Home-page: https://github.com/nikitanovosibirsk/blahblah
 Author: Nikita Tsvetkov
 Author-email: nikitanovosibirsk@yandex.com
 License: Apache-2.0
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # blahblah
```

### Comparing `blahblah-1.4.1/blahblah.egg-info/SOURCES.txt` & `blahblah-1.5.0/blahblah.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 blahblah/_version.py
 blahblah/py.typed
 blahblah.egg-info/PKG-INFO
 blahblah.egg-info/SOURCES.txt
 blahblah.egg-info/dependency_links.txt
 blahblah.egg-info/requires.txt
 blahblah.egg-info/top_level.txt
+tests/alias/__init__.py
+tests/alias/test_alias_generation.py
 tests/any/__init__.py
 tests/any/test_any_generation.py
 tests/bool/__init__.py
 tests/bool/test_bool_generation.py
 tests/bytes/__init__.py
 tests/bytes/test_bytes_generation.py
 tests/const/__init__.py
```

### Comparing `blahblah-1.4.1/setup.cfg` & `blahblah-1.5.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.4.1
+current_version = 1.5.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
 
@@ -37,12 +37,14 @@
 
 [tool:pytest]
 testpaths = tests/
 python_files = test_*.py
 python_classes = 
 python_functions = test_*
 markers = only
+filterwarnings = 
+	ignore:.*schema.const.*:FutureWarning
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `blahblah-1.4.1/setup.py` & `blahblah-1.5.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,31 +9,28 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="blahblah",
-    version="1.4.1",
+    version="1.5.0",
     description="Fake data generator for district42 schema",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="nikitanovosibirsk@yandex.com",
     python_requires=">=3.8",
     url="https://github.com/nikitanovosibirsk/blahblah",
     license="Apache-2.0",
     packages=find_packages(exclude=("tests",)),
     package_data={"blahblah": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Topic :: Software Development",
         "Typing :: Typed",
     ],
 )
```

### Comparing `blahblah-1.4.1/tests/any/test_any_generation.py` & `blahblah-1.5.0/tests/any/test_any_generation.py`

 * *Files identical despite different names*

### Comparing `blahblah-1.4.1/tests/bool/test_bool_generation.py` & `blahblah-1.5.0/tests/bool/test_bool_generation.py`

 * *Files identical despite different names*

### Comparing `blahblah-1.4.1/tests/bytes/test_bytes_generation.py` & `blahblah-1.5.0/tests/bytes/test_bytes_generation.py`

 * *Files identical despite different names*

### Comparing `blahblah-1.4.1/tests/const/test_const_generation.py` & `blahblah-1.5.0/tests/const/test_const_generation.py`

 * *Files identical despite different names*

### Comparing `blahblah-1.4.1/tests/dict/test_dict_generation.py` & `blahblah-1.5.0/tests/dict/test_dict_generation.py`

 * *Files identical despite different names*

### Comparing `blahblah-1.4.1/tests/float/test_float_generation.py` & `blahblah-1.5.0/tests/float/test_float_generation.py`

 * *Files identical despite different names*

### Comparing `blahblah-1.4.1/tests/int/test_int_generation.py` & `blahblah-1.5.0/tests/int/test_int_generation.py`

 * *Files identical despite different names*

### Comparing `blahblah-1.4.1/tests/list/test_list_generation.py` & `blahblah-1.5.0/tests/list/test_list_generation.py`

 * *Files identical despite different names*

### Comparing `blahblah-1.4.1/tests/str/test_str_generation.py` & `blahblah-1.5.0/tests/str/test_str_generation.py`

 * *Files identical despite different names*

