# Comparing `tmp/featurepy-0.1.1.tar.gz` & `tmp/featurepy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurepy-0.1.1.tar", max compression
+gzip compressed data, was "featurepy-0.2.0.tar", max compression
```

## Comparing `featurepy-0.1.1.tar` & `featurepy-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    35129 2023-04-16 16:56:28.332885 featurepy-0.1.1/LICENSE
--rw-r--r--   0        0        0        8 2023-05-10 21:32:16.081018 featurepy-0.1.1/README.md
--rw-r--r--   0        0        0      729 2023-05-18 01:57:23.242787 featurepy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      113 2023-05-12 16:12:13.998544 featurepy-0.1.1/src/featurepy/__init__.py
--rw-r--r--   0        0        0       20 2023-05-18 01:57:23.243033 featurepy-0.1.1/src/featurepy/flask/__init__.py
--rw-r--r--   0        0        0      640 2023-05-18 01:57:23.243406 featurepy-0.1.1/src/featurepy/flask/views.py
--rw-r--r--   0        0        0        0 2023-05-10 23:04:00.786133 featurepy-0.1.1/src/featurepy/scripts/__init__.py
--rw-r--r--   0        0        0      493 2023-05-15 20:05:33.947104 featurepy-0.1.1/src/featurepy/scripts/features.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 featurepy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35129 2023-04-16 16:56:28.332885 featurepy-0.2.0/LICENSE
+-rw-r--r--   0        0        0        8 2023-05-10 21:32:16.081018 featurepy-0.2.0/README.md
+-rw-r--r--   0        0        0      788 2023-06-06 10:57:15.617883 featurepy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      197 2023-06-05 07:46:53.683700 featurepy-0.2.0/src/featurepy/__init__.py
+-rw-r--r--   0        0        0     1346 2023-06-06 10:34:33.732327 featurepy-0.2.0/src/featurepy/feature_class.py
+-rw-r--r--   0        0        0       20 2023-05-18 01:57:23.243033 featurepy-0.2.0/src/featurepy/flask/__init__.py
+-rw-r--r--   0        0        0      640 2023-05-18 01:57:23.243406 featurepy-0.2.0/src/featurepy/flask/views.py
+-rw-r--r--   0        0        0     2938 2023-06-06 10:52:23.396560 featurepy-0.2.0/src/featurepy/model_constraints.py
+-rw-r--r--   0        0        0        0 2023-05-10 23:04:00.786133 featurepy-0.2.0/src/featurepy/scripts/__init__.py
+-rw-r--r--   0        0        0      493 2023-05-15 20:05:33.947104 featurepy-0.2.0/src/featurepy/scripts/features.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 featurepy-0.2.0/PKG-INFO
```

### Comparing `featurepy-0.1.1/LICENSE` & `featurepy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `featurepy-0.1.1/src/featurepy/flask/views.py` & `featurepy-0.2.0/src/featurepy/flask/views.py`

 * *Files identical despite different names*

