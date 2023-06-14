# Comparing `tmp/countess-0.0.29.tar.gz` & `tmp/countess-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.29.tar", last modified: Wed May 31 04:03:08 2023, max compression
+gzip compressed data, was "countess-0.0.30.tar", last modified: Wed Jun 14 04:40:08 2023, max compression
```

## Comparing `countess-0.0.29.tar` & `countess-0.0.30.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.934222 countess-0.0.29/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.29/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       26 2023-05-25 01:44:18.000000 countess-0.0.29/MANIFEST.in
--rw-rw-r--   0 nick      (1000) nick      (1000)     3477 2023-05-31 04:03:08.934222 countess-0.0.29/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-05-31 04:01:08.000000 countess-0.0.29/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.926222 countess-0.0.29/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-05-31 04:00:59.000000 countess-0.0.29/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.930222 countess-0.0.29/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.29/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      415 2023-05-25 01:44:18.000000 countess-0.0.29/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4157 2023-05-25 01:44:18.000000 countess-0.0.29/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1910 2023-05-25 01:44:18.000000 countess-0.0.29/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    16561 2023-05-31 03:55:05.000000 countess-0.0.29/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5938 2023-05-26 07:05:39.000000 countess-0.0.29/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    13419 2023-05-31 03:55:05.000000 countess-0.0.29/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.930222 countess-0.0.29/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.29/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    18816 2023-05-31 03:55:05.000000 countess-0.0.29/countess/gui/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5947 2023-05-25 01:44:18.000000 countess-0.0.29/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    14766 2023-05-31 03:55:05.000000 countess-0.0.29/countess/gui/main.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    13294 2023-05-30 06:54:25.000000 countess-0.0.29/countess/gui/tabular.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    19791 2023-05-30 01:24:26.000000 countess-0.0.29/countess/gui/tree.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.934222 countess-0.0.29/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.29/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5969 2023-05-31 03:55:05.000000 countess-0.0.29/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3711 2023-05-31 03:55:05.000000 countess-0.0.29/countess/plugins/data_table.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1236 2023-05-25 01:44:18.000000 countess-0.0.29/countess/plugins/expression.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2160 2023-05-25 01:44:18.000000 countess-0.0.29/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4699 2023-05-31 03:57:07.000000 countess-0.0.29/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1744 2023-05-25 01:44:18.000000 countess-0.0.29/countess/plugins/hdf5.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3051 2023-05-31 03:55:05.000000 countess-0.0.29/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      347 2023-05-25 01:44:18.000000 countess-0.0.29/countess/plugins/log_score.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2562 2023-05-25 01:44:18.000000 countess-0.0.29/countess/plugins/mutagenize.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5520 2023-05-31 03:55:05.000000 countess-0.0.29/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1560 2023-05-31 03:55:05.000000 countess-0.0.29/countess/plugins/python.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6280 2023-05-31 03:57:59.000000 countess-0.0.29/countess/plugins/regex.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2194 2023-05-31 03:55:05.000000 countess-0.0.29/countess/plugins/sequence.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2238 2023-05-31 03:58:42.000000 countess-0.0.29/countess/plugins/variant.py
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.29/countess/py.typed
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.934222 countess-0.0.29/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.29/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    12859 2023-05-25 01:44:18.000000 countess-0.0.29/countess/utils/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.926222 countess-0.0.29/countess.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     3477 2023-05-31 04:03:08.000000 countess-0.0.29/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1089 2023-05-31 04:03:08.000000 countess-0.0.29/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-31 04:03:08.000000 countess-0.0.29/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      997 2023-05-31 04:03:08.000000 countess-0.0.29/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      201 2023-05-31 04:03:08.000000 countess-0.0.29/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-05-31 04:03:08.000000 countess-0.0.29/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     2809 2023-05-26 06:01:26.000000 countess-0.0.29/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-31 04:03:08.934222 countess-0.0.29/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.29/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.934222 countess-0.0.29/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      480 2023-05-25 01:44:18.000000 countess-0.0.29/tests/test_gui.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 04:40:08.673934 countess-0.0.30/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.30/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       26 2023-05-25 01:44:18.000000 countess-0.0.30/MANIFEST.in
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3477 2023-06-14 04:40:08.673934 countess-0.0.30/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-06-14 04:39:26.000000 countess-0.0.30/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 04:40:08.669934 countess-0.0.30/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-06-14 04:39:33.000000 countess-0.0.30/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 04:40:08.673934 countess-0.0.30/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.30/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      415 2023-05-25 01:44:18.000000 countess-0.0.30/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4157 2023-05-25 01:44:18.000000 countess-0.0.30/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1910 2023-05-25 01:44:18.000000 countess-0.0.30/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    16562 2023-06-05 01:49:35.000000 countess-0.0.30/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     7480 2023-06-07 01:05:48.000000 countess-0.0.30/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13419 2023-06-14 04:38:55.000000 countess-0.0.30/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 04:40:08.673934 countess-0.0.30/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.30/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18816 2023-06-14 04:38:55.000000 countess-0.0.30/countess/gui/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5947 2023-05-25 01:44:18.000000 countess-0.0.30/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    15051 2023-06-14 04:38:55.000000 countess-0.0.30/countess/gui/main.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    14244 2023-06-13 05:51:04.000000 countess-0.0.30/countess/gui/tabular.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    20013 2023-06-13 03:08:55.000000 countess-0.0.30/countess/gui/tree.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 04:40:08.673934 countess-0.0.30/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.30/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5969 2023-06-14 04:38:55.000000 countess-0.0.30/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3711 2023-06-14 04:38:55.000000 countess-0.0.30/countess/plugins/data_table.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1642 2023-06-14 04:38:55.000000 countess-0.0.30/countess/plugins/expression.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2160 2023-06-01 00:52:52.000000 countess-0.0.30/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4713 2023-06-14 04:38:55.000000 countess-0.0.30/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1744 2023-05-25 01:44:18.000000 countess-0.0.30/countess/plugins/hdf5.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3287 2023-06-14 04:38:55.000000 countess-0.0.30/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      347 2023-05-25 01:44:18.000000 countess-0.0.30/countess/plugins/log_score.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2562 2023-05-25 01:44:18.000000 countess-0.0.30/countess/plugins/mutagenize.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4165 2023-06-14 04:31:25.000000 countess-0.0.30/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1560 2023-05-31 03:55:05.000000 countess-0.0.30/countess/plugins/python.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6500 2023-06-14 04:38:55.000000 countess-0.0.30/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2194 2023-06-14 04:38:55.000000 countess-0.0.30/countess/plugins/sequence.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2238 2023-06-14 04:38:55.000000 countess-0.0.30/countess/plugins/variant.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.30/countess/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 04:40:08.673934 countess-0.0.30/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.30/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    12859 2023-05-25 01:44:18.000000 countess-0.0.30/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 04:40:08.673934 countess-0.0.30/countess.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3477 2023-06-14 04:40:08.000000 countess-0.0.30/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1089 2023-06-14 04:40:08.000000 countess-0.0.30/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-06-14 04:40:08.000000 countess-0.0.30/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      997 2023-06-14 04:40:08.000000 countess-0.0.30/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      201 2023-06-14 04:40:08.000000 countess-0.0.30/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-06-14 04:40:08.000000 countess-0.0.30/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2809 2023-05-26 06:01:26.000000 countess-0.0.30/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-06-14 04:40:08.673934 countess-0.0.30/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.30/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 04:40:08.673934 countess-0.0.30/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      480 2023-05-25 01:44:18.000000 countess-0.0.30/tests/test_gui.py
```

### Comparing `countess-0.0.29/LICENSE.txt` & `countess-0.0.30/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/PKG-INFO` & `countess-0.0.30/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.29
+Version: 0.0.30
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -12,15 +12,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.29
+# CountESS 0.0.30
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.29/README.md` & `countess-0.0.30/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS 0.0.29
+# CountESS 0.0.30
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.29/countess/core/config.py` & `countess-0.0.30/countess/core/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess/core/logger.py` & `countess-0.0.30/countess/core/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess/core/parameters.py` & `countess-0.0.30/countess/core/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 
 
 class DataTypeChoiceParam(ChoiceParam):
     DATA_TYPES: Mapping[str, tuple[type, Any, Type[SimpleParam]]] = {
         "string": (str, None, StringParam),
         "number": (float, None, FloatParam),
         "integer": (int, 0, IntegerParam),
-        "boolean": (bool, None, BooleanParam),
+        "boolean": (bool, False, BooleanParam),
     }
 
     def __init__(
         self, label: str, value: Optional[str] = None, choices: Optional[Iterable[str]] = None
     ):
         if not choices:
             choices = list(self.DATA_TYPES.keys())
