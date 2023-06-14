# Comparing `tmp/lazer-0.1.1.tar.gz` & `tmp/lazer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazer-0.1.1.tar", max compression
+gzip compressed data, was "lazer-0.1.2.tar", max compression
```

## Comparing `lazer-0.1.1.tar` & `lazer-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-14 00:44:57.233905 lazer-0.1.1/README.md
--rw-r--r--   0        0        0     1865 2023-06-14 03:04:35.823905 lazer-0.1.1/lazer/__init__.py
--rw-r--r--   0        0        0      377 2023-06-14 03:05:38.583905 lazer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 lazer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      208 2023-06-14 03:12:43.853905 lazer-0.1.2/README.md
+-rw-r--r--   0        0        0     2352 2023-06-14 04:10:34.493905 lazer-0.1.2/lazer/__init__.py
+-rw-r--r--   0        0        0      377 2023-06-14 04:11:55.413905 lazer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 lazer-0.1.2/PKG-INFO
```

### Comparing `lazer-0.1.1/lazer/__init__.py` & `lazer-0.1.2/lazer/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,63 +3,64 @@
 from icecream import ic
 from typing import Callable
 
 from pytojsonschema.functions import process_function_def
 from pytojsonschema.common import init_schema_map, init_typing_namespace
 
 
-_schema_map = init_schema_map()
-_type_namespace = init_typing_namespace()
+class Lazer:
+    def __init__(self):
+        self._schema_map = init_schema_map()
+        self._type_namespace = init_typing_namespace()
+        self._functions = []
+        self._name_to_func = {}
+        self._previous_get_functions_result = None
+
+    def dispatch(self, function_name: str, function_args: dict):
+        f = self._name_to_func.get(function_name, lambda: "Couldn't find that function")
+        return f(**function_args)
+
+    def get_functions(self) -> list[dict]:
+        if self._previous_get_functions_result:
+            return self._previous_get_functions_result
+        result = self._functions_to_schemas(self._functions)
+        self._previous_get_functions_result = result
+        return result
+
+    def use(self, func):
+        self._functions.append(func)
+        self._name_to_func[func.__name__] = func
+
+        def wrapper(*args, **kwargs):
+            return func(*args, **kwargs)
+
+        return wrapper
+
+    def _fill_in_schema(self, name: str, doc: str, base_schema: dict) -> dict:
+        """Take the schema generated from pytojsonschema and fill it out to fit OpenAI's format"""
+        final_schema = {}
+        final_schema["name"] = name
+        final_schema["description"] = doc
+        final_schema["parameters"] = base_schema
+        # TODO: add in per-variable descriptions
+        return final_schema
+
+    def _functions_to_schemas(self, functions: list[Callable]) -> list[dict]:
+        schemas: list[dict] = []
+
+        for function in functions:
+            name = function.__name__
+            doc = function.__doc__ or "No Description"
+            src = ast.parse(inspect.getsource(function)).body
+            node = src[0]
+
+            base_schema = process_function_def(node, self._type_namespace, self._schema_map)  # type: ignore
+            del base_schema[
+                "$schema"
+            ]  # unsued for OpenAI's purposes, probably doesn't hurt to leave it though
 
+            del base_schema["additionalProperties"]
 
-_functions = []
-_previous_get_functions_result = None
+            openai_compliant_schema = self._fill_in_schema(name, doc, base_schema)
+            schemas.append(openai_compliant_schema)
 
-
-def get_functions() -> list[dict]:
-    global _functions, _previous_get_functions_result
-    if _previous_get_functions_result:
-        return _previous_get_functions_result
-    result = _functions_to_schemas(_functions)
-    _previous_get_functions_result = result
-    return result
-
-
-def lazer(func):
-    global _functions
-    _functions.append(func)
-
-    def wrapper(*args, **kwargs):
-        return func(*args, **kwargs)
-
-    return wrapper
-
-
-def _fill_in_schema(name: str, doc: str, base_schema: dict) -> dict:
-    """Take the schema generated from pytojsonschema and fill it out to fit OpenAI's format"""
-    final_schema = {}
-    final_schema["name"] = name
-    final_schema["description"] = doc
-    final_schema["parameters"] = base_schema
-    # TODO: add in per-variable descriptions
-    return final_schema
-
-
-def _functions_to_schemas(functions: list[Callable]) -> list[dict]:
-    global _schema_map, _type_namespace
-    schemas: list[dict] = []
-
-    for function in functions:
-        name = function.__name__
-        doc = function.__doc__ or "No Description"
-        src = ast.parse(inspect.getsource(function)).body
-        node = src[0]
-
-        base_schema = process_function_def(node, _type_namespace, _schema_map)  # type: ignore
-        del base_schema[
-            "$schema"
-        ]  # unsued for OpenAI's purposes, probably doesn't hurt to leave it though
-
-        openai_compliant_schema = _fill_in_schema(name, doc, base_schema)
-        schemas.append(openai_compliant_schema)
-
-    return schemas
+        return schemas
```

