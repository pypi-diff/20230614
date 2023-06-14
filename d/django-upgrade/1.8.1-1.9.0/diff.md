# Comparing `tmp/django-upgrade-1.8.1.tar.gz` & `tmp/django-upgrade-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-upgrade-1.8.1.tar", last modified: Thu Aug 25 08:29:23 2022, max compression
+gzip compressed data, was "django-upgrade-1.9.0.tar", last modified: Thu Aug 25 13:50:25 2022, max compression
```

## Comparing `django-upgrade-1.8.1.tar` & `django-upgrade-1.9.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-25 08:29:23.831058 django-upgrade-1.8.1/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4871 2022-08-25 08:29:21.000000 django-upgrade-1.8.1/HISTORY.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:00.000000 django-upgrade-1.8.1/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      101 2022-06-03 11:59:00.000000 django-upgrade-1.8.1/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)    16579 2022-08-25 08:29:23.831174 django-upgrade-1.8.1/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)    15330 2022-08-15 08:19:46.000000 django-upgrade-1.8.1/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      459 2022-08-15 08:50:18.000000 django-upgrade-1.8.1/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1609 2022-08-25 08:29:23.831648 django-upgrade-1.8.1/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-25 08:29:23.825950 django-upgrade-1.8.1/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-25 08:29:23.827769 django-upgrade-1.8.1/src/django_upgrade/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      150 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/__main__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      652 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/ast.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      322 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/compat.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4440 2022-08-15 08:19:46.000000 django-upgrade-1.8.1/src/django_upgrade/data.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-25 08:29:23.830943 django-upgrade-1.8.1/src/django_upgrade/fixers/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1386 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/compatibility_imports_1_11.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1135 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/compatibility_imports_1_9.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1690 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/crypto_get_random_string.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1198 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/default_app_config.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4613 2022-08-15 08:19:46.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/django_urls.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1430 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/email_validator.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1620 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/jsonfield.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2537 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/null_boolean_field.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1921 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/on_delete.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1244 2022-07-05 08:51:06.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/password_reset_timeout_days.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1585 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/postgres_float_range_field.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1810 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/queryset_paginator.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3031 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/request_headers.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2682 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/signal_providing_args.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1483 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/testcase_databases.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2668 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/timezone_fixedoffset.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1834 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/utils_encoding.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1054 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/utils_functional.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2879 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/utils_http.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1673 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/utils_text.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1845 2022-08-25 08:28:43.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/utils_timezone.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2024 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/fixers/utils_translation.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3740 2022-08-15 08:51:08.000000 django-upgrade-1.8.1/src/django_upgrade/main.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:02.000000 django-upgrade-1.8.1/src/django_upgrade/py.typed
--rw-r--r--   0 adamjohnson   (501) staff       (20)     9077 2022-08-15 08:51:05.000000 django-upgrade-1.8.1/src/django_upgrade/tokens.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-25 08:29:23.828493 django-upgrade-1.8.1/src/django_upgrade.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    16579 2022-08-25 08:29:23.000000 django-upgrade-1.8.1/src/django_upgrade.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1669 2022-08-25 08:29:23.000000 django-upgrade-1.8.1/src/django_upgrade.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-08-25 08:29:23.000000 django-upgrade-1.8.1/src/django_upgrade.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       60 2022-08-25 08:29:23.000000 django-upgrade-1.8.1/src/django_upgrade.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-08-25 08:29:23.000000 django-upgrade-1.8.1/src/django_upgrade.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       19 2022-08-25 08:29:23.000000 django-upgrade-1.8.1/src/django_upgrade.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       15 2022-08-25 08:29:23.000000 django-upgrade-1.8.1/src/django_upgrade.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-25 13:50:25.447633 django-upgrade-1.9.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5482 2022-08-25 13:50:23.000000 django-upgrade-1.9.0/HISTORY.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:00.000000 django-upgrade-1.9.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      101 2022-06-03 11:59:00.000000 django-upgrade-1.9.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    18633 2022-08-25 13:50:25.447737 django-upgrade-1.9.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    17384 2022-08-25 13:06:37.000000 django-upgrade-1.9.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      459 2022-08-25 10:42:51.000000 django-upgrade-1.9.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1609 2022-08-25 13:50:25.448134 django-upgrade-1.9.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-25 13:50:25.442361 django-upgrade-1.9.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-25 13:50:25.443843 django-upgrade-1.9.0/src/django_upgrade/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      150 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/__main__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      652 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/ast.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      322 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/compat.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4440 2022-08-25 10:58:47.000000 django-upgrade-1.9.0/src/django_upgrade/data.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-25 13:50:25.447470 django-upgrade-1.9.0/src/django_upgrade/fixers/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1386 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/compatibility_imports_1_11.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1135 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/compatibility_imports_1_9.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1690 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/crypto_get_random_string.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1017 2022-08-25 10:42:51.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/default_app_config.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5963 2022-08-25 13:27:18.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/django_urls.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1430 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/email_validator.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1620 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/jsonfield.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2537 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/null_boolean_field.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1921 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/on_delete.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1244 2022-08-25 08:50:39.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/password_reset_timeout_days.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1585 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/postgres_float_range_field.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1810 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/queryset_paginator.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3031 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/request_headers.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2682 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/signal_providing_args.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1459 2022-08-25 10:42:51.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/testcase_databases.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2668 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/timezone_fixedoffset.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      983 2022-08-25 10:42:51.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/use_l10n.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1834 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/utils_encoding.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1054 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/utils_functional.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2879 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/utils_http.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1673 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/utils_text.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1845 2022-08-25 10:42:51.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/utils_timezone.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2024 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/utils_translation.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3418 2022-08-25 10:42:51.000000 django-upgrade-1.9.0/src/django_upgrade/fixers/versioned_branches.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3740 2022-08-25 10:42:51.000000 django-upgrade-1.9.0/src/django_upgrade/main.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:02.000000 django-upgrade-1.9.0/src/django_upgrade/py.typed
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    14141 2022-08-25 10:42:51.000000 django-upgrade-1.9.0/src/django_upgrade/tokens.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-25 13:50:25.444633 django-upgrade-1.9.0/src/django_upgrade.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    18633 2022-08-25 13:50:25.000000 django-upgrade-1.9.0/src/django_upgrade.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1755 2022-08-25 13:50:25.000000 django-upgrade-1.9.0/src/django_upgrade.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-08-25 13:50:25.000000 django-upgrade-1.9.0/src/django_upgrade.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       60 2022-08-25 13:50:25.000000 django-upgrade-1.9.0/src/django_upgrade.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-08-25 13:50:25.000000 django-upgrade-1.9.0/src/django_upgrade.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       19 2022-08-25 13:50:25.000000 django-upgrade-1.9.0/src/django_upgrade.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       15 2022-08-25 13:50:25.000000 django-upgrade-1.9.0/src/django_upgrade.egg-info/top_level.txt
```

### Comparing `django-upgrade-1.8.1/HISTORY.rst` & `django-upgrade-1.9.0/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 =======
 History
 =======
 
