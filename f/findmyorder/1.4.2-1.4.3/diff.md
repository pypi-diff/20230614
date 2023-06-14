# Comparing `tmp/findmyorder-1.4.2.tar.gz` & `tmp/findmyorder-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.4.2.tar", max compression
+gzip compressed data, was "findmyorder-1.4.3.tar", max compression
```

## Comparing `findmyorder-1.4.2.tar` & `findmyorder-1.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-11 11:51:17.810741 findmyorder-1.4.2/LICENSE
--rw-r--r--   0        0        0     1995 2023-06-11 11:51:17.810741 findmyorder-1.4.2/README.md
--rw-r--r--   0        0        0      113 2023-06-11 11:51:34.026855 findmyorder-1.4.2/findmyorder/__init__.py
--rw-r--r--   0        0        0      629 2023-06-11 11:51:17.810741 findmyorder-1.4.2/findmyorder/config.py
--rw-r--r--   0        0        0     2265 2023-06-11 11:51:17.810741 findmyorder-1.4.2/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5555 2023-06-11 11:51:17.810741 findmyorder-1.4.2/findmyorder/main.py
--rw-r--r--   0        0        0     1745 2023-06-11 11:51:34.026855 findmyorder-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 findmyorder-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-14 13:50:20.531311 findmyorder-1.4.3/LICENSE
+-rw-r--r--   0        0        0     1995 2023-06-14 13:50:20.531311 findmyorder-1.4.3/README.md
+-rw-r--r--   0        0        0      113 2023-06-14 13:50:45.899405 findmyorder-1.4.3/findmyorder/__init__.py
+-rw-r--r--   0        0        0      629 2023-06-14 13:50:20.531311 findmyorder-1.4.3/findmyorder/config.py
+-rw-r--r--   0        0        0     2265 2023-06-14 13:50:20.531311 findmyorder-1.4.3/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5555 2023-06-14 13:50:20.531311 findmyorder-1.4.3/findmyorder/main.py
+-rw-r--r--   0        0        0     1745 2023-06-14 13:50:45.899405 findmyorder-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 findmyorder-1.4.3/PKG-INFO
```

### Comparing `findmyorder-1.4.2/LICENSE` & `findmyorder-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.2/README.md` & `findmyorder-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.2/findmyorder/config.py` & `findmyorder-1.4.3/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.2/findmyorder/default_settings.toml` & `findmyorder-1.4.3/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.2/findmyorder/main.py` & `findmyorder-1.4.3/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.2/pyproject.toml` & `findmyorder-1.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.4.2"
+version = "1.4.3"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
```

### Comparing `findmyorder-1.4.2/PKG-INFO` & `findmyorder-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.4.2
+Version: 1.4.3
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

