# Comparing `tmp/django-read-only-1.8.0.tar.gz` & `tmp/django-read-only-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-read-only-1.8.0.tar", last modified: Tue May 10 05:16:06 2022, max compression
+gzip compressed data, was "django-read-only-1.9.0.tar", last modified: Sun Jun  5 15:26:46 2022, max compression
```

## Comparing `django-read-only-1.8.0.tar` & `django-read-only-1.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-10 05:16:06.553998 django-read-only-1.8.0/
--rw-r--r--   0 chainz     (501) staff       (20)     1098 2022-05-10 05:15:58.000000 django-read-only-1.8.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1069 2022-01-19 15:29:38.000000 django-read-only-1.8.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      101 2022-04-27 09:19:10.000000 django-read-only-1.8.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)     6158 2022-05-10 05:16:06.554193 django-read-only-1.8.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     5052 2022-05-10 05:15:24.000000 django-read-only-1.8.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      687 2022-01-19 11:13:54.000000 django-read-only-1.8.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1397 2022-05-10 05:16:06.555035 django-read-only-1.8.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       74 2022-01-19 11:13:54.000000 django-read-only-1.8.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-10 05:16:06.546809 django-read-only-1.8.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-10 05:16:06.552022 django-read-only-1.8.0/src/django_read_only/
--rw-r--r--   0 chainz     (501) staff       (20)     2825 2022-05-10 05:15:24.000000 django-read-only-1.8.0/src/django_read_only/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)      103 2022-01-19 11:13:54.000000 django-read-only-1.8.0/src/django_read_only/apps.py
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-14 09:02:31.000000 django-read-only-1.8.0/src/django_read_only/py.typed
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-10 05:16:06.553780 django-read-only-1.8.0/src/django_read_only.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)     6158 2022-05-10 05:16:06.000000 django-read-only-1.8.0/src/django_read_only.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      430 2022-05-10 05:16:06.000000 django-read-only-1.8.0/src/django_read_only.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-10 05:16:06.000000 django-read-only-1.8.0/src/django_read_only.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-10 05:16:04.000000 django-read-only-1.8.0/src/django_read_only.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       12 2022-05-10 05:16:06.000000 django-read-only-1.8.0/src/django_read_only.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)       17 2022-05-10 05:16:06.000000 django-read-only-1.8.0/src/django_read_only.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-06-05 15:26:46.799505 django-read-only-1.9.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1184 2022-06-05 15:26:43.000000 django-read-only-1.9.0/HISTORY.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:58:53.000000 django-read-only-1.9.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      101 2022-06-03 11:58:53.000000 django-read-only-1.9.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6228 2022-06-05 15:26:46.799576 django-read-only-1.9.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5052 2022-06-05 10:48:26.000000 django-read-only-1.9.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      687 2022-06-03 11:58:53.000000 django-read-only-1.9.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1465 2022-06-05 15:26:46.799906 django-read-only-1.9.0/setup.cfg
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       74 2022-06-03 11:58:53.000000 django-read-only-1.9.0/setup.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-06-05 15:26:46.797072 django-read-only-1.9.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-06-05 15:26:46.798648 django-read-only-1.9.0/src/django_read_only/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2825 2022-06-03 11:58:53.000000 django-read-only-1.9.0/src/django_read_only/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2022-06-03 11:58:53.000000 django-read-only-1.9.0/src/django_read_only/apps.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:53.000000 django-read-only-1.9.0/src/django_read_only/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-06-05 15:26:46.799377 django-read-only-1.9.0/src/django_read_only.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6228 2022-06-05 15:26:46.000000 django-read-only-1.9.0/src/django_read_only.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      430 2022-06-05 15:26:46.000000 django-read-only-1.9.0/src/django_read_only.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-06-05 15:26:46.000000 django-read-only-1.9.0/src/django_read_only.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-06-05 15:26:46.000000 django-read-only-1.9.0/src/django_read_only.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2022-06-05 15:26:46.000000 django-read-only-1.9.0/src/django_read_only.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       17 2022-06-05 15:26:46.000000 django-read-only-1.9.0/src/django_read_only.egg-info/top_level.txt
```

### Comparing `django-read-only-1.8.0/LICENSE` & `django-read-only-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-read-only-1.8.0/PKG-INFO` & `django-read-only-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: django-read-only
-Version: 1.8.0
+Version: 1.9.0
 Summary: Disable Django database writes.
 Home-page: https://github.com/adamchainz/django-read-only
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-read-only/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: Django
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ================
 django-read-only
 ================
