# Comparing `tmp/django_auto_prefetch-1.5.1.tar.gz` & `tmp/django_auto_prefetch-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_auto_prefetch-1.5.1.tar", last modified: Wed Mar 29 14:42:24 2023, max compression
+gzip compressed data, was "django_auto_prefetch-1.6.0.tar", last modified: Wed Jun 14 08:03:00 2023, max compression
```

## Comparing `django_auto_prefetch-1.5.1.tar` & `django_auto_prefetch-1.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-03-29 14:42:24.915446 django_auto_prefetch-1.5.1/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1573 2023-03-29 14:42:21.000000 django_auto_prefetch-1.5.1/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1522 2022-11-09 21:18:25.000000 django_auto_prefetch-1.5.1/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-28 10:51:44.000000 django_auto_prefetch-1.5.1/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8496 2023-03-29 14:42:24.915528 django_auto_prefetch-1.5.1/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7198 2023-01-28 10:51:44.000000 django_auto_prefetch-1.5.1/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      813 2023-02-28 09:05:50.000000 django_auto_prefetch-1.5.1/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1569 2023-03-29 14:42:24.915862 django_auto_prefetch-1.5.1/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-03-29 14:42:24.912984 django_auto_prefetch-1.5.1/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-03-29 14:42:24.914108 django_auto_prefetch-1.5.1/src/auto_prefetch/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4920 2023-03-29 14:42:16.000000 django_auto_prefetch-1.5.1/src/auto_prefetch/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:23.000000 django_auto_prefetch-1.5.1/src/auto_prefetch/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-03-29 14:42:24.915193 django_auto_prefetch-1.5.1/src/django_auto_prefetch.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8496 2023-03-29 14:42:24.000000 django_auto_prefetch-1.5.1/src/django_auto_prefetch.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2023-03-29 14:42:24.000000 django_auto_prefetch-1.5.1/src/django_auto_prefetch.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-03-29 14:42:24.000000 django_auto_prefetch-1.5.1/src/django_auto_prefetch.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-03-29 14:42:24.000000 django_auto_prefetch-1.5.1/src/django_auto_prefetch.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-03-29 14:42:24.000000 django_auto_prefetch-1.5.1/src/django_auto_prefetch.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       14 2023-03-29 14:42:24.000000 django_auto_prefetch-1.5.1/src/django_auto_prefetch.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-03-29 14:42:24.915338 django_auto_prefetch-1.5.1/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8129 2023-03-29 14:42:16.000000 django_auto_prefetch-1.5.1/tests/test_basic.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 08:03:00.252470 django_auto_prefetch-1.6.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1639 2023-06-14 08:02:57.000000 django_auto_prefetch-1.6.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1522 2022-11-09 21:18:25.000000 django_auto_prefetch-1.6.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-28 10:51:44.000000 django_auto_prefetch-1.6.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8547 2023-06-14 08:03:00.252569 django_auto_prefetch-1.6.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7198 2023-06-13 21:03:18.000000 django_auto_prefetch-1.6.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      813 2023-05-20 20:40:33.000000 django_auto_prefetch-1.6.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1610 2023-06-14 08:03:00.253467 django_auto_prefetch-1.6.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 08:03:00.242979 django_auto_prefetch-1.6.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 08:03:00.244545 django_auto_prefetch-1.6.0/src/auto_prefetch/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4920 2023-05-20 20:40:33.000000 django_auto_prefetch-1.6.0/src/auto_prefetch/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:23.000000 django_auto_prefetch-1.6.0/src/auto_prefetch/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 08:03:00.252038 django_auto_prefetch-1.6.0/src/django_auto_prefetch.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8547 2023-06-14 08:03:00.000000 django_auto_prefetch-1.6.0/src/django_auto_prefetch.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2023-06-14 08:03:00.000000 django_auto_prefetch-1.6.0/src/django_auto_prefetch.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-14 08:03:00.000000 django_auto_prefetch-1.6.0/src/django_auto_prefetch.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-14 08:03:00.000000 django_auto_prefetch-1.6.0/src/django_auto_prefetch.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-06-14 08:03:00.000000 django_auto_prefetch-1.6.0/src/django_auto_prefetch.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       14 2023-06-14 08:03:00.000000 django_auto_prefetch-1.6.0/src/django_auto_prefetch.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 08:03:00.252162 django_auto_prefetch-1.6.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8129 2023-05-20 20:40:33.000000 django_auto_prefetch-1.6.0/tests/test_basic.py
```

### Comparing `django_auto_prefetch-1.5.1/CHANGELOG.rst` & `django_auto_prefetch-1.6.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 =========
 Changelog
 =========
 
