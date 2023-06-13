# Comparing `tmp/reactivated-0.9.0.tar.gz` & `tmp/reactivated-3.0.0a64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/reactivated-0.9.0.tar", last modified: Mon Jun 29 12:21:07 2020, max compression
+gzip compressed data, was "dist/reactivated-3.0.0a64.tar", last modified: Wed Sep 30 21:48:02 2020, max compression
```

## Comparing `reactivated-0.9.0.tar` & `reactivated-3.0.0a64.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.033400 reactivated-0.9.0/
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      857 2020-06-29 12:21:07.033103 reactivated-0.9.0/PKG-INFO
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      335 2020-06-01 01:33:20.000000 reactivated-0.9.0/README.md
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.016828 reactivated-0.9.0/reactivated/
--rw-r--r--   0 silviogutierrez   (501) staff       (20)    15477 2020-06-29 12:17:54.000000 reactivated-0.9.0/reactivated/__init__.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/admin.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     3784 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/apps.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     3526 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/backend.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     3005 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/forms.py
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.018445 reactivated-0.9.0/reactivated/management/
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/management/__init__.py
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.019231 reactivated-0.9.0/reactivated/management/commands/
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/management/commands/__init__.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      309 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/management/commands/generate_settings.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      334 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/management/commands/generate_types_schema.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      501 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/middleware.py
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.019641 reactivated-0.9.0/reactivated/migrations/
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/migrations/__init__.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     1571 2020-06-22 16:24:08.000000 reactivated-0.9.0/reactivated/models.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     6614 2020-06-29 12:17:54.000000 reactivated-0.9.0/reactivated/pick.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     3529 2020-06-29 12:17:54.000000 reactivated-0.9.0/reactivated/plugin.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/py.typed
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     1714 2020-06-22 16:24:08.000000 reactivated-0.9.0/reactivated/renderer.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)    21630 2020-06-29 12:17:54.000000 reactivated-0.9.0/reactivated/serialization.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     1043 2020-06-29 12:17:54.000000 reactivated-0.9.0/reactivated/stubs.py
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.007489 reactivated-0.9.0/reactivated/templates/
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.020544 reactivated-0.9.0/reactivated/templates/reactivated/
--rw-r--r--   0 silviogutierrez   (501) staff       (20)       47 2020-06-24 02:35:04.000000 reactivated-0.9.0/reactivated/templates/reactivated/autocomplete
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      695 2020-06-29 12:17:54.000000 reactivated-0.9.0/reactivated/templates/reactivated/interface.html
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     3342 2020-06-29 12:17:54.000000 reactivated-0.9.0/reactivated/templates.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/tests.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     1759 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/utils.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      595 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/views.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     1332 2020-06-01 01:33:20.000000 reactivated-0.9.0/reactivated/widgets.py
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.018175 reactivated-0.9.0/reactivated.egg-info/
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      857 2020-06-29 12:21:06.000000 reactivated-0.9.0/reactivated.egg-info/PKG-INFO
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     1906 2020-06-29 12:21:06.000000 reactivated-0.9.0/reactivated.egg-info/SOURCES.txt
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        1 2020-06-29 12:21:06.000000 reactivated-0.9.0/reactivated.egg-info/dependency_links.txt
--rw-r--r--   0 silviogutierrez   (501) staff       (20)       25 2020-06-29 12:21:06.000000 reactivated-0.9.0/reactivated.egg-info/top_level.txt
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.021052 reactivated-0.9.0/sample/
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/__init__.py
--rwxr-xr-x   0 silviogutierrez   (501) staff       (20)      634 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/manage.py
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.024149 reactivated-0.9.0/sample/server/
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/__init__.py
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.024567 reactivated-0.9.0/sample/server/apps/
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/apps/__init__.py
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.027308 reactivated-0.9.0/sample/server/apps/samples/
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/apps/samples/__init__.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/apps/samples/admin.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)       89 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/apps/samples/apps.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     1097 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/apps/samples/forms.py
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.029771 reactivated-0.9.0/sample/server/apps/samples/migrations/
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     1399 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/apps/samples/migrations/0001_initial.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      376 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/apps/samples/migrations/0002_opera_has_piano_transcription.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     1922 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/apps/samples/migrations/0003_auto_20190913_0303.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     1958 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/apps/samples/migrations/0004_auto_20190913_2051.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      758 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/apps/samples/migrations/0005_auto_20190914_0221.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/apps/samples/migrations/__init__.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     2896 2020-06-22 16:24:08.000000 reactivated-0.9.0/sample/server/apps/samples/models.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      851 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/apps/samples/templates.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/apps/samples/tests.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     3849 2020-06-22 16:24:08.000000 reactivated-0.9.0/sample/server/apps/samples/views.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      126 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/forms.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     3506 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/settings.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     1398 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/urls.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      395 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/views.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      389 2020-06-01 01:33:20.000000 reactivated-0.9.0/sample/server/wsgi.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)       38 2020-06-29 12:21:07.033482 reactivated-0.9.0/setup.cfg
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      764 2020-06-29 12:19:13.000000 reactivated-0.9.0/setup.py
-drwxr-xr-x   0 silviogutierrez   (501) staff       (20)        0 2020-06-29 12:21:07.032569 reactivated-0.9.0/tests/
--rw-r--r--   0 silviogutierrez   (501) staff       (20)        0 2020-06-01 01:33:20.000000 reactivated-0.9.0/tests/__init__.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     1326 2020-06-01 01:33:20.000000 reactivated-0.9.0/tests/autocomplete.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     1071 2020-06-01 01:33:20.000000 reactivated-0.9.0/tests/renderer.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)     4932 2020-06-28 14:31:58.000000 reactivated-0.9.0/tests/serialization.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      931 2020-06-01 01:33:20.000000 reactivated-0.9.0/tests/templates.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)    10844 2020-06-29 12:17:54.000000 reactivated-0.9.0/tests/types.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      123 2020-06-01 01:33:20.000000 reactivated-0.9.0/tests/urls.py
--rw-r--r--   0 silviogutierrez   (501) staff       (20)      622 2020-06-22 16:24:08.000000 reactivated-0.9.0/tests/views.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.839618 reactivated-3.0.0a64/
+-rw-r--r--   0 runner    (1001) docker     (116)      860 2020-09-30 21:48:02.839618 reactivated-3.0.0a64/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      335 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.815618 reactivated-3.0.0a64/packages/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.823618 reactivated-3.0.0a64/packages/reactivated/
+-rw-r--r--   0 runner    (1001) docker     (116)     1589 2020-09-30 21:47:47.000000 reactivated-3.0.0a64/packages/reactivated/package.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.831618 reactivated-3.0.0a64/reactivated/
+-rw-r--r--   0 runner    (1001) docker     (116)    15518 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/admin.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5140 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/apps.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3038 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/backend.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2809 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9164 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/fields.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3574 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.831618 reactivated-3.0.0a64/reactivated/management/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.835618 reactivated-3.0.0a64/reactivated/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      309 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/management/commands/generate_settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)      334 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/management/commands/generate_types_schema.py
+-rw-r--r--   0 runner    (1001) docker     (116)      501 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.835618 reactivated-3.0.0a64/reactivated/migrations/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1571 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/models.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6614 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/pick.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3529 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/py.typed
+-rw-r--r--   0 runner    (1001) docker     (116)     1714 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24693 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1043 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.819618 reactivated-3.0.0a64/reactivated/templates/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.835618 reactivated-3.0.0a64/reactivated/templates/reactivated/
+-rw-r--r--   0 runner    (1001) docker     (116)       47 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/templates/reactivated/autocomplete
+-rw-r--r--   0 runner    (1001) docker     (116)      695 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/templates/reactivated/interface.html
+-rw-r--r--   0 runner    (1001) docker     (116)     4701 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/templates.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1759 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/views.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1390 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/reactivated/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.831618 reactivated-3.0.0a64/reactivated.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      860 2020-09-30 21:48:02.000000 reactivated-3.0.0a64/reactivated.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1731 2020-09-30 21:48:02.000000 reactivated-3.0.0a64/reactivated.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-30 21:48:02.000000 reactivated-3.0.0a64/reactivated.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       25 2020-09-30 21:48:02.000000 reactivated-3.0.0a64/reactivated.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.835618 reactivated-3.0.0a64/sample/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      634 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.835618 reactivated-3.0.0a64/sample/server/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.835618 reactivated-3.0.0a64/sample/server/apps/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.835618 reactivated-3.0.0a64/sample/server/apps/samples/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/apps/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/apps/samples/admin.py
+-rw-r--r--   0 runner    (1001) docker     (116)       89 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/apps/samples/apps.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1123 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/apps/samples/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.835618 reactivated-3.0.0a64/sample/server/apps/samples/migrations/
+-rw-r--r--   0 runner    (1001) docker     (116)     5529 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/apps/samples/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/apps/samples/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3193 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/apps/samples/models.py
+-rw-r--r--   0 runner    (1001) docker     (116)      851 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/apps/samples/templates.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/apps/samples/tests.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5611 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/apps/samples/views.py
+-rw-r--r--   0 runner    (1001) docker     (116)      126 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/forms.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3812 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1398 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (116)      395 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/views.py
+-rw-r--r--   0 runner    (1001) docker     (116)      389 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/sample/server/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-09-30 21:48:02.839618 reactivated-3.0.0a64/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      950 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-30 21:48:02.839618 reactivated-3.0.0a64/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2512 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/tests/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1090 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3374 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/tests/fields.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1071 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/tests/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5766 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/tests/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1769 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/tests/templates.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12267 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/tests/types.py
+-rw-r--r--   0 runner    (1001) docker     (116)      199 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1034 2020-09-30 21:46:56.000000 reactivated-3.0.0a64/tests/views.py
```

### Comparing `reactivated-0.9.0/PKG-INFO` & `reactivated-3.0.0a64/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactivated
-Version: 0.9.0
+Version: 3.0.0a64
 Summary: A statically typed framework to create Django sites with a React frontend.
 Home-page: https://github.com/silviogutierrez/django-react
 Author: Silvio Gutierrez
 Author-email: silviogutierrez@gmail.com
 License: UNKNOWN
 Description: A library to make it as easy as possible to render Django using React, all server side. The browser then hydrates seamlessly, allowing you to add dynamic behavior. Best of both worlds.
