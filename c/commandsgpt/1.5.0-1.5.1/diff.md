# Comparing `tmp/commandsgpt-1.5.0.tar.gz` & `tmp/commandsgpt-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandsgpt-1.5.0.tar", last modified: Mon Jun  5 07:15:52 2023, max compression
+gzip compressed data, was "commandsgpt-1.5.1.tar", last modified: Wed Jun 14 02:10:30 2023, max compression
```

## Comparing `commandsgpt-1.5.0.tar` & `commandsgpt-1.5.1.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:52.916031 commandsgpt-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-05 07:15:41.000000 commandsgpt-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-05 07:15:52.916031 commandsgpt-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-05 07:15:41.000000 commandsgpt-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:52.912031 commandsgpt-1.5.0/commands_gpt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:52.912031 commandsgpt-1.5.0/commands_gpt/commands_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:41.000000 commandsgpt-1.5.0/commands_gpt/commands_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-05 07:15:41.000000 commandsgpt-1.5.0/commands_gpt/commands_gpt/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:52.916031 commandsgpt-1.5.0/commands_gpt/commands_gpt/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:41.000000 commandsgpt-1.5.0/commands_gpt/commands_gpt/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-05 07:15:41.000000 commandsgpt-1.5.0/commands_gpt/commands_gpt/commands/commands_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-06-05 07:15:41.000000 commandsgpt-1.5.0/commands_gpt/commands_gpt/commands/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-05 07:15:41.000000 commandsgpt-1.5.0/commands_gpt/commands_gpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-05 07:15:41.000000 commandsgpt-1.5.0/commands_gpt/commands_gpt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    25514 2023-06-05 07:15:41.000000 commandsgpt-1.5.0/commands_gpt/commands_gpt/recognizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-05 07:15:41.000000 commandsgpt-1.5.0/commands_gpt/commands_gpt/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:52.916031 commandsgpt-1.5.0/commands_gpt/commandsgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-05 07:15:52.000000 commandsgpt-1.5.0/commands_gpt/commandsgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-05 07:15:52.000000 commandsgpt-1.5.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:15:52.000000 commandsgpt-1.5.0/commands_gpt/commandsgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 07:15:52.000000 commandsgpt-1.5.0/commands_gpt/commandsgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-05 07:15:41.000000 commandsgpt-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-05 07:15:52.916031 commandsgpt-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:30.313845 commandsgpt-1.5.1/commands_gpt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/commands_gpt/commands_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/commands_gpt/commands_gpt/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/commands/commands_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/commands/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25599 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/recognizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/commands_gpt/commands_gpt/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/commands_gpt/commands_gpt/util/math_expr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-14 02:10:30.000000 commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-14 02:10:30.000000 commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:10:30.000000 commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 02:10:30.000000 commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 02:10:18.000000 commandsgpt-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-14 02:10:30.317845 commandsgpt-1.5.1/setup.cfg
```

### Comparing `commandsgpt-1.5.0/LICENSE` & `commandsgpt-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.0/PKG-INFO` & `commandsgpt-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.5.0
+Version: 1.5.1
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `commandsgpt-1.5.0/README.md` & `commandsgpt-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.0/commands_gpt/commands_gpt/chat.py` & `commandsgpt-1.5.1/commands_gpt/commands_gpt/chat.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.0/commands_gpt/commands_gpt/commands/commands_funcs.py` & `commandsgpt-1.5.1/commands_gpt/commands_gpt/commands/commands_funcs.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.0/commands_gpt/commands_gpt/commands/graphs.py` & `commandsgpt-1.5.1/commands_gpt/commands_gpt/commands/graphs.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.0/commands_gpt/commands_gpt/config.py` & `commandsgpt-1.5.1/commands_gpt/commands_gpt/config.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.0/commands_gpt/commands_gpt/recognizers.py` & `commandsgpt-1.5.1/commands_gpt/commands_gpt/recognizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,19 +89,21 @@
                 """\nTo reference data generated by a command, use __&i.data__. 'i' is the ID of the command; 'data' is the name of the generated data."""
                 """\nAlways consider the DATA TYPE of the data you are referencing (e.g. string-types can not have indices like '__&i.thought[j]__'; data does not have attributes unless specified)."""
                 """\nYou can ONLY reference data in the arguments of the nodes."""
                 """\nThe structure will ultimately be like a graph. The next_command_id defines which command will be executed next; dependent_on_data is the name of the data generated by the current command which will be used as a condition (*null if the next command will be executed no matter what the results of the current command where*), and required_value is what value the dependent_on_data must have to execute the next command (null if dependent_on_data was also null)."""
                 """\nNote that dependent_on_data is NOT a data reference for the next command; it's just what will be used as a CONDITION to determine if the next command will be executed."""
                 """\ndependent_on_data field CAN NOT be 'dependent_on_data'. It must be null if it doesn't matter."""
                 """\nA command can execute multiple next commands."""
+                # TODO: Improve context passing to commands
+
                 # """\nBe concise but *solid* with the structure."""
-                """\n*Consider that the user might write incorrectly and their inputs might be ambiguous*."""
+                """\n*IMPORTANT*: Consider that the user might write incorrectly and their inputs might be ambiguous."""
                 """\nThe only way to reference the data of other commands is by using the __&i.data__ referencing. Commands DO NOT KNOW each other's data."""
                 """\nProvide all the relevant context in the arguments of the commands, so that you're not ambiguous."""
-                """\nNote that each command DOES NOT know about the other commands. You have to use DATA REFERENCES as ARGUMENTS to pass context."""
+                """\n*IMPORTANT*: Note that each command DOES NOT know about the other commands. You have to use DATA REFERENCES as ARGUMENTS to pass context."""
                 """\nBe creative and logic when using the commands' arguments and data references."""
 
                 """\n\nFor example:"""
 
                 """\n\nExample 1:"""
                 """\nUser prompt: 'Write an article about Lenz's Law, copy it to my clipboard and save it as a file.'"""
                 """\nYour response might be: '[1, "THINK", {"about": "Article about Lenz's Law"}, [[2, null, null]]]\n[2, "WRITE_CLIPBOARD", {"content": "__&1.thought__"}, [[3, null, null]]]\n[3, "WRITE_FILE", {"content": "__&1.thought__", "file_name": "Article about Lenz's Law"}, []]'"""
```

