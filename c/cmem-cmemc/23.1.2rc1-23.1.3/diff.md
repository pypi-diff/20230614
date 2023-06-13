# Comparing `tmp/cmem_cmemc-23.1.2rc1.tar.gz` & `tmp/cmem_cmemc-23.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_cmemc-23.1.2rc1.tar", max compression
+gzip compressed data, was "cmem_cmemc-23.1.3.tar", max compression
```

## Comparing `cmem_cmemc-23.1.2rc1.tar` & `cmem_cmemc-23.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-01-18 07:15:37.943836 cmem_cmemc-23.1.2rc1/LICENSE
--rw-r--r--   0        0        0      808 2023-01-18 07:15:37.943900 cmem_cmemc-23.1.2rc1/README-public.md
--rw-r--r--   0        0        0      109 2023-01-18 07:15:37.944108 cmem_cmemc-23.1.2rc1/cmem/__init__.py
--rw-r--r--   0        0        0       28 2023-01-18 07:15:37.944190 cmem_cmemc-23.1.2rc1/cmem/cmemc/__init__.py
--rw-r--r--   0        0        0     5571 2023-04-28 12:54:24.692339 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/__init__.py
--rw-r--r--   0        0        0     3311 2023-02-14 08:17:24.862278 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/__init__.py
--rw-r--r--   0        0        0     6709 2023-04-21 12:08:15.190979 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/admin.py
--rw-r--r--   0        0        0     5562 2023-03-15 16:42:29.626951 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/config.py
--rw-r--r--   0        0        0    27505 2023-04-21 06:37:45.132177 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/dataset.py
--rw-r--r--   0        0        0    27110 2023-03-15 16:42:29.627797 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/graph.py
--rw-r--r--   0        0        0     7808 2023-03-15 16:42:29.628159 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/metrics.py
--rw-r--r--   0        0        0    17612 2023-03-15 16:42:29.628389 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/project.py
--rw-r--r--   0        0        0     6948 2023-03-15 16:42:29.628590 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/python.py
--rw-r--r--   0        0        0    27725 2023-03-15 16:42:29.628916 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/query.py
--rw-r--r--   0        0        0     7556 2023-03-15 16:42:29.629062 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/resource.py
--rw-r--r--   0        0        0     8192 2023-03-15 16:42:29.629342 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/scheduler.py
--rw-r--r--   0        0        0     6961 2023-03-15 16:42:29.629976 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/store.py
--rw-r--r--   0        0        0    10654 2023-02-15 15:36:55.698463 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/user.py
--rw-r--r--   0        0        0    16218 2023-03-15 16:42:29.630243 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/vocabulary.py
--rw-r--r--   0        0        0    21832 2023-03-15 16:42:29.630535 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/workflow.py
--rw-r--r--   0        0        0     4761 2023-03-15 16:42:29.630851 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/workspace.py
--rw-r--r--   0        0        0    38221 2023-04-21 06:37:45.133132 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/completion.py
--rw-r--r--   0        0        0    15648 2023-04-24 20:44:46.137043 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/context.py
--rw-r--r--   0        0        0      139 2023-01-18 07:15:37.946025 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/exceptions.py
--rw-r--r--   0        0        0       43 2023-01-18 07:15:37.946113 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/__init__.py
--rw-r--r--   0        0        0     3261 2023-01-18 07:15:37.946179 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/graph.py
--rw-r--r--   0        0        0    11127 2023-04-28 12:54:24.692606 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/multi_page.py
--rw-r--r--   0        0        0     1303 2023-01-18 07:15:37.946315 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/single_page.py
--rw-r--r--   0        0        0     8086 2023-04-24 20:44:46.137197 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/utils.py
--rw-r--r--   0        0        0     2384 2023-05-05 14:31:45.416295 cmem_cmemc-23.1.2rc1/pyproject.toml
--rw-r--r--   0        0        0     2545 1970-01-01 00:00:00.000000 cmem_cmemc-23.1.2rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-13 21:54:44.577486 cmem_cmemc-23.1.3/LICENSE
+-rw-r--r--   0        0        0      808 2023-06-13 21:54:44.577486 cmem_cmemc-23.1.3/README-public.md
+-rw-r--r--   0        0        0      109 2023-06-13 21:54:44.577486 cmem_cmemc-23.1.3/cmem/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-13 21:54:44.577486 cmem_cmemc-23.1.3/cmem/cmemc/__init__.py
+-rw-r--r--   0        0        0     5571 2023-06-13 21:54:44.577486 cmem_cmemc-23.1.3/cmem/cmemc/cli/__init__.py
+-rw-r--r--   0        0        0     3311 2023-06-13 21:54:44.577486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6709 2023-06-13 21:54:44.577486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/admin.py
+-rw-r--r--   0        0        0     5562 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/config.py
+-rw-r--r--   0        0        0    27505 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/dataset.py
+-rw-r--r--   0        0        0    27110 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/graph.py
+-rw-r--r--   0        0        0     7808 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/metrics.py
+-rw-r--r--   0        0        0    17612 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/project.py
+-rw-r--r--   0        0        0     6948 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/python.py
+-rw-r--r--   0        0        0    27725 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/query.py
+-rw-r--r--   0        0        0     7556 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/resource.py
+-rw-r--r--   0        0        0     8192 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/scheduler.py
+-rw-r--r--   0        0        0     6961 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/store.py
+-rw-r--r--   0        0        0    10654 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/user.py
+-rw-r--r--   0        0        0    16218 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/vocabulary.py
+-rw-r--r--   0        0        0    21832 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/workflow.py
+-rw-r--r--   0        0        0     4761 2023-06-13 21:54:44.581486 cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/workspace.py
+-rw-r--r--   0        0        0    38221 2023-06-13 21:54:44.585486 cmem_cmemc-23.1.3/cmem/cmemc/cli/completion.py
+-rw-r--r--   0        0        0    15648 2023-06-13 21:54:44.585486 cmem_cmemc-23.1.3/cmem/cmemc/cli/context.py
+-rw-r--r--   0        0        0      139 2023-06-13 21:54:44.585486 cmem_cmemc-23.1.3/cmem/cmemc/cli/exceptions.py
+-rw-r--r--   0        0        0       43 2023-06-13 21:54:44.585486 cmem_cmemc-23.1.3/cmem/cmemc/cli/manual_helper/__init__.py
+-rw-r--r--   0        0        0     3261 2023-06-13 21:54:44.585486 cmem_cmemc-23.1.3/cmem/cmemc/cli/manual_helper/graph.py
+-rw-r--r--   0        0        0    11127 2023-06-13 21:54:44.585486 cmem_cmemc-23.1.3/cmem/cmemc/cli/manual_helper/multi_page.py
+-rw-r--r--   0        0        0     1303 2023-06-13 21:54:44.585486 cmem_cmemc-23.1.3/cmem/cmemc/cli/manual_helper/single_page.py
+-rw-r--r--   0        0        0     8086 2023-06-13 21:54:44.585486 cmem_cmemc-23.1.3/cmem/cmemc/cli/utils.py
+-rw-r--r--   0        0        0     2383 2023-06-13 21:55:10.521464 cmem_cmemc-23.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 cmem_cmemc-23.1.3/PKG-INFO
```

### Comparing `cmem_cmemc-23.1.2rc1/LICENSE` & `cmem_cmemc-23.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/README-public.md` & `cmem_cmemc-23.1.3/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/__init__.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/__init__.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/admin.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/admin.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/config.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/dataset.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/dataset.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/graph.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/graph.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/metrics.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/project.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/project.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/python.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/python.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/query.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/resource.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/resource.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/scheduler.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/scheduler.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/store.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/store.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/user.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/user.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/vocabulary.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/vocabulary.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/workflow.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/workflow.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/workspace.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/commands/workspace.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/completion.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/completion.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/context.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/context.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/graph.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/manual_helper/graph.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/multi_page.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/manual_helper/multi_page.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/single_page.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/manual_helper/single_page.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/utils.py` & `cmem_cmemc-23.1.3/cmem/cmemc/cli/utils.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2rc1/pyproject.toml` & `cmem_cmemc-23.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [tool.poetry]
 name = "cmem-cmemc"
