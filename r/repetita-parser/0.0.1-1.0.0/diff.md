# Comparing `tmp/repetita_parser-0.0.1.tar.gz` & `tmp/repetita_parser-1.0.0.tar.gz`

## Comparing `repetita_parser-0.0.1.tar` & `repetita_parser-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/src/repetita_parser/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/src/repetita_parser/__init__.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/src/repetita_parser/demands.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/src/repetita_parser/errors.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/src/repetita_parser/instance.py
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/src/repetita_parser/topology.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/paths.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/test_demands.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/test_errors.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/test_instance.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/test_topology.py
--rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/data/DeutscheTelekom.0000.demands
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/data/DeutscheTelekom.graph
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/data/bad/bad_edge_fields.graph
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/data/bad/bad_edge_header.graph
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/data/bad/bad_edge_memo.graph
--rw-r--r--   0        0        0    18701 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/data/bad/bad_fields.demands
--rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/data/bad/bad_header.demands
--rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/data/bad/bad_memo.demands
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/data/bad/bad_node_fields.graph
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/data/bad/bad_node_header.graph
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/tests/data/bad/bad_node_memo.graph
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/LICENSE
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/README.md
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 repetita_parser-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/src/repetita_parser/__init__.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/src/repetita_parser/demands.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/src/repetita_parser/errors.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/src/repetita_parser/instance.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/src/repetita_parser/topology.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/paths.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/test_demands.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/test_errors.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/test_instance.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/test_topology.py
+-rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/data/DeutscheTelekom.0000.demands
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/data/DeutscheTelekom.graph
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/data/bad/bad_edge_fields.graph
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/data/bad/bad_edge_header.graph
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/data/bad/bad_edge_memo.graph
+-rw-r--r--   0        0        0    18701 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/data/bad/bad_fields.demands
+-rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/data/bad/bad_header.demands
+-rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/data/bad/bad_memo.demands
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/data/bad/bad_node_fields.graph
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/data/bad/bad_node_header.graph
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/tests/data/bad/bad_node_memo.graph
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/LICENSE
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/README.md
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 repetita_parser-1.0.0/PKG-INFO
```

### Comparing `repetita_parser-0.0.1/src/repetita_parser/demands.py` & `repetita_parser-1.0.0/src/repetita_parser/demands.py`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/src/repetita_parser/errors.py` & `repetita_parser-1.0.0/src/repetita_parser/errors.py`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/src/repetita_parser/instance.py` & `repetita_parser-1.0.0/src/repetita_parser/instance.py`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/src/repetita_parser/topology.py` & `repetita_parser-1.0.0/src/repetita_parser/topology.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 class Topology:
     def __init__(self, nodes: List[Node], edges: List[Edge]) -> None:
         self.nodes: List[Node] = nodes
         self.edges: List[Edge] = edges
 
-    def as_nx_graph(self) -> nx.MultiDiGraph:  # pyright: ignore [reportUnboundVariable]
+    def as_nx_graph(self):
         """
         Convert the topology to a `networkx.MultiDiGraph`. In the graph, nodes
         are represented by their index into `self.nodes`. Node and edge objects
         carry their respective `Node` and `Edge` objects in their attributes
         under the `obj` key.
 
         This function requires NetworkX to be installed. If you call this
```

### Comparing `repetita_parser-0.0.1/tests/test_demands.py` & `repetita_parser-1.0.0/tests/test_demands.py`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/tests/test_topology.py` & `repetita_parser-1.0.0/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/tests/data/DeutscheTelekom.0000.demands` & `repetita_parser-1.0.0/tests/data/DeutscheTelekom.0000.demands`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/tests/data/DeutscheTelekom.graph` & `repetita_parser-1.0.0/tests/data/DeutscheTelekom.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/tests/data/bad/bad_edge_fields.graph` & `repetita_parser-1.0.0/tests/data/bad/bad_edge_fields.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/tests/data/bad/bad_edge_header.graph` & `repetita_parser-1.0.0/tests/data/bad/bad_edge_header.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/tests/data/bad/bad_edge_memo.graph` & `repetita_parser-1.0.0/tests/data/bad/bad_edge_memo.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/tests/data/bad/bad_fields.demands` & `repetita_parser-1.0.0/tests/data/bad/bad_fields.demands`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/tests/data/bad/bad_header.demands` & `repetita_parser-1.0.0/tests/data/bad/bad_header.demands`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/tests/data/bad/bad_memo.demands` & `repetita_parser-1.0.0/tests/data/bad/bad_memo.demands`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/tests/data/bad/bad_node_fields.graph` & `repetita_parser-1.0.0/tests/data/bad/bad_node_fields.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/tests/data/bad/bad_node_header.graph` & `repetita_parser-1.0.0/tests/data/bad/bad_node_header.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/tests/data/bad/bad_node_memo.graph` & `repetita_parser-1.0.0/tests/data/bad/bad_node_memo.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/.gitignore` & `repetita_parser-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/LICENSE` & `repetita_parser-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/README.md` & `repetita_parser-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `repetita_parser-0.0.1/pyproject.toml` & `repetita_parser-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "repetita-parser"
-dynamic = ["version"]
+version = "1.0.0"
 description = "A parser for the REPETITA format"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 authors = [
   { name="Leon Richardt", email="pip@leon.dev" },
 ]
@@ -34,17 +34,14 @@
 Source = "https://github.com/leon-richardt/repetita-parser"
 
 [tool.hatch.build]
 exclude = [
     "examples"
 ]
 
-[tool.hatch.version]
-path = "src/repetita_parser/__about__.py"
-
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
 ]
 features = ["networkx"]
```

### Comparing `repetita_parser-0.0.1/PKG-INFO` & `repetita_parser-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repetita-parser
-Version: 0.0.1
+Version: 1.0.0
 Summary: A parser for the REPETITA format
 Project-URL: Documentation, https://github.com/leon-richardt/repetita-parser#readme
 Project-URL: Issues, https://github.com/leon-richardt/repetita-parser/issues
 Project-URL: Source, https://github.com/leon-richardt/repetita-parser
 Author-email: Leon Richardt <pip@leon.dev>
 License-Expression: MIT
 License-File: LICENSE
```

