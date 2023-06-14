# Comparing `tmp/robotcode_robot-0.41.0.tar.gz` & `tmp/robotcode_robot-0.43.0.tar.gz`

## Comparing `robotcode_robot-0.41.0.tar` & `robotcode_robot-0.43.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.41.0/src/robotcode/robot/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.41.0/src/robotcode/robot/__version__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.41.0/src/robotcode/robot/py.typed
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.41.0/src/robotcode/robot/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.41.0/src/robotcode/robot/config/__init__.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 robotcode_robot-0.41.0/src/robotcode/robot/config/loader.py
--rw-r--r--   0        0        0    78409 2020-02-02 00:00:00.000000 robotcode_robot-0.41.0/src/robotcode/robot/config/model.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 robotcode_robot-0.41.0/src/robotcode/robot/config/utils.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.41.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.41.0/LICENSE.txt
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.41.0/README.md
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 robotcode_robot-0.41.0/pyproject.toml
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 robotcode_robot-0.41.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.43.0/src/robotcode/robot/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.43.0/src/robotcode/robot/__version__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.43.0/src/robotcode/robot/py.typed
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.43.0/src/robotcode/robot/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.43.0/src/robotcode/robot/config/__init__.py
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 robotcode_robot-0.43.0/src/robotcode/robot/config/loader.py
+-rw-r--r--   0        0        0    79675 2020-02-02 00:00:00.000000 robotcode_robot-0.43.0/src/robotcode/robot/config/model.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 robotcode_robot-0.43.0/src/robotcode/robot/config/utils.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.43.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.43.0/LICENSE.txt
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.43.0/README.md
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 robotcode_robot-0.43.0/pyproject.toml
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 robotcode_robot-0.43.0/PKG-INFO
```

### Comparing `robotcode_robot-0.41.0/src/robotcode/robot/config/loader.py` & `robotcode_robot-0.43.0/src/robotcode/robot/config/loader.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.41.0/src/robotcode/robot/config/model.py` & `robotcode_robot-0.43.0/src/robotcode/robot/config/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -533,14 +533,29 @@
 
             corresponds to the `-d --outputdir dir` option of _robot_
             """,
         robot_name="outputdir",
         robot_priority=500,
         robot_short_name="d",
     )
+    parse_include: Optional[List[Union[str, StringExpression]]] = field(
+        description="""\
+            Parse only files matching `pattern`. It can be:
+            - a file name or pattern like `example.robot` or
+            `*.robot` to parse all files matching that name,
+            - a file path like `path/to/example.robot`, or
+            - a directory path like `path/to/example` to parse
+            all files in that directory, recursively.
+
+            corresponds to the `-I --parseinclude pattern *` option of _robot_
+            """,
+        robot_name="parseinclude",
+        robot_priority=500,
+        robot_short_name="I",
+    )
     pre_rebot_modifiers: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
             Class to programmatically modify the result
             model before creating reports and logs. Accepts
             arguments the same way as with --listener.
 
             corresponds to the `--prerebotmodifier modifier *` option of _robot_
@@ -937,14 +952,28 @@
             Set metadata of the top level suite. Value can
             contain formatting and be read from a file similarly
             as --doc. Example: --metadata Version:1.2
 
             corresponds to the `-M --metadata name:value *` option of _robot_
             """,
     )
+    extra_parse_include: Optional[List[Union[str, StringExpression]]] = field(
+        description="""\
+            Appends entries to the --parseinclude option.
+
+            Parse only files matching `pattern`. It can be:
+            - a file name or pattern like `example.robot` or
+            `*.robot` to parse all files matching that name,
+            - a file path like `path/to/example.robot`, or
+            - a directory path like `path/to/example` to parse
+            all files in that directory, recursively.
+
+            corresponds to the `-I --parseinclude pattern *` option of _robot_
+            """,
+    )
     extra_pre_rebot_modifiers: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
             Appends entries to the --prerebotmodifier option.
 
             Class to programmatically modify the result
             model before creating reports and logs. Accepts
             arguments the same way as with --listener.
@@ -1484,17 +1513,17 @@
             variables with string value are supported and name is
             given without `${}`. See --variablefile for a more
             powerful variable setting mechanism.
 
             Examples:
 
             ```
-            --variable str:Hello       =>  ${str} = `Hello`
-            -v hi:Hi_World -E space:_  =>  ${hi} = `Hi World`
-            -v x: -v y:42              =>  ${x} = ``, ${y} = `42`
+            --variable name:Robot  =>  ${name} = `Robot`
+            -v "hello:Hello world" =>  ${hello} = `Hello world`
+            -v x: -v y:42          =>  ${x} = ``, ${y} = `42`
             ```
 
             corresponds to the `-v --variable name:value *` option of _robot_
             """,
         robot_name="variable",
         robot_priority=500,
         robot_short_name="v",
@@ -1603,17 +1632,17 @@
             variables with string value are supported and name is
             given without `${}`. See --variablefile for a more
             powerful variable setting mechanism.
 
             Examples:
 
             ```
-            --variable str:Hello       =>  ${str} = `Hello`
-            -v hi:Hi_World -E space:_  =>  ${hi} = `Hi World`
-            -v x: -v y:42              =>  ${x} = ``, ${y} = `42`
+            --variable name:Robot  =>  ${name} = `Robot`
+            -v "hello:Hello world" =>  ${hello} = `Hello world`
+            -v x: -v y:42          =>  ${x} = ``, ${y} = `42`
             ```
 
             corresponds to the `-v --variable name:value *` option of _rebot_
             """,
     )
     extra_variable_files: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
```

### Comparing `robotcode_robot-0.41.0/src/robotcode/robot/config/utils.py` & `robotcode_robot-0.43.0/src/robotcode/robot/config/utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.41.0/.gitignore` & `robotcode_robot-0.43.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.41.0/LICENSE.txt` & `robotcode_robot-0.43.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.41.0/README.md` & `robotcode_robot-0.43.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.41.0/pyproject.toml` & `robotcode_robot-0.43.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
   "tomli>=1.1.0; python_version < '3.11'",
-  "robotcode-core==0.41.0",
+  "robotcode-core==0.43.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
```

### Comparing `robotcode_robot-0.41.0/PKG-INFO` & `robotcode_robot-0.43.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-robot
-Version: 0.41.0
+Version: 0.43.0
 Summary: Support classes for RobotCode for handling Robot Framework projects.
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-core==0.41.0
+Requires-Dist: robotcode-core==0.43.0
 Requires-Dist: robotframework>=4.1.0
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # robotcode-robot
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-robot.svg)](https://pypi.org/project/robotcode-robot)
```

