# Comparing `tmp/elapse_secrets-0.1.1.tar.gz` & `tmp/elapse_secrets-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elapse_secrets-0.1.1.tar", max compression
+gzip compressed data, was "elapse_secrets-0.1.2.tar", max compression
```

## Comparing `elapse_secrets-0.1.1.tar` & `elapse_secrets-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1982 2023-06-14 18:52:21.097937 elapse_secrets-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-14 13:26:59.932979 elapse_secrets-0.1.1/elapse_secrets/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 13:35:44.092844 elapse_secrets-0.1.1/elapse_secrets/db/__init__.py
--rw-r--r--   0        0        0     4874 2023-06-14 14:29:38.262009 elapse_secrets-0.1.1/elapse_secrets/db/rules-elapse-stable.yml
--rw-r--r--   0        0        0      396 2023-06-14 13:43:54.532718 elapse_secrets-0.1.1/elapse_secrets/debug.py
--rw-r--r--   0        0        0     1565 2023-06-14 18:52:21.107937 elapse_secrets-0.1.1/elapse_secrets/main.py
--rw-r--r--   0        0        0      411 2023-06-14 18:52:17.127938 elapse_secrets-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 elapse_secrets-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1982 2023-06-14 18:52:21.097937 elapse_secrets-0.1.2/README.md
+-rw-r--r--   0        0        0       71 2023-06-14 19:02:59.857773 elapse_secrets-0.1.2/elapse_secrets/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:35:44.092844 elapse_secrets-0.1.2/elapse_secrets/db/__init__.py
+-rw-r--r--   0        0        0     4874 2023-06-14 14:29:38.262009 elapse_secrets-0.1.2/elapse_secrets/db/rules-elapse-stable.yml
+-rw-r--r--   0        0        0      396 2023-06-14 13:43:54.532718 elapse_secrets-0.1.2/elapse_secrets/debug.py
+-rw-r--r--   0        0        0     1565 2023-06-14 18:52:21.107937 elapse_secrets-0.1.2/elapse_secrets/main.py
+-rw-r--r--   0        0        0      411 2023-06-14 19:03:02.757773 elapse_secrets-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 elapse_secrets-0.1.2/PKG-INFO
```

### Comparing `elapse_secrets-0.1.1/README.md` & `elapse_secrets-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `elapse_secrets-0.1.1/elapse_secrets/db/rules-elapse-stable.yml` & `elapse_secrets-0.1.2/elapse_secrets/db/rules-elapse-stable.yml`

 * *Files identical despite different names*

### Comparing `elapse_secrets-0.1.1/elapse_secrets/main.py` & `elapse_secrets-0.1.2/elapse_secrets/main.py`

 * *Files identical despite different names*

### Comparing `elapse_secrets-0.1.1/PKG-INFO` & `elapse_secrets-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elapse-secrets
-Version: 0.1.1
+Version: 0.1.2
 Summary: Detects and removes sensitive information from the client-side to secure a user's data.
 Author: kdcokenny
 Author-email: kenny@kdco.llc
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

