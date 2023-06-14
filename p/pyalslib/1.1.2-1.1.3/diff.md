# Comparing `tmp/pyalslib-1.1.2.tar.gz` & `tmp/pyalslib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalslib-1.1.2.tar", last modified: Tue Jun 13 18:06:36 2023, max compression
+gzip compressed data, was "pyalslib-1.1.3.tar", last modified: Wed Jun 14 05:39:20 2023, max compression
```

## Comparing `pyalslib-1.1.2.tar` & `pyalslib-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-13 18:06:36.638049 pyalslib-1.1.2/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    35149 2023-06-13 17:51:00.000000 pyalslib-1.1.2/LICENSE
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-06-13 18:06:36.637049 pyalslib-1.1.2/PKG-INFO
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1186 2023-06-13 17:51:00.000000 pyalslib-1.1.2/README.md
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-13 18:06:36.637049 pyalslib-1.1.2/pyalslib/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     5995 2023-06-13 17:51:00.000000 pyalslib-1.1.2/pyalslib/ALSCatalog.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     7265 2023-06-13 17:51:00.000000 pyalslib-1.1.2/pyalslib/ALSCatalogCache.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    16896 2023-06-13 17:51:00.000000 pyalslib-1.1.2/pyalslib/ALSGraph.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1859 2023-06-13 17:51:00.000000 pyalslib-1.1.2/pyalslib/ALSRewriter.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    17375 2023-06-13 17:51:00.000000 pyalslib-1.1.2/pyalslib/ALSSMT.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2117 2023-06-13 17:51:00.000000 pyalslib-1.1.2/pyalslib/Utility.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    11381 2023-06-13 18:06:04.000000 pyalslib-1.1.2/pyalslib/YosysHelper.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      405 2023-06-13 18:06:11.000000 pyalslib-1.1.2/pyalslib/__init__.py
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-13 18:06:36.637049 pyalslib-1.1.2/pyalslib.egg-info/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-06-13 18:06:36.000000 pyalslib-1.1.2/pyalslib.egg-info/PKG-INFO
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      365 2023-06-13 18:06:36.000000 pyalslib-1.1.2/pyalslib.egg-info/SOURCES.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)        1 2023-06-13 18:06:36.000000 pyalslib-1.1.2/pyalslib.egg-info/dependency_links.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)       49 2023-06-13 18:06:36.000000 pyalslib-1.1.2/pyalslib.egg-info/requires.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)        9 2023-06-13 18:06:36.000000 pyalslib-1.1.2/pyalslib.egg-info/top_level.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)       38 2023-06-13 18:06:36.638049 pyalslib-1.1.2/setup.cfg
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1735 2023-06-13 18:06:20.000000 pyalslib-1.1.2/setup.py
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-14 05:39:20.688910 pyalslib-1.1.3/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    35149 2023-06-13 17:51:00.000000 pyalslib-1.1.3/LICENSE
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-06-14 05:39:20.687910 pyalslib-1.1.3/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1186 2023-06-13 17:51:00.000000 pyalslib-1.1.3/README.md
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-14 05:39:20.686910 pyalslib-1.1.3/pyalslib/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     5995 2023-06-13 17:51:00.000000 pyalslib-1.1.3/pyalslib/ALSCatalog.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     7265 2023-06-13 17:51:00.000000 pyalslib-1.1.3/pyalslib/ALSCatalogCache.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    17129 2023-06-14 05:38:51.000000 pyalslib-1.1.3/pyalslib/ALSGraph.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1859 2023-06-13 17:51:00.000000 pyalslib-1.1.3/pyalslib/ALSRewriter.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    17375 2023-06-13 17:51:00.000000 pyalslib-1.1.3/pyalslib/ALSSMT.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2117 2023-06-13 17:51:00.000000 pyalslib-1.1.3/pyalslib/Utility.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    11381 2023-06-13 18:06:04.000000 pyalslib-1.1.3/pyalslib/YosysHelper.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      405 2023-06-14 05:39:07.000000 pyalslib-1.1.3/pyalslib/__init__.py
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-14 05:39:20.687910 pyalslib-1.1.3/pyalslib.egg-info/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-06-14 05:39:20.000000 pyalslib-1.1.3/pyalslib.egg-info/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      365 2023-06-14 05:39:20.000000 pyalslib-1.1.3/pyalslib.egg-info/SOURCES.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)        1 2023-06-14 05:39:20.000000 pyalslib-1.1.3/pyalslib.egg-info/dependency_links.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)       49 2023-06-14 05:39:20.000000 pyalslib-1.1.3/pyalslib.egg-info/requires.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)        9 2023-06-14 05:39:20.000000 pyalslib-1.1.3/pyalslib.egg-info/top_level.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)       38 2023-06-14 05:39:20.688910 pyalslib-1.1.3/setup.cfg
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1735 2023-06-14 05:39:03.000000 pyalslib-1.1.3/setup.py
```

### Comparing `pyalslib-1.1.2/LICENSE` & `pyalslib-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.2/PKG-INFO` & `pyalslib-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalslib
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
 Home-page: https://github.com/SalvatoreBarone/pyALSlib
 Author: Salvatore Barone
 Author-email: salvatore.barone@unina.it
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/pyALSlib/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/pyALSlib
 Keywords: Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