### Comparing `commandsgpt-1.5.0/commands_gpt/commands_gpt/regex.py` & `commandsgpt-1.5.1/commands_gpt/commands_gpt/regex.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.5.0/commands_gpt/commandsgpt.egg-info/PKG-INFO` & `commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.5.0
+Version: 1.5.1
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `commandsgpt-1.5.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt` & `commandsgpt-1.5.1/commands_gpt/commandsgpt.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,11 +7,13 @@
 commands_gpt/commands_gpt/config.py
 commands_gpt/commands_gpt/models.py
 commands_gpt/commands_gpt/recognizers.py
 commands_gpt/commands_gpt/regex.py
 commands_gpt/commands_gpt/commands/__init__.py
 commands_gpt/commands_gpt/commands/commands_funcs.py
 commands_gpt/commands_gpt/commands/graphs.py
+commands_gpt/commands_gpt/util/__init__.py
+commands_gpt/commands_gpt/util/math_expr.py
 commands_gpt/commandsgpt.egg-info/PKG-INFO
 commands_gpt/commandsgpt.egg-info/SOURCES.txt
 commands_gpt/commandsgpt.egg-info/dependency_links.txt
 commands_gpt/commandsgpt.egg-info/top_level.txt
```

### Comparing `commandsgpt-1.5.0/setup.cfg` & `commandsgpt-1.5.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = commandsgpt
-version = 1.5.0
+version = 1.5.1
 author = Martín Alexis Martínez Andrade
 author_email = alexis.martinez.contacto@gmail.com
 description = An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/AlexisAndradeDev/CommandsGPT
 project_urls =
```

