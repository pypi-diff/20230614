# Comparing `tmp/bento_lib-7.0.0a2.tar.gz` & `tmp/bento_lib-7.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_lib-7.0.0a2.tar", last modified: Wed Jun 14 14:17:15 2023, max compression
+gzip compressed data, was "bento_lib-7.0.0a3.tar", last modified: Wed Jun 14 18:10:38 2023, max compression
```

## Comparing `bento_lib-7.0.0a2.tar` & `bento_lib-7.0.0a3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.493345 bento_lib-7.0.0a2/bento_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.493345 bento_lib-7.0.0a2/bento_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.493345 bento_lib-7.0.0a2/bento_lib/auth/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/middleware/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/middleware/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/middleware/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/middleware/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.493345 bento_lib-7.0.0a2/bento_lib/drs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/drs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/bento_lib/events/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/events/_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/events/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/package.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/bento_lib/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/responses/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/responses/fastapi_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/responses/flask_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/bento_lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/bento.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/bento_data_use.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/bento_ingest.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/ga4gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/ga4gh_service_info.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/bento_lib/search/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/search/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/search/data_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/search/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/search/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.493345 bento_lib-7.0.0a2/bento_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-14 14:17:15.000000 bento_lib-7.0.0a2/bento_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-14 14:17:15.000000 bento_lib-7.0.0a2/bento_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:17:15.000000 bento_lib-7.0.0a2/bento_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-14 14:17:15.000000 bento_lib-7.0.0a2/bento_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 14:17:15.000000 bento_lib-7.0.0a2/bento_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.470480 bento_lib-7.0.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-14 18:10:38.470480 bento_lib-7.0.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib/auth/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/middleware/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/middleware/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/middleware/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/middleware/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/drs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/events/_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/events/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/package.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/responses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/responses/fastapi_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/responses/flask_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.470480 bento_lib-7.0.0a3/bento_lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/bento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/bento_data_use.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/bento_ingest.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/ga4gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/ga4gh_service_info.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.470480 bento_lib-7.0.0a3/bento_lib/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/search/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/search/data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/search/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/search/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-14 18:10:38.000000 bento_lib-7.0.0a3/bento_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-14 18:10:38.000000 bento_lib-7.0.0a3/bento_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:10:38.000000 bento_lib-7.0.0a3/bento_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-14 18:10:38.000000 bento_lib-7.0.0a3/bento_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 18:10:38.000000 bento_lib-7.0.0a3/bento_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:10:38.470480 bento_lib-7.0.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/setup.py
```

### Comparing `bento_lib-7.0.0a2/LICENSE` & `bento_lib-7.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/PKG-INFO` & `bento_lib-7.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento_lib
-Version: 7.0.0a2
+Version: 7.0.0a3
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-7.0.0a2/README.md` & `bento_lib-7.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/auth/middleware/base.py` & `bento_lib-7.0.0a3/bento_lib/auth/middleware/base.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/auth/middleware/django.py` & `bento_lib-7.0.0a3/bento_lib/auth/middleware/django.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/auth/middleware/fastapi.py` & `bento_lib-7.0.0a3/bento_lib/auth/middleware/fastapi.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/auth/middleware/flask.py` & `bento_lib-7.0.0a3/bento_lib/auth/middleware/flask.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/drs/utils.py` & `bento_lib-7.0.0a3/bento_lib/drs/utils.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/events/_event_bus.py` & `bento_lib-7.0.0a3/bento_lib/events/_event_bus.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/events/notifications.py` & `bento_lib-7.0.0a3/bento_lib/events/notifications.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/events/types.py` & `bento_lib-7.0.0a3/bento_lib/events/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/responses/errors.py` & `bento_lib-7.0.0a3/bento_lib/responses/errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/responses/fastapi_errors.py` & `bento_lib-7.0.0a3/bento_lib/responses/fastapi_errors.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,47 +4,65 @@
 from fastapi import status
 from fastapi.exceptions import HTTPException, RequestValidationError
 from fastapi.requests import Request
 from fastapi.responses import JSONResponse
 from starlette.responses import Response
 from typing import Callable
 
+from ..auth.middleware.fastapi import FastApiAuthMiddleware
 from ..auth.exceptions import BentoAuthException
 from .errors import http_error
 
 __all__ = [
     "http_exception_handler_factory",
     "bento_auth_exception_handler_factory",
-    "validation_exception_handler",
+    "validation_exception_handler_factory",
 ]
 
 
 def _log_if_500(logger: logging.Logger, code: int, exc: Exception) -> None:
     if code == status.HTTP_500_INTERNAL_SERVER_ERROR:
         logger.error(f"Encountered error:\n{traceback.format_exception(type(exc), exc, exc.__traceback__)}")
 
 
-def http_exception_handler_factory(logger: logging.Logger) -> Callable[[Request, HTTPException], Response]:
-    def http_exception_handler(_request: Request, exc: HTTPException) -> JSONResponse:
+def http_exception_handler_factory(
+    logger: logging.Logger,
+    authz: FastApiAuthMiddleware | None = None,
+) -> Callable[[Request, HTTPException], Response]:
+    def http_exception_handler(request: Request, exc: HTTPException) -> JSONResponse:
+        if authz:
+            authz.mark_authz_done(request)
         code = exc.status_code
         _log_if_500(logger, code, exc)
         return JSONResponse(http_error(code, exc.detail), status_code=code)
 
     return http_exception_handler
 
 