```

### Comparing `countess-0.0.29/countess/core/pipeline.py` & `countess-0.0.30/countess/core/pipeline.py`

 * *Files 23% similar despite different names*

```diff
@@ -172,7 +172,54 @@
             node.prepare(logger)
             node.execute(logger)
 
     def reset(self):
         for node in self.nodes:
             node.result = None
             node.is_dirty = True
+
+    def tidy(self):
+        """Tidies the graph (sets all the node positions)"""
+
+        # XXX This is very arbitrary and not particularly efficient.
+        # Some kind of FDP-like algorithm might be nice.
+
+        nodes = list(self.traverse_nodes())
+
+        # first calculate a stratum for each node.
+
+        stratum = {}
+        for node in nodes:
+            if not node.parent_nodes:
+                stratum[node] = 0
+            else:
+                stratum[node] = max(stratum[n] for n in node.parent_nodes) + 1
+        for node in nodes[::-1]:
+            if node.child_nodes:
+                stratum[node] = min(stratum[n] for n in node.child_nodes) - 1
+        max_stratum = max(stratum.values())
+
+        position = {}
+        for s in range(0, max_stratum + 1):
+            y = (s + 0.5) / (max_stratum + 1)
+
+            # now sort all the nodes by the average position of their parents,
+            # to try and stop them forming a big tangle
+
+            snodes = [
+                (
+                    sum(position[p] for p in node.parent_nodes) / len(node.parent_nodes)
+                    if node.parent_nodes
+                    else 0.5,
+                    n,
+                )
+                for n, node in enumerate(nodes)
+                if stratum[node] == s
+            ]
+            snodes.sort()
+
+            # Assign node positions
+
+            for p, (_, n) in enumerate(snodes):
+                x = (p + 0.5) / len(snodes)
+                nodes[n].position = (y, x)
+                position[nodes[n]] = x
```

### Comparing `countess-0.0.29/countess/core/plugins.py` & `countess-0.0.30/countess/core/plugins.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess/gui/config.py` & `countess-0.0.30/countess/gui/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess/gui/logger.py` & `countess-0.0.30/countess/gui/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess/gui/main.py` & `countess-0.0.30/countess/gui/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -262,14 +262,15 @@
         ButtonMenu(
             tk_parent,
             [
                 ("New Config", self.config_new),
                 ("Load Config", self.config_load),
                 ("Save Config", self.config_save),
                 ("Export Config", self.config_export),
+                ("Tidy Graph", self.graph_tidy),
                 ("Run", self.program_run),
                 ("Exit", self.program_exit),
             ],
         )
 
         self.frame = tk.Frame(tk_parent)
         self.frame.grid(sticky=tk.NSEW)