@@ -48,17 +49,17 @@
    :alt: pre-commit
 
 Disable Django database writes.
 
 Requirements
 ------------
 
-Python 3.7 to 3.10 supported.
+Python 3.7 to 3.11 supported.
 
-Django 3.2 to 4.0 supported.
+Django 3.2 to 4.1 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers django-read-only, IPython, and many other tools.
 
 ----
@@ -155,9 +156,7 @@
 However, this has limitations - Django doesn’t support modifying the ``DATABASES`` setting live, so sessions would not be able to temporarily allow writes.
 
 Instead, django-read-only uses `always installed database instrumentation <https://adamj.eu/tech/2020/07/23/how-to-make-always-installed-django-database-instrumentation/>`__ to inspect executed queries and only allow those which look like reads.
 It uses a “fail closed” philosophy, so anything unknown will fail, which should be fairly reasonable.
 
 Because django-read-only uses Django database instrumentation, it cannot block queries running through the underlying database connection (accesses through ``django.db.connection.connection``), and it cannot filter operations within stored procedures (which use ``connection.callproc()``).
 These are very rare in practice though, so django-read-only’s method works well for most projects.
-
-
```

### Comparing `django-read-only-1.8.0/README.rst` & `django-read-only-1.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,17 @@
    :alt: pre-commit
 
 Disable Django database writes.
 
 Requirements
 ------------
 
-Python 3.7 to 3.10 supported.
+Python 3.7 to 3.11 supported.
 
-Django 3.2 to 4.0 supported.
+Django 3.2 to 4.1 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers django-read-only, IPython, and many other tools.
 
 ----
```

### Comparing `django-read-only-1.8.0/pyproject.toml` & `django-read-only-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-read-only-1.8.0/setup.cfg` & `django-read-only-1.9.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-read-only
-version = 1.8.0
+version = 1.9.0
 description = Disable Django database writes.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Adam Johnson
 author_email = me@adamj.eu
 url = https://github.com/adamchainz/django-read-only
 project_urls = 
@@ -12,24 +12,26 @@
 	Twitter = https://twitter.com/adamchainz
 license = MIT
 keywords = Django
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
+	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 install_requires =
```

### Comparing `django-read-only-1.8.0/src/django_read_only/__init__.py` & `django-read-only-1.9.0/src/django_read_only/__init__.py`

 * *Files identical despite different names*

### Comparing `django-read-only-1.8.0/src/django_read_only.egg-info/PKG-INFO` & `django-read-only-1.9.0/src/django_read_only.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: django-read-only
-Version: 1.8.0
+Version: 1.9.0
 Summary: Disable Django database writes.
 Home-page: https://github.com/adamchainz/django-read-only
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-read-only/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: Django
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ================
 django-read-only
 ================
@@ -48,17 +49,17 @@
    :alt: pre-commit
 
 Disable Django database writes.
 
 Requirements
 ------------
 
-Python 3.7 to 3.10 supported.
+Python 3.7 to 3.11 supported.
 
-Django 3.2 to 4.0 supported.
+Django 3.2 to 4.1 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers django-read-only, IPython, and many other tools.
 
 ----
@@ -155,9 +156,7 @@
 However, this has limitations - Django doesn’t support modifying the ``DATABASES`` setting live, so sessions would not be able to temporarily allow writes.
 
 Instead, django-read-only uses `always installed database instrumentation <https://adamj.eu/tech/2020/07/23/how-to-make-always-installed-django-database-instrumentation/>`__ to inspect executed queries and only allow those which look like reads.
 It uses a “fail closed” philosophy, so anything unknown will fail, which should be fairly reasonable.
 
 Because django-read-only uses Django database instrumentation, it cannot block queries running through the underlying database connection (accesses through ``django.db.connection.connection``), and it cannot filter operations within stored procedures (which use ``connection.callproc()``).
 These are very rare in practice though, so django-read-only’s method works well for most projects.
-
-
```

