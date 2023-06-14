# Comparing `tmp/lazer-0.1.2.tar.gz` & `tmp/lazer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazer-0.1.2.tar", max compression
+gzip compressed data, was "lazer-0.1.3.tar", max compression
```

## Comparing `lazer-0.1.2.tar` & `lazer-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      208 2023-06-14 03:12:43.853905 lazer-0.1.2/README.md
--rw-r--r--   0        0        0     2352 2023-06-14 04:10:34.493905 lazer-0.1.2/lazer/__init__.py
--rw-r--r--   0        0        0      377 2023-06-14 04:11:55.413905 lazer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 lazer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-06-14 04:20:08.313905 lazer-0.1.3/README.md
+-rw-r--r--   0        0        0     3710 2023-06-14 04:40:37.133905 lazer-0.1.3/lazer/__init__.py
+-rw-r--r--   0        0        0      377 2023-06-14 04:41:33.263905 lazer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 lazer-0.1.3/PKG-INFO
```

### Comparing `lazer-0.1.2/lazer/__init__.py` & `lazer-0.1.3/lazer/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import ast
+import json
 import inspect
+import openai
 from icecream import ic
-from typing import Callable
+from typing import Callable, Any
+from dotenv import load_dotenv
 
 from pytojsonschema.functions import process_function_def
 from pytojsonschema.common import init_schema_map, init_typing_namespace
 
+load_dotenv()
+
 
 class Lazer:
     def __init__(self):
         self._schema_map = init_schema_map()
         self._type_namespace = init_typing_namespace()
         self._functions = []
         self._name_to_func = {}
@@ -60,7 +65,44 @@
 
             del base_schema["additionalProperties"]
 
             openai_compliant_schema = self._fill_in_schema(name, doc, base_schema)
             schemas.append(openai_compliant_schema)
 
         return schemas
+
+
+class LazerConversation:
+    def __init__(self, lazer: Lazer, chatCompletionArgs: dict[str, Any]):
+        self.messages = []
+        self.lazer = lazer
+        self.args = chatCompletionArgs
+
+        assert "messages" not in self.args
+        assert "functions" not in self.args
+        assert "function_call" not in self.args
+
+        self.args["messages"] = self.messages
+        self.args["functions"] = lazer.get_functions()
+        self.args["function_call"] = "auto"
+
+    async def talk(self, content: str) -> str:
+        self.messages.append({"role": "user", "content": content})
+
+        while True:
+            response = openai.ChatCompletion.create(**self.args)
+
+            message = response["choices"][0]["message"]  # type: ignore
+            if not message.get("function_call"):
+                return message["content"]
+
+            function_name = message["function_call"]["name"]
+            function_args = json.loads(message["function_call"]["arguments"])
+            function_response = self.lazer.dispatch(function_name, function_args)
+
+            self.messages.append(
+                {
+                    "role": "function",
+                    "name": function_name,
+                    "content": function_response,
+                }
+            )
```

### Comparing `lazer-0.1.2/PKG-INFO` & `lazer-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazer
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: icecream (>=2.1.3,<3.0.0)
@@ -22,9 +22,11 @@
 ### Installation
 
 `$ pip install lazer`
 
 
 ### Usage
 
-Go check `lazer/user/app.py` for a dummy app
+Go check `lazer/demo/app.py` for a dummy app
+
+To run this `python -m demo.app`
```

