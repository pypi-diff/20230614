# Comparing `tmp/django_version_checks-1.8.0.tar.gz` & `tmp/django_version_checks-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_version_checks-1.8.0.tar", last modified: Sat Feb 25 07:24:46 2023, max compression
+gzip compressed data, was "django_version_checks-1.9.0.tar", last modified: Wed Jun 14 19:15:33 2023, max compression
```

## Comparing `django_version_checks-1.8.0.tar` & `django_version_checks-1.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:24:46.823714 django_version_checks-1.8.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1214 2023-02-25 07:24:44.000000 django_version_checks-1.8.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:03.000000 django_version_checks-1.8.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:09:58.000000 django_version_checks-1.8.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8719 2023-02-25 07:24:46.823796 django_version_checks-1.8.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7316 2023-01-20 11:36:47.000000 django_version_checks-1.8.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      460 2023-02-15 21:55:45.000000 django_version_checks-1.8.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1694 2023-02-25 07:24:46.824099 django_version_checks-1.8.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:24:46.821035 django_version_checks-1.8.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:24:46.822718 django_version_checks-1.8.0/src/django_version_checks/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:03.000000 django_version_checks-1.8.0/src/django_version_checks/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      655 2022-11-04 11:16:31.000000 django_version_checks-1.8.0/src/django_version_checks/apps.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8811 2022-11-04 11:16:31.000000 django_version_checks-1.8.0/src/django_version_checks/checks.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:03.000000 django_version_checks-1.8.0/src/django_version_checks/py.typed
--rw-r--r--   0 adamjohnson   (501) staff       (20)      180 2022-11-04 11:16:31.000000 django_version_checks-1.8.0/src/django_version_checks/typing.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:24:46.823460 django_version_checks-1.8.0/src/django_version_checks.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8719 2023-02-25 07:24:46.000000 django_version_checks-1.8.0/src/django_version_checks.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      561 2023-02-25 07:24:46.000000 django_version_checks-1.8.0/src/django_version_checks.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:24:46.000000 django_version_checks-1.8.0/src/django_version_checks.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:24:46.000000 django_version_checks-1.8.0/src/django_version_checks.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       28 2023-02-25 07:24:46.000000 django_version_checks-1.8.0/src/django_version_checks.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       22 2023-02-25 07:24:46.000000 django_version_checks-1.8.0/src/django_version_checks.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:24:46.823578 django_version_checks-1.8.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    12294 2022-11-04 11:16:31.000000 django_version_checks-1.8.0/tests/test_checks.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 19:15:33.621696 django_version_checks-1.9.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1277 2023-06-14 19:15:30.000000 django_version_checks-1.9.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:03.000000 django_version_checks-1.9.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:09:58.000000 django_version_checks-1.9.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8770 2023-06-14 19:15:33.621766 django_version_checks-1.9.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7316 2023-06-14 19:10:50.000000 django_version_checks-1.9.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      500 2023-02-28 09:05:55.000000 django_version_checks-1.9.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1735 2023-06-14 19:15:33.622055 django_version_checks-1.9.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 19:15:33.618819 django_version_checks-1.9.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 19:15:33.620621 django_version_checks-1.9.0/src/django_version_checks/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:03.000000 django_version_checks-1.9.0/src/django_version_checks/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      655 2022-11-04 11:16:31.000000 django_version_checks-1.9.0/src/django_version_checks/apps.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8811 2022-11-04 11:16:31.000000 django_version_checks-1.9.0/src/django_version_checks/checks.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:03.000000 django_version_checks-1.9.0/src/django_version_checks/py.typed
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      180 2022-11-04 11:16:31.000000 django_version_checks-1.9.0/src/django_version_checks/typing.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 19:15:33.621418 django_version_checks-1.9.0/src/django_version_checks.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8770 2023-06-14 19:15:33.000000 django_version_checks-1.9.0/src/django_version_checks.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      561 2023-06-14 19:15:33.000000 django_version_checks-1.9.0/src/django_version_checks.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-14 19:15:33.000000 django_version_checks-1.9.0/src/django_version_checks.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-14 19:15:33.000000 django_version_checks-1.9.0/src/django_version_checks.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       28 2023-06-14 19:15:33.000000 django_version_checks-1.9.0/src/django_version_checks.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       22 2023-06-14 19:15:33.000000 django_version_checks-1.9.0/src/django_version_checks.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 19:15:33.621545 django_version_checks-1.9.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    12294 2022-11-04 11:16:31.000000 django_version_checks-1.9.0/tests/test_checks.py
```

### Comparing `django_version_checks-1.8.0/CHANGELOG.rst` & `django_version_checks-1.9.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+1.9.0 (2023-06-14)
+------------------
+
+* Support Python 3.12.
+
 1.8.0 (2023-02-25)
 ------------------
 
 * Support Django 4.2.
 
 1.7.0 (2022-06-05)
 ------------------
```

### Comparing `django_version_checks-1.8.0/LICENSE` & `django_version_checks-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_version_checks-1.8.0/PKG-INFO` & `django_version_checks-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_version_checks
-Version: 1.8.0
+Version: 1.9.0
 Summary: System checks for your project's environment.
 Home-page: https://github.com/adamchainz/django-version-checks
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-version-checks/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -22,14 +22,15 @@
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
 
 =====================
@@ -53,15 +54,15 @@
    :alt: pre-commit
 
 System checks for your project's environment.
 
 Requirements
 ============
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
```

### Comparing `django_version_checks-1.8.0/README.rst` & `django_version_checks-1.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
    :alt: pre-commit
 
 System checks for your project's environment.
 
 Requirements
 ============
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
```

### Comparing `django_version_checks-1.8.0/setup.cfg` & `django_version_checks-1.9.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = django_version_checks
-version = 1.8.0
+version = 1.9.0
 description = System checks for your project's environment.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/django-version-checks
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
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
 keywords = Django
 project_urls = 
 	Changelog = https://github.com/adamchainz/django-version-checks/blob/main/CHANGELOG.rst
 	Mastodon = https://fosstodon.org/@adamchainz
 	Twitter = https://twitter.com/adamchainz
```

### Comparing `django_version_checks-1.8.0/src/django_version_checks/apps.py` & `django_version_checks-1.9.0/src/django_version_checks/apps.py`

 * *Files identical despite different names*

### Comparing `django_version_checks-1.8.0/src/django_version_checks/checks.py` & `django_version_checks-1.9.0/src/django_version_checks/checks.py`

 * *Files identical despite different names*

### Comparing `django_version_checks-1.8.0/src/django_version_checks.egg-info/PKG-INFO` & `django_version_checks-1.9.0/src/django_version_checks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-version-checks
-Version: 1.8.0
+Version: 1.9.0
 Summary: System checks for your project's environment.
 Home-page: https://github.com/adamchainz/django-version-checks
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-version-checks/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -22,14 +22,15 @@
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
 
 =====================
@@ -53,15 +54,15 @@
    :alt: pre-commit
 
 System checks for your project's environment.
 
 Requirements
 ============
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
```

### Comparing `django_version_checks-1.8.0/src/django_version_checks.egg-info/SOURCES.txt` & `django_version_checks-1.9.0/src/django_version_checks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_version_checks-1.8.0/tests/test_checks.py` & `django_version_checks-1.9.0/tests/test_checks.py`

 * *Files identical despite different names*

