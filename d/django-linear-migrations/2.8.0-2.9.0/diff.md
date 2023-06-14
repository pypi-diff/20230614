# Comparing `tmp/django_linear_migrations-2.8.0.tar.gz` & `tmp/django_linear_migrations-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_linear_migrations-2.8.0.tar", last modified: Mon May 29 23:07:23 2023, max compression
+gzip compressed data, was "django_linear_migrations-2.9.0.tar", last modified: Wed Jun 14 13:56:06 2023, max compression
```

## Comparing `django_linear_migrations-2.8.0.tar` & `django_linear_migrations-2.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.116070 django_linear_migrations-2.8.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4384 2023-05-29 23:07:19.000000 django_linear_migrations-2.8.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:58:38.000000 django_linear_migrations-2.8.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:09:56.000000 django_linear_migrations-2.8.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)    13835 2023-05-29 23:07:23.116186 django_linear_migrations-2.8.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)    12434 2023-05-29 23:04:19.000000 django_linear_migrations-2.8.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      500 2023-02-28 09:05:50.000000 django_linear_migrations-2.8.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1678 2023-05-29 23:07:23.116783 django_linear_migrations-2.8.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.105797 django_linear_migrations-2.8.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.113160 django_linear_migrations-2.8.0/src/django_linear_migrations/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8487 2023-02-27 20:47:44.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/apps.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    25637 2023-02-07 15:19:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/compat.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.114213 django_linear_migrations-2.8.0/src/django_linear_migrations/management/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/management/__init__.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.115052 django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3239 2023-01-03 10:31:33.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/create_max_migration_files.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1084 2022-11-04 10:44:50.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/makemigrations.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8652 2023-05-29 23:04:19.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/rebase_migration.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.114064 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    13835 2023-05-29 23:07:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1003 2023-05-29 23:07:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-29 23:07:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-29 23:07:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-05-29 23:07:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       25 2023-05-29 23:07:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.115882 django_linear_migrations-2.8.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1094 2022-06-03 11:58:39.000000 django_linear_migrations-2.8.0/tests/test_apps.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5495 2023-01-03 10:31:33.000000 django_linear_migrations-2.8.0/tests/test_checks.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7207 2023-01-03 10:31:33.000000 django_linear_migrations-2.8.0/tests/test_create_max_migration_files.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2799 2022-11-04 10:44:50.000000 django_linear_migrations-2.8.0/tests/test_makemigrations.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    19076 2023-05-29 23:04:19.000000 django_linear_migrations-2.8.0/tests/test_rebase_migration.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 13:56:06.729286 django_linear_migrations-2.9.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4447 2023-06-14 13:56:04.000000 django_linear_migrations-2.9.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:58:38.000000 django_linear_migrations-2.9.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:09:56.000000 django_linear_migrations-2.9.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    13886 2023-06-14 13:56:06.729379 django_linear_migrations-2.9.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    12434 2023-06-14 13:54:20.000000 django_linear_migrations-2.9.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      500 2023-02-28 09:05:50.000000 django_linear_migrations-2.9.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1719 2023-06-14 13:56:06.729713 django_linear_migrations-2.9.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 13:56:06.722972 django_linear_migrations-2.9.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 13:56:06.727154 django_linear_migrations-2.9.0/src/django_linear_migrations/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.9.0/src/django_linear_migrations/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8487 2023-02-27 20:47:44.000000 django_linear_migrations-2.9.0/src/django_linear_migrations/apps.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    25637 2023-02-07 15:19:23.000000 django_linear_migrations-2.9.0/src/django_linear_migrations/compat.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 13:56:06.728035 django_linear_migrations-2.9.0/src/django_linear_migrations/management/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.9.0/src/django_linear_migrations/management/__init__.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 13:56:06.728525 django_linear_migrations-2.9.0/src/django_linear_migrations/management/commands/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.9.0/src/django_linear_migrations/management/commands/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3239 2023-01-03 10:31:33.000000 django_linear_migrations-2.9.0/src/django_linear_migrations/management/commands/create_max_migration_files.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1084 2022-11-04 10:44:50.000000 django_linear_migrations-2.9.0/src/django_linear_migrations/management/commands/makemigrations.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8652 2023-05-29 23:04:19.000000 django_linear_migrations-2.9.0/src/django_linear_migrations/management/commands/rebase_migration.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.9.0/src/django_linear_migrations/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 13:56:06.727907 django_linear_migrations-2.9.0/src/django_linear_migrations.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    13886 2023-06-14 13:56:06.000000 django_linear_migrations-2.9.0/src/django_linear_migrations.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1003 2023-06-14 13:56:06.000000 django_linear_migrations-2.9.0/src/django_linear_migrations.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-14 13:56:06.000000 django_linear_migrations-2.9.0/src/django_linear_migrations.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-14 13:56:06.000000 django_linear_migrations-2.9.0/src/django_linear_migrations.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-06-14 13:56:06.000000 django_linear_migrations-2.9.0/src/django_linear_migrations.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       25 2023-06-14 13:56:06.000000 django_linear_migrations-2.9.0/src/django_linear_migrations.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 13:56:06.729161 django_linear_migrations-2.9.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1094 2022-06-03 11:58:39.000000 django_linear_migrations-2.9.0/tests/test_apps.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5495 2023-01-03 10:31:33.000000 django_linear_migrations-2.9.0/tests/test_checks.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7207 2023-01-03 10:31:33.000000 django_linear_migrations-2.9.0/tests/test_create_max_migration_files.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2799 2022-11-04 10:44:50.000000 django_linear_migrations-2.9.0/tests/test_makemigrations.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    19076 2023-05-29 23:04:19.000000 django_linear_migrations-2.9.0/tests/test_rebase_migration.py
```

### Comparing `django_linear_migrations-2.8.0/CHANGELOG.rst` & `django_linear_migrations-2.9.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+2.9.0 (2023-06-14)
+------------------
+
+* Support Python 3.12.
+
 2.8.0 (2023-05-30)
 ------------------
 
 * Extend ``rebase_migration`` to detect Git in-progress merges and select the correct migration to rebase.
 
   Thanks to Dmitry Sleptsov in `PR #260 <https://github.com/adamchainz/django-linear-migrations/pull/260>`__.
