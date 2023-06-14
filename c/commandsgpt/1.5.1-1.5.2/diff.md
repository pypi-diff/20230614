# Comparing `tmp/commandsgpt-1.5.1.tar.gz` & `tmp/commandsgpt-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandsgpt-1.5.1.tar", last modified: Wed Jun 14 02:10:30 2023, max compression
+gzip compressed data, was "commandsgpt-1.5.2.tar", last modified: Wed Jun 14 21:50:39 2023, max compression
```

## Comparing `commandsgpt-1.5.1.tar` & `commandsgpt-1.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:30.313845 commandsgpt-1.5.1/commands_gpt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/commands_gpt/commands_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/commands_gpt/commands_gpt/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/commands/commands_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/commands/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    25599 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/recognizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/commands_gpt/commands_gpt/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/util/math_expr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-14 02:10:30.000000 commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-14 02:10:30.000000 commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:10:30.000000 commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 02:10:30.000000 commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:50:39.317790 commandsgpt-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-14 21:50:39.317790 commandsgpt-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:50:39.309790 commandsgpt-1.5.2/commands_gpt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:50:39.313790 commandsgpt-1.5.2/commands_gpt/commands_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/commands_gpt/commands_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/commands_gpt/commands_gpt/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:50:39.313790 commandsgpt-1.5.2/commands_gpt/commands_gpt/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/commands_gpt/commands_gpt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/commands_gpt/commands_gpt/commands/commands_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/commands_gpt/commands_gpt/commands/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/commands_gpt/commands_gpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/commands_gpt/commands_gpt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25599 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/commands_gpt/commands_gpt/recognizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/commands_gpt/commands_gpt/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:50:39.313790 commandsgpt-1.5.2/commands_gpt/commands_gpt/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/commands_gpt/commands_gpt/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/commands_gpt/commands_gpt/util/math_expr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:50:39.317790 commandsgpt-1.5.2/commands_gpt/commandsgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-14 21:50:39.000000 commandsgpt-1.5.2/commands_gpt/commandsgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-14 21:50:39.000000 commandsgpt-1.5.2/commands_gpt/commandsgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:50:39.000000 commandsgpt-1.5.2/commands_gpt/commandsgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 21:50:39.000000 commandsgpt-1.5.2/commands_gpt/commandsgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 21:50:27.000000 commandsgpt-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-14 21:50:39.317790 commandsgpt-1.5.2/setup.cfg
```

### Comparing `commandsgpt-1.5.1/LICENSE` & `commandsgpt-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.1/PKG-INFO` & `commandsgpt-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.5.1
+Version: 1.5.2
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `commandsgpt-1.5.1/README.md` & `commandsgpt-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.1/commands_gpt/commands_gpt/chat.py` & `commandsgpt-1.5.2/commands_gpt/commands_gpt/chat.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.1/commands_gpt/commands_gpt/commands/commands_funcs.py` & `commandsgpt-1.5.2/commands_gpt/commands_gpt/commands/commands_funcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             "about": {"description": "What to think about. Example: 'Three-paragraph article about Lenz's Law.'", "type": "string"},
         },
         "generates_data": {
             "thought": {"description": "Text generated by thinking.", "type": "string"},
         },
     },
     "IF": {
-        "description": "Returns the Boolean value of a condition.",
+        "description": "Returns the Boolean value of a condition. ALWAYS use this command to compare values, answers and expressions, even in natural language.",
         "arguments": {
             "condition": {"description": "Condition. Can be in natural language.", "type": "string"},
         },
         "generates_data": {
             "result": {"description": "Result of the condition: 0 or 1.", "type": "boolean"},
         },
     },
@@ -68,20 +68,21 @@
     }
     return results
 
 def if_command(config: Config, graph: Graph, condition: str) -> dict[str, Any]:
     messages = [
         {
             "role": "system", 
-            "content": f"You are a model that evaluates conditions, both in natural language and symbolic language. Given a condition, you respond with the number «1» (true) or «0» (false). DO NOT write ANYTHING ELSE EVER.",
+            "content": f"You are a model that evaluates conditions, both in natural language and symbolic language. Given a condition, you respond with the number «1» (true) or «0» (false). DO NOT write ANYTHING ELSE EVER. Ex.: \"'yes' == 'no'\" -> 0, \"'yea' == 'yes'\" -> 1.",
         },
     ]
     result = get_answer_from_model(condition, config.chat_model, messages)
+
     try:
-        result = bool(result)
+        result = bool(int(result))
     except Exception as e:
         print(f"Could not convert result from IF command '{result}' to boolean.")
         raise e
 
     results = {
         "result": result,
     }
```

### Comparing `commandsgpt-1.5.1/commands_gpt/commands_gpt/commands/graphs.py` & `commandsgpt-1.5.2/commands_gpt/commands_gpt/commands/graphs.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.1/commands_gpt/commands_gpt/config.py` & `commandsgpt-1.5.2/commands_gpt/commands_gpt/config.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.1/commands_gpt/commands_gpt/recognizers.py` & `commandsgpt-1.5.2/commands_gpt/commands_gpt/recognizers.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.1/commands_gpt/commands_gpt/regex.py` & `commandsgpt-1.5.2/commands_gpt/commands_gpt/regex.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.1/commands_gpt/commands_gpt/util/math_expr.py` & `commandsgpt-1.5.2/commands_gpt/commands_gpt/util/math_expr.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/PKG-INFO` & `commandsgpt-1.5.2/commands_gpt/commandsgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.5.1
+Version: 1.5.2
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/SOURCES.txt` & `commandsgpt-1.5.2/commands_gpt/commandsgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.1/setup.cfg` & `commandsgpt-1.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = commandsgpt
-version = 1.5.1
+version = 1.5.2
 author = Martín Alexis Martínez Andrade
 author_email = alexis.martinez.contacto@gmail.com
 description = An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/AlexisAndradeDev/CommandsGPT
 project_urls =
```

