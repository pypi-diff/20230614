# Comparing `tmp/kestrel-jupyter-1.0.8.tar.gz` & `tmp/kestrel-jupyter-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel-jupyter-1.0.8.tar", last modified: Thu May 18 02:01:24 2023, max compression
+gzip compressed data, was "kestrel-jupyter-1.0.9.tar", last modified: Wed Jun 14 15:56:39 2023, max compression
```

## Comparing `kestrel-jupyter-1.0.8.tar` & `kestrel-jupyter-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/src/kestrel_ipython/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_ipython/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-18 02:01:24.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-18 02:01:24.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 02:01:24.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-18 02:01:24.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 02:01:24.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/codemirror/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/codemirror/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/codemirror/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/tests/test_kernel_install.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/tests/test_notebook_syntax_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:56:39.439997 kestrel-jupyter-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-14 15:56:39.439997 kestrel-jupyter-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-14 15:56:39.439997 kestrel-jupyter-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:56:39.439997 kestrel-jupyter-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:56:39.439997 kestrel-jupyter-1.0.9/src/kestrel_ipython/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/src/kestrel_ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/src/kestrel_ipython/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:56:39.439997 kestrel-jupyter-1.0.9/src/kestrel_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-14 15:56:39.000000 kestrel-jupyter-1.0.9/src/kestrel_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-14 15:56:39.000000 kestrel-jupyter-1.0.9/src/kestrel_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:56:39.000000 kestrel-jupyter-1.0.9/src/kestrel_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-14 15:56:39.000000 kestrel-jupyter-1.0.9/src/kestrel_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 15:56:39.000000 kestrel-jupyter-1.0.9/src/kestrel_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:56:39.439997 kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:56:39.439997 kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/codemirror/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/codemirror/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/codemirror/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:56:39.439997 kestrel-jupyter-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/tests/test_kernel_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-14 15:56:04.000000 kestrel-jupyter-1.0.9/tests/test_notebook_syntax_gen.py
```

### Comparing `kestrel-jupyter-1.0.8/LICENSE` & `kestrel-jupyter-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kestrel-jupyter-1.0.8/PKG-INFO` & `kestrel-jupyter-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-jupyter
-Version: 1.0.8
+Version: 1.0.9
 Summary: Kestrel Jupyter Kernel
 Home-page: https://github.com/IBM/kestrel-jupyter
 License: Apache 2.0 License
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `kestrel-jupyter-1.0.8/README.rst` & `kestrel-jupyter-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `kestrel-jupyter-1.0.8/setup.cfg` & `kestrel-jupyter-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kestrel-jupyter
-version = 1.0.8
+version = 1.0.9
 description = Kestrel Jupyter Kernel
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = 
 	domain specific language
 	cyber threat hunting
 	extended detection and response
```

### Comparing `kestrel-jupyter-1.0.8/src/kestrel_ipython/magic.py` & `kestrel-jupyter-1.0.9/src/kestrel_ipython/magic.py`

 * *Files identical despite different names*

### Comparing `kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/PKG-INFO` & `kestrel-jupyter-1.0.9/src/kestrel_jupyter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-jupyter
-Version: 1.0.8
+Version: 1.0.9
 Summary: Kestrel Jupyter Kernel
 Home-page: https://github.com/IBM/kestrel-jupyter
 License: Apache 2.0 License
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/SOURCES.txt` & `kestrel-jupyter-1.0.9/src/kestrel_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js` & `kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -17,40 +17,51 @@
 
         var smallRE = /[a-z_]/;
         var largeRE = /[A-Z]/;
         var digitRE = /[0-9]/;
         var hexitRE = /[0-9A-Fa-f]/;
         var octitRE = /[0-7]/;
         var idRE = /[a-z_A-Z0-9\']/;
+        var typeRE = /[a-zA-Z0-9-]/;
         var symbolRE = /[-!#$%&*+.\/<=>?@\\^|~:]/;
         var specialRE = /[(),;[\]`{}]/;
         var whiteCharRE = /[ \t\v\f]/; // newlines are handled in tokenizer
         var isoTimestamp = /[0-9:.\-TZ]/;
 
         function normal() {
             return function(source, setState) {
                 if (source.eatWhile(whiteCharRE)) {
                     return null;
                 }
 
                 var ch = source.next();
 
+                if (ch == '#') {
+                    source.skipToEnd();
+                    return "comment";
+                }
+
                 if (ch == '\'') {
                     return switchState(source, setState, stringLiteral);
                 }
 
                 if (ch == 't') {
                     if (source.eat('\'')) {
                         source.eatWhile(isoTimestamp);
                         if (source.eat('\'')) {
                             return "string-2";
                         }
                     }
                 }
 
+                if (typeRE.test(source)) {
+                    source.eatWhile(typeRE);
+                    return "type";
+                }
+
                 if (largeRE.test(ch)) {
                     source.eatWhile(idRE);
                     return "error";
                 }
 
                 if (smallRE.test(ch)) {
                     source.eatWhile(idRE);
@@ -113,14 +124,19 @@
             var wkw = {};
 
             var keywords = << < KEYWORDS >>> ;
 
             for (var i = keywords.length; i--;)
                 wkw[keywords[i]] = "keyword";
 
+            var ops = ["IN", "NOT", "LIKE", "MATCHES", "ISSUBSET", "in", "not", "like", "matches", "isubset", "=", "!=", "<", ">", "<=", ">=", ];
+
+            for (var i = ops.length; i--;)
+                wkw[ops[i]] = "operator";
+
             return wkw;
         })();
 
         return {
             startState: function() {
                 return {
                     f: normal()
```

### Comparing `kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/codemirror/setup.py` & `kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/codemirror/setup.py`

 * *Files identical despite different names*

### Comparing `kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/kernel.py` & `kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/setup.py` & `kestrel-jupyter-1.0.9/src/kestrel_jupyter_kernel/setup.py`

 * *Files identical despite different names*