@@ -336,14 +337,20 @@
             filename = filedialog.asksaveasfilename(
                 initialfile=initialfile, filetypes=[("Graphviz File", "*.dot")]
             )
         if not filename:
             return
         export_config_graphviz(self.graph, filename)
 
+    def graph_tidy(self):
+        self.graph.tidy()
+        # XXX there should be a self.graph_wrapper.refresh()
+        self.graph_wrapper.destroy()
+        self.graph_wrapper = GraphWrapper(self.canvas, self.graph, self.node_select)
+
     def program_run(self):
         # XXX should be handled in a different thread
         logger = ConsoleLogger()
         self.graph.run(logger)
 
     def program_exit(self):
         if not self.config_changed or messagebox.askokcancel(
```

### Comparing `countess-0.0.29/countess/gui/tabular.py` & `countess-0.0.30/countess/gui/tabular.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,18 @@
     else:
         return "%s"
 
 
 def format_value(value, column_format):
     if value is None or (type(value) is float and isnan(value)):
         return "—"
+    if value is True:
+        return "—T"
+    if value is False:
+        return "—F"
 
     # remove trailing 0's from floats (%g doesn't align correctly)
     try:
         if column_format.endswith("f"):
             return (column_format % value).rstrip("0")
         else:
             return column_format % value
@@ -61,14 +65,17 @@
     height = 1000
     length = 0
     select_rows = None
     labels: list[tk.Label] = []
     columns: list[tk.Text] = []
     column_formats: list[str] = []
     scrollbar = None
+    index_cols = 0
+    sort_by_col = None
+    sort_ascending = True
 
     def reset(self):
         if self.subframe:
             self.subframe.destroy()
         self.rowconfigure(0, weight=1)
         self.columnconfigure(0, weight=1)
         self.subframe = tk.Frame(self)
@@ -86,47 +93,51 @@
             # MultiIndex case
             column_names = list(self.dataframe.index.names) + list(self.dataframe.columns)
             column_dtypes = list(self.dataframe.index.dtypes) + list(self.dataframe.dtypes)
             index_frame = self.dataframe.index.to_frame()
             self.column_formats = [
                 column_format_for(index_frame[name]) for name in dataframe.index.names
             ] + [column_format_for(dataframe[name]) for name in dataframe.columns]
-            index_cols = len(self.dataframe.index.names)
+            self.index_cols = len(self.dataframe.index.names)
         elif self.dataframe.index.name:
             # a simple Index, with a name
             column_names = [self.dataframe.index.name] + list(self.dataframe.columns)
             column_dtypes = [self.dataframe.index.dtype] + list(self.dataframe.dtypes)
             self.column_formats = [column_format_for(dataframe.index)] + [
                 column_format_for(dataframe[name]) for name in dataframe.columns
             ]
-            index_cols = 1
+            self.index_cols = 1
         else:
             # if it doesn't have a name, don't bother displaying it
             # XXX it's probably just a RangeIndex, should we display it anyway?
             column_names = list(self.dataframe.columns)
             column_dtypes = list(self.dataframe.dtypes)
             self.column_formats = [column_format_for(dataframe[name]) for name in dataframe.columns]
-            index_cols = 0
+            self.index_cols = 0
 
         if len(column_names) == 0:
             label = tk.Label(self.subframe, text="Dataframe Preview\n\nno data")
             label.grid(row=0, column=0, sticky=tk.NSEW)
             return
 
         title = tk.Label(self.subframe, text=f"Dataframe Preview {len(self.dataframe)} rows")
         title.grid(row=0, column=0, columnspan=len(column_names), sticky=tk.NSEW, pady=5)
 
+        ### XXX add in proper handling for MultiIndexes here
+
         self.labels = []
         for num, (name, dtype) in enumerate(zip(column_names, column_dtypes)):
             if type(name) is tuple:
-                name = "\n".join(name)
-            is_index = " (index)" if num < index_cols else ""
+                name = "\n".join([str(n) for n in name])
+            else:
+                name = str(name)
+            is_index = " (index)" if num < self.index_cols else ""
             label = tk.Label(self.subframe, text=f"{name}\n{dtype}{is_index}")
             label.grid(row=1, column=num, sticky=tk.EW)
-            # label.bind("<Button-1>", partial(self.__label_button_1, num))
+            label.bind("<Button-1>", partial(self.__label_button_1, num))
             label.bind("<B1-Motion>", partial(self.__label_b1_motion, num))
             self.subframe.columnconfigure(num, minsize=10, weight=1)
             self.labels.append(label)
 
         if len(self.dataframe) == 0:
             label = tk.Label(self.subframe, text="no data")
             label.grid(row=2, column=0, columnspan=len(column_names), sticky=tk.NSEW)
@@ -214,14 +225,27 @@
         else:
             self.scrollbar.set(0, 1)
 
     def scrollto(self, new_offset):
         self.offset = min(max(int(new_offset), 0), self.length - self.height)
         self.refresh()
 
+    def __label_button_1(self, num, event):
+        label_width = self.labels[num].winfo_width()
+        if 2 * label_width / 5 < event.x < 3 * label_width / 5:
+            self.sort_ascending = (num != self.sort_by_col) or not self.sort_ascending
+            self.sort_by_col = num
+            if num < self.index_cols:
+                self.dataframe = self.dataframe.sort_index(level=num, ascending=self.sort_ascending)
+            else:
+                self.dataframe = self.dataframe.sort_values(
+                    self.dataframe.columns[num - self.index_cols], ascending=self.sort_ascending
+                )
+            self.refresh()
+
     def __label_b1_motion(self, num, event):
         # Detect label drags left and right.
         # XXX not quite right yet
         label = self.labels[num]
         label_width = label.winfo_width()
 
         if num < len(self.labels) - 1 and event.x > label_width:
```

### Comparing `countess-0.0.29/countess/gui/tree.py` & `countess-0.0.30/countess/gui/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,63 +158,68 @@
 
         self.widget1_bind = self.widget1.bind("<Configure>", self.update_line, add=True)
         self.widget2_bind = self.widget2.bind("<Configure>", self.update_line, add=True)
         self.canvas_bind = self.canvas.bind("<Configure>", self.update_line, add=True)
         self.update_line()
 
     def update_line(self, event=None):
+        _xc, _yc, wc, hc = _geometry(self.canvas)
+
+        # size factor to allow for different screen geometries.
+        k = (wc + hc) / 100
+
         x1, y1, w1, h1 = _geometry(self.widget1)
         x2, y2, w2, h2 = _geometry(self.widget2)
 
         # special case for dragging invisible frames
         # XXX bit of a hack just to get it to look nice
+        # based on the cursor size not `k`.
         if w2 == 1 and h2 == 1:
-            x2, y2, w2, h2 = x2 - 20, y2 - 20, 40, 40
+            x2, y2, w2, h2 = x2 - 16, y2 - 16, 32, 32
 
         # Control points set up a nice spline, and a little extra padding
         # on the destination end to allow for the arrow head.
-        _xc, _yc, wc, hc = _geometry(self.canvas)
-
         if wc > hc:
             if self.switch and x1 > x2:
                 x1, y1, w1, h1, x2, y2, w2, h2 = x2, y2, w2, h2, x1, y1, w1, h1
             coords = (
                 x1 + w1,
                 y1 + h1 // 2,
-                x1 + w1 + 20,
+                x1 + w1 + k,
                 y1 + h1 // 2,
-                x2 - 40,
+                x2 - k * 2,
                 y2 + h2 // 2,
                 x2,
                 y2 + h2 // 2,
             )
         else:
             if self.switch and y1 > y2:
                 x1, y1, w1, h1, x2, y2, w2, h2 = x2, y2, w2, h2, x1, y1, w1, h1
             coords = (
                 x1 + w1 // 2,
                 y1 + h1,
                 x1 + w1 // 2,
-                y1 + h1 + 20,
+                y1 + h1 + k,
                 x2 + w2 // 2,
-                y2 - 40,
+                y2 - k * 2,
                 x2 + w2 // 2,
                 y2,
             )
 
+        arrowshape = (15, 20, 6) if k > 20 else (k * 2 / 3, k, k / 3)
         if self.line:
             self.canvas.coords(self.line, *coords)
-            self.canvas.itemconfig(self.line, smooth=len(coords) > 6)
+            self.canvas.itemconfig(self.line, smooth=True, arrowshape=arrowshape)
         else:
             self.line = self.canvas.create_line(
                 *coords,
                 smooth=True,
                 width=3,
                 arrow="last",
-                arrowshape=(15, 15, 6),
+                arrowshape=arrowshape,
                 fill=self.color,
             )
 
     def destroy(self):
         self.canvas.delete(self.line)
         self.canvas.unbind("<Configure>", self.canvas_bind)
         self.widget1.unbind("<Configure>", self.widget1_bind)
```

### Comparing `countess-0.0.29/countess/plugins/csv.py` & `countess-0.0.30/countess/plugins/csv.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess/plugins/data_table.py` & `countess-0.0.30/countess/plugins/data_table.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess/plugins/expression.py` & `countess-0.0.30/countess/plugins/expression.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
-from countess.core.parameters import TextParam
+from countess.core.parameters import ArrayParam, BooleanParam, PerColumnArrayParam, TextParam
 from countess.core.plugins import PandasTransformPlugin
 
 
 def process(df: pd.DataFrame, codes, logger: Logger):
     for code in codes:
         if not code:
             continue
@@ -29,15 +29,26 @@
 
 
 class ExpressionPlugin(PandasTransformPlugin):
     name = "Expression"
     description = "Apply simple expressions"
     version = VERSION
 
-    parameters = {"code": TextParam("Expressions")}
+    parameters = {
+        "code": TextParam("Expressions"),
+        "drop": PerColumnArrayParam("Drop Columns", BooleanParam("Drop")),
+    }
 
     def run_df(self, df, logger: Logger) -> pd.DataFrame:
         assert isinstance(self.parameters["code"], TextParam)
+        assert isinstance(self.parameters["drop"], ArrayParam)
 
         codes = [c.replace("\n", " ").strip() for c in self.parameters["code"].value.split("\n\n")]
 
-        return process(df, codes, logger)
+        df = process(df, codes, logger)
+
+        drop_columns = [
+            col for col, param in zip(self.input_columns, self.parameters["drop"]) if param.value
+        ]
+
+        print(drop_columns)
+        return df.drop(columns=drop_columns)
```

### Comparing `countess-0.0.29/countess/plugins/fastq.py` & `countess-0.0.30/countess/plugins/fastq.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess/plugins/group_by.py` & `countess-0.0.30/countess/plugins/group_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             )
             for col, col_param in column_parameters
             if any(pp.value for k, pp in col_param.params.items() if k != "index")
         )
 
         try:
             if agg_ops:
-                dfo = df.groupby(index_cols or df.index).agg(agg_ops)
+                dfo = df.reset_index().groupby(index_cols or df.index).agg(agg_ops)
                 dfo.columns = [_column_renamer(col) for col in dfo.columns.values]  # type: ignore
             else:
                 # defaults to just a 'count' column.
                 dfo = df.assign(count=1).groupby(index_cols or df.index).count()
         except ValueError as exc:
             logger.exception(exc)
             return pd.DataFrame()
```

### Comparing `countess-0.0.29/countess/plugins/hdf5.py` & `countess-0.0.30/countess/plugins/hdf5.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess/plugins/join.py` & `countess-0.0.30/countess/plugins/join.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,15 +43,21 @@
             raise NotImplementedError("Only two-way joins supported right now")
         if not all((isinstance(df, pd.DataFrame) for _, df in data_items)):
             raise NotImplementedError("Feed me dataframes")
 
         enumerate_inputs = enumerate(zip(inputs_param, data.items()))
         for number, (input_param, (source_name, source_ddf)) in enumerate_inputs:
             input_param.label = f"Input {number+1}: {source_name}"
-            input_param["join_on"].choices = [INDEX] + list(source_ddf.columns)
+            if hasattr(source_ddf.index, "names"):
+                input_columns = [n for n in source_ddf.index.names if n] + list(source_ddf.columns)
+            elif source_ddf.index.name:
+                input_columns = [source_ddf.index.name] + list(source_ddf.columns)
+            else:
+                input_columns = list(source_ddf.columns)
+            input_param["join_on"].choices = [INDEX] + input_columns
 
     def run(
         self,
         data,
         logger: Logger,
         row_limit: Optional[int] = None,
     ):
