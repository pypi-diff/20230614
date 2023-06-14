# Comparing `tmp/interactivenlp-0.0.4.tar.gz` & `tmp/interactivenlp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactivenlp-0.0.4.tar", last modified: Thu May 18 20:43:31 2023, max compression
+gzip compressed data, was "interactivenlp-0.1.0.tar", last modified: Wed Jun 14 20:37:56 2023, max compression
```

## Comparing `interactivenlp-0.0.4.tar` & `interactivenlp-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 20:43:31.588727 interactivenlp-0.0.4/
--rw-rw-rw-   0        0        0     1090 2023-05-18 19:27:11.000000 interactivenlp-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      358 2023-05-18 20:43:31.579322 interactivenlp-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-05-18 19:26:55.000000 interactivenlp-0.0.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-18 20:43:31.558277 interactivenlp-0.0.4/interactivenlp/
--rw-rw-rw-   0        0        0      211 2023-05-18 20:43:07.000000 interactivenlp-0.0.4/interactivenlp/__init__.py
--rw-rw-rw-   0        0        0      930 2023-05-18 20:42:30.000000 interactivenlp-0.0.4/interactivenlp/server.py
--rw-rw-rw-   0        0        0     1354 2023-05-18 20:42:51.000000 interactivenlp-0.0.4/interactivenlp/types.py
-drwxrwxrwx   0        0        0        0 2023-05-18 20:43:31.578325 interactivenlp-0.0.4/interactivenlp.egg-info/
--rw-rw-rw-   0        0        0      358 2023-05-18 20:43:31.000000 interactivenlp-0.0.4/interactivenlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-18 20:43:31.000000 interactivenlp-0.0.4/interactivenlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 20:43:31.000000 interactivenlp-0.0.4/interactivenlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-18 20:43:31.000000 interactivenlp-0.0.4/interactivenlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-18 20:43:31.000000 interactivenlp-0.0.4/interactivenlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 20:43:31.588727 interactivenlp-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      616 2023-05-18 20:43:26.000000 interactivenlp-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:37:56.457948 interactivenlp-0.1.0/
+-rw-rw-rw-   0        0        0     1093 2023-06-14 20:18:06.000000 interactivenlp-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      358 2023-06-14 20:37:56.456944 interactivenlp-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-05-18 19:26:55.000000 interactivenlp-0.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 20:37:56.436398 interactivenlp-0.1.0/interactivenlp/
+-rw-rw-rw-   0        0        0      211 2023-05-18 20:43:07.000000 interactivenlp-0.1.0/interactivenlp/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-06-14 20:34:18.000000 interactivenlp-0.1.0/interactivenlp/server.py
+-rw-rw-rw-   0        0        0     2184 2023-06-14 20:33:38.000000 interactivenlp-0.1.0/interactivenlp/types.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:37:56.456009 interactivenlp-0.1.0/interactivenlp.egg-info/
+-rw-rw-rw-   0        0        0      358 2023-06-14 20:37:56.000000 interactivenlp-0.1.0/interactivenlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-14 20:37:56.000000 interactivenlp-0.1.0/interactivenlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 20:37:56.000000 interactivenlp-0.1.0/interactivenlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-14 20:37:56.000000 interactivenlp-0.1.0/interactivenlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-14 20:37:56.000000 interactivenlp-0.1.0/interactivenlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 20:37:56.457948 interactivenlp-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      616 2023-06-14 20:36:16.000000 interactivenlp-0.1.0/setup.py
```

### Comparing `interactivenlp-0.0.4/LICENSE` & `interactivenlp-0.1.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2023 interactivenlps
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `interactivenlp-0.0.4/interactivenlp/server.py` & `interactivenlp-0.1.0/interactivenlp/server.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 from flask import Flask, jsonify, request
 from flask_cors import CORS
-from .types import InteractiveRssType, InteractiveFunctionType
+from .types import InteractiveRssType, ModelConfigurationType
 
 
 class Server:
-    def __init__(self, interactive_function: InteractiveFunctionType):
+    def __init__(self, config: ModelConfigurationType):
         self.app = Flask(__name__)
+        self.config = config
+
+        self.functions = config.functions
+
+
 
         CORS(self.app)
 
         @self.app.route('/')
         def index():
             return "Hello, World!"
-
-        @self.app.route('/model', methods=['POST'])
-        def model():
+        
+        @self.app.route('/model/<name>', methods=['POST'])
+        def model_route(name):
+            target_function = next(
+                filter(lambda function: function.name == name, self.functions), None)
+            
+            if target_function is None:
+                return {
+                    "success": False,
+                    "message": "Function not found"
+                }
+            
             rss = request.get_json()
-            # print(rss)
             rss_modeled = InteractiveRssType(
                 "", rss['paragraphs'])
-
-            res = interactive_function(rss_modeled)
+            
+            res = target_function.function(rss_modeled)
             return jsonify([block.__dict__ for block in res])
 
+
         @self.app.route('/submit', methods=['POST'])
         def submit():
             return {
                 "success": True
             }
 
     def run(self):
```

### Comparing `interactivenlp-0.0.4/interactivenlp/types.py` & `interactivenlp-0.1.0/interactivenlp/types.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.type = type
         self.level = level
         self.subBlocks = subBlocks
 
     def __dict__(self):
         subBlocks = []
         if self.subBlocks is not None:
-            subBlocks = [subBlock.__dict__() for subBlock in self.subBlocks]
+            subBlocks = [subBlock.__dict__ for subBlock in self.subBlocks]
 
         return {
             "content": self.content,
             "type": self.type.value,
             "level": self.level.value,
             "subBlocks": subBlocks
         }
@@ -47,7 +47,32 @@
 class InteractiveRssType:
     def __init__(self, article: str, paragraphs: list[str]):
         self.article = article
         self.paragraphs = paragraphs
 
 
 InteractiveFunctionType = Callable[[InteractiveRssType], List[Block]]
+
+class InteractiveFunctionConfigurationType:
+    def __init__(self, function: InteractiveFunctionType, name: str, description: str = None):
+        self.name = name
+        self.function = function
+        self.description = description
+
+    def __dict__(self):
+        return {
+            "name": self.name,
+            "description": self.description
+        }
+
+class ModelConfigurationType:
+    def __init__(self, name: str, description: str, functions: List[InteractiveFunctionConfigurationType],):
+        self.name = name
+        self.description = description
+        self.functions = functions
+
+    def __dict__(self):
+        return {
+            "name": self.name,
+            "description": self.description,
+            "functions": [function.__dict__() for function in self.functions]
+        }
```

### Comparing `interactivenlp-0.0.4/setup.py` & `interactivenlp-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open('README.rst', "r") as f:
     long_description = f.read()
 
 setup(
     name='interactivenlp',
-    version='0.0.4',
+    version='0.1.0',
     description='Interactive NLP',
     long_description=long_description,
     author="Chunxu Yang",
     author_email="chunxuyang@ucla.edu",
     install_requires=[
         'flask',
         'flask-cors',
```

