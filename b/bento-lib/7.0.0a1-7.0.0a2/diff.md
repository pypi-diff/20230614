# Comparing `tmp/bento_lib-7.0.0a1.tar.gz` & `tmp/bento_lib-7.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_lib-7.0.0a1.tar", last modified: Tue Jun 13 12:15:22 2023, max compression
+gzip compressed data, was "bento_lib-7.0.0a2.tar", last modified: Wed Jun 14 14:17:15 2023, max compression
```

## Comparing `bento_lib-7.0.0a1.tar` & `bento_lib-7.0.0a2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.841275 bento_lib-7.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-13 12:15:22.837275 bento_lib-7.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.833275 bento_lib-7.0.0a1/bento_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.833275 bento_lib-7.0.0a1/bento_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.833275 bento_lib-7.0.0a1/bento_lib/auth/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/middleware/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/middleware/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/middleware/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/middleware/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.837275 bento_lib-7.0.0a1/bento_lib/drs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/drs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.837275 bento_lib-7.0.0a1/bento_lib/events/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/events/_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/events/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/package.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.837275 bento_lib-7.0.0a1/bento_lib/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/responses/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/responses/fastapi_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/responses/flask_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.837275 bento_lib-7.0.0a1/bento_lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/bento.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/bento_data_use.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/bento_ingest.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/ga4gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/ga4gh_service_info.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.837275 bento_lib-7.0.0a1/bento_lib/search/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/search/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/search/data_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/search/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/search/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.833275 bento_lib-7.0.0a1/bento_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-13 12:15:22.000000 bento_lib-7.0.0a1/bento_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-13 12:15:22.000000 bento_lib-7.0.0a1/bento_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:15:22.000000 bento_lib-7.0.0a1/bento_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 12:15:22.000000 bento_lib-7.0.0a1/bento_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 12:15:22.000000 bento_lib-7.0.0a1/bento_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 12:15:22.841275 bento_lib-7.0.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.493345 bento_lib-7.0.0a2/bento_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.493345 bento_lib-7.0.0a2/bento_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.493345 bento_lib-7.0.0a2/bento_lib/auth/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/middleware/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/middleware/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/middleware/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/auth/middleware/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.493345 bento_lib-7.0.0a2/bento_lib/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/drs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/bento_lib/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/events/_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/events/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/package.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/bento_lib/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/responses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/responses/fastapi_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/responses/flask_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/bento_lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/bento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/bento_data_use.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/bento_ingest.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/ga4gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/schemas/ga4gh_service_info.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/bento_lib/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/search/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/search/data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/search/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/search/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/bento_lib/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:15.493345 bento_lib-7.0.0a2/bento_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-14 14:17:15.000000 bento_lib-7.0.0a2/bento_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-14 14:17:15.000000 bento_lib-7.0.0a2/bento_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:17:15.000000 bento_lib-7.0.0a2/bento_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-14 14:17:15.000000 bento_lib-7.0.0a2/bento_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 14:17:15.000000 bento_lib-7.0.0a2/bento_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 14:17:15.497345 bento_lib-7.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-14 14:17:06.000000 bento_lib-7.0.0a2/setup.py
```

### Comparing `bento_lib-7.0.0a1/LICENSE` & `bento_lib-7.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/PKG-INFO` & `bento_lib-7.0.0a2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento_lib
-Version: 7.0.0a1
+Version: 7.0.0a2
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -57,48 +57,26 @@
 releasing. If the API is broken in any way, including minor differences in the
 way a function behaves given an identical set of parameters (excluding bugfixes
 for unintentional behaviour), the MAJOR version must be incremented. In this 
 way, we guarantee that projects relying on this API do not accidentally break
 upon upgrading.
 
 
-### 2. Releasing from the Command Line
+### 2. Releasing automatically
 
-```bash
-# IF NECESSARY: Install twine OUTSIDE of the virtual environment
-python3 -m pip install twine
-
-# Switch to the correct branch and make sure it's up to date
-git checkout master
-git pull
-
-# If needed, enter the project virtual environment
-source env/bin/activate
-
-# Remove existing build files
-rm -rf build/ dist/ bento_lib.egg-info/
-
-# Build the new package
-python3 setup.py sdist bdist_wheel
-
-# In between these steps - test out the package... make sure everything works
-# before uploading it to production PyPI.
-
-# Upload it to PyPI
-twine upload dist/*
-```
+When a version is tagged on GitHub, a build + release CI pipeline is automatically triggered.
+Make sure that the tagged version is a valid semantic versioning translation of the version in
+`package.cfg`, and that the versions otherwise match.
 
 
 ## Modules
 
 ### `auth`
 