@@ -79,17 +85,15 @@
         }
 
         dfs = list(data.values())
 
         if not ip1.join_on.value or ip1.join_on.value == INDEX:
             join_params["left_index"] = True
         else:
-            dfs[0] = dfs[0].reset_index(drop=True)
             join_params["left_on"] = ip1.join_on.value
 
         if not ip2.join_on.value or ip2.join_on.value == INDEX:
             join_params["right_index"] = True
         else:
-            dfs[1] = dfs[1].reset_index(drop=True)
             join_params["right_on"] = ip2["join_on"].value
 
         return dfs[0].merge(dfs[1], **join_params)
```

### Comparing `countess-0.0.29/countess/plugins/mutagenize.py` & `countess-0.0.30/countess/plugins/mutagenize.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess/plugins/python.py` & `countess-0.0.30/countess/plugins/python.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess/plugins/regex.py` & `countess-0.0.30/countess/plugins/regex.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,44 +11,14 @@
     IntegerParam,
     MultiParam,
     StringParam,
 )
 from countess.core.plugins import PandasInputPlugin, PandasTransformPlugin
 
 
-def _process_row(value: str, compiled_re, output_params, logger) -> pd.Series:
-    match = compiled_re.match(value)
-    if match:
-        return pd.Series(
-            dict(
-                (output_params[n]["name"].value, output_params[n].datatype.cast_value(g))
-                for n, g in enumerate(match.groups())
-            )
-        )
-    else:
-        logger.warning("Didn't Match", detail=repr(value))
-        return pd.Series({})
-
-
-def _process_row_multi(value: str, compiled_re, output_params, logger) -> pd.Series:
-    matches = compiled_re.findall(value)
-    if len(matches) == 0:
-        return pd.Series({})
-    if compiled_re.groups > 1:
-        return pd.Series(
-            dict(
-                (op["name"].value, [op.datatype.cast_value(match[num]) for match in matches])
-                for num, op in enumerate(output_params)
-            )
-        )
-    else:
-        op = output_params[0]
-        return pd.Series({op["name"].value: [op.datatype.cast_value(match) for match in matches]})
-
-
 class RegexToolPlugin(PandasTransformPlugin):
     name = "Regex Tool"
     description = "Apply regular expressions to a column to make new column(s)"
     link = "https://countess-project.github.io/CountESS/plugins/#regex-tool"
     version = VERSION
 
     parameters = {
@@ -60,14 +30,15 @@
                 "Col",
                 {
                     "name": StringParam("Column Name"),
                     "datatype": DataTypeChoiceParam(
                         "Column Type",
                         "string",
                     ),
+                    "index": BooleanParam("Index?"),
                 },
             ),
         ),
         "multi": BooleanParam("Multi Match", False),
         "drop_column": BooleanParam("Drop Column", False),
         "drop_unmatch": BooleanParam("Drop Unmatched Rows", False),
     }