```

### Comparing `reactivated-0.9.0/reactivated/__init__.py` & `reactivated-3.0.0a64/reactivated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from .templates import Action as Action  # noqa: F401
 from .templates import interface as interface  # noqa: F401
 from .templates import template as template  # noqa: F401
 
 default_app_config = "reactivated.apps.ReactivatedConfig"
 
 type_registry: Dict[str, Tuple[Any]] = {}
+global_types: Dict[str, Tuple[Any]] = {}
 template_registry: Dict[str, Tuple[Any]] = {}
 
 
 _SingleSerializable = Union[
     None,
     str,
     bool,
```

### Comparing `reactivated-0.9.0/reactivated/apps.py` & `reactivated-3.0.0a64/reactivated/apps.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 import os
 import subprocess
 from typing import Any, Dict, NamedTuple, Tuple
 
 from django.apps import AppConfig
 from django.conf import settings
 
-from . import extract_views_from_urlpatterns, template_registry, type_registry
+from . import (
+    extract_views_from_urlpatterns,
+    global_types,
+    template_registry,
+    type_registry,
+)
 from .serialization import create_schema
 
 logger = logging.getLogger("django.server")
 
 
 def get_urls_schema() -> Dict[str, Any]:
     urlconf = importlib.import_module(settings.ROOT_URLCONF)
@@ -43,19 +48,54 @@
             },
         }
 
     return reverse
 
 
 def get_types_schema() -> Any:
+    """ The package json-schema-to-typescript does expose a way to
+    automatically export any interface it sees. However, this can bloat our
+    generated files.
+
+    Instead, while creating the schema, we occasionally run into types that we
+    want available globally but are not directly referenced by templates.
+
+    These aren't exported by `json-schem-to-typescript` because they're
+    referenced using `tsType`, so the libraary is unaware of their usage.
+
+    So we register them in `globals` and force `json-schema-to-typescript` to
+    expose them.
+
+    We can't just add these types to the `type_registry` because that's only
+    parsed once when generating the parent tuple.
+
+    We could explore doing two passes in the future.
+
+    See `unreachableDefinitions` in json-schema-to-typescript
+    """
+    type_registry["globals"] = Any  # type: ignore[assignment]
     ParentTuple = NamedTuple("ParentTuple", type_registry.items())  # type: ignore[misc]
     parent_schema = create_schema(ParentTuple, {})
+
     return {
         "definitions": parent_schema.definitions,
-        **parent_schema.definitions["reactivated.apps.ParentTuple"],
+        **{
+            **parent_schema.definitions["reactivated.apps.ParentTuple"],
+            "properties": {
+                **parent_schema.definitions["reactivated.apps.ParentTuple"][
+                    "properties"
+                ],
+                "globals": {
+                    "type": "object",
+                    "additionalProperties": False,
+                    "required": list(global_types.keys()),
+                    "properties": global_types,
+                },
+            },
+        },
     }
 
 
 def get_templates() -> Dict[str, Tuple[Any]]:
     return template_registry
```

### Comparing `reactivated-0.9.0/reactivated/backend.py` & `reactivated-3.0.0a64/reactivated/backend.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 from django.conf import settings
-from django.template import TemplateDoesNotExist
+from django.template import TemplateDoesNotExist, TemplateSyntaxError
 from django.template.backends.base import BaseEngine
 from django.template.backends.utils import csrf_token_lazy
 from django.utils.functional import cached_property
 from django.utils.module_loading import import_string
 
 from .renderer import render_jsx_to_string
 
@@ -21,43 +21,27 @@
 
         self.context_processors = options.pop("context_processors", [])
         super().__init__(params)
 
         # self.engine = foobar.Engine(**options)
 
     def from_string(self, template_code):
-        return "ABC"
-        """
-        try:
-          return Template(self.engine.from_string(template_code))
-        except foobar.TemplateCompilationFailed as exc:
-            raise TemplateSyntaxError(exc.args)
-        """
+        raise TemplateSyntaxError("Unsupported with JSX")
 
     def get_template(self, template_name):
         adapter = self.template_adapters.get(template_name)
 
         if adapter is not None:
             return AdapterTemplate(adapter, self)
 
-        """ Get rid of this?
-        if template_name.endswith(".html"):
-            jsx_template_name = template_name.replace(".html", ".tsx")
-
-            if os.path.isfile(
-                os.path.join(settings.BASE_DIR, "client/templates", jsx_template_name)
-            ):
-                return Template(jsx_template_name, self)
-        """
-
         if template_name.endswith(".tsx") or template_name.endswith(".jsx"):
             if os.path.isfile(
                 os.path.join(settings.BASE_DIR, "client/templates", template_name)
             ):
-                return Template(template_name, self)
+                return JSXTemplate(template_name, self)
 
         raise TemplateDoesNotExist([], backend=self)
 
     @cached_property
     def template_adapters(self):
         adapters = {}
 
@@ -69,15 +53,15 @@
         return adapters
 
     @cached_property
     def template_context_processors(self):
         return [import_string(path) for path in self.context_processors]
 
 
-class Template:
+class JSXTemplate:
     def __init__(self, jsx_template_name, backend):
         self.jsx_template_name = jsx_template_name
         self.backend = backend
 
     def render(self, context=None, request=None):
         template_name = self.jsx_template_name.replace(".tsx", "").replace(".jsx", "")
 
@@ -94,15 +78,15 @@
             return render_jsx_to_string(request, template_name, context, props)
 
         assert (
             False
         ), "At this time, only templates with the request object can be rendered with reactivated"
 
 
-class AdapterTemplate(Template):
+class AdapterTemplate(JSXTemplate):
     def __init__(self, adapter, backend):
         self.adapter = adapter
         super().__init__(f"{self.adapter.__name__}.tsx", backend)
 
     def render(self, context=None, request=None):
         to_be_serialized = self.adapter(**context)
         jsx_context = to_be_serialized.get_serialized()
```

### Comparing `reactivated-0.9.0/reactivated/forms.py` & `reactivated-3.0.0a64/reactivated/forms.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,31 @@
+import enum
 import re
 from typing import Any, Dict, NamedTuple, Optional, TypeVar, Union, cast
 
 from django import forms as django_forms
 from django.http import HttpRequest, HttpResponse, JsonResponse
 from django.template.response import TemplateResponse
 
 from .widgets import Autocomplete as Autocomplete
 
