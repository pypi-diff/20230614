# Comparing `tmp/hayloft-0.1.3.tar.gz` & `tmp/hayloft-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.1.3.tar", max compression
+gzip compressed data, was "hayloft-0.1.4.tar", max compression
```

## Comparing `hayloft-0.1.3.tar` & `hayloft-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.3/LICENSE
--rw-r--r--   0        0        0      293 2023-06-13 17:37:06.188148 hayloft-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.3/hayloft/__init__.py
--rw-r--r--   0        0        0     3185 2023-06-13 17:03:36.638281 hayloft-0.1.3/hayloft/app.py
--rw-r--r--   0        0        0      455 2023-06-13 17:02:40.814396 hayloft-0.1.3/hayloft/logger.py
--rw-r--r--   0        0        0    18046 2023-06-13 15:26:59.212520 hayloft-0.1.3/hayloft/public/assets/index-144454fa.css
--rw-r--r--   0        0        0   174554 2023-06-13 15:26:59.215854 hayloft-0.1.3/hayloft/public/assets/index-efbd5a31.js
--rw-r--r--   0        0        0      442 2023-06-13 15:26:59.215854 hayloft-0.1.3/hayloft/public/index.html
--rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.3/hayloft/schema.py
--rw-r--r--   0        0        0      430 2023-06-13 17:46:13.723561 hayloft-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 hayloft-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.4/LICENSE
+-rw-r--r--   0        0        0      295 2023-06-14 14:43:21.952821 hayloft-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.4/hayloft/__init__.py
+-rw-r--r--   0        0        0     3139 2023-06-14 14:51:34.732443 hayloft-0.1.4/hayloft/app.py
+-rw-r--r--   0        0        0      457 2023-06-14 14:43:49.279652 hayloft-0.1.4/hayloft/logger.py
+-rw-r--r--   0        0        0    18046 2023-06-14 14:46:56.924111 hayloft-0.1.4/hayloft/public/assets/index-144454fa.css
+-rw-r--r--   0        0        0   174556 2023-06-14 14:46:56.924111 hayloft-0.1.4/hayloft/public/assets/index-ad0b845f.js
+-rw-r--r--   0        0        0      382 2023-06-14 14:48:21.944620 hayloft-0.1.4/hayloft/public/index.html
+-rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.4/hayloft/schema.py
+-rw-r--r--   0        0        0      430 2023-06-14 14:54:01.546657 hayloft-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 hayloft-0.1.4/PKG-INFO
```

### Comparing `hayloft-0.1.3/LICENSE` & `hayloft-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.3/hayloft/app.py` & `hayloft-0.1.4/hayloft/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from flask import request, jsonify, send_file, send_from_directory, Response, cli
+from flask import request, jsonify, send_file, send_from_directory, Response
 from flask_cors import CORS
 from hayloft.schema import app, db, sse, Event, Session
 import argparse
 import time
 
 CORS(app)  # for development
-cli.show_server_banner = lambda *x: None
 
 
 @app.route("/", methods=["GET"])
 def index():
     return send_file("public/index.html")
```

### Comparing `hayloft-0.1.3/hayloft/public/assets/index-144454fa.css` & `hayloft-0.1.4/hayloft/public/assets/index-144454fa.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.3/hayloft/public/assets/index-efbd5a31.js` & `hayloft-0.1.4/hayloft/public/assets/index-ad0b845f.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -8820,15 +8820,15 @@
                                     onClick: o => {
                                         !r.folded && t(da(n.id, r.id)), o.preventDefault()
                                     },
                                     children: [`${n.events.length-l}. ${r.title}`, " ", T.jsx("span", {
                                         className: Nn("py-0 px-2 text-sm font-normal text-gray-300 rounded-lg", {
                                             "bg-cyan-900": r.type === "info",
                                             "bg-indigo-900": r.type === "prompt",
-                                            "bg-orange-900": r.type === "response"
+                                            "bg-orange-900": r.type === "completion"
                                         }),
                                         children: r.type
                                     })]
                                 }), T.jsx("p", {
                                     className: Nn("text-base ", {
                                         "text-gray-500 line-clamp-2": r.folded,
                                         "text-gray-400": !r.folded
```

### Comparing `hayloft-0.1.3/hayloft/schema.py` & `hayloft-0.1.4/hayloft/schema.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.3/PKG-INFO` & `hayloft-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.1.3
+Version: 0.1.4
 Summary: UI tool for LLM frameworks
 License: MIT
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,15 +13,15 @@
 Requires-Dist: flask-sqlalchemy (>=3.0.3,<4.0.0)
 Requires-Dist: nanoid (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Hayloft
 
-UI tool for LLM frameworks to make easy prompt/response tracking, store and comparison of different sessions.
+UI tool for LLM frameworks to make easy prompt/completion tracking, store and comparison of different sessions.
 
 Install package with pip
 
 ```
 pip install hayloft
 ```
```

