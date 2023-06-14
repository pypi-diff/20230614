# Comparing `tmp/python-printr-3.0.tar.gz` & `tmp/python-printr-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-printr-3.0.tar", last modified: Sun Jun 11 14:12:23 2023, max compression
+gzip compressed data, was "python-printr-3.1.tar", last modified: Wed Jun 14 13:43:52 2023, max compression
```

## Comparing `python-printr-3.0.tar` & `python-printr-3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 14:12:23.933689 python-printr-3.0/
--rw-rw-rw-   0        0        0       66 2022-04-13 16:11:03.000000 python-printr-3.0/.gitignore
--rw-rw-rw-   0        0        0     3347 2023-06-11 14:12:23.933689 python-printr-3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3089 2023-06-11 14:12:17.000000 python-printr-3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 14:12:23.927694 python-printr-3.0/printr/
--rw-rw-rw-   0        0        0     8183 2023-06-11 14:11:57.000000 python-printr-3.0/printr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:12:23.932690 python-printr-3.0/python_printr.egg-info/
--rw-rw-rw-   0        0        0     3347 2023-06-11 14:12:23.000000 python-printr-3.0/python_printr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-06-11 14:12:23.000000 python-printr-3.0/python_printr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 14:12:23.000000 python-printr-3.0/python_printr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-11 14:12:23.000000 python-printr-3.0/python_printr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 14:12:23.000000 python-printr-3.0/python_printr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-11 14:12:23.934689 python-printr-3.0/setup.cfg
--rw-rw-rw-   0        0        0      427 2023-06-11 14:12:03.000000 python-printr-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:43:52.303928 python-printr-3.1/
+-rw-rw-rw-   0        0        0       64 2023-06-14 13:12:02.000000 python-printr-3.1/.gitignore
+-rw-rw-rw-   0        0        0     3347 2023-06-14 13:43:52.303928 python-printr-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3089 2023-06-11 14:12:17.000000 python-printr-3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 13:43:52.297932 python-printr-3.1/printr/
+-rw-rw-rw-   0        0        0     7600 2023-06-14 13:43:47.000000 python-printr-3.1/printr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:43:52.302929 python-printr-3.1/python_printr.egg-info/
+-rw-rw-rw-   0        0        0     3347 2023-06-14 13:43:51.000000 python-printr-3.1/python_printr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-06-14 13:43:52.000000 python-printr-3.1/python_printr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 13:43:51.000000 python-printr-3.1/python_printr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-14 13:43:51.000000 python-printr-3.1/python_printr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-14 13:43:51.000000 python-printr-3.1/python_printr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-14 13:43:52.304927 python-printr-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      427 2023-06-14 13:43:39.000000 python-printr-3.1/setup.py
```

### Comparing `python-printr-3.0/PKG-INFO` & `python-printr-3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-printr
-Version: 3.0
+Version: 3.1
 Summary: printr
 Home-page: https://github.com/xjxckk/python-printr/
 Download-URL: https://github.com/xjxckk/python-printr/archive/refs/tags/v0.1.tar.gz
 Description-Content-Type: text/markdown
 
 ### python-printr
 Python print functions to beautify output
```

### Comparing `python-printr-3.0/README.md` & `python-printr-3.1/README.md`

 * *Files identical despite different names*

### Comparing `python-printr-3.0/printr/__init__.py` & `python-printr-3.1/printr/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys, logging, json, os, shutil, coloredlogs
 from pathlib import Path
 from datetime import datetime
 
 class logger:
-    def __init__(self, log_filepath=None, max_lines=100_000, level='info', name=None, log_to_file=True):
+    def __init__(self, log_filepath=None, max_lines=100_000, level='info', name=None, log_to_file=False):
         filename = Path(sys.argv[0]).stem
         self.filename = filename
         if not log_filepath:
             log_filepath = f'{os.getcwd()}/{filename}.txt'
         self.log_filepath = log_filepath
         self.max_lines = max_lines
         self.log_to_file = log_to_file
@@ -38,29 +38,15 @@
         
         if not name:
             name = filename
         self.current_time('Starting', name)
         self.log()
 
     def log(self, *items, level='info', beautify=True):