+1.9.0 (2022-08-25)
+------------------
+
+* Add Django 4.0+ fixer to remove ``USE_L10N = True`` setting.
+
+  Thanks to Johnny Metz in `PR #173 <https://github.com/adamchainz/django-upgrade/pull/173>`__.
+
+* Add fixer to remove outdated blocks based on comparing ``django.VERSION`` to old versions:
+
+  .. code-block:: diff
+
+      -if django.VERSION > (4, 1):
+      -    constraint.validate()
+      +constraint.validate()
+
+* Update Django 2.0+ URL fixer to rewrite ``re_path()`` calls into ``path()`` when eligible.
+
+  Thanks to Thibaut Decombe in `PR #167 <https://github.com/adamchainz/django-upgrade/pull/167>`__.
+
 1.8.1 (2022-08-25)
 ------------------
 
 * Fix ``timezone.utc`` fixer to import and use ``timezone.utc`` correctly.
 
   Thanks to Víðir Valberg Guðmundsson for the report in `Issue #172 <https://github.com/adamchainz/django-upgrade/issues/172>`__.
```

### Comparing `django-upgrade-1.8.1/LICENSE` & `django-upgrade-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/PKG-INFO` & `django-upgrade-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-upgrade
-Version: 1.8.1
+Version: 1.9.0
 Summary: Automatically upgrade your Django projects.
 Home-page: https://github.com/adamchainz/django-upgrade
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-upgrade/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
@@ -67,15 +67,15 @@
 
 .. code-block:: yaml
 
     -   repo: https://github.com/adamchainz/django-upgrade
         rev: ''  # replace with latest tag on GitHub
         hooks:
         -   id: django-upgrade
-            args: [--target-version, "3.2"]   # Replace with Django version
+            args: [--target-version, "4.1"]   # Replace with Django version
 
 ----
 
 **Want to improve your code quality?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers using  pre-commit, django-upgrade, and many other tools.
 I wrote django-upgrade whilst working on the book!
 
@@ -87,15 +87,15 @@
 ``django-upgrade`` is a commandline tool that rewrites files in place.
 Pass your Django version as ``<major>.<minor>`` to the ``--target-version`` flag.
 The built-in fixers will rewrite your code to avoid some ``DeprecationWarning``\s and use some new features on your Django version.
 For example:
 
 .. code-block:: sh
 
-    django-upgrade --target-version 3.2 example/core/models.py example/settings.py
+    django-upgrade --target-version 4.1 example/core/models.py example/settings.py
 
 The ``--target-version`` flag defaults to 2.2, the oldest supported version when this project was created.
 For more on usage run ``django-upgrade --help``.
 
 ``django-upgrade`` focuses on upgrading your code and not on making it look nice.
 Run django-upgrade before formatters like `Black <https://black.readthedocs.io/en/stable/>`__.
 
@@ -119,14 +119,47 @@
 
 For a quick benchmark: running django-codemod against a medium Django repository with 153k lines of Python takes 133 seconds.
 pyupgrade and django-upgrade both take less than 0.5 seconds.
 
 Fixers
 ======
 
+All Versions
+------------
+
+The below fixers run regardless of the target version.
+
+Versioned blocks
+~~~~~~~~~~~~~~~~
+
+Removes outdated comparisons and blocks from ``if`` statements comparing to ``django.VERSION``.
+Supports comparisons of the form:
+
+.. code-block:: text
+
+    if django.VERSION <comparator> (<X>, <Y>):
+        ...
+
+Where ``<comparator>`` is one of ``<``, ``<=`` , ``>``, or ``>=``, and ``<X>`` and ``<Y>`` are integer literals.
+A single ``else`` block may be present, but ``elif`` is not supported.
+
+.. code-block:: diff
+
+    -if django.VERSION < (4, 1):
+    -    class RenameIndex:
+    -        ...
+
+    -if django.VERSION >= (4, 1):
+    -    constraint.validate()
+    -else:
+    -    custom_validation(constraint)
+    +constraint.validate()
+
+See also `pyupgrade’s similar feature <https://github.com/asottile/pyupgrade/#python2-and-old-python3x-blocks>`__ that removes outdated code from checks on the Python version.
+
 Django 1.9
 -----------
 
 `Release Notes <https://github.com/django/django/blob/main/docs/releases/1.9.txt>`__
 
 ``on_delete`` argument
 ~~~~~~~~~~~~~~~~~~~~~~
