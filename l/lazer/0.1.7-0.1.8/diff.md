# Comparing `tmp/lazer-0.1.7.tar.gz` & `tmp/lazer-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazer-0.1.7.tar", max compression
+gzip compressed data, was "lazer-0.1.8.tar", max compression
```

## Comparing `lazer-0.1.7.tar` & `lazer-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-06-14 00:37:54.243905 lazer-0.1.7/LICENSE
--rw-r--r--   0        0        0     1391 2023-06-14 06:13:54.883905 lazer-0.1.7/README.md
--rw-r--r--   0        0        0     3923 2023-06-14 05:32:15.583905 lazer-0.1.7/lazer/__init__.py
--rw-r--r--   0        0        0      377 2023-06-14 06:15:31.853905 lazer-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1893 1970-01-01 00:00:00.000000 lazer-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-14 00:37:54.243905 lazer-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1427 2023-06-14 07:59:02.843905 lazer-0.1.8/README.md
+-rw-r--r--   0        0        0     3979 2023-06-14 08:03:18.993905 lazer-0.1.8/lazer/__init__.py
+-rw-r--r--   0        0        0      377 2023-06-14 08:03:26.433905 lazer-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 lazer-0.1.8/PKG-INFO
```

### Comparing `lazer-0.1.7/LICENSE` & `lazer-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lazer-0.1.7/README.md` & `lazer-0.1.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 # GPT is now made aware of your function `qux`
 @lazer.use
 def qux(num: int, name: str) -> str:
     """Retrieve a number and a name from the user and compute the qux of it"""
     return str(num + len(name) * 13)
 
-conversation = LazerConversation(lazer)
+conversation = LazerConversation(backdoor, {"model": "gpt-3.5-turbo-0613"})
 response = conversation.talk("What is the qux of 3 and steven")
 print(response)
 # ... 117 ...
 ```
 
 > **Note** You do not have to use the LazerConversation GPT frontend, you can simply use
 the Lazer functions `.use` (decorator) and `.get_functions()` as well as
```

### Comparing `lazer-0.1.7/lazer/__init__.py` & `lazer-0.1.8/lazer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import ast
-import json
 import inspect
-import openai
+import json
+import os
 import sys
-from icecream import ic
-from typing import Callable, Any
-from dotenv import load_dotenv
+from typing import Any, Callable
 
-from pytojsonschema.functions import process_function_def
+from dotenv import load_dotenv
+from icecream import ic
+import openai
 from pytojsonschema.common import init_schema_map, init_typing_namespace
+from pytojsonschema.functions import process_function_def
 
 load_dotenv()
 
+openai.api_key = os.getenv("OPENAI_API_KEY")
+
 
 class Lazer:
     def __init__(self):
         self._schema_map = init_schema_map()
         self._type_namespace = init_typing_namespace()
         self._functions = []
         self._name_to_func = {}
```

### Comparing `lazer-0.1.7/PKG-INFO` & `lazer-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazer
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: icecream (>=2.1.3,<3.0.0)
@@ -45,15 +45,15 @@
 
 # GPT is now made aware of your function `qux`
 @lazer.use
 def qux(num: int, name: str) -> str:
     """Retrieve a number and a name from the user and compute the qux of it"""
     return str(num + len(name) * 13)
 
-conversation = LazerConversation(lazer)
+conversation = LazerConversation(backdoor, {"model": "gpt-3.5-turbo-0613"})
 response = conversation.talk("What is the qux of 3 and steven")
 print(response)
 # ... 117 ...
 ```
 
 > **Note** You do not have to use the LazerConversation GPT frontend, you can simply use
 the Lazer functions `.use` (decorator) and `.get_functions()` as well as
```