+
+class EnumChoiceField(django_forms.TypedChoiceField):
+    """
+    Enum choices must be serialized to their name rather than their enum
+    representation for the existing value in forms. Choices themselves are
+    handled by the `choices` argument in form and model fields.
+    """
+
+    def prepare_value(self, value: Optional[enum.Enum]) -> Optional[str]:
+        if isinstance(value, enum.Enum):
+            return value.name
+        return value
+
+
 T = TypeVar("T")
 
 
 class FormOrFormSetDescriptor(NamedTuple):
     prefix: Optional[str]
     field_name: str
 
@@ -72,19 +87,20 @@
             form is not None
             and descriptor.field_name in form.fields
             and isinstance(
                 form.fields[descriptor.field_name], django_forms.ModelChoiceField
             )
             and isinstance(form.fields[descriptor.field_name].widget, Autocomplete)
         ):
+            autocomplete_field = form.fields[descriptor.field_name]
+            to_field_name = autocomplete_field.to_field_name or "pk"
+
             results = [
-                {"value": result.pk, "label": str(result)}
-                for result in form.fields[descriptor.field_name].queryset.autocomplete(
-                    query
-                )[:50]
+                {"value": getattr(result, to_field_name), "label": str(result)}
+                for result in autocomplete_field.queryset.autocomplete(query)[:50]
             ]
 
             return JsonResponse({"results": results})
 
         return response
 
     return cast(T, wrapped_view)
```

### Comparing `reactivated-0.9.0/reactivated/models.py` & `reactivated-3.0.0a64/reactivated/models.py`

 * *Files identical despite different names*

### Comparing `reactivated-0.9.0/reactivated/pick.py` & `reactivated-3.0.0a64/reactivated/pick.py`

 * *Files identical despite different names*

### Comparing `reactivated-0.9.0/reactivated/plugin.py` & `reactivated-3.0.0a64/reactivated/plugin.py`

 * *Files identical despite different names*

### Comparing `reactivated-0.9.0/reactivated/renderer.py` & `reactivated-3.0.0a64/reactivated/renderer.py`

 * *Files identical despite different names*

### Comparing `reactivated-0.9.0/reactivated/serialization.py` & `reactivated-3.0.0a64/reactivated/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import datetime
+import enum
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Literal,
     Mapping,
     NamedTuple,
     Optional,
     Protocol,
     Sequence,
+    Tuple,
     Type,
     Union,
     get_type_hints,
 )
 
 from django import forms as django_forms
 from django.conf import settings
 from django.db import models
 from django.utils.module_loading import import_string
 
-from . import stubs
+from . import fields, stubs
 from .models import ComputedRelation
 
 Schema = Mapping[Any, Any]
 
 Definitions = Mapping[str, Schema]
 
 JSON = Any
@@ -75,14 +77,40 @@
                 "type": "number",
                 "serializer": "reactivated.serialization.ForeignKeyType",
             },
             definitions=definitions,
         )
 
 
+class OptgroupMember(NamedTuple):
+    name: str
+    value: Union[str, int, bool, None]
+    label: str
+    selected: bool
+
+
+Optgroup = Tuple[None, Tuple[OptgroupMember], int]
+
+"""
+type Optgroup = [
+    null,
+    [
+        {
+            name: string;
+            // value: string|number|boolean|null;
+            value: string | number | boolean | null;
+            label: string;
+            selected: boolean;
+        },
+    ],
+    number,
+];
+"""
+
+
 class FieldType(NamedTuple):
     name: str
     label: str
     help_text: str
 
     # TODO: way to mark this as a custom property we define. This is just so it is
     # marked as required.