@@ -189,28 +222,46 @@
 
 Rewrites imports of ``include()`` and ``url()`` from ``django.conf.urls`` to ``django.urls``.
 ``url()`` calls using compatible regexes are rewritten to the |new path() syntax|__, otherwise they are converted to call ``re_path()``.
 
 .. |new path() syntax| replace:: new ``path()`` syntax
 __ https://docs.djangoproject.com/en/2.0/releases/2.0/#simplified-url-routing-syntax
 
+For some cases, this change alters the type of the arguments passed to the view, from ``str`` to the converted type (e.g. ``int``).
+This is not guaranteed backwards compatible: there is a chance that the view expects a string, rather than the converted type.
+But, pragmatically, it seems 99.9% of views do not require strings, and instead work with either strings or the converted type.
+Thus, you should test affected paths after this fixer makes any changes.
+
 .. code-block:: diff
 
     -from django.conf.urls import include, url
     +from django.urls import include, path, re_path
 
      urlpatterns = [
     -    url(r'^$', views.index, name='index'),
     +    path('', views.index, name='index'),
     -    url(r'^about/$', views.about, name='about'),
     +    path('about/', views.about, name='about'),
     -    url(r'^post/(?P<slug>[-a-zA-Z0-9_]+)/$', views.post, name='post'),
-    +    re_path(r'^post/(?P<slug>[w-]+)/$', views.post, name='post'),
-    -    url(r'^weblog/', include('blog.urls')),
-    +    path('weblog/', include('blog.urls')),
+    +    path('post/<slug:slug>/', views.post, name='post'),
+    -    url(r'^weblog', include('blog.urls')),
+    +    re_path(r'^weblog', include('blog.urls')),
+     ]
+
+Existing ``re_path()`` calls are also rewritten to the ``path()`` syntax when eligible.
+
+.. code-block:: diff
+
+    -from django.urls import include, re_path
+    +from django.urls import include, path, re_path
+
+     urlpatterns = [
+    -    re_path(r'^about/$', views.about, name='about'),
+    +    path('about/', views.about, name='about'),
+         re_path(r'^post/(?P<slug>[w-]+)/$', views.post, name='post'),
      ]
 
 ``lru_cache``
 ~~~~~~~~~~~~~
 
 Rewrites imports of ``lru_cache`` from ``django.utils.functional`` to use ``functools``.
 
@@ -461,16 +512,25 @@
     -default_app_config = 'my_app.apps.AppConfig'
 
 Django 4.0
 ----------
 
 `Release Notes <https://docs.djangoproject.com/en/4.0/releases/4.0/#features-deprecated-in-4-0>`__
 
-There are no fixers for Django 4.0 at current.
-Most of its deprecations don’t seem automatically fixable.
+``USE_L10N``
+~~~~~~~~~~~~
+
+Removes the deprecated ``USE_L10N`` setting if set to its default value of ``True``.
+
+Settings files are heuristically detected as modules with the whole word “settings” somewhere in their path.
+For example ``myproject/settings.py`` or ``myproject/settings/production.py``.
+
+.. code-block:: diff
+
+    -USE_L10N = True
 
 Django 4.1
 ----------
 
 `Release Notes <https://docs.djangoproject.com/en/4.1/releases/4.1/#features-deprecated-in-4-1>`__
 
 ``django.utils.timezone.utc`` deprecations
```

### Comparing `django-upgrade-1.8.1/README.rst` & `django-upgrade-1.9.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 .. code-block:: yaml
 
     -   repo: https://github.com/adamchainz/django-upgrade
         rev: ''  # replace with latest tag on GitHub
         hooks:
         -   id: django-upgrade
-            args: [--target-version, "3.2"]   # Replace with Django version
+            args: [--target-version, "4.1"]   # Replace with Django version
 
 ----
 
 **Want to improve your code quality?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers using  pre-commit, django-upgrade, and many other tools.
 I wrote django-upgrade whilst working on the book!
 
@@ -55,15 +55,15 @@
 ``django-upgrade`` is a commandline tool that rewrites files in place.
 Pass your Django version as ``<major>.<minor>`` to the ``--target-version`` flag.
 The built-in fixers will rewrite your code to avoid some ``DeprecationWarning``\s and use some new features on your Django version.
 For example:
 
 .. code-block:: sh
 
-    django-upgrade --target-version 3.2 example/core/models.py example/settings.py
+    django-upgrade --target-version 4.1 example/core/models.py example/settings.py
 
 The ``--target-version`` flag defaults to 2.2, the oldest supported version when this project was created.
 For more on usage run ``django-upgrade --help``.
 
 ``django-upgrade`` focuses on upgrading your code and not on making it look nice.
 Run django-upgrade before formatters like `Black <https://black.readthedocs.io/en/stable/>`__.
 
@@ -87,14 +87,47 @@
 
 For a quick benchmark: running django-codemod against a medium Django repository with 153k lines of Python takes 133 seconds.
 pyupgrade and django-upgrade both take less than 0.5 seconds.
 
 Fixers
 ======
 