@@ -76,36 +47,62 @@
         compiled_re = re.compile(self.parameters["regex"].value)
 
         while compiled_re.groups > len(self.parameters["output"].params):
             self.parameters["output"].add_row()
 
         output_params = self.parameters["output"].params
         output_names = [pp["name"].value for pp in output_params]
+        index_names = [pp["name"].value for pp in output_params if pp["index"].value]
 
         column = self.parameters["column"].get_column(df)
 
         if self.parameters["multi"].value:
-            func = _process_row_multi
+
+            def func(value):
+                matches = compiled_re.findall(str(value))
+                if matches:
+                    return [[m[n] for m in matches] for n in range(0, compiled_re.groups)]
+                else:
+                    return [[None]] * compiled_re.groups
+
         else:
-            func = _process_row
 
-        df = df.join(column.apply(func, args=(compiled_re, output_params, logger)))
+            def func(value):
+                if match := compiled_re.match(value):
+                    return [
+                        op.datatype.cast_value(g) for op, g in zip(output_params, match.groups())
+                    ]
+                else:
+                    logger.info("Didn't Match: " + repr(value))
+                    return [None] * compiled_re.groups
 
-        if self.parameters["drop_unmatch"].value:
-            df = df.dropna(subset=output_names)
+        # make a series of tuples, then turn those back into a dataframe,
+        # then copy those new columns over.
+        # XXX this isn't particularly elegant but it does seem to be fairly quick
+        # XXX should be a special case for a single output column
+
+        series = column.apply(func)
+        output_df = pd.DataFrame(series.tolist(), columns=output_names, index=series.index)
+        df = df.assign(**{column_name: output_df[column_name] for column_name in output_names})
 
         if self.parameters["multi"].value:
             df = df.explode(output_names)
 
