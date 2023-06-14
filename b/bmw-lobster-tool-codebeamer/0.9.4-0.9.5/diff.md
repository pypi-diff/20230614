# Comparing `tmp/bmw-lobster-tool-codebeamer-0.9.4.tar.gz` & `tmp/bmw-lobster-tool-codebeamer-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-codebeamer-0.9.4.tar", last modified: Tue Jun 13 09:18:56 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-codebeamer-0.9.5.tar", last modified: Wed Jun 14 14:03:19 2023, max compression
```

## Comparing `bmw-lobster-tool-codebeamer-0.9.4.tar` & `bmw-lobster-tool-codebeamer-0.9.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.841244 bmw-lobster-tool-codebeamer-0.9.4/
--rw-r--r--   0 florian   (1000) florian   (1000)     1756 2023-06-13 09:18:56.841244 bmw-lobster-tool-codebeamer-0.9.4/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      816 2023-06-13 09:17:37.000000 bmw-lobster-tool-codebeamer-0.9.4/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.841244 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     1756 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      402 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       80 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       39 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.837244 bmw-lobster-tool-codebeamer-0.9.4/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.837244 bmw-lobster-tool-codebeamer-0.9.4/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.841244 bmw-lobster-tool-codebeamer-0.9.4/lobster/tools/codebeamer/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/lobster/tools/codebeamer/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     9495 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/lobster/tools/codebeamer/codebeamer.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-13 09:18:56.841244 bmw-lobster-tool-codebeamer-0.9.4/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2296 2023-05-08 15:03:18.000000 bmw-lobster-tool-codebeamer-0.9.4/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1241 2023-06-14 14:03:10.000000 bmw-lobster-tool-codebeamer-0.9.5/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      402 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       80 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       39 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/lobster/tools/codebeamer/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/lobster/tools/codebeamer/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     9763 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/lobster/tools/codebeamer/codebeamer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2296 2023-05-08 15:03:18.000000 bmw-lobster-tool-codebeamer-0.9.5/setup.py
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.4/PKG-INFO` & `bmw-lobster-tool-codebeamer-0.9.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-codebeamer
-Version: 0.9.4
+Version: 0.9.5
 Summary: LOBSTER Tool for Codebeamer
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
@@ -29,14 +29,29 @@
 requirements management tool
 [Codebeamer](https://intland.com/codebeamer).
 
 ## Tools
 
 * `lobster-codebeamer`: Extrat requirements from codebeamer.
 
+## Usage
+
+There are two ways you can use this tool:
+
+* Download all requirements mentioned by another lobster trace (this
+  way you do not get a completeness check) (using `--import-tagged`)
+
+* Download all requirements generated by a saved codebeamer query
+  (using `--import-query`)
+
+## Limitations
+
+The key limitation is item text, which is currently not
+imported. However we do plan to also import item text eventually.
+
 ## Copyright & License information
 
 The copyright holder of LOBSTER is the Bayerische Motoren Werke
 Aktiengesellschaft (BMW AG), and LOBSTER is published under the [GNU
 Affero General Public License, Version 3](../LICENSE.md).
 
 This tool has no actual dependency on, or with, Codebeamer. It just
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.4/README.md` & `bmw-lobster-tool-codebeamer-0.9.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,29 @@
 requirements management tool
 [Codebeamer](https://intland.com/codebeamer).
 
 ## Tools
 
 * `lobster-codebeamer`: Extrat requirements from codebeamer.
 
+## Usage
+
+There are two ways you can use this tool:
+
+* Download all requirements mentioned by another lobster trace (this
+  way you do not get a completeness check) (using `--import-tagged`)
+
+* Download all requirements generated by a saved codebeamer query
+  (using `--import-query`)
+
+## Limitations
+
+The key limitation is item text, which is currently not
+imported. However we do plan to also import item text eventually.
+
 ## Copyright & License information
 
 The copyright holder of LOBSTER is the Bayerische Motoren Werke
 Aktiengesellschaft (BMW AG), and LOBSTER is published under the [GNU
 Affero General Public License, Version 3](../LICENSE.md).
 
 This tool has no actual dependency on, or with, Codebeamer. It just
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO` & `bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-codebeamer
-Version: 0.9.4
+Version: 0.9.5
 Summary: LOBSTER Tool for Codebeamer
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
@@ -29,14 +29,29 @@
 requirements management tool
 [Codebeamer](https://intland.com/codebeamer).
 
 ## Tools
 
 * `lobster-codebeamer`: Extrat requirements from codebeamer.
 
+## Usage
+
+There are two ways you can use this tool:
+
+* Download all requirements mentioned by another lobster trace (this
+  way you do not get a completeness check) (using `--import-tagged`)
+
+* Download all requirements generated by a saved codebeamer query
+  (using `--import-query`)
+
+## Limitations
+
+The key limitation is item text, which is currently not
+imported. However we do plan to also import item text eventually.
+
 ## Copyright & License information
 
 The copyright holder of LOBSTER is the Bayerische Motoren Werke
 Aktiengesellschaft (BMW AG), and LOBSTER is published under the [GNU
 Affero General Public License, Version 3](../LICENSE.md).
 
 This tool has no actual dependency on, or with, Codebeamer. It just
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.4/lobster/tools/codebeamer/codebeamer.py` & `bmw-lobster-tool-codebeamer-0.9.5/lobster/tools/codebeamer/codebeamer.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,22 +105,29 @@
     assert isinstance(query_id, int)
     rv = []
     page_id = 1
     total_items = None
 
     while total_items is None or len(rv) < total_items:
         print("Fetching page %u of query..." % page_id)
-        data = query_cb_single(cb_config,
-                               "%s/query/%u/page/%u?pagesize=100" %
-                               (cb_config["base"],
-                                query_id,
-                                page_id))
+        url = "%s/query/%u/page/%u?pagesize=100" % \
+            (cb_config["base"],
+             query_id,
+             page_id)
+        data = query_cb_single(cb_config, url)
         assert len(data) == 1
         data = data["trackerItems"]
 
+        if page_id == 1 and len(data["items"]) == 0:
+            print("This query doesn't generate items. Please check:")
+            print(" * is the number actually correct?")
+            print(" * do you have permissions to access it?")
+            print("You can try to access %s manually to check" % url)
+            sys.exit(1)
+
         assert page_id == data["page"]
         if page_id == 1:
             total_items = data["total"]
         else:
             assert total_items == data["total"]
 
         rv += [to_lobster(cb_config, cb_item)
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.4/setup.py` & `bmw-lobster-tool-codebeamer-0.9.5/setup.py`

 * *Files identical despite different names*