-version = "23.1.2rc1"
+version = "23.1.3"
 description = "Command line client for eccenca Corporate Memory"
 license = "Apache 2.0"
 classifiers = ["Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Intended Audience :: Science/Research", "Intended Audience :: System Administrators", "License :: OSI Approved :: Apache Software License", "Programming Language :: Python :: 3.9", "Topic :: Software Development :: Testing", "Topic :: Database", "Topic :: Utilities"]
 homepage = "https://eccenca.com/go/cmemc"
 authors = ["eccenca <cmempy-developer@eccenca.com>", "Sebastian Tramp <sebastian.tramp@eccenca.com>"]
 readme = "README-public.md"
 packages = [
     { include = "cmem" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 beautifulsoup4 = "^4.12.2"
-certifi = ">=2022.12.7"
+certifi = ">=2023.5.7"
 click = "==7.1.2"
 click-didyoumean = "^0.3.0"
 click-help-colors = "^0.9.1"
-cmem-cmempy = "==23.1"
+cmem-cmempy = "==23.1.1"
 # cmem-cmempy = { path = "cmempy", develop = true }
 configparser = "^5.3.0"
 jinja2 = "^3.1.2"
 natsort = "^8.3.1"
 prometheus-client = "^0.16.0"
 pygments = "^2.15.1"
-pyjwt = "^2.6.0"
-requests = "^2.30.0"
+pyjwt = "^2.7.0"
+requests = "^2.31.0"
 six = "^1.16.0"
 tabulate = "^0.9.0"
 timeago = "^1.0.16"
 treelib = "^1.6.4"
-urllib3 = "^1.26.5"
+urllib3 = "^1.26.16"
 
 [tool.poetry.scripts]
 cmemc = 'cmem.cmemc.cli:main'
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.4"
 coverage = "^6.3.2"
```

### Comparing `cmem_cmemc-23.1.2rc1/PKG-INFO` & `cmem_cmemc-23.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-cmemc
-Version: 23.1.2rc1
+Version: 23.1.3
 Summary: Command line client for eccenca Corporate Memory
 Home-page: https://eccenca.com/go/cmemc
 License: Apache 2.0
 Author: eccenca
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,31 +18,31 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: certifi (>=2022.12.7)
+Requires-Dist: certifi (>=2023.5.7)
 Requires-Dist: click (==7.1.2)
 Requires-Dist: click-didyoumean (>=0.3.0,<0.4.0)
 Requires-Dist: click-help-colors (>=0.9.1,<0.10.0)
-Requires-Dist: cmem-cmempy (==23.1)
+Requires-Dist: cmem-cmempy (==23.1.1)
 Requires-Dist: configparser (>=5.3.0,<6.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: natsort (>=8.3.1,<9.0.0)
 Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
-Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
-Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: pyjwt (>=2.7.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: timeago (>=1.0.16,<2.0.0)
 Requires-Dist: treelib (>=1.6.4,<2.0.0)
-Requires-Dist: urllib3 (>=1.26.5,<2.0.0)
+Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Description-Content-Type: text/markdown
 
 # cmemc
 
 cmemc is the official command line client for [eccenca Corporate Memory](https://documentation.eccenca.com/).
 
 ## Installation
```