+        if self.parameters["drop_unmatch"].value:
+            df = df.dropna(subset=output_names, how="all")
+
         if self.parameters["drop_column"].value:
             column_name = self.parameters["column"].value
             if column_name not in df.columns:
                 df = df.reset_index()
             df = df.drop(columns=column_name)
 
+        if index_names:
+            df = df.set_index(index_names)
+
         return df
 
 
 class RegexReaderPlugin(PandasInputPlugin):
     name = "Regex Reader"
     description = """Loads arbitrary data from line-delimited files, applying a regular expression
       to each line to extract fields.  If you're trying to read generic CSV or TSV files, use the CSV
@@ -173,11 +170,12 @@
                         pd.DataFrame.from_records(records, columns=columns, index=index_columns)
                     )
                     records = []
 
         if len(records) > 0:
             pdfs.append(pd.DataFrame.from_records(records, columns=columns, index=index_columns))
 
-        if len(pdfs) > 0:
-            return pd.concat(pdfs)
+        if len(pdfs) == 0:
+            return pd.DataFrame([], columns=columns)
 
-        return pd.DataFrame([], columns=columns)
+        df = pd.concat(pdfs)
+        return df
```

### Comparing `countess-0.0.29/countess/plugins/sequence.py` & `countess-0.0.30/countess/plugins/sequence.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess/plugins/variant.py` & `countess-0.0.30/countess/plugins/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess/utils/variant.py` & `countess-0.0.30/countess/utils/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess.egg-info/PKG-INFO` & `countess-0.0.30/countess.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.29
+Version: 0.0.30
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -12,15 +12,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.29
+# CountESS 0.0.30
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.29/countess.egg-info/SOURCES.txt` & `countess-0.0.30/countess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/countess.egg-info/entry_points.txt` & `countess-0.0.30/countess.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.29/pyproject.toml` & `countess-0.0.30/pyproject.toml`

 * *Files identical despite different names*

