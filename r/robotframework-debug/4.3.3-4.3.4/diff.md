# Comparing `tmp/robotframework-debug-4.3.3.tar.gz` & `tmp/robotframework-debug-4.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-debug-4.3.3.tar", last modified: Fri May  5 16:32:41 2023, max compression
+gzip compressed data, was "robotframework-debug-4.3.4.tar", last modified: Wed Jun 14 00:09:46 2023, max compression
```

## Comparing `robotframework-debug-4.3.3.tar` & `robotframework-debug-4.3.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-05 16:32:41.693233 robotframework-debug-4.3.3/
--rw-r--r--   0 rener      (502) wheel        (0)      545 2022-09-28 17:53:40.000000 robotframework-debug-4.3.3/.coveragerc
--rw-r--r--   0 rener      (502) wheel        (0)      272 2022-09-28 17:53:40.000000 robotframework-debug-4.3.3/.gitpod.yml
--rw-r--r--   0 rener      (502) wheel        (0)     5811 2022-09-28 17:53:40.000000 robotframework-debug-4.3.3/ChangeLog
--rw-r--r--   0 rener      (502) wheel        (0)      139 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/CreateWheel.sh
--rw-r--r--   0 rener      (502) wheel        (0)     1471 2022-09-28 17:53:40.000000 robotframework-debug-4.3.3/LICENSE
--rw-r--r--   0 rener      (502) wheel        (0)      215 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/MANIFEST.in
--rw-r--r--   0 rener      (502) wheel        (0)     6027 2023-05-05 16:32:41.693328 robotframework-debug-4.3.3/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)     5047 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/README.rst
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-05 16:32:41.691743 robotframework-debug-4.3.3/RobotDebug/
--rw-r--r--   0 rener      (502) wheel        (0)     5878 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/RobotDebug.py
--rw-r--r--   0 rener      (502) wheel        (0)      154 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/__init__.py
--rw-r--r--   0 rener      (502) wheel        (0)    12567 2023-05-05 16:27:48.000000 robotframework-debug-4.3.3/RobotDebug/cmdcompleter.py
--rw-r--r--   0 rener      (502) wheel        (0)     9931 2023-05-05 16:26:16.000000 robotframework-debug-4.3.3/RobotDebug/debugcmd.py
--rw-r--r--   0 rener      (502) wheel        (0)      396 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/globals.py
--rw-r--r--   0 rener      (502) wheel        (0)     4195 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/history_app.py
--rw-r--r--   0 rener      (502) wheel        (0)     9135 2023-05-05 16:27:39.000000 robotframework-debug-4.3.3/RobotDebug/lexer.py
--rw-r--r--   0 rener      (502) wheel        (0)    13309 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/prompttoolkitcmd.py
--rw-r--r--   0 rener      (502) wheel        (0)     3330 2023-05-05 16:18:45.000000 robotframework-debug-4.3.3/RobotDebug/robotkeyword.py
--rw-r--r--   0 rener      (502) wheel        (0)     1892 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/robotlib.py
--rw-r--r--   0 rener      (502) wheel        (0)     1286 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/shell.py
--rw-r--r--   0 rener      (502) wheel        (0)     4279 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/sourcelines.py
--rw-r--r--   0 rener      (502) wheel        (0)     2587 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/styles.py
--rw-r--r--   0 rener      (502) wheel        (0)       18 2023-05-05 16:29:42.000000 robotframework-debug-4.3.3/RobotDebug/version.py
--rw-r--r--   0 rener      (502) wheel        (0)       26 2022-09-28 17:53:40.000000 robotframework-debug-4.3.3/_config.yml
--rw-r--r--   0 rener      (502) wheel        (0)      738 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/pyproject.toml
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-05 16:32:41.692729 robotframework-debug-4.3.3/robotframework_debug.egg-info/
--rw-r--r--   0 rener      (502) wheel        (0)     6027 2023-05-05 16:32:41.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)      832 2023-05-05 16:32:41.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/SOURCES.txt
--rw-r--r--   0 rener      (502) wheel        (0)        1 2023-05-05 16:32:41.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/dependency_links.txt
--rw-r--r--   0 rener      (502) wheel        (0)       86 2023-05-05 16:32:41.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/entry_points.txt
--rw-r--r--   0 rener      (502) wheel        (0)        1 2022-09-28 17:59:17.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/not-zip-safe
--rw-r--r--   0 rener      (502) wheel        (0)       77 2023-05-05 16:32:41.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/requires.txt
--rw-r--r--   0 rener      (502) wheel        (0)       11 2023-05-05 16:32:41.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/top_level.txt
--rw-r--r--   0 rener      (502) wheel        (0)      159 2023-05-05 16:32:41.693613 robotframework-debug-4.3.3/setup.cfg
--rwxr-xr-x   0 rener      (502) wheel        (0)     2112 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/setup.py
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-05 16:32:41.693112 robotframework-debug-4.3.3/tests/
--rw-r--r--   0 rener      (502) wheel        (0)        0 2022-09-28 17:53:40.000000 robotframework-debug-4.3.3/tests/__init__.py
--rw-r--r--   0 rener      (502) wheel        (0)      609 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/tests/step.robot
--rw-r--r--   0 rener      (502) wheel        (0)     6067 2022-09-28 18:50:01.000000 robotframework-debug-4.3.3/tests/test_debuglibrary.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-14 00:09:46.010474 robotframework-debug-4.3.4/
+-rw-r--r--   0 rener      (502) wheel        (0)      545 2022-09-28 17:53:40.000000 robotframework-debug-4.3.4/.coveragerc
+-rw-r--r--   0 rener      (502) wheel        (0)      272 2022-09-28 17:53:40.000000 robotframework-debug-4.3.4/.gitpod.yml
+-rw-r--r--   0 rener      (502) wheel        (0)     5811 2022-09-28 17:53:40.000000 robotframework-debug-4.3.4/ChangeLog
+-rw-r--r--   0 rener      (502) wheel        (0)      139 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/CreateWheel.sh
+-rw-r--r--   0 rener      (502) wheel        (0)     1471 2022-09-28 17:53:40.000000 robotframework-debug-4.3.4/LICENSE
+-rw-r--r--   0 rener      (502) wheel        (0)      215 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/MANIFEST.in
+-rw-r--r--   0 rener      (502) wheel        (0)     6027 2023-06-14 00:09:46.010550 robotframework-debug-4.3.4/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)     5047 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/README.rst
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-14 00:09:46.009026 robotframework-debug-4.3.4/RobotDebug/
+-rw-r--r--   0 rener      (502) wheel        (0)     5878 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/RobotDebug/RobotDebug.py
+-rw-r--r--   0 rener      (502) wheel        (0)      154 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/RobotDebug/__init__.py
+-rw-r--r--   0 rener      (502) wheel        (0)    12573 2023-06-14 00:05:36.000000 robotframework-debug-4.3.4/RobotDebug/cmdcompleter.py
+-rw-r--r--   0 rener      (502) wheel        (0)     9931 2023-05-05 16:26:16.000000 robotframework-debug-4.3.4/RobotDebug/debugcmd.py
+-rw-r--r--   0 rener      (502) wheel        (0)      396 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/RobotDebug/globals.py
+-rw-r--r--   0 rener      (502) wheel        (0)     4195 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/RobotDebug/history_app.py
+-rw-r--r--   0 rener      (502) wheel        (0)     9135 2023-05-05 16:27:39.000000 robotframework-debug-4.3.4/RobotDebug/lexer.py
+-rw-r--r--   0 rener      (502) wheel        (0)    13309 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/RobotDebug/prompttoolkitcmd.py
+-rw-r--r--   0 rener      (502) wheel        (0)     3330 2023-05-05 16:18:45.000000 robotframework-debug-4.3.4/RobotDebug/robotkeyword.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1892 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/RobotDebug/robotlib.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1286 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/RobotDebug/shell.py
+-rw-r--r--   0 rener      (502) wheel        (0)     4279 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/RobotDebug/sourcelines.py
+-rw-r--r--   0 rener      (502) wheel        (0)     2587 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/RobotDebug/styles.py
+-rw-r--r--   0 rener      (502) wheel        (0)       18 2023-06-14 00:07:23.000000 robotframework-debug-4.3.4/RobotDebug/version.py
+-rw-r--r--   0 rener      (502) wheel        (0)       26 2022-09-28 17:53:40.000000 robotframework-debug-4.3.4/_config.yml
+-rw-r--r--   0 rener      (502) wheel        (0)      738 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/pyproject.toml
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-14 00:09:46.009962 robotframework-debug-4.3.4/robotframework_debug.egg-info/
+-rw-r--r--   0 rener      (502) wheel        (0)     6027 2023-06-14 00:09:45.000000 robotframework-debug-4.3.4/robotframework_debug.egg-info/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)      832 2023-06-14 00:09:45.000000 robotframework-debug-4.3.4/robotframework_debug.egg-info/SOURCES.txt
+-rw-r--r--   0 rener      (502) wheel        (0)        1 2023-06-14 00:09:45.000000 robotframework-debug-4.3.4/robotframework_debug.egg-info/dependency_links.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       86 2023-06-14 00:09:45.000000 robotframework-debug-4.3.4/robotframework_debug.egg-info/entry_points.txt
+-rw-r--r--   0 rener      (502) wheel        (0)        1 2022-09-28 17:59:17.000000 robotframework-debug-4.3.4/robotframework_debug.egg-info/not-zip-safe
+-rw-r--r--   0 rener      (502) wheel        (0)       77 2023-06-14 00:09:45.000000 robotframework-debug-4.3.4/robotframework_debug.egg-info/requires.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       11 2023-06-14 00:09:45.000000 robotframework-debug-4.3.4/robotframework_debug.egg-info/top_level.txt
+-rw-r--r--   0 rener      (502) wheel        (0)      159 2023-06-14 00:09:46.010824 robotframework-debug-4.3.4/setup.cfg
+-rwxr-xr-x   0 rener      (502) wheel        (0)     2112 2023-06-12 13:44:59.000000 robotframework-debug-4.3.4/setup.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-14 00:09:46.010354 robotframework-debug-4.3.4/tests/
+-rw-r--r--   0 rener      (502) wheel        (0)        0 2022-09-28 17:53:40.000000 robotframework-debug-4.3.4/tests/__init__.py
+-rw-r--r--   0 rener      (502) wheel        (0)      609 2023-05-05 15:42:55.000000 robotframework-debug-4.3.4/tests/step.robot
+-rw-r--r--   0 rener      (502) wheel        (0)     6067 2022-09-28 18:50:01.000000 robotframework-debug-4.3.4/tests/test_debuglibrary.py
```

### Comparing `robotframework-debug-4.3.3/.coveragerc` & `robotframework-debug-4.3.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/ChangeLog` & `robotframework-debug-4.3.4/ChangeLog`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/LICENSE` & `robotframework-debug-4.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/PKG-INFO` & `robotframework-debug-4.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-debug
-Version: 4.3.3
+Version: 4.3.4
 Summary: RobotFramework debug shell
 Home-page: https://github.com/imbus/robotframework-debug/
 Author: René Rohner
 Author-email: snooz@postoe.de
 License: New BSD
 Keywords: robotframework,debug,shell,repl
 Platform: Linux
```