+All Versions
+------------
+
+The below fixers run regardless of the target version.
+
+Versioned blocks
+~~~~~~~~~~~~~~~~
+
+Removes outdated comparisons and blocks from ``if`` statements comparing to ``django.VERSION``.
+Supports comparisons of the form:
+
+.. code-block:: text
+
+    if django.VERSION <comparator> (<X>, <Y>):
+        ...
+
+Where ``<comparator>`` is one of ``<``, ``<=`` , ``>``, or ``>=``, and ``<X>`` and ``<Y>`` are integer literals.
+A single ``else`` block may be present, but ``elif`` is not supported.
+
+.. code-block:: diff
+
+    -if django.VERSION < (4, 1):
+    -    class RenameIndex:
+    -        ...
+
+    -if django.VERSION >= (4, 1):
+    -    constraint.validate()
+    -else:
+    -    custom_validation(constraint)
+    +constraint.validate()
+
+See also `pyupgrade’s similar feature <https://github.com/asottile/pyupgrade/#python2-and-old-python3x-blocks>`__ that removes outdated code from checks on the Python version.
+
 Django 1.9
 -----------
 
 `Release Notes <https://github.com/django/django/blob/main/docs/releases/1.9.txt>`__
 
 ``on_delete`` argument
 ~~~~~~~~~~~~~~~~~~~~~~
@@ -157,28 +190,46 @@
 
 Rewrites imports of ``include()`` and ``url()`` from ``django.conf.urls`` to ``django.urls``.
 ``url()`` calls using compatible regexes are rewritten to the |new path() syntax|__, otherwise they are converted to call ``re_path()``.
 
 .. |new path() syntax| replace:: new ``path()`` syntax
 __ https://docs.djangoproject.com/en/2.0/releases/2.0/#simplified-url-routing-syntax
 
+For some cases, this change alters the type of the arguments passed to the view, from ``str`` to the converted type (e.g. ``int``).
+This is not guaranteed backwards compatible: there is a chance that the view expects a string, rather than the converted type.
+But, pragmatically, it seems 99.9% of views do not require strings, and instead work with either strings or the converted type.
+Thus, you should test affected paths after this fixer makes any changes.
+
 .. code-block:: diff
 
     -from django.conf.urls import include, url
     +from django.urls import include, path, re_path
 
      urlpatterns = [
     -    url(r'^$', views.index, name='index'),
     +    path('', views.index, name='index'),
     -    url(r'^about/$', views.about, name='about'),
     +    path('about/', views.about, name='about'),
     -    url(r'^post/(?P<slug>[-a-zA-Z0-9_]+)/$', views.post, name='post'),
-    +    re_path(r'^post/(?P<slug>[w-]+)/$', views.post, name='post'),
-    -    url(r'^weblog/', include('blog.urls')),
-    +    path('weblog/', include('blog.urls')),
+    +    path('post/<slug:slug>/', views.post, name='post'),
+    -    url(r'^weblog', include('blog.urls')),
+    +    re_path(r'^weblog', include('blog.urls')),
+     ]
+
+Existing ``re_path()`` calls are also rewritten to the ``path()`` syntax when eligible.
+
+.. code-block:: diff
+
+    -from django.urls import include, re_path
+    +from django.urls import include, path, re_path
+
+     urlpatterns = [
+    -    re_path(r'^about/$', views.about, name='about'),
+    +    path('about/', views.about, name='about'),
+         re_path(r'^post/(?P<slug>[w-]+)/$', views.post, name='post'),
      ]
 
 ``lru_cache``
 ~~~~~~~~~~~~~
 
 Rewrites imports of ``lru_cache`` from ``django.utils.functional`` to use ``functools``.
 
@@ -429,16 +480,25 @@
     -default_app_config = 'my_app.apps.AppConfig'
 
 Django 4.0
 ----------
 
 `Release Notes <https://docs.djangoproject.com/en/4.0/releases/4.0/#features-deprecated-in-4-0>`__
 
-There are no fixers for Django 4.0 at current.
-Most of its deprecations don’t seem automatically fixable.
+``USE_L10N``
+~~~~~~~~~~~~
+
+Removes the deprecated ``USE_L10N`` setting if set to its default value of ``True``.
+
+Settings files are heuristically detected as modules with the whole word “settings” somewhere in their path.
+For example ``myproject/settings.py`` or ``myproject/settings/production.py``.
+
+.. code-block:: diff
+
+    -USE_L10N = True
 
 Django 4.1
 ----------
 
 `Release Notes <https://docs.djangoproject.com/en/4.1/releases/4.1/#features-deprecated-in-4-1>`__
 
 ``django.utils.timezone.utc`` deprecations
```

### Comparing `django-upgrade-1.8.1/setup.cfg` & `django-upgrade-1.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-upgrade
-version = 1.8.1
+version = 1.9.0
 description = Automatically upgrade your Django projects.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Adam Johnson
 author_email = me@adamj.eu
 url = https://github.com/adamchainz/django-upgrade
 project_urls =
```

### Comparing `django-upgrade-1.8.1/src/django_upgrade/ast.py` & `django-upgrade-1.9.0/src/django_upgrade/ast.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/data.py` & `django-upgrade-1.9.0/src/django_upgrade/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         return test_re.search(self.filename) is not None
 
     def looks_like_dunder_init_file(self) -> bool:
         return dunder_init_re.search(self.filename) is not None
 
 
 AST_T = TypeVar("AST_T", bound=ast.AST)
