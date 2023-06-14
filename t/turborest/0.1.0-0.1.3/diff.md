# Comparing `tmp/turborest-0.1.0.tar.gz` & `tmp/turborest-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turborest-0.1.0.tar", last modified: Wed Jun 14 09:12:14 2023, max compression
+gzip compressed data, was "turborest-0.1.3.tar", last modified: Wed Jun 14 12:34:43 2023, max compression
```

## Comparing `turborest-0.1.0.tar` & `turborest-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:12:14.538406 turborest-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-14 09:12:14.538406 turborest-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-14 09:12:04.000000 turborest-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-14 09:12:14.542406 turborest-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-14 09:12:04.000000 turborest-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:12:14.538406 turborest-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:12:14.538406 turborest-0.1.0/src/turborest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-14 09:12:14.000000 turborest-0.1.0/src/turborest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-14 09:12:14.000000 turborest-0.1.0/src/turborest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:12:14.000000 turborest-0.1.0/src/turborest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 09:12:14.000000 turborest-0.1.0/src/turborest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:12:14.000000 turborest-0.1.0/src/turborest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:34:43.019371 turborest-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-14 12:34:43.019371 turborest-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-14 12:34:22.000000 turborest-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-14 12:34:22.000000 turborest-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:34:43.019371 turborest-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-14 12:34:22.000000 turborest-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:34:43.015370 turborest-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:34:43.019371 turborest-0.1.3/src/turborest/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 12:34:22.000000 turborest-0.1.3/src/turborest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-14 12:34:22.000000 turborest-0.1.3/src/turborest/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:34:43.019371 turborest-0.1.3/src/turborest/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 12:34:22.000000 turborest-0.1.3/src/turborest/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-14 12:34:22.000000 turborest-0.1.3/src/turborest/cmd/ping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:34:43.019371 turborest-0.1.3/src/turborest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-14 12:34:43.000000 turborest-0.1.3/src/turborest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-14 12:34:43.000000 turborest-0.1.3/src/turborest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:34:43.000000 turborest-0.1.3/src/turborest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 12:34:43.000000 turborest-0.1.3/src/turborest.egg-info/top_level.txt
```

### Comparing `turborest-0.1.0/PKG-INFO` & `turborest-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: turborest
-Version: 0.1.0
-Summary: A simple REST client for Python
+Version: 0.1.3
+Summary: A library for monitoring files and directories for changes
 Home-page: https://github.com/bytesentinel-io/turborest
 Author: ByteSentinel.io
 Author-email: dev@bytesentinel.io
-License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 
 # TurboREST
 
 TurboREST is a REST API framework for Python 3.7+.
 
 ## Installation
 
@@ -25,25 +23,49 @@
 
 ## Usage
 
 ```python
 from turborest import Client
 
 def main():
+    client = Client(format="json")
+    client.get("https://api.bytesentinel.io/test")
+```
+
+## Authentication
+
+```python
+from turborest import Client
+
+def main():
     auth = ("Bearer", "xyz")
     client = Client(format="json", auth=auth)
     client.get("https://api.bytesentinel.io/test")
 ```
 
+## Proxy
+
+```python
+from turborest import Client
+
+def main():
+    proxy = "http://localhost:8080"
+    client = Client(format="json", proxy=proxy)
+    client.get("https://api.bytesentinel.io/test")
+```
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
 ## License
 
 ### MIT License
 
 ```text
 MIT License
 
 TurboREST - A REST API framework for Python 3.7+.
 
-
 ...
     
 ```
```

### Comparing `turborest-0.1.0/src/turborest.egg-info/PKG-INFO` & `turborest-0.1.3/src/turborest.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: turborest
-Version: 0.1.0
-Summary: A simple REST client for Python
+Version: 0.1.3
+Summary: A library for monitoring files and directories for changes
 Home-page: https://github.com/bytesentinel-io/turborest
 Author: ByteSentinel.io
 Author-email: dev@bytesentinel.io
-License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 
 # TurboREST
 
 TurboREST is a REST API framework for Python 3.7+.
 
 ## Installation
 
@@ -25,25 +23,49 @@
 
 ## Usage
 
 ```python
 from turborest import Client
 
 def main():
+    client = Client(format="json")
+    client.get("https://api.bytesentinel.io/test")
+```
+
+## Authentication
+
+```python
+from turborest import Client
+
+def main():
     auth = ("Bearer", "xyz")
     client = Client(format="json", auth=auth)
     client.get("https://api.bytesentinel.io/test")
 ```
 
+## Proxy
+
+```python
+from turborest import Client
+
+def main():
+    proxy = "http://localhost:8080"
+    client = Client(format="json", proxy=proxy)
+    client.get("https://api.bytesentinel.io/test")
+```
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
 ## License
 
 ### MIT License
 
 ```text
 MIT License
 
 TurboREST - A REST API framework for Python 3.7+.
 
-
 ...
     
 ```
```