```

### Comparing `pyalslib-1.1.2/README.md` & `pyalslib-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.2/pyalslib/ALSCatalog.py` & `pyalslib-1.1.3/pyalslib/ALSCatalog.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.2/pyalslib/ALSCatalogCache.py` & `pyalslib-1.1.3/pyalslib/ALSCatalogCache.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.2/pyalslib/ALSGraph.py` & `pyalslib-1.1.3/pyalslib/ALSGraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,19 +109,24 @@
                     out_idx += 2 ** i
             if configuration is None:
                 cell_values[cell] = cell["spec"][out_idx] == "1"
                 if cell["name"] not in lut_io_info:
                     lut_io_info[cell["name"]] = {"spec": cell["spec"], "freq" : [0] * len(cell["spec"])}       
                 lut_io_info[cell["name"]]["freq"][out_idx] += 1
             else:
-                cell_conf = configuration[cell["name"]]
-                if cell["name"] not in lut_io_info:
-                    lut_io_info[cell["name"]] = {"spec": cell_conf["axspec"], "freq" : [0] * len(cell["spec"])}       
-                lut_io_info[cell["name"]]["freq"][out_idx] += 1
-                cell_values[cell] = cell_conf["axspec"][out_idx] == "1"
+                if cell["name"] == "Constant 0":
+                    cell_values[cell] = False
+                elif cell["name"] == "Constant 1":
+                    cell_values[cell] = True
+                else:
+                    cell_conf = configuration[cell["name"]]
+                    if cell["name"] not in lut_io_info:
+                        lut_io_info[cell["name"]] = {"spec": cell_conf["axspec"], "freq" : [0] * len(cell["spec"])}       
+                    lut_io_info[cell["name"]]["freq"][out_idx] += 1
+                    cell_values[cell] = cell_conf["axspec"][out_idx] == "1"
         return cell_values[cell], lut_io_info
 
 
     def plot(self):
         layout = self.__graph.layout("sugiyama")
         layout.rotate(270)
         ig.plot(self.__graph, layout = layout, bbox=(2000, 2000), margin=120, hovermode='closest', vertex_label_dist = 2.5)
```

### Comparing `pyalslib-1.1.2/pyalslib/ALSRewriter.py` & `pyalslib-1.1.3/pyalslib/ALSRewriter.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.2/pyalslib/ALSSMT.py` & `pyalslib-1.1.3/pyalslib/ALSSMT.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.2/pyalslib/Utility.py` & `pyalslib-1.1.3/pyalslib/Utility.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.2/pyalslib/YosysHelper.py` & `pyalslib-1.1.3/pyalslib/YosysHelper.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.2/pyalslib.egg-info/PKG-INFO` & `pyalslib-1.1.3/pyalslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalslib
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
 Home-page: https://github.com/SalvatoreBarone/pyALSlib
 Author: Salvatore Barone
 Author-email: salvatore.barone@unina.it
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/pyALSlib/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/pyALSlib
 Keywords: Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
```

### Comparing `pyalslib-1.1.2/setup.py` & `pyalslib-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pyalslib",
-    version="1.1.2",
+    version="1.1.3",
     description="Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique",
     long_description="Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique. Please visit https://github.com/SalvatoreBarone/pyALSlib",
     url="https://github.com/SalvatoreBarone/pyALSlib",
     author="Salvatore Barone",
     author_email="salvatore.barone@unina.it",
     classifiers=[
         "Intended Audience :: Information Technology",
```