-TokenFunc = Callable[[int, List[Token]], None]
+TokenFunc = Callable[[List[Token], int], None]
 ASTFunc = Callable[[State, AST_T, ast.AST], Iterable[Tuple[Offset, TokenFunc]]]
 
 if TYPE_CHECKING:  # pragma: no cover
     from typing import Protocol
 else:
     Protocol = object
```

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/compatibility_imports_1_11.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/compatibility_imports_1_11.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/compatibility_imports_1_9.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/compatibility_imports_1_9.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/crypto_get_random_string.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/crypto_get_random_string.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/default_app_config.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/default_app_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 """
 from __future__ import annotations
 
 import ast
 from functools import partial
 from typing import Iterable
 
-from tokenize_rt import Offset, Token
+from tokenize_rt import Offset
 
 from django_upgrade.ast import ast_start_offset
 from django_upgrade.data import Fixer, State, TokenFunc
-from django_upgrade.tokens import LOGICAL_NEWLINE, find
+from django_upgrade.tokens import erase_node
 
 fixer = Fixer(
     __name__,
     min_version=(3, 2),
 )
 
 
@@ -31,13 +31,8 @@
         and isinstance(parent, ast.Module)
         and len(node.targets) == 1
         and isinstance(node.targets[0], ast.Name)
         and node.targets[0].id == "default_app_config"
         and isinstance(node.value, ast.Constant)
         and isinstance(node.value.value, str)
     ):
-        yield ast_start_offset(node), partial(remove_assignment, node=node)
-
-
-def remove_assignment(tokens: list[Token], i: int, *, node: ast.Assign) -> None:
-    j = find(tokens, i, name=LOGICAL_NEWLINE)
-    tokens[i : j + 1] = []
+        yield ast_start_offset(node), partial(erase_node, node=node)
```

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/django_urls.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/django_urls.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from tokenize_rt import Offset, Token
 
 from django_upgrade.ast import ast_start_offset, is_rewritable_import_from
 from django_upgrade.compat import str_removeprefix
 from django_upgrade.data import Fixer, State, TokenFunc
 from django_upgrade.tokens import (
     STRING,
+    erase_node,
     extract_indent,
     find,
     insert,
     replace,
     update_import_names,
 )
 
@@ -38,53 +39,80 @@
 ) -> Iterable[tuple[Offset, TokenFunc]]:
     if (
         node.module == "django.conf.urls"
         and is_rewritable_import_from(node)
         and any(alias.name in ("include", "url") for alias in node.names)
     ):
         yield ast_start_offset(node), partial(
-            update_import,
+            update_django_conf_import,
+            node=node,
+            state=state,
+        )
+    elif (
+        node.module == "django.urls"
+        and is_rewritable_import_from(node)
+        and any(alias.name == "re_path" for alias in node.names)
+    ):
+        yield ast_start_offset(node), partial(
+            update_django_urls_import,
             node=node,
             state=state,
         )
 
 
 # Track which of path and re_path have been used for this current file
 # Then when backtracking into an import statement, we can use the set of names
 # to determine what names to import.
 state_used_names: MutableMapping[State, set[str]] = WeakKeyDictionary()
 
 
