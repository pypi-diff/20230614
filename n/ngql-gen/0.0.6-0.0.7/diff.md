# Comparing `tmp/ngql_gen-0.0.6.tar.gz` & `tmp/ngql_gen-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngql_gen-0.0.6.tar", last modified: Sat Jun 10 07:54:56 2023, max compression
+gzip compressed data, was "ngql_gen-0.0.7.tar", last modified: Wed Jun 14 02:33:48 2023, max compression
```

## Comparing `ngql_gen-0.0.6.tar` & `ngql_gen-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 07:54:56.993489 ngql_gen-0.0.6/
--rw-rw-rw-   0        0        0     9229 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/LICENSE
--rw-rw-rw-   0        0        0    10214 2023-06-10 07:54:56.991985 ngql_gen-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      103 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 07:54:56.951796 ngql_gen-0.0.6/ngql_gen/
--rw-rw-rw-   0        0        0        0 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/ngql_gen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:54:56.971835 ngql_gen-0.0.6/ngql_gen/config/
--rw-rw-rw-   0        0        0       21 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/ngql_gen/config/__init__.py
--rw-rw-rw-   0        0        0      719 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/ngql_gen/config/config.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:54:56.988979 ngql_gen-0.0.6/ngql_gen/generator/
--rw-rw-rw-   0        0        0      155 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/ngql_gen/generator/__init__.py
--rw-rw-rw-   0        0        0      641 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/ngql_gen/generator/edge.py
--rw-rw-rw-   0        0        0      769 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/ngql_gen/generator/edge_type.py
--rw-rw-rw-   0        0        0     2475 2023-06-10 07:52:05.000000 ngql_gen-0.0.6/ngql_gen/generator/select.py
--rw-rw-rw-   0        0        0     1178 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/ngql_gen/generator/space.py
--rw-rw-rw-   0        0        0      883 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/ngql_gen/generator/tag.py
--rw-rw-rw-   0        0        0     3691 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/ngql_gen/generator/utils.py
--rw-rw-rw-   0        0        0      504 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/ngql_gen/generator/vertex.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:54:56.991985 ngql_gen-0.0.6/ngql_gen/model/
--rw-rw-rw-   0        0        0       44 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/ngql_gen/model/__init__.py
--rw-rw-rw-   0        0        0      163 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/ngql_gen/model/edge_type.py
--rw-rw-rw-   0        0        0      158 2023-06-10 07:45:14.000000 ngql_gen-0.0.6/ngql_gen/model/tag.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:54:56.969834 ngql_gen-0.0.6/ngql_gen.egg-info/
--rw-rw-rw-   0        0        0    10214 2023-06-10 07:54:56.000000 ngql_gen-0.0.6/ngql_gen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      573 2023-06-10 07:54:56.000000 ngql_gen-0.0.6/ngql_gen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 07:54:56.000000 ngql_gen-0.0.6/ngql_gen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-10 07:54:56.000000 ngql_gen-0.0.6/ngql_gen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-10 07:54:56.000000 ngql_gen-0.0.6/ngql_gen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      491 2023-06-10 07:52:31.000000 ngql_gen-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 07:54:56.993489 ngql_gen-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 02:33:48.097355 ngql_gen-0.0.7/
+-rw-rw-rw-   0        0        0     9229 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0    10214 2023-06-14 02:33:48.097355 ngql_gen-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 02:33:48.062352 ngql_gen-0.0.7/ngql_gen/
+-rw-rw-rw-   0        0        0        0 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:33:48.079352 ngql_gen-0.0.7/ngql_gen/config/
+-rw-rw-rw-   0        0        0       21 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/config/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/config/config.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:33:48.093355 ngql_gen-0.0.7/ngql_gen/generator/
+-rw-rw-rw-   0        0        0      155 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/__init__.py
+-rw-rw-rw-   0        0        0      641 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/edge.py
+-rw-rw-rw-   0        0        0      769 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/edge_type.py
+-rw-rw-rw-   0        0        0     3405 2023-06-14 02:32:50.000000 ngql_gen-0.0.7/ngql_gen/generator/select.py
+-rw-rw-rw-   0        0        0     1178 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/space.py
+-rw-rw-rw-   0        0        0      883 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/tag.py
+-rw-rw-rw-   0        0        0     3691 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/utils.py
+-rw-rw-rw-   0        0        0      504 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/vertex.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:33:48.096356 ngql_gen-0.0.7/ngql_gen/model/
+-rw-rw-rw-   0        0        0       44 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/model/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/model/edge_type.py
+-rw-rw-rw-   0        0        0      158 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/model/tag.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:33:48.077351 ngql_gen-0.0.7/ngql_gen.egg-info/
+-rw-rw-rw-   0        0        0    10214 2023-06-14 02:33:48.000000 ngql_gen-0.0.7/ngql_gen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2023-06-14 02:33:48.000000 ngql_gen-0.0.7/ngql_gen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 02:33:48.000000 ngql_gen-0.0.7/ngql_gen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-14 02:33:48.000000 ngql_gen-0.0.7/ngql_gen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 02:33:48.000000 ngql_gen-0.0.7/ngql_gen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      491 2023-06-14 02:33:01.000000 ngql_gen-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 02:33:48.097355 ngql_gen-0.0.7/setup.cfg
```

### Comparing `ngql_gen-0.0.6/LICENSE` & `ngql_gen-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.6/PKG-INFO` & `ngql_gen-0.0.7/ngql_gen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ngql_gen
-Version: 0.0.6
+Name: ngql-gen
+Version: 0.0.7
 Summary: Nebula Graph Query Language Generator
 Author-email: 东南dnf <zjy2414@outlook.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ngql_gen-0.0.6/ngql_gen/config/config.py` & `ngql_gen-0.0.7/ngql_gen/config/config.py`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.6/ngql_gen/generator/edge.py` & `ngql_gen-0.0.7/ngql_gen/generator/edge.py`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.6/ngql_gen/generator/edge_type.py` & `ngql_gen-0.0.7/ngql_gen/generator/edge_type.py`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.6/ngql_gen/generator/select.py` & `ngql_gen-0.0.7/ngql_gen/generator/select.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,19 +37,33 @@
     def GetConnectedVertexs(obj:object, prop_name: str,prop_value: str):
         v1 = config['default_v1_name']
         v2 = config['default_v2_name']
 
         return f"MATCH ({v1}: {obj.__class__.__name__}{{{prop_name}: '{prop_value}'}})--({v2}) RETURN {v2};"
     
     # 通过一个点获取所有与之相连的点，限定边的类型
-    def GetConnectedVertexsWidthEdgeType(v1_obj: object, prop_name: str,prop_value: str, edge_obj: object = None, v2_obj: object = None):
+    def GetConnectedVertexsWithEdgeType(v1_obj: object, prop_name: str,prop_value: str, edge_obj: object = None, v2_obj: object = None):
         v1 = config['default_v1_name']
         v2 = config['default_v2_name']
 
         if edge_obj is None and v2_obj is None:
             return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})--({v2}) RETURN {v2};"
         elif edge_obj is None:
             return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})--({v2}: {v2_obj.__name__}) RETURN {v2};"
         elif v2_obj is None:
             return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})-[e: {edge_obj.__name__}]-({v2}) RETURN {v2};"
         else:
-            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})-[e: {edge_obj.__name__}]-({v2}: {v2_obj.__name__}) RETURN {v2};"
+            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})-[e: {edge_obj.__name__}]-({v2}: {v2_obj.__name__}) RETURN {v2};"
+        
+        # 通过一个点获取所有与之相连的点的连接边
+    def GetConnectedEdgesWithEdgeType(v1_obj: object, prop_name: str,prop_value: str, edge_obj: object = None, v2_obj: object = None):
+        v1 = config['default_v1_name']
+        v2 = config['default_v2_name']
+
+        if edge_obj is None and v2_obj is None:
+            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})--({v2}) RETURN {e};"
+        elif edge_obj is None:
+            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})--({v2}: {v2_obj.__name__}) RETURN {e};"
+        elif v2_obj is None:
+            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})-[e: {edge_obj.__name__}]-({v2}) RETURN {e};"
+        else:
+            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})-[e: {edge_obj.__name__}]-({v2}: {v2_obj.__name__}) RETURN e;"
```

### Comparing `ngql_gen-0.0.6/ngql_gen/generator/space.py` & `ngql_gen-0.0.7/ngql_gen/generator/space.py`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.6/ngql_gen/generator/tag.py` & `ngql_gen-0.0.7/ngql_gen/generator/tag.py`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.6/ngql_gen/generator/utils.py` & `ngql_gen-0.0.7/ngql_gen/generator/utils.py`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.6/ngql_gen.egg-info/PKG-INFO` & `ngql_gen-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ngql-gen
-Version: 0.0.6
+Name: ngql_gen
+Version: 0.0.7
 Summary: Nebula Graph Query Language Generator
 Author-email: 东南dnf <zjy2414@outlook.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ngql_gen-0.0.6/ngql_gen.egg-info/SOURCES.txt` & `ngql_gen-0.0.7/ngql_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