-def bento_auth_exception_handler_factory(logger: logging.Logger) -> Callable[[Request, BentoAuthException], Response]:
-    def bento_auth_exception_handler(_request: Request, exc: BentoAuthException) -> JSONResponse:
+def bento_auth_exception_handler_factory(
+    logger: logging.Logger,
+    authz: FastApiAuthMiddleware | None = None,
+) -> Callable[[Request, BentoAuthException], Response]:
+    def bento_auth_exception_handler(request: Request, exc: BentoAuthException) -> JSONResponse:
+        if authz:
+            authz.mark_authz_done(request)
         code = exc.status_code
         _log_if_500(logger, code, exc)
         return JSONResponse(http_error(code, exc.message), status_code=code)
 
     return bento_auth_exception_handler
 
 
-def validation_exception_handler(_request: Request, exc: RequestValidationError) -> JSONResponse:
-    code = status.HTTP_400_BAD_REQUEST
-    return JSONResponse(
-        http_error(
-            code,
-            *((".".join(map(str, e["loc"])) + ": " + e["msg"]) if e.get("loc") else e["msg"] for e in exc.errors())),
-        status_code=code)
+def validation_exception_handler_factory(
+    authz: FastApiAuthMiddleware | None = None,
+) -> Callable[[Request, RequestValidationError], Response]:
+    def validation_exception_handler(request: Request, exc: RequestValidationError) -> JSONResponse:
+        if authz:
+            authz.mark_authz_done(request)
+        code = status.HTTP_400_BAD_REQUEST
+        return JSONResponse(
+            http_error(
+                code,
+                *((".".join(map(str, e["loc"])) + ": " + e["msg"])
+                  if e.get("loc") else e["msg"] for e in exc.errors())),
+            status_code=code)
+    return validation_exception_handler
```

### Comparing `bento_lib-7.0.0a2/bento_lib/responses/flask_errors.py` & `bento_lib-7.0.0a3/bento_lib/responses/flask_errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sys
 import traceback
 
-from flask import jsonify
+from flask import jsonify, request
 from functools import partial
 from typing import Callable
 
+from bento_lib.auth.middleware.flask import FlaskAuthMiddleware
 from bento_lib.responses import errors
 
 
 __all__ = [
     "flask_error_wrap_with_traceback",
     "flask_error_wrap",
 
@@ -31,35 +32,48 @@
     while also printing a traceback. Optionally, the keyword argument service_name can be passed in to make the error
     logging more precise.
     :param fn: The flask error-generating function to wrap
     :return: The wrapped function
     """
 
     service_name = kwargs.pop("service_name", "Bento Service")
+
     logger = kwargs.pop("logger", None)
+    authz: FlaskAuthMiddleware | None = kwargs.pop("authz", None)
 
     def handle_error(e):
         if logger:
             logger.error(f"Encountered error:\n{traceback.format_exception(type(e), e, e.__traceback__)}")
         else:
             print(f"[{service_name}] Encountered error:", file=sys.stderr)
             # TODO: py3.10: print_exception(e)
             traceback.print_exception(type(e), e, e.__traceback__)
+        if authz:
+            authz.mark_authz_done(request)
         return fn(str(e), *args, **kwargs)
+
     return handle_error
 
 
 def flask_error_wrap(fn: Callable, *args, **kwargs) -> Callable:
     """
     Function to wrap flask_* error creators with something that supports the application.register_error_handler method
     and pass in the exception as a message.
     :param fn: The flask error-generating function to wrap
     :return: The wrapped function
     """
-    return lambda e: fn(str(e), *args, **kwargs)
+
+    authz: FlaskAuthMiddleware | None = kwargs.pop("authz", None)
+
+    def handle_error(e):
+        if authz:
+            authz.mark_authz_done(request)
+        return fn(str(e), *args, **kwargs)
+
+    return handle_error
 
 
 def flask_error(code: int, *errs, drs_compat: bool = False, sr_compat: bool = False):
     return jsonify(errors.http_error(code, *errs, drs_compat=drs_compat, sr_compat=sr_compat)), code
 
 
 def _flask_error(code: int) -> Callable:
```

### Comparing `bento_lib-7.0.0a2/bento_lib/schemas/bento_data_use.schema.json` & `bento_lib-7.0.0a3/bento_lib/schemas/bento_data_use.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/schemas/bento_ingest.schema.json` & `bento_lib-7.0.0a3/bento_lib/schemas/bento_ingest.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/schemas/ga4gh_service_info.schema.json` & `bento_lib-7.0.0a3/bento_lib/schemas/ga4gh_service_info.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/search/data_structure.py` & `bento_lib-7.0.0a3/bento_lib/search/data_structure.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/search/operations.py` & `bento_lib-7.0.0a3/bento_lib/search/operations.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/search/postgres.py` & `bento_lib-7.0.0a3/bento_lib/search/postgres.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/search/queries.py` & `bento_lib-7.0.0a3/bento_lib/search/queries.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/types.py` & `bento_lib-7.0.0a3/bento_lib/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib/workflows.py` & `bento_lib-7.0.0a3/bento_lib/workflows.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/bento_lib.egg-info/PKG-INFO` & `bento_lib-7.0.0a3/bento_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento-lib
-Version: 7.0.0a2
+Version: 7.0.0a3
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-7.0.0a2/bento_lib.egg-info/SOURCES.txt` & `bento_lib-7.0.0a3/bento_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a2/setup.py` & `bento_lib-7.0.0a3/setup.py`

 * *Files identical despite different names*