```

### Comparing `django_linear_migrations-2.8.0/LICENSE` & `django_linear_migrations-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.8.0/PKG-INFO` & `django_linear_migrations-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_linear_migrations
-Version: 2.8.0
+Version: 2.9.0
 Summary: Ensure your migrations are linear.
 Home-page: https://github.com/adamchainz/django-linear-migrations
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-linear-migrations/blob/main/CHANGELOG.rst
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
 
 ========================
@@ -55,15 +56,15 @@
 Ensure your migration history is linear.
 
 For a bit of background, see the `introductory blog post <https://adamj.eu/tech/2020/12/10/introducing-django-linear-migrations/>`__.
 
 Requirements
 ============
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers django-linear-migrations and many other tools to improve your development experience.
```

### Comparing `django_linear_migrations-2.8.0/README.rst` & `django_linear_migrations-2.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 Ensure your migration history is linear.
 
 For a bit of background, see the `introductory blog post <https://adamj.eu/tech/2020/12/10/introducing-django-linear-migrations/>`__.
 
 Requirements
 ============
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers django-linear-migrations and many other tools to improve your development experience.
```

### Comparing `django_linear_migrations-2.8.0/setup.cfg` & `django_linear_migrations-2.9.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = django_linear_migrations
-version = 2.8.0
+version = 2.9.0
 description = Ensure your migrations are linear.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/django-linear-migrations
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
 	Changelog = https://github.com/adamchainz/django-linear-migrations/blob/main/CHANGELOG.rst
 	Mastodon = https://fosstodon.org/@adamchainz
 	Twitter = https://twitter.com/adamchainz
```

### Comparing `django_linear_migrations-2.8.0/src/django_linear_migrations/apps.py` & `django_linear_migrations-2.9.0/src/django_linear_migrations/apps.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.8.0/src/django_linear_migrations/compat.py` & `django_linear_migrations-2.9.0/src/django_linear_migrations/compat.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/create_max_migration_files.py` & `django_linear_migrations-2.9.0/src/django_linear_migrations/management/commands/create_max_migration_files.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/makemigrations.py` & `django_linear_migrations-2.9.0/src/django_linear_migrations/management/commands/makemigrations.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/rebase_migration.py` & `django_linear_migrations-2.9.0/src/django_linear_migrations/management/commands/rebase_migration.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/PKG-INFO` & `django_linear_migrations-2.9.0/src/django_linear_migrations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-linear-migrations
-Version: 2.8.0
+Version: 2.9.0
 Summary: Ensure your migrations are linear.
 Home-page: https://github.com/adamchainz/django-linear-migrations
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-linear-migrations/blob/main/CHANGELOG.rst
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
 
 ========================
@@ -55,15 +56,15 @@
 Ensure your migration history is linear.
 
 For a bit of background, see the `introductory blog post <https://adamj.eu/tech/2020/12/10/introducing-django-linear-migrations/>`__.
 
 Requirements
 ============
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers django-linear-migrations and many other tools to improve your development experience.
```

### Comparing `django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/SOURCES.txt` & `django_linear_migrations-2.9.0/src/django_linear_migrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.8.0/tests/test_apps.py` & `django_linear_migrations-2.9.0/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.8.0/tests/test_checks.py` & `django_linear_migrations-2.9.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.8.0/tests/test_create_max_migration_files.py` & `django_linear_migrations-2.9.0/tests/test_create_max_migration_files.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.8.0/tests/test_makemigrations.py` & `django_linear_migrations-2.9.0/tests/test_makemigrations.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.8.0/tests/test_rebase_migration.py` & `django_linear_migrations-2.9.0/tests/test_rebase_migration.py`

 * *Files identical despite different names*