-`auth` provides Python service decorators and Django / DRF backends for dealing
-with the Bento container authentication headers (derived from
-`lua-resty-openidc`, set by the internal container NGINX instance.)
+`auth` provides Python service middleware for dealing with the Bento authorization service.
 
 ### `drs`
 
 `drs` provides utilities for fetching data and record metadata from 
 GA4GH-compatible DRS services, and Bento's own implementation (which has some 
 non-standard extensions.)
 
@@ -108,14 +86,19 @@
 microservices. Serialized objects can be at most 512 MB.
 
 Events should have a lower-case type which is type-insensitively unique and
 adequately describes the associated data.
 
 All Bento channels are prefixed with `bento.`.
 
+### `responses`
+
+`responses` contains standardized error message-generating functions 
+and exception handling functions for different Python web frameworks.
+
 ### `schemas`
 
 `schemas` contains common JSON schemas which may be useful to a variety of
 different Bento services.
 
 `schemas.bento` contains Bento-specific schemas, and `schemas.ga4gh` contains
 GA4GH-standardized schemas (possibly not exactly to spec.)
@@ -139,16 +122,17 @@
 `psycopg2`-provided
 [intermediate representation (IR)](https://www.psycopg.org/docs/sql.html) for
 PostgreSQL, allowing safe queries against a Postgres database.
 
 `search.queries` provides definitions for the Bento query AST and some helper
 methods for creating and processing ASTs.
 
-### `utils`
+### `types`
 
-`utils` contains miscellaneous utilities commonly required by Bento services.
+`types` contains Python type hints for different standard Bento 
+dictionaries/objects.
 
 ### `workflows`
 
 `workflows` contains common code used for handling workflow metadata processing
 and response generation, as well as code associated with Bento's ingestion
 routines across the different data services.
```

### Comparing `bento_lib-7.0.0a1/README.md` & `bento_lib-7.0.0a2/bento_lib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: bento-lib
+Version: 7.0.0a2
+Summary: A set of common utilities and helpers for Bento platform services.
+Home-page: https://github.com/bento-platform/bento_lib
+Author: David Lougheed, Paul Pillot
+Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
+License: LGPLv3
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+Provides-Extra: flask
+Provides-Extra: django
+Provides-Extra: fastapi
+License-File: LICENSE
+
 # Bento Library (for Python Bento microservices)
 
 ![Test Status](https://github.com/bento-platform/bento_lib/workflows/Test/badge.svg)
 ![Lint Status](https://github.com/bento-platform/bento_lib/workflows/Lint/badge.svg)
 [![codecov](https://codecov.io/gh/bento-platform/bento_lib/branch/master/graph/badge.svg)](https://codecov.io/gh/bento-platform/bento_lib)
 [![PyPI version](https://badge.fury.io/py/bento-lib.svg)](https://badge.fury.io/py/bento-lib)
 
@@ -39,48 +57,26 @@
 releasing. If the API is broken in any way, including minor differences in the
 way a function behaves given an identical set of parameters (excluding bugfixes
 for unintentional behaviour), the MAJOR version must be incremented. In this 
 way, we guarantee that projects relying on this API do not accidentally break
 upon upgrading.
 
 
-### 2. Releasing from the Command Line
-
-```bash
-# IF NECESSARY: Install twine OUTSIDE of the virtual environment
-python3 -m pip install twine
-
-# Switch to the correct branch and make sure it's up to date
-git checkout master
-git pull
-
-# If needed, enter the project virtual environment
-source env/bin/activate
-
-# Remove existing build files
-rm -rf build/ dist/ bento_lib.egg-info/
+### 2. Releasing automatically
 
-# Build the new package
-python3 setup.py sdist bdist_wheel
-
-# In between these steps - test out the package... make sure everything works
-# before uploading it to production PyPI.
-
-# Upload it to PyPI
-twine upload dist/*
-```
+When a version is tagged on GitHub, a build + release CI pipeline is automatically triggered.
+Make sure that the tagged version is a valid semantic versioning translation of the version in
+`package.cfg`, and that the versions otherwise match.
 
 
 ## Modules
 
 ### `auth`
 
-`auth` provides Python service decorators and Django / DRF backends for dealing
-with the Bento container authentication headers (derived from
-`lua-resty-openidc`, set by the internal container NGINX instance.)
+`auth` provides Python service middleware for dealing with the Bento authorization service.
 
 ### `drs`
 
 `drs` provides utilities for fetching data and record metadata from 
 GA4GH-compatible DRS services, and Bento's own implementation (which has some 
 non-standard extensions.)
 
@@ -90,14 +86,19 @@
 microservices. Serialized objects can be at most 512 MB.
 
 Events should have a lower-case type which is type-insensitively unique and
 adequately describes the associated data.
 
 All Bento channels are prefixed with `bento.`.
 
+### `responses`
+
+`responses` contains standardized error message-generating functions 
+and exception handling functions for different Python web frameworks.
+
 ### `schemas`
 
 `schemas` contains common JSON schemas which may be useful to a variety of
 different Bento services.
 
 `schemas.bento` contains Bento-specific schemas, and `schemas.ga4gh` contains
 GA4GH-standardized schemas (possibly not exactly to spec.)
@@ -121,16 +122,17 @@
 `psycopg2`-provided
 [intermediate representation (IR)](https://www.psycopg.org/docs/sql.html) for
 PostgreSQL, allowing safe queries against a Postgres database.
 
 `search.queries` provides definitions for the Bento query AST and some helper
 methods for creating and processing ASTs.
 
-### `utils`
+### `types`
 
-`utils` contains miscellaneous utilities commonly required by Bento services.
+`types` contains Python type hints for different standard Bento 
+dictionaries/objects.
 
 ### `workflows`
 
 `workflows` contains common code used for handling workflow metadata processing
 and response generation, as well as code associated with Bento's ingestion
 routines across the different data services.
```

### Comparing `bento_lib-7.0.0a1/bento_lib/auth/middleware/base.py` & `bento_lib-7.0.0a2/bento_lib/auth/middleware/base.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/auth/middleware/django.py` & `bento_lib-7.0.0a2/bento_lib/auth/middleware/django.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/auth/middleware/fastapi.py` & `bento_lib-7.0.0a2/bento_lib/auth/middleware/fastapi.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/auth/middleware/flask.py` & `bento_lib-7.0.0a2/bento_lib/auth/middleware/flask.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/drs/utils.py` & `bento_lib-7.0.0a2/bento_lib/drs/utils.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/events/_event_bus.py` & `bento_lib-7.0.0a2/bento_lib/events/_event_bus.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/events/notifications.py` & `bento_lib-7.0.0a2/bento_lib/events/notifications.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/events/types.py` & `bento_lib-7.0.0a2/bento_lib/events/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/responses/errors.py` & `bento_lib-7.0.0a2/bento_lib/responses/errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/responses/fastapi_errors.py` & `bento_lib-7.0.0a2/bento_lib/responses/fastapi_errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/responses/flask_errors.py` & `bento_lib-7.0.0a2/bento_lib/responses/flask_errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/schemas/bento_data_use.schema.json` & `bento_lib-7.0.0a2/bento_lib/schemas/bento_data_use.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/schemas/bento_ingest.schema.json` & `bento_lib-7.0.0a2/bento_lib/schemas/bento_ingest.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/schemas/ga4gh_service_info.schema.json` & `bento_lib-7.0.0a2/bento_lib/schemas/ga4gh_service_info.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/search/data_structure.py` & `bento_lib-7.0.0a2/bento_lib/search/data_structure.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/search/operations.py` & `bento_lib-7.0.0a2/bento_lib/search/operations.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/search/postgres.py` & `bento_lib-7.0.0a2/bento_lib/search/postgres.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/search/queries.py` & `bento_lib-7.0.0a2/bento_lib/search/queries.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/types.py` & `bento_lib-7.0.0a2/bento_lib/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib/workflows.py` & `bento_lib-7.0.0a2/bento_lib/workflows.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/bento_lib.egg-info/PKG-INFO` & `bento_lib-7.0.0a2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: bento-lib
-Version: 7.0.0a1
-Summary: A set of common utilities and helpers for Bento platform services.
-Home-page: https://github.com/bento-platform/bento_lib
-Author: David Lougheed, Paul Pillot
-Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
-License: LGPLv3
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-Provides-Extra: flask
-Provides-Extra: django
-Provides-Extra: fastapi
-License-File: LICENSE
-
 # Bento Library (for Python Bento microservices)
 
 ![Test Status](https://github.com/bento-platform/bento_lib/workflows/Test/badge.svg)
 ![Lint Status](https://github.com/bento-platform/bento_lib/workflows/Lint/badge.svg)
 [![codecov](https://codecov.io/gh/bento-platform/bento_lib/branch/master/graph/badge.svg)](https://codecov.io/gh/bento-platform/bento_lib)
 [![PyPI version](https://badge.fury.io/py/bento-lib.svg)](https://badge.fury.io/py/bento-lib)
 
@@ -57,48 +39,26 @@
 releasing. If the API is broken in any way, including minor differences in the
 way a function behaves given an identical set of parameters (excluding bugfixes
 for unintentional behaviour), the MAJOR version must be incremented. In this 
 way, we guarantee that projects relying on this API do not accidentally break
 upon upgrading.
 
 
-### 2. Releasing from the Command Line
-
-```bash
-# IF NECESSARY: Install twine OUTSIDE of the virtual environment
-python3 -m pip install twine
-
-# Switch to the correct branch and make sure it's up to date
-git checkout master
-git pull
-
-# If needed, enter the project virtual environment
-source env/bin/activate
-
-# Remove existing build files
-rm -rf build/ dist/ bento_lib.egg-info/
+### 2. Releasing automatically
 
-# Build the new package
-python3 setup.py sdist bdist_wheel
-
-# In between these steps - test out the package... make sure everything works
-# before uploading it to production PyPI.
-
-# Upload it to PyPI
-twine upload dist/*
-```
+When a version is tagged on GitHub, a build + release CI pipeline is automatically triggered.
+Make sure that the tagged version is a valid semantic versioning translation of the version in
+`package.cfg`, and that the versions otherwise match.
 
 
 ## Modules
 
 ### `auth`
 
-`auth` provides Python service decorators and Django / DRF backends for dealing
-with the Bento container authentication headers (derived from
-`lua-resty-openidc`, set by the internal container NGINX instance.)
+`auth` provides Python service middleware for dealing with the Bento authorization service.
 
 ### `drs`
 
 `drs` provides utilities for fetching data and record metadata from 
 GA4GH-compatible DRS services, and Bento's own implementation (which has some 
 non-standard extensions.)
 
@@ -108,14 +68,19 @@
 microservices. Serialized objects can be at most 512 MB.
 
 Events should have a lower-case type which is type-insensitively unique and
 adequately describes the associated data.
 
 All Bento channels are prefixed with `bento.`.
 
+### `responses`
+
+`responses` contains standardized error message-generating functions 
+and exception handling functions for different Python web frameworks.
+
 ### `schemas`
 
 `schemas` contains common JSON schemas which may be useful to a variety of
 different Bento services.
 
 `schemas.bento` contains Bento-specific schemas, and `schemas.ga4gh` contains
 GA4GH-standardized schemas (possibly not exactly to spec.)
@@ -139,16 +104,17 @@
 `psycopg2`-provided
 [intermediate representation (IR)](https://www.psycopg.org/docs/sql.html) for
 PostgreSQL, allowing safe queries against a Postgres database.
 
 `search.queries` provides definitions for the Bento query AST and some helper
 methods for creating and processing ASTs.
 
-### `utils`
+### `types`
 
-`utils` contains miscellaneous utilities commonly required by Bento services.
+`types` contains Python type hints for different standard Bento 
+dictionaries/objects.
 
 ### `workflows`
 
 `workflows` contains common code used for handling workflow metadata processing
 and response generation, as well as code associated with Bento's ingestion
 routines across the different data services.
```

### Comparing `bento_lib-7.0.0a1/bento_lib.egg-info/SOURCES.txt` & `bento_lib-7.0.0a2/bento_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a1/setup.py` & `bento_lib-7.0.0a2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         "psycopg2-binary>=2.9.5,<3.0",
         "redis>=4.5.4,<5.0",
         "requests>=2.28.1,<3",
         "Werkzeug>=2.2.3,<3",
     ],
     extras_require={
         "flask": ["Flask>=2.2.5,<3"],
-        "django": ["Django>=4.1.9,<5", "djangorestframework>=3.14.0,<3.15"],
-        "fastapi": ["fastapi>=0.95.2,<0.96"],
+        "django": ["Django>=4.2.1,<5", "djangorestframework>=3.14.0,<3.15"],
+        "fastapi": ["fastapi>=0.95.2,<0.98"],
     },
 
     author=config["package"]["authors"],
     author_email=config["package"]["author_emails"],
 
     description="A set of common utilities and helpers for Bento platform services.",
     long_description=long_description,
```

