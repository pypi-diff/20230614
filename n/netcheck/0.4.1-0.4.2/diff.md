# Comparing `tmp/netcheck-0.4.1.tar.gz` & `tmp/netcheck-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netcheck-0.4.1.tar", max compression
+gzip compressed data, was "netcheck-0.4.2.tar", max compression
```

## Comparing `netcheck-0.4.1.tar` & `netcheck-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-22 04:59:55.211509 netcheck-0.4.1/LICENSE
--rw-r--r--   0        0        0     8655 2023-05-22 04:59:55.211509 netcheck-0.4.1/README.md
--rw-r--r--   0        0        0        0 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/__init__.py
--rw-r--r--   0        0        0     6019 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/cli.py
--rw-r--r--   0        0        0     3790 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/context.py
--rw-r--r--   0        0        0     2374 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/dns.py
--rw-r--r--   0        0        0     2150 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/http.py
--rw-r--r--   0        0        0     5730 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/runner.py
--rw-r--r--   0        0        0     2207 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/validation.py
--rw-r--r--   0        0        0      214 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/version.py
--rw-r--r--   0        0        0      868 2023-05-22 04:59:55.235509 netcheck-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     9447 1970-01-01 00:00:00.000000 netcheck-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-13 23:24:25.977658 netcheck-0.4.2/LICENSE
+-rw-r--r--   0        0        0     8655 2023-06-13 23:24:25.977658 netcheck-0.4.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 23:24:25.989658 netcheck-0.4.2/netcheck/__init__.py
+-rw-r--r--   0        0        0     6019 2023-06-13 23:24:25.989658 netcheck-0.4.2/netcheck/cli.py
+-rw-r--r--   0        0        0     3790 2023-06-13 23:24:25.989658 netcheck-0.4.2/netcheck/context.py
+-rw-r--r--   0        0        0     2374 2023-06-13 23:24:25.989658 netcheck-0.4.2/netcheck/dns.py
+-rw-r--r--   0        0        0     2150 2023-06-13 23:24:25.989658 netcheck-0.4.2/netcheck/http.py
+-rw-r--r--   0        0        0     5730 2023-06-13 23:24:25.989658 netcheck-0.4.2/netcheck/runner.py
+-rw-r--r--   0        0        0     2207 2023-06-13 23:24:25.989658 netcheck-0.4.2/netcheck/validation.py
+-rw-r--r--   0        0        0      214 2023-06-13 23:24:25.989658 netcheck-0.4.2/netcheck/version.py
+-rw-r--r--   0        0        0      868 2023-06-13 23:24:25.997659 netcheck-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     9447 1970-01-01 00:00:00.000000 netcheck-0.4.2/PKG-INFO
```

### Comparing `netcheck-0.4.1/LICENSE` & `netcheck-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netcheck-0.4.1/README.md` & `netcheck-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `netcheck-0.4.1/netcheck/cli.py` & `netcheck-0.4.2/netcheck/cli.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.4.1/netcheck/context.py` & `netcheck-0.4.2/netcheck/context.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.4.1/netcheck/dns.py` & `netcheck-0.4.2/netcheck/dns.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.4.1/netcheck/http.py` & `netcheck-0.4.2/netcheck/http.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.4.1/netcheck/runner.py` & `netcheck-0.4.2/netcheck/runner.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.4.1/netcheck/validation.py` & `netcheck-0.4.2/netcheck/validation.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.4.1/pyproject.toml` & `netcheck-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netcheck"
-version = "0.4.1"
+version = "0.4.2"
 description = "Netchecks is a cloud native tool for specifying and regularly checking assertions about network conditions. Use netchecks to proactively verify whether security controls are working as intended, alerting on misconfiguration."
 authors = ["Brian Thorne <brian@hardbyte.nz>"]
 readme = "README.md"
 packages = [{include = "netcheck"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `netcheck-0.4.1/PKG-INFO` & `netcheck-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netcheck
-Version: 0.4.1
+Version: 0.4.2
 Summary: Netchecks is a cloud native tool for specifying and regularly checking assertions about network conditions. Use netchecks to proactively verify whether security controls are working as intended, alerting on misconfiguration.
 Author: Brian Thorne
 Author-email: brian@hardbyte.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