-        message = ''
-        for item in items:
-            if message and '\n' not in message:
-                message += ' ' # Add space in between variables
-            if beautify and (isinstance(item, dict) or isinstance(item, list)):
-                try:
-                    if message and '\n' not in message: # Add line breaks before and after
-                        formatted_item = '\n'
-                    else:
-                        formatted_item = ''
-                    formatted_item += json.dumps(item, indent=4) # Beautify JSON objects
-                    item = formatted_item + '\n'
-                except TypeError:
-                    pass
-            message += str(item)
+        message = prettify(items, beautify=beautify)
 
         if not message:
             if self.log_to_file:
                 log_format = logging.Formatter(fmt=self.indent + '%(message)s')
                 self.log_file.setFormatter(log_format)
             coloredlogs.install(level=self.level, logger=self.logger, fmt='%(message)s')
 
@@ -124,39 +110,29 @@
         coloredlogs.install(level=self.level, logger=self.logger, fmt='%(message)s') # Reset to default log format
         self.indent = ''
 
 say = print
 class print:
     '''printr'''
     def __init__(self, *items, same_line=False, current_time=False, check_for_log=True, level='info', beautify=True):
-        if len(items) == 1:
-            message = items[0]
-            if beautify and (isinstance(message, dict) or isinstance(message, list)):
-                try: message = json.dumps(message, indent=4) # Beautify JSON objects
-                except TypeError: pass
-        else:
-            message = ''
-            for item in items:
-                if message:
-                    message += ' ' # Add space in between variables
-                if isinstance(item, dict) or isinstance(item, list):
-                    try: item = json.dumps(item, indent=4) # Beautify JSON objects
-                    except TypeError: pass
-                message += str(item)
+        message = prettify(items, beautify)
+
         if current_time:
             current_time = datetime.now()
             current_time = current_time.strftime('%H:%M:%S:%f')
             message = f'{current_time}: {message}'
+
         if same_line:
             terminal_size = shutil.get_terminal_size() # Uses shutil rather than os to support piping output to file
             max_characters = terminal_size.columns - 1
             say(' ' * max_characters, end='') # Clear previous output
             say('\r', end='')
             say(message, end='')
             say('\r', end='')
+
         else:
             if not check_for_log:
                 say(message)
             else:
                 logger = logging.getLogger()
                 if logger.level != 30:
                     if level == 'debug':
@@ -164,19 +140,36 @@
                     elif level == 'error':
                         logger.error(message)
                     else:
                         logger.info(message)
                 elif level != 'debug':
                     say(message)
 
-
-class printr:
-    def __init__(self, *items, same_line=False, current_time=False, check_for_log=True, level='info', beautify=True):
-        print(*items, same_line=same_line, current_time=current_time, check_for_log=check_for_log, level=level, beautify=beautify)
-
 class current_time:
     def __init__(self, *items, same_line=False, check_for_log=True, beautify=True):
         print(*items, same_line=same_line, current_time=True, check_for_log=check_for_log, beautify=beautify)
 
 class same_line:
     def __init__(self, *items, current_time=False, check_for_log=True, beautify=True):
-        print(*items, same_line=same_line, current_time=current_time, check_for_log=check_for_log, beautify=beautify)
+        print(*items, same_line=same_line, current_time=current_time, check_for_log=check_for_log, beautify=beautify)
+
+class printr:
+    def __init__(self, *items, same_line=False, current_time=False, check_for_log=True, level='info', beautify=True):
+        print(*items, same_line=same_line, current_time=current_time, check_for_log=check_for_log, level=level, beautify=beautify)
+
+def prettify(items, beautify):
+    message = ''
+    for item in items:
+        if message and '\n' not in message:
+            message += ' ' # Add space in between variables
+        if beautify and (isinstance(item, dict) or isinstance(item, list)):
+            try:
+                if message and '\n' not in message: # Add line breaks before and after
+                    formatted_item = '\n'
+                else:
+                    formatted_item = ''
+                formatted_item += json.dumps(item, indent=4) # Beautify JSON objects
+                item = formatted_item + '\n'
+            except TypeError:
+                pass
+        message += str(item)
+    return message
```

### Comparing `python-printr-3.0/python_printr.egg-info/PKG-INFO` & `python-printr-3.1/python_printr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-printr
-Version: 3.0
+Version: 3.1
 Summary: printr
 Home-page: https://github.com/xjxckk/python-printr/
 Download-URL: https://github.com/xjxckk/python-printr/archive/refs/tags/v0.1.tar.gz
 Description-Content-Type: text/markdown
 
 ### python-printr
 Python print functions to beautify output
```

