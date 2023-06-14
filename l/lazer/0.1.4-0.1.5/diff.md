# Comparing `tmp/lazer-0.1.4.tar.gz` & `tmp/lazer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazer-0.1.4.tar", max compression
+gzip compressed data, was "lazer-0.1.5.tar", max compression
```

## Comparing `lazer-0.1.4.tar` & `lazer-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      892 2023-06-14 04:56:06.903905 lazer-0.1.4/README.md
--rw-r--r--   0        0        0     3715 2023-06-14 05:04:54.553905 lazer-0.1.4/lazer/__init__.py
--rw-r--r--   0        0        0      377 2023-06-14 05:05:47.433905 lazer-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1394 1970-01-01 00:00:00.000000 lazer-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-14 00:37:54.243905 lazer-0.1.5/LICENSE
+-rw-r--r--   0        0        0      914 2023-06-14 05:47:38.043905 lazer-0.1.5/README.md
+-rw-r--r--   0        0        0     3923 2023-06-14 05:32:15.583905 lazer-0.1.5/lazer/__init__.py
+-rw-r--r--   0        0        0      377 2023-06-14 05:43:59.253905 lazer-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 lazer-0.1.5/PKG-INFO
```

### Comparing `lazer-0.1.4/README.md` & `lazer-0.1.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Lazer
 
 Lazer is a Python library that provides a convenient way to expose Python functions as schemas for OpenAI chat models.
 
 ### What it Does
 
-Allows you to more easily inform GPT about your
+Allows you to more easily inform GPT about functions in your code 😊
+
+> **Warning** don't RCE yourself lol
 
 ## Installation
 
 To install Lazer, simply run:
 
 ```bash
 pip install lazer
@@ -33,16 +35,13 @@
 response = await conversation.talk("What is the qux of 3 and steven")
 print(response)
 # ... 117 ...
 ```
 
 ### Demo
 
-Go check `lazer/demo/app.py` for a dummy app
-
-To run this `python -m demo.app`
-
+Go to [demo/](demo/) for some demo code.
 
 #### Authors:
 
 * @JustinStitt
 * @diamondburned
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lazer-0.1.4/lazer/__init__.py` & `lazer-0.1.5/lazer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import ast
 import json
 import inspect
 import openai
+import sys
 from icecream import ic
 from typing import Callable, Any
 from dotenv import load_dotenv
 
 from pytojsonschema.functions import process_function_def
 from pytojsonschema.common import init_schema_map, init_typing_namespace
 
@@ -80,27 +81,32 @@
         assert "messages" not in self.args
         assert "functions" not in self.args
         assert "function_call" not in self.args
 
         self.args["messages"] = self.messages
         self.args["function_call"] = "auto"
 
-    async def talk(self, content: str) -> str:
+    def talk(self, content: str, debug=False) -> str:
         self.args["functions"] = self.lazer.get_functions()
         self.messages.append({"role": "user", "content": content})
 
         while True:
             response = openai.ChatCompletion.create(**self.args)
 
             message = response["choices"][0]["message"]  # type: ignore
             if not message.get("function_call"):
                 return message["content"]
 
             function_name = message["function_call"]["name"]
             function_args = json.loads(message["function_call"]["arguments"])
+            if debug:
+                print(
+                    f"🔧 Running Function : {function_name} with args {function_args}",
+                    file=sys.stderr,
+                )
             function_response = self.lazer.dispatch(function_name, function_args)
 
             self.messages.append(
                 {
                     "role": "function",
                     "name": function_name,
                     "content": function_response,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lazer-0.1.4/PKG-INFO` & `lazer-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazer
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: icecream (>=2.1.3,<3.0.0)
@@ -16,15 +16,17 @@
 
 # Lazer
 
 Lazer is a Python library that provides a convenient way to expose Python functions as schemas for OpenAI chat models.
 
 ### What it Does
 
-Allows you to more easily inform GPT about your
+Allows you to more easily inform GPT about functions in your code 😊
+
+> **Warning** don't RCE yourself lol
 
 ## Installation
 
 To install Lazer, simply run:
 
 ```bash
 pip install lazer
@@ -49,17 +51,14 @@
 response = await conversation.talk("What is the qux of 3 and steven")
 print(response)
 # ... 117 ...
 ```
 
 ### Demo
 
-Go check `lazer/demo/app.py` for a dummy app
-
-To run this `python -m demo.app`
-
+Go to [demo/](demo/) for some demo code.
 
 #### Authors:
 
 * @JustinStitt
 * @diamondburned
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