### Comparing `robotframework-debug-4.3.3/README.rst` & `robotframework-debug-4.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/RobotDebug/RobotDebug.py` & `robotframework-debug-4.3.4/RobotDebug/RobotDebug.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/RobotDebug/cmdcompleter.py` & `robotframework-debug-4.3.4/RobotDebug/cmdcompleter.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     def get_completions(self, document, complete_event):
         """Compute suggestions."""
         # RobotFrameworkLocalLexer().parse_doc(document)
         text = document.current_line_before_cursor
         cursor_col = document.cursor_position_col
         cursor_row = document.cursor_position_row
         token_list = list(get_robot_token(document.text))
-        statements = list(_tokens_to_statements(token_list))
+        statements = list(_tokens_to_statements(token_list, None))
         statement_info = StatementInformation(cursor_col, cursor_row, statements)
         self.current_statement = statement_info
         statement_type = statement_info.statement_type
         previous_token = statement_info.previous_token
         token = statement_info.token
         cursor_pos = statement_info.cursor_pos
```

### Comparing `robotframework-debug-4.3.3/RobotDebug/debugcmd.py` & `robotframework-debug-4.3.4/RobotDebug/debugcmd.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/RobotDebug/history_app.py` & `robotframework-debug-4.3.4/RobotDebug/history_app.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/RobotDebug/lexer.py` & `robotframework-debug-4.3.4/RobotDebug/lexer.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/RobotDebug/prompttoolkitcmd.py` & `robotframework-debug-4.3.4/RobotDebug/prompttoolkitcmd.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/RobotDebug/robotkeyword.py` & `robotframework-debug-4.3.4/RobotDebug/robotkeyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/RobotDebug/robotlib.py` & `robotframework-debug-4.3.4/RobotDebug/robotlib.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/RobotDebug/shell.py` & `robotframework-debug-4.3.4/RobotDebug/shell.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/RobotDebug/sourcelines.py` & `robotframework-debug-4.3.4/RobotDebug/sourcelines.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/RobotDebug/styles.py` & `robotframework-debug-4.3.4/RobotDebug/styles.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/pyproject.toml` & `robotframework-debug-4.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/robotframework_debug.egg-info/PKG-INFO` & `robotframework-debug-4.3.4/robotframework_debug.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-debug
-Version: 4.3.3
+Version: 4.3.4
 Summary: RobotFramework debug shell
 Home-page: https://github.com/imbus/robotframework-debug/
 Author: René Rohner
 Author-email: snooz@postoe.de
 License: New BSD
 Keywords: robotframework,debug,shell,repl
 Platform: Linux
```

### Comparing `robotframework-debug-4.3.3/robotframework_debug.egg-info/SOURCES.txt` & `robotframework-debug-4.3.4/robotframework_debug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/setup.py` & `robotframework-debug-4.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/tests/step.robot` & `robotframework-debug-4.3.4/tests/step.robot`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.3/tests/test_debuglibrary.py` & `robotframework-debug-4.3.4/tests/test_debuglibrary.py`

 * *Files identical despite different names*