@@ -123,16 +151,29 @@
 
     So we monkeypatch the widget's internal renderer to return JSON directly
     without being wrapped by `mark_safe`.
     """
     field.field.widget._render = (  # type: ignore[attr-defined]
         lambda template_name, context, renderer: context
     )
-    context = field.as_widget()["widget"]  # type: ignore[index]
-    return context  # type: ignore[return-value]
+    context: Any = field.as_widget()["widget"]  # type: ignore[index]
+    optgroups = context.get("optgroups", None)
+
+    # This is our first foray into properly serializing widgets using the
+    # serialization framework.
+    #
+    # Eventually all widgets can be serialized this way and the frontend widget
+    # types can disappear and be generated from the code here.
+    if optgroups is not None:
+        optgroup_schema = create_schema(Optgroup, {})  # type: ignore[misc]
+        context["optgroups"] = [
+            serialize(optgroup, optgroup_schema) for optgroup in optgroups
+        ]
+
+    return context  # type: ignore[no-any-return]
 
 
 class FormType(NamedTuple):
     name: str
     errors: Optional[FormErrors]
     fields: Dict[str, FieldType]
     iterator: List[str]
@@ -234,14 +275,15 @@
         models.DateField: datetime.date,
         models.DateTimeField: datetime.datetime,
         models.EmailField: str,
         models.UUIDField: str,
         models.IntegerField: int,
         models.PositiveIntegerField: int,
         models.DecimalField: str,
+        fields.EnumField: str,
     }
 
     try:
         from django_extensions.db import fields as django_extension_fields  # type: ignore[import]
 
         mapping = {
             **mapping,
@@ -319,14 +361,29 @@
         return Thing(
             schema={"type": "string", "enum": Type.__args__}, definitions=definitions
         )
 
     assert False, f"Unsupported _GenericAlias {Type}"
 
 
+def enum_schema(Type: Type[enum.Enum], definitions: Definitions) -> Thing:
+    definition_name = f"{Type.__module__}.{Type.__qualname__}"
+
+    return Thing(
+        schema={"$ref": f"#/definitions/{definition_name}"},
+        definitions={
+            **definitions,
+            definition_name: {
+                "type": "string",
+                "enum": list(member.name for member in Type),
+            },
+        },
+    )
+
+
 def named_tuple_schema(Type: Any, definitions: Definitions) -> Thing:
     definition_name = f"{Type.__module__}.{Type.__qualname__}"
 
     if definition_name in definitions:
         return Thing(
             schema={"$ref": f"#/definitions/{definition_name}"}, definitions=definitions
         )
@@ -338,14 +395,27 @@
     for field_name, Subtype in get_type_hints(Type).items():
         field_schema = create_schema(Subtype, definitions)
         definitions = {**definitions, **field_schema.definitions}
 
         required.append(field_name)
         properties[field_name] = field_schema.schema
 
+    for field_name in dir(Type):
+        if field_name in properties:
+            continue
+
+        possible_method_or_property = getattr(Type, field_name)
+
+        if isinstance(possible_method_or_property, property):
+            annotations = get_type_hints(possible_method_or_property.fget)
+            field_schema = create_schema(annotations["return"], definitions)
+            definitions = {**definitions, **field_schema.definitions}
+            required.append(field_name)
+            properties[field_name] = field_schema.schema
+
     return Thing(
         schema={"$ref": f"#/definitions/{definition_name}"},
         definitions={
             **definitions,
             definition_name: {
                 "serializer": definition_name
                 if callable(getattr(Type, "get_serialized_value", None))
@@ -391,19 +461,45 @@
         if SourceWidget.__module__ != "django.forms.widgets":
             SourceWidget = SubType.widget.__class__.__bases__[0]
 
         assert (
             SourceWidget.__module__ == "django.forms.widgets"
         ), f"Only core widgets and depth-1 inheritance widgets are currently supported. Check {SubType.widget.__class__}"
 
+        ts_type = f"widgets.{SourceWidget.__name__}"
+
+        # Special treatment to register global Enum types and reference them
+        # through `tsType`
+
+        # Tightly coupled, for now. Can likely be improved once we have proper
+        # widget schema generation.
+        if isinstance(SubType, django_forms.TypedChoiceField) and (
+            choices := list(SubType.choices)
+        ):
+            choice = SubType.coerce(choices[0][0])
+
+            choice_schema, definitions = create_schema(type(choice), definitions)
+
+            if (ref := choice_schema.get("$ref", None)) :
+                generic_name = "".join(
+                    part.capitalize()
+                    for part in ref.replace("#/definitions/", "").split(".")
+                )
+
+                from . import global_types
+
+                global_types[generic_name] = choice_schema  # type: ignore[assignment]
+
+                ts_type = f'widgets.{SourceWidget.__name__}<Types["globals"]["{generic_name}"]>'
+
         properties[field_name] = {
             **field_type_definition,
             "properties": {
                 **field_type_definition["properties"],
-                "widget": {"tsType": f"widgets.{SourceWidget.__name__}"},
+                "widget": {"tsType": ts_type},
             },
         }
         error_properties[field_name] = error_definition
 
     definitions = {
         **definitions,
         definition_name: {
@@ -543,14 +639,16 @@
         return Thing(schema={"type": "string"}, definitions={})
     elif Type is type(None):  # noqa: E721
         return Thing(schema={"type": "null"}, definitions={})
     elif issubclass(Type, django_forms.BaseForm):
         return form_schema(Type, definitions)
     elif issubclass(Type, stubs.BaseFormSet):
         return form_set_schema(Type, definitions)
+    elif issubclass(Type, enum.Enum):
+        return enum_schema(Type, definitions)
 
     additional_schema_module: Optional[str] = getattr(
         settings, "REACTIVATED_SERIALIZATION", None
     )
 
     if additional_schema_module is not None:
         additional_schema: Callable[
```

### Comparing `reactivated-0.9.0/reactivated/stubs.py` & `reactivated-3.0.0a64/reactivated/stubs.py`

 * *Files identical despite different names*

### Comparing `reactivated-0.9.0/reactivated/templates/reactivated/interface.html` & `reactivated-3.0.0a64/reactivated/templates/reactivated/interface.html`

 * *Files identical despite different names*

### Comparing `reactivated-0.9.0/reactivated/utils.py` & `reactivated-3.0.0a64/reactivated/utils.py`

 * *Files identical despite different names*

### Comparing `reactivated-0.9.0/reactivated/views.py` & `reactivated-3.0.0a64/reactivated/views.py`

 * *Files identical despite different names*

### Comparing `reactivated-0.9.0/reactivated/widgets.py` & `reactivated-3.0.0a64/reactivated/widgets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict, Optional, cast
 
 from django import forms
+from django.core.exceptions import ValidationError
 from django.forms.models import ModelChoiceIterator
 
 
 class Autocomplete(forms.Select):
     template_name = "reactivated/autocomplete"
 
     def get_context(
@@ -19,17 +20,18 @@
 
         to_field_name = choices.field.to_field_name or "pk"
 
         # context = forms.Widget.get_context(self, name, value, attrs)
         # self.choices.queryset = self.choices.queryset._clone()[:10]
         # context = super().get_context(name, value, attrs)
         context = forms.Widget.get_context(self, name, value, attrs)
-        selected = (
-            choices.queryset.filter(**{to_field_name: value}).first() if value else None
-        )
+        try:
+            selected = choices.field.to_python(value)
+        except ValidationError:
+            selected = None
 
         if selected is not None:
             context["widget"]["selected"] = {
                 "value": getattr(selected, to_field_name),
                 "label": str(selected),
             }
         else:
```

### Comparing `reactivated-0.9.0/reactivated.egg-info/PKG-INFO` & `reactivated-3.0.0a64/reactivated.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactivated
-Version: 0.9.0
+Version: 3.0.0a64
 Summary: A statically typed framework to create Django sites with a React frontend.
 Home-page: https://github.com/silviogutierrez/django-react
 Author: Silvio Gutierrez
 Author-email: silviogutierrez@gmail.com
 License: UNKNOWN
 Description: A library to make it as easy as possible to render Django using React, all server side. The browser then hydrates seamlessly, allowing you to add dynamic behavior. Best of both worlds.
```

### Comparing `reactivated-0.9.0/reactivated.egg-info/SOURCES.txt` & `reactivated-3.0.0a64/reactivated.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 README.md
 setup.py
+packages/reactivated/package.json
 reactivated/__init__.py
 reactivated/admin.py
 reactivated/apps.py
 reactivated/backend.py
+reactivated/constraints.py
+reactivated/fields.py
 reactivated/forms.py
 reactivated/middleware.py
 reactivated/models.py
 reactivated/pick.py
 reactivated/plugin.py
 reactivated/py.typed
 reactivated/renderer.py
 reactivated/serialization.py
 reactivated/stubs.py
 reactivated/templates.py
-reactivated/tests.py
 reactivated/utils.py
 reactivated/views.py
 reactivated/widgets.py
 reactivated.egg-info/PKG-INFO
 reactivated.egg-info/SOURCES.txt
 reactivated.egg-info/dependency_links.txt
 reactivated.egg-info/top_level.txt
@@ -43,20 +45,18 @@
 sample/server/apps/samples/apps.py
 sample/server/apps/samples/forms.py
 sample/server/apps/samples/models.py
 sample/server/apps/samples/templates.py
 sample/server/apps/samples/tests.py
 sample/server/apps/samples/views.py
 sample/server/apps/samples/migrations/0001_initial.py
-sample/server/apps/samples/migrations/0002_opera_has_piano_transcription.py
-sample/server/apps/samples/migrations/0003_auto_20190913_0303.py
-sample/server/apps/samples/migrations/0004_auto_20190913_2051.py
-sample/server/apps/samples/migrations/0005_auto_20190914_0221.py
 sample/server/apps/samples/migrations/__init__.py
 tests/__init__.py
 tests/autocomplete.py
+tests/conftest.py
+tests/fields.py
 tests/renderer.py
 tests/serialization.py
 tests/templates.py
 tests/types.py
 tests/urls.py
 tests/views.py
```

### Comparing `reactivated-0.9.0/sample/manage.py` & `reactivated-3.0.0a64/sample/manage.py`

 * *Files identical despite different names*

### Comparing `reactivated-0.9.0/sample/server/apps/samples/forms.py` & `reactivated-3.0.0a64/sample/server/apps/samples/forms.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from reactivated.forms import Autocomplete
 from sample.server.apps.samples import models
 
 
 class PlaygroundForm(forms.Form):
     choice_field = forms.ChoiceField(
-        choices=(("", "- blank -"), ("first", "First"), ("second", "Second"))
+        choices=(("", "- blank -"), ("first", "First"), ("second", "Second")),
+        initial="first",
     )
 
     # TODO: figure out why adding this class makes the plugin work.
     # Something in
     # plugin.py#ctx.api.add_symbol_table_node(ctx.name, SymbolTableNode(GDEF, info))
     # causes a recursion error when using the plugin together with django-stubs
     # plugin.
```

### Comparing `reactivated-0.9.0/sample/server/apps/samples/models.py` & `reactivated-3.0.0a64/sample/server/apps/samples/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,41 @@
+import enum
 from typing import Optional, cast
 
 from django.db import models
 
 from reactivated import computed_relation
+from reactivated.fields import EnumField
 
 models.QuerySet.__class_getitem__ = classmethod(  # type: ignore[assignment]
     lambda cls, key: cls
 )
 models.Manager.__class_getitem__ = classmethod(  # type: ignore[assignment]
     lambda cls, key: cls
 )
 
 
 class Continent(models.Model):
+    class Hemisphere(enum.Enum):
+        SOUTHERN = "Southern"
+        NORTHERN = "Northern"
+
     name = models.CharField(max_length=100)
-    hemisphere = models.CharField(max_length=20)
+    hemisphere = EnumField(enum=Hemisphere, default=Hemisphere.SOUTHERN)
 
 
 class Country(models.Model):
     name = models.CharField(max_length=100)
     continent = models.ForeignKey(
         Continent, on_delete=models.CASCADE, related_name="countries"
     )
 
+    def __str__(self) -> str:
+        return self.name
+
 
 class ComposerCountry(models.Model):
     country = models.ForeignKey(
         Country, on_delete=models.CASCADE, related_name="composer_countries"
     )
     composer = models.ForeignKey(
         "Composer", on_delete=models.CASCADE, related_name="composer_countries"
@@ -71,24 +80,28 @@
 
 class OperaQuerySet(models.QuerySet["Opera"]):
     def autocomplete(self, query: str) -> models.QuerySet["Opera"]:
         return self.filter(name__icontains=query)
 
 
 class Opera(models.Model):
+    class Style(enum.Enum):
+        VERISMO = "Verismo"
+        BUFFA = "Opera Buffa"
+        GRAND = "Grand Opera"
+
     name = models.CharField(max_length=100)
     composer = models.ForeignKey(
         "Composer", on_delete=models.CASCADE, related_name="operas"
     )
+    style = EnumField(enum=Style, default=Style.GRAND)
     has_piano_transcription = models.BooleanField(default=False)
 
     objects = cast(OperaManager, OperaManager.from_queryset(OperaQuerySet)())
 
-    # objects: DayQuerySet = cast(DayQuerySet, DayQuerySet.as_manager())  # type: ignore[assignment]
-
     def __str__(self) -> str:
         return f"{self.name}: {self.composer.name}"
 
     def get_birthplace_of_composer(self) -> Optional[str]:
         country = self.composer.countries.filter(
             composer_countries__was_born=True
         ).first()
```

### Comparing `reactivated-0.9.0/sample/server/apps/samples/templates.py` & `reactivated-3.0.0a64/sample/server/apps/samples/templates.py`

 * *Files identical despite different names*

### Comparing `reactivated-0.9.0/sample/server/settings.py` & `reactivated-3.0.0a64/sample/server/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -78,22 +78,27 @@
             ]
         },
     },
 ]
 
 WSGI_APPLICATION = "server.wsgi.application"
 
-
 # Database
 # https://docs.djangoproject.com/en/2.2/ref/settings/#databases
 
 DATABASES = {
     "default": {
-        "ENGINE": "django.db.backends.sqlite3",
-        "NAME": os.path.join(BASE_DIR, "db.sqlite3"),
+        "ENGINE": "django.db.backends.postgresql",
+        "NAME": os.environ["DATABASE_NAME"],
+        "USER": os.environ.get("DATABASE_USER", None),
+        "PASSWORD": os.environ.get("DATABASE_PASSWORD", None),
+        "HOST": os.environ.get("DATABASE_HOST", None),
+        "PORT": os.environ.get("DATABASE_PORT", None),
+        # Already set by the environment.
+        # "PORT": os.environ.get("PGPORT"),
     }
 }
 
 
 # Password validation
 # https://docs.djangoproject.com/en/2.2/ref/settings/#auth-password-validators
 
@@ -122,13 +127,12 @@
 
 
 # Static files (CSS, JavaScript, Images)
 # https://docs.djangoproject.com/en/2.2/howto/static-files/
 
 STATIC_URL = "/static/"
 
-
 DEBUG_PORT = int(os.environ.get("DEBUG_PORT", 8000))
 
 RUNSERVERPLUS_SERVER_ADDRESS_PORT = f"0.0.0.0:{DEBUG_PORT}"
 
 REACTIVATED_SERVER = f"http://0.0.0.0:{DEBUG_PORT + 200}"
```

### Comparing `reactivated-0.9.0/sample/server/urls.py` & `reactivated-3.0.0a64/sample/server/urls.py`

 * *Files identical despite different names*

### Comparing `reactivated-0.9.0/tests/autocomplete.py` & `reactivated-3.0.0a64/tests/autocomplete.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     composer = models.Composer.objects.create(name="Richard Wagner")
     models.Composer.objects.create(name="Wolfgang Amadeus Mozart")
 
     assert client.get("/autocomplete-view/").status_code == 200
 
     assert (
         client.post(
-            "/autocomplete-view/", {"name": "Zarzuela", "composer": composer.pk}
+            "/autocomplete-view/",
+            {"name": "Zarzuela", "style": "BUFFA", "composer": composer.pk},
         ).status_code
         == 302
     )
 
     response = client.get(
         "/autocomplete-view/", {"autocomplete": "name", "query": "Wagner"}
     )
@@ -26,14 +27,50 @@
 
     response = client.get(
         "/autocomplete-view/", {"autocomplete": "composer", "query": "Wagner"}
     )
     assert response.json()["results"][0]["label"] == "Richard Wagner"
 
 
+@pytest.mark.django_db
+@pytest.mark.urls("tests.urls")
+def test_invalid_value(client):
+    response = client.post(
+        "/autocomplete-view/", {"name": "Zarzuela", "composer": "21s7"}
+    )
+    assert "Select a valid choice" in response.context["form"].errors["composer"][0]
+    assert response.context["form"]["composer"].value() == "21s7"
+
+
+@pytest.mark.django_db
+@pytest.mark.urls("tests.urls")
+def test_typed_autocomplete(client):
+    composer = models.Composer.objects.create(name="Richard Wagner")
+    models.Composer.objects.create(name="Wolfgang Amadeus Mozart")
+
+    assert client.get("/typed-autocomplete-view/").status_code == 200
+
+    assert (
+        client.post(
+            "/typed-autocomplete-view/", {"name": "Zarzuela", "composer": composer.pk}
+        ).status_code
+        == 302
+    )
+
+    response = client.get(
+        "/typed-autocomplete-view/", {"autocomplete": "name", "query": "Wagner"}
+    )
+    assert "" in str(response.content)
+
+    response = client.get(
+        "/typed-autocomplete-view/", {"autocomplete": "composer", "query": "Wagner"}
+    )
+    assert response.json()["results"][0]["label"] == "Richard Wagner"
+
+
 def test_prefix_calculation(client):
     assert forms.get_form_or_form_set_descriptor("opera_form_set-0-composer_field") == (
         "opera_form_set",
         "composer_field",
     )
 
     assert forms.get_form_or_form_set_descriptor("opera_form-composer_field") == (
```

### Comparing `reactivated-0.9.0/tests/renderer.py` & `reactivated-3.0.0a64/tests/renderer.py`

 * *Files identical despite different names*

### Comparing `reactivated-0.9.0/tests/serialization.py` & `reactivated-3.0.0a64/tests/serialization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, List, Literal, NamedTuple, Tuple
 
 import pytest
 import simplejson
+from django.forms.models import ModelChoiceIteratorValue
 from jsonschema import validate
 
 from reactivated import Pick
 from reactivated.serialization import create_schema, serialize
 from sample.server.apps.samples import forms, models
 
 
@@ -118,14 +119,39 @@
     form_with_errors.is_valid()
     serialized_form = serialize(form_with_errors, generated_schema)
     assert "name" in serialized_form.errors
     convert_to_json_and_validate(serialized_form, generated_schema)
 
 
 @pytest.mark.django_db
+def test_form_with_model_choice_iterator_value():
+    models.Country.objects.create(
+        name="USA",
+        continent=models.Continent.objects.create(
+            name="America", hemisphere="NORTHERN"
+        ),
+    )
+    iterator = (
+        forms.ComposerForm()
+        .fields["countries"]
+        .widget.optgroups("countries", "")[0][1][0]["value"]
+    )
+
+    assert isinstance(iterator, ModelChoiceIteratorValue)
+
+    generated_schema = create_schema(forms.ComposerForm, {})
+    form = forms.ComposerForm()
+    serialized_form = serialize(form, generated_schema)
+    convert_to_json_and_validate(serialized_form, generated_schema)
+    serialized_form.fields["countries"].widget["optgroups"][0][1][0][
+        "value"
+    ] == iterator.value
+
+
+@pytest.mark.django_db
 def test_form_set():
     generated_schema = create_schema(forms.OperaFormSet, {})
     form_set = forms.OperaFormSet()
     serialized_form_set = serialize(form_set, generated_schema)
     convert_to_json_and_validate(serialized_form_set, generated_schema)
 
     form_set_with_errors = forms.OperaFormSet(
```

### Comparing `reactivated-0.9.0/tests/types.py` & `reactivated-3.0.0a64/tests/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import enum
 from io import StringIO
 from typing import Any, Dict, List, Literal, NamedTuple, Tuple, TypedDict, Union
 
 import pytest
 import simplejson
 from django.core.exceptions import FieldDoesNotExist
 from django.core.management import call_command
@@ -13,14 +14,18 @@
 
 
 class NamedTupleType(NamedTuple):
     first: str
     second: bool
     third: int
 
+    @property
+    def fourth_as_property(self) -> int:
+        return 5
+
 
 class TypedDictType(TypedDict):
     first: str
     second: bool
     third: int
 
 
@@ -30,23 +35,36 @@
         {
             "tests.types.NamedTupleType": {
                 "additionalProperties": False,
                 "properties": {
                     "first": {"type": "string"},
                     "second": {"type": "boolean"},
                     "third": {"type": "number"},
+                    "fourth_as_property": {"type": "number"},
                 },
-                "required": ["first", "second", "third"],
+                "required": ["first", "second", "third", "fourth_as_property"],
                 "serializer": None,
                 "type": "object",
             }
         },
     )
 
 
+class EnumType(enum.Enum):
+    ONE = "One"
+    TWO = "Two"
+
+
+def test_enum():
+    assert create_schema(EnumType, {}) == (
+        {"$ref": "#/definitions/tests.types.EnumType"},
+        {"tests.types.EnumType": {"type": "string", "enum": ["ONE", "TWO"],}},
+    )
+
+
 def test_literal():
     assert create_schema(Literal["hello"], {}) == (
         {"type": "string", "enum": ("hello",)},
         {},
     )
 
 
@@ -137,14 +155,15 @@
                         "properties": {
                             "composer": {"items": {"type": "string"}, "type": "array"},
                             "has_piano_transcription": {
                                 "items": {"type": "string"},
                                 "type": "array",
                             },
                             "name": {"items": {"type": "string"}, "type": "array"},
+                            "style": {"items": {"type": "string"}, "type": "array"},
                         },
                         "type": "object",
                     },
                     {"type": "null"},
                 ]
             },
             "fields": {
@@ -182,21 +201,35 @@
                             "name": {"type": "string"},
                             "widget": {"tsType": "widgets.TextInput"},
                         },
                         "required": ["name", "label", "help_text", "widget"],
                         "serializer": "field_serializer",
                         "type": "object",
                     },
+                    "style": {
+                        "additionalProperties": False,
+                        "properties": {
+                            "help_text": {"type": "string"},
+                            "label": {"type": "string"},
+                            "name": {"type": "string"},
+                            "widget": {
+                                "tsType": 'widgets.Select<Types["globals"]["SampleServerAppsSamplesModelsOperaStyle"]>'
+                            },
+                        },
+                        "required": ["name", "label", "help_text", "widget"],
+                        "serializer": "field_serializer",
+                        "type": "object",
+                    },
                 },
-                "required": ["name", "composer", "has_piano_transcription"],
+                "required": ["name", "composer", "style", "has_piano_transcription"],
                 "type": "object",
             },
             "iterator": {
                 "items": {
-                    "enum": ["name", "composer", "has_piano_transcription"],
+                    "enum": ["name", "composer", "style", "has_piano_transcription"],
                     "type": "string",
                 },
                 "type": "array",
             },
             "prefix": {"type": "string"},
         },
         "required": ["name", "prefix", "fields", "iterator", "errors"],
@@ -319,15 +352,17 @@
         schema["properties"]["a"]["properties"]["multiple"]["items"]["properties"][
             "second_single"
         ]["type"]
         == "object"
     )
 
 
-def test_generate_types_schema():
+def test_generate_types_schema(settings):
+    # This technically loads the full sample site, which expects to be run
+    # from the sample subdirectory.
+    settings.ROOT_URLCONF = "sample.server.urls"
     output = StringIO()
-
     call_command("generate_types_schema", stdout=output)
     schema = simplejson.loads(output.getvalue())
     assert "types" in schema
     assert "urls" in schema
     assert "templates" in schema
```