+1.6.0 (2023-06-14)
+------------------
+
+* Support Python 3.12.
+
 1.5.1 (2023-03-29)
 ------------------
 
 * Fix the system check for ``Meta.base_manager_name`` to work with multiple inheritance of ``Meta`` classes.
 
-  Thanks to Julius Seporaitis for the report in `Issue #228 <https://github.com/adamchainz/django-upgrade/issues/228>`__.
+  Thanks to Julius Seporaitis for the report in `Issue #228 <https://github.com/tolomea/django-auto-prefetch/issues/228>`__.
 
 1.5.0 (2023-02-25)
 ------------------
 
 * Support Django 4.2.
 
 1.4.0 (2022-11-09)
```

### Comparing `django_auto_prefetch-1.5.1/LICENSE` & `django_auto_prefetch-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_auto_prefetch-1.5.1/PKG-INFO` & `django_auto_prefetch-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_auto_prefetch
-Version: 1.5.1
+Version: 1.6.0
 Summary: Automatically prefetch foreign key values as needed.
 Home-page: https://github.com/tolomea/django-auto-prefetch
 Author: Gordon Wrigley
 Author-email: gordon.wrigley@gmail.com
 License: BSD-3-Clause
 Project-URL: Changelog, https://github.com/tolomea/django-auto-prefetch/blob/main/CHANGELOG.rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 django-auto-prefetch
@@ -56,15 +57,15 @@
 the same ``QuerySet`` as the current model instance. This is enabled at the
 model level and totally automatic and transparent for users of the
 model.
 
 Requirements
 ------------
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 Usage
 -----
 
 1. Install with ``python -m pip install django-auto-prefetch``.
```

### Comparing `django_auto_prefetch-1.5.1/README.rst` & `django_auto_prefetch-1.6.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 the same ``QuerySet`` as the current model instance. This is enabled at the
 model level and totally automatic and transparent for users of the
 model.
 
 Requirements
 ------------
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 Usage
 -----
 
 1. Install with ``python -m pip install django-auto-prefetch``.
```

### Comparing `django_auto_prefetch-1.5.1/pyproject.toml` & `django_auto_prefetch-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_auto_prefetch-1.5.1/setup.cfg` & `django_auto_prefetch-1.6.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = django_auto_prefetch
-version = 1.5.1
+version = 1.6.0
 description = Automatically prefetch foreign key values as needed.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/tolomea/django-auto-prefetch
 author = Gordon Wrigley
 author_email = gordon.wrigley@gmail.com
 license = BSD-3-Clause
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Framework :: Django :: 4.2
 	Intended Audience :: Developers
@@ -22,14 +22,15 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Typing :: Typed
 project_urls = 
 	Changelog = https://github.com/tolomea/django-auto-prefetch/blob/main/CHANGELOG.rst
 
 [options]
 packages = find:
```

### Comparing `django_auto_prefetch-1.5.1/src/auto_prefetch/__init__.py` & `django_auto_prefetch-1.6.0/src/auto_prefetch/__init__.py`

 * *Files identical despite different names*

### Comparing `django_auto_prefetch-1.5.1/src/django_auto_prefetch.egg-info/PKG-INFO` & `django_auto_prefetch-1.6.0/src/django_auto_prefetch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-auto-prefetch
-Version: 1.5.1
+Version: 1.6.0
 Summary: Automatically prefetch foreign key values as needed.
 Home-page: https://github.com/tolomea/django-auto-prefetch
 Author: Gordon Wrigley
 Author-email: gordon.wrigley@gmail.com
 License: BSD-3-Clause
 Project-URL: Changelog, https://github.com/tolomea/django-auto-prefetch/blob/main/CHANGELOG.rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 django-auto-prefetch
@@ -56,15 +57,15 @@
 the same ``QuerySet`` as the current model instance. This is enabled at the
 model level and totally automatic and transparent for users of the
 model.
 
 Requirements
 ------------
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 Usage
 -----
 
 1. Install with ``python -m pip install django-auto-prefetch``.
```

### Comparing `django_auto_prefetch-1.5.1/tests/test_basic.py` & `django_auto_prefetch-1.6.0/tests/test_basic.py`

 * *Files identical despite different names*

