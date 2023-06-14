# Comparing `tmp/iamlistening-0.1.8.tar.gz` & `tmp/iamlistening-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.1.8.tar", max compression
+gzip compressed data, was "iamlistening-0.1.9.tar", max compression
```

## Comparing `iamlistening-0.1.8.tar` & `iamlistening-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-04 18:20:51.612398 iamlistening-0.1.8/LICENSE
--rw-r--r--   0        0        0     1719 2023-06-04 18:20:51.612398 iamlistening-0.1.8/README.md
--rw-r--r--   0        0        0       99 2023-06-04 18:20:52.272405 iamlistening-0.1.8/iamlistening/__init__.py
--rw-r--r--   0        0        0      630 2023-06-04 18:20:51.612398 iamlistening-0.1.8/iamlistening/config.py
--rw-r--r--   0        0        0      229 2023-06-04 18:20:51.612398 iamlistening-0.1.8/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     4053 2023-06-04 18:20:51.612398 iamlistening-0.1.8/iamlistening/main.py
--rw-r--r--   0        0        0     1692 2023-06-04 18:20:52.272405 iamlistening-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 iamlistening-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-05 19:08:23.478476 iamlistening-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1719 2023-06-05 19:08:23.478476 iamlistening-0.1.9/README.md
+-rw-r--r--   0        0        0       99 2023-06-05 19:08:24.166486 iamlistening-0.1.9/iamlistening/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-05 19:08:23.478476 iamlistening-0.1.9/iamlistening/config.py
+-rw-r--r--   0        0        0      229 2023-06-05 19:08:23.478476 iamlistening-0.1.9/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     4053 2023-06-05 19:08:23.478476 iamlistening-0.1.9/iamlistening/main.py
+-rw-r--r--   0        0        0     1692 2023-06-05 19:08:24.166486 iamlistening-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 iamlistening-0.1.9/PKG-INFO
```

### Comparing `iamlistening-0.1.8/LICENSE` & `iamlistening-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.8/README.md` & `iamlistening-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.8/iamlistening/config.py` & `iamlistening-0.1.9/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.8/iamlistening/main.py` & `iamlistening-0.1.9/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.8/pyproject.toml` & `iamlistening-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamlistening"
-version = "0.1.8"
+version = "0.1.9"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
```

### Comparing `iamlistening-0.1.8/PKG-INFO` & `iamlistening-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