-def update_import(
+def update_django_conf_import(
     tokens: list[Token], i: int, *, node: ast.ImportFrom, state: State
 ) -> None:
-    """ """
-    removals = set()
-    additions = set()
+    re_path_imported = "re_path" in state.from_imports["django.urls"]
     used_names = state_used_names.pop(state, set())
+    removals = set()
 
     for alias in node.names:
         if alias.asname is not None:
             continue
-        if alias.name == "include":
-            removals.add("include")
-            additions.add("include")
-        elif alias.name == "url" and used_names:
-            removals.add("url")
-            additions.update(used_names)
+        if alias.name in ("include", "url") and (used_names or re_path_imported):
+            removals.add(alias.name)
 
     if removals:
         j, indent = extract_indent(tokens, i)
         update_import_names(
             tokens,
             i,
             node=node,
             name_map={name: "" for name in removals},
         )
-        joined_names = ", ".join(sorted(additions))
+        if not re_path_imported:
+            joined_names = ", ".join(sorted(used_names))
+            insert(
+                tokens,
+                j,
+                new_src=f"{indent}from django.urls import {joined_names}\n",
+            )
+        else:
+            state_used_names[state] = used_names
+
+
+def update_django_urls_import(
+    tokens: list[Token], i: int, *, node: ast.ImportFrom, state: State
+) -> None:
+    used_names = state_used_names.pop(state, set())
+
+    if used_names:
+        initial_names = state.from_imports["django.urls"] - {"re_path"}
+        used_names.update(initial_names)
+
+        j, indent = extract_indent(tokens, i)
+        erase_node(tokens, i, node=node)
+        joined_names = ", ".join(sorted(used_names))
         insert(
             tokens,
             j,
             new_src=f"{indent}from django.urls import {joined_names}\n",
         )
 
 
@@ -92,16 +120,21 @@
 def visit_Call(
     state: State,
     node: ast.Call,
     parent: ast.AST,
 ) -> Iterable[tuple[Offset, TokenFunc]]:
     if (
         isinstance(node.func, ast.Name)
-        and node.func.id == "url"
-        and "url" in state.from_imports["django.conf.urls"]
+        and (
+            (node.func.id == "url" and "url" in state.from_imports["django.conf.urls"])
+            or (
+                node.func.id == "re_path"
+                and "re_path" in state.from_imports["django.urls"]
+            )
+        )
         # cannot convert where called with all kwargs as names don't align
         and len(node.args) >= 1
     ):
         regex_path: str | None = None
         if isinstance(node.args[0], ast.Constant) and isinstance(
             node.args[0].value, str
         ):
@@ -109,14 +142,21 @@
 
         yield ast_start_offset(node), partial(
             fix_url_call,
             regex_path=regex_path,
             state=state,
         )
 
+    if (
+        isinstance(node.func, ast.Name)
+        and node.func.id == "include"
+        and "include" in state.from_imports["django.conf.urls"]
+    ):
+        state_used_names.setdefault(state, set()).add("include")
+
 
 def fix_url_call(
     tokens: list[Token], i: int, *, regex_path: str | None, state: State
 ) -> None:
     new_name = "re_path"
     if regex_path is not None:
         path = convert_path_syntax(regex_path)
```

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/email_validator.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/email_validator.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/jsonfield.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/jsonfield.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/null_boolean_field.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/null_boolean_field.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/on_delete.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/on_delete.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/password_reset_timeout_days.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/password_reset_timeout_days.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/postgres_float_range_field.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/postgres_float_range_field.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/queryset_paginator.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/queryset_paginator.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/request_headers.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/request_headers.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/signal_providing_args.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/signal_providing_args.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/testcase_databases.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/testcase_databases.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,14 @@
             replace_assignment, node=node, value=node.value.value
         )
 
 
 def replace_assignment(
     tokens: list[Token], i: int, *, node: ast.Assign, value: bool
 ) -> None:
-    print("???", value)
     new_src = "databases = "
     if value:
         new_src += '"__all__"'
     else:
         new_src += "[]"
     j = find_final_token(tokens, i, node=node)
     tokens[i:j] = [Token(name=CODE, src=new_src)]
```

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/timezone_fixedoffset.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/timezone_fixedoffset.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/utils_encoding.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/utils_encoding.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/utils_functional.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/utils_functional.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/utils_http.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/utils_http.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/utils_text.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/utils_text.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/utils_timezone.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/utils_timezone.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/fixers/utils_translation.py` & `django-upgrade-1.9.0/src/django_upgrade/fixers/utils_translation.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/main.py` & `django-upgrade-1.9.0/src/django_upgrade/main.py`

 * *Files identical despite different names*

### Comparing `django-upgrade-1.8.1/src/django_upgrade/tokens.py` & `django-upgrade-1.9.0/src/django_upgrade/tokens.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import ast
 from collections import defaultdict
 
-from tokenize_rt import UNIMPORTANT_WS, Token, tokens_to_src
+from tokenize_rt import NON_CODING_TOKENS, UNIMPORTANT_WS, Token, tokens_to_src
 
 # Token name aliases
 CODE = "CODE"  # Token name meaning 'replaced by us'
 COMMENT = "COMMENT"
 DEDENT = "DEDENT"
 INDENT = "INDENT"
 LOGICAL_NEWLINE = "NEWLINE"
@@ -97,15 +97,15 @@
     return (  # type: ignore [no-any-return]
         tokens[start_idx - 2].name == PHYSICAL_NEWLINE
         and tokens[start_idx - 1].name == UNIMPORTANT_WS
         and tokens[end_idx + 1].name == PHYSICAL_NEWLINE
     )
 
 
-# More complex mini-parser functions
+# More complex mini-parsers
 
 
 BRACES = {"(": ")", "[": "]", "{": "}"}
 
 
 def parse_call_args(
     tokens: list[Token],
@@ -136,14 +136,170 @@
                 args.append((arg_start, i))
 
         i += 1
 
     return args, i
 
 
+BRACES = {"(": ")", "[": "]", "{": "}"}
+OPENING, CLOSING = frozenset(BRACES), frozenset(BRACES.values())
+
+
+def find_block_start(tokens: list[Token], i: int) -> int:
+    depth = 0
+    while depth or tokens[i].src != ":":
+        if tokens[i].src in OPENING:
+            depth += 1
+        elif tokens[i].src in CLOSING:
+            depth -= 1
+        i += 1
+    return i
+
+
+class Block:  # pragma: no cover
+    """
+    Adapted from pyupgrade:
+    https://github.com/asottile/pyupgrade/blob/ad5d9db9a206bfd221760fd81e407bf6040c808c/pyupgrade/_token_helpers.py#L179
+
+    Copyright (c) 2017 Anthony Sottile
+
+    MIT Licensed
+    """
+
+    def __init__(
+        self, start: int, colon: int, block: int, end: int, line: bool
+    ) -> None:
+        self.start = start
+        self.colon = colon
+        self.block = block
+        self.end = end
+        self.line = line
+
+    def _initial_indent(self, tokens: list[Token]) -> int:
+        if tokens[self.start].src.isspace():
+            return len(tokens[self.start].src)
+        else:
+            return 0
+
+    def _minimum_indent(self, tokens: list[Token]) -> int:
+        block_indent: int | None = None
+        for i in range(self.block, self.end):
+            if (
+                tokens[i - 1].name in ("NL", "NEWLINE")
+                and tokens[i].name in ("INDENT", UNIMPORTANT_WS)
+                and
+                # comments can have arbitrary indentation so ignore them
+                tokens[i + 1].name != "COMMENT"
+            ):
+                token_indent = len(tokens[i].src)
+                if block_indent is None:
+                    block_indent = token_indent
+                else:
+                    block_indent = min(block_indent, token_indent)
+
+        assert block_indent is not None
+        return block_indent
+
+    def dedent(self, tokens: list[Token]) -> None:
+        if self.line:
+            return
+        initial_indent = self._initial_indent(tokens)
+        diff = self._minimum_indent(tokens) - initial_indent
+        for i in range(self.block, self.end):
+            if tokens[i - 1].name in ("DEDENT", "NL", "NEWLINE") and tokens[i].name in (
+                "INDENT",
+                UNIMPORTANT_WS,
+            ):
+                # make sure we preserve *at least* the initial indent
+                s = tokens[i].src
+                s = s[:initial_indent] + s[initial_indent + diff :]
+                tokens[i] = tokens[i]._replace(src=s)
+
+    def replace_condition(self, tokens: list[Token], new: list[Token]) -> None:
+        start = self.start
+        while tokens[start].name == "UNIMPORTANT_WS":
+            start += 1
+        tokens[start : self.colon] = new
+
+    def _trim_end(self, tokens: list[Token]) -> Block:
+        """the tokenizer reports the end of the block at the beginning of
+        the next block
+        """
+        i = last_token = self.end - 1
+        while tokens[i].name in NON_CODING_TOKENS | {"DEDENT", "NEWLINE"}:
+            # if we find an indented comment inside our block, keep it
+            if (
+                tokens[i].name in {"NL", "NEWLINE"}
+                and tokens[i + 1].name == UNIMPORTANT_WS
+                and len(tokens[i + 1].src) > self._initial_indent(tokens)
+            ):
+                break
+            # otherwise we've found another line to remove
+            elif tokens[i].name in {"NL", "NEWLINE"}:
+                last_token = i
+            i -= 1
+        return self.__class__(
+            start=self.start,
+            colon=self.colon,
+            block=self.block,
+            end=last_token + 1,
+            line=self.line,
+        )
+
+    @classmethod
+    def find(
+        cls,
+        tokens: list[Token],
+        i: int,
+        trim_end: bool = False,
+    ) -> Block:
+        if i > 0 and tokens[i - 1].name in {"INDENT", UNIMPORTANT_WS}:
+            i -= 1
+        start = i
+        colon = find_block_start(tokens, i)
+
+        j = colon + 1
+        while tokens[j].name != "NEWLINE" and tokens[j].name in NON_CODING_TOKENS:
+            j += 1
+
+        if tokens[j].name == "NEWLINE":  # multi line block
+            block = j + 1
+            while tokens[j].name != "INDENT":
+                j += 1
+            level = 1
+            j += 1
+            while level:
+                level += {"INDENT": 1, "DEDENT": -1}.get(tokens[j].name, 0)
+                j += 1
+            ret = cls(start, colon, block, j, line=False)
+            if trim_end:
+                return ret._trim_end(tokens)
+            else:
+                return ret
+        else:  # single line block
+            block = j
+            j = find_end(tokens, j)
+            return cls(start, colon, block, j, line=True)
+
+
+def find_end(tokens: list[Token], i: int) -> int:  # pragma: no cover
+    while tokens[i].name not in {"NEWLINE", "ENDMARKER"}:
+        i += 1
+
+    # depending on the version of python, some will not emit
+    # NEWLINE('') at the end of a file which does not end with a
+    # newline (for example 3.7.0)
+    if tokens[i].name == "ENDMARKER":
+        i -= 1
+    else:
+        i += 1
+
+    return i
+
+
 # Rewriting functions
 
 
 def insert(tokens: list[Token], i: int, *, new_src: str) -> None:
     """
     Insert a generated token with the given new source.
     """
```

### Comparing `django-upgrade-1.8.1/src/django_upgrade.egg-info/PKG-INFO` & `django-upgrade-1.9.0/src/django_upgrade.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-upgrade
-Version: 1.8.1
+Version: 1.9.0
 Summary: Automatically upgrade your Django projects.
 Home-page: https://github.com/adamchainz/django-upgrade
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-upgrade/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
@@ -67,15 +67,15 @@
 
 .. code-block:: yaml
 
     -   repo: https://github.com/adamchainz/django-upgrade
         rev: ''  # replace with latest tag on GitHub
         hooks:
         -   id: django-upgrade
-            args: [--target-version, "3.2"]   # Replace with Django version
+            args: [--target-version, "4.1"]   # Replace with Django version
 
 ----
 
 **Want to improve your code quality?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers using  pre-commit, django-upgrade, and many other tools.
 I wrote django-upgrade whilst working on the book!
 
@@ -87,15 +87,15 @@
 ``django-upgrade`` is a commandline tool that rewrites files in place.
 Pass your Django version as ``<major>.<minor>`` to the ``--target-version`` flag.
 The built-in fixers will rewrite your code to avoid some ``DeprecationWarning``\s and use some new features on your Django version.
 For example:
 
 .. code-block:: sh
 
-    django-upgrade --target-version 3.2 example/core/models.py example/settings.py
+    django-upgrade --target-version 4.1 example/core/models.py example/settings.py
 
 The ``--target-version`` flag defaults to 2.2, the oldest supported version when this project was created.
 For more on usage run ``django-upgrade --help``.
 
 ``django-upgrade`` focuses on upgrading your code and not on making it look nice.
 Run django-upgrade before formatters like `Black <https://black.readthedocs.io/en/stable/>`__.
 
@@ -119,14 +119,47 @@
 
 For a quick benchmark: running django-codemod against a medium Django repository with 153k lines of Python takes 133 seconds.
 pyupgrade and django-upgrade both take less than 0.5 seconds.
 
 Fixers
 ======
 
+All Versions
+------------
+
+The below fixers run regardless of the target version.
+
+Versioned blocks
+~~~~~~~~~~~~~~~~
+
+Removes outdated comparisons and blocks from ``if`` statements comparing to ``django.VERSION``.
+Supports comparisons of the form:
+
+.. code-block:: text
+
+    if django.VERSION <comparator> (<X>, <Y>):
+        ...
+
+Where ``<comparator>`` is one of ``<``, ``<=`` , ``>``, or ``>=``, and ``<X>`` and ``<Y>`` are integer literals.
+A single ``else`` block may be present, but ``elif`` is not supported.
+
+.. code-block:: diff
+
+    -if django.VERSION < (4, 1):
+    -    class RenameIndex:
+    -        ...
+
+    -if django.VERSION >= (4, 1):
+    -    constraint.validate()
+    -else:
+    -    custom_validation(constraint)
+    +constraint.validate()
+
+See also `pyupgrade’s similar feature <https://github.com/asottile/pyupgrade/#python2-and-old-python3x-blocks>`__ that removes outdated code from checks on the Python version.
+
 Django 1.9
 -----------
 
 `Release Notes <https://github.com/django/django/blob/main/docs/releases/1.9.txt>`__
 
 ``on_delete`` argument
 ~~~~~~~~~~~~~~~~~~~~~~
@@ -189,28 +222,46 @@
 
 Rewrites imports of ``include()`` and ``url()`` from ``django.conf.urls`` to ``django.urls``.
 ``url()`` calls using compatible regexes are rewritten to the |new path() syntax|__, otherwise they are converted to call ``re_path()``.
 
 .. |new path() syntax| replace:: new ``path()`` syntax
 __ https://docs.djangoproject.com/en/2.0/releases/2.0/#simplified-url-routing-syntax
 
+For some cases, this change alters the type of the arguments passed to the view, from ``str`` to the converted type (e.g. ``int``).
+This is not guaranteed backwards compatible: there is a chance that the view expects a string, rather than the converted type.
+But, pragmatically, it seems 99.9% of views do not require strings, and instead work with either strings or the converted type.
+Thus, you should test affected paths after this fixer makes any changes.
+
 .. code-block:: diff
 
     -from django.conf.urls import include, url
     +from django.urls import include, path, re_path
 
      urlpatterns = [
     -    url(r'^$', views.index, name='index'),
     +    path('', views.index, name='index'),
     -    url(r'^about/$', views.about, name='about'),
     +    path('about/', views.about, name='about'),
     -    url(r'^post/(?P<slug>[-a-zA-Z0-9_]+)/$', views.post, name='post'),
-    +    re_path(r'^post/(?P<slug>[w-]+)/$', views.post, name='post'),
-    -    url(r'^weblog/', include('blog.urls')),
-    +    path('weblog/', include('blog.urls')),
+    +    path('post/<slug:slug>/', views.post, name='post'),
+    -    url(r'^weblog', include('blog.urls')),
+    +    re_path(r'^weblog', include('blog.urls')),
+     ]
+
+Existing ``re_path()`` calls are also rewritten to the ``path()`` syntax when eligible.
+
+.. code-block:: diff
+
+    -from django.urls import include, re_path
+    +from django.urls import include, path, re_path
+
+     urlpatterns = [
+    -    re_path(r'^about/$', views.about, name='about'),
+    +    path('about/', views.about, name='about'),
+         re_path(r'^post/(?P<slug>[w-]+)/$', views.post, name='post'),
      ]
 
 ``lru_cache``
 ~~~~~~~~~~~~~
 
 Rewrites imports of ``lru_cache`` from ``django.utils.functional`` to use ``functools``.
 
@@ -461,16 +512,25 @@
     -default_app_config = 'my_app.apps.AppConfig'
 
 Django 4.0
 ----------
 
 `Release Notes <https://docs.djangoproject.com/en/4.0/releases/4.0/#features-deprecated-in-4-0>`__
 
-There are no fixers for Django 4.0 at current.
-Most of its deprecations don’t seem automatically fixable.
+``USE_L10N``
+~~~~~~~~~~~~
+
+Removes the deprecated ``USE_L10N`` setting if set to its default value of ``True``.
+
+Settings files are heuristically detected as modules with the whole word “settings” somewhere in their path.
+For example ``myproject/settings.py`` or ``myproject/settings/production.py``.
+
+.. code-block:: diff
+
+    -USE_L10N = True
 
 Django 4.1
 ----------
 
 `Release Notes <https://docs.djangoproject.com/en/4.1/releases/4.1/#features-deprecated-in-4-1>`__
 
 ``django.utils.timezone.utc`` deprecations
```

### Comparing `django-upgrade-1.8.1/src/django_upgrade.egg-info/SOURCES.txt` & `django-upgrade-1.9.0/src/django_upgrade.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -32,13 +32,15 @@
 src/django_upgrade/fixers/password_reset_timeout_days.py
 src/django_upgrade/fixers/postgres_float_range_field.py
 src/django_upgrade/fixers/queryset_paginator.py
 src/django_upgrade/fixers/request_headers.py
 src/django_upgrade/fixers/signal_providing_args.py
 src/django_upgrade/fixers/testcase_databases.py
 src/django_upgrade/fixers/timezone_fixedoffset.py
+src/django_upgrade/fixers/use_l10n.py
 src/django_upgrade/fixers/utils_encoding.py
 src/django_upgrade/fixers/utils_functional.py
 src/django_upgrade/fixers/utils_http.py
 src/django_upgrade/fixers/utils_text.py
 src/django_upgrade/fixers/utils_timezone.py
-src/django_upgrade/fixers/utils_translation.py
+src/django_upgrade/fixers/utils_translation.py
+src/django_upgrade/fixers/versioned_branches.py
```

