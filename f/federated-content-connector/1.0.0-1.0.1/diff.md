# Comparing `tmp/federated-content-connector-1.0.0.tar.gz` & `tmp/federated-content-connector-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "federated-content-connector-1.0.0.tar", last modified: Wed Jun  7 11:20:26 2023, max compression
+gzip compressed data, was "federated-content-connector-1.0.1.tar", last modified: Wed Jun 14 13:20:24 2023, max compression
```

## Comparing `federated-content-connector-1.0.0.tar` & `federated-content-connector-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.788159 federated-content-connector-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8317 2023-06-07 11:20:26.788159 federated-content-connector-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.780159 federated-content-connector-1.0.0/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     8965 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/course_metadata_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/filters/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/management/commands/import_course_runs_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.776158 federated-content-connector-1.0.0/federated_content_connector/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector/templates/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/templates/federated_content_connector/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8317 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.788159 federated-content-connector-1.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-07 11:20:26.788159 federated-content-connector-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.788159 federated-content-connector-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/tests/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8397 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.459163 federated-content-connector-1.0.1/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9672 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/course_metadata_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.459163 federated-content-connector-1.0.1/federated_content_connector/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/filters/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.459163 federated-content-connector-1.0.1/federated_content_connector/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.459163 federated-content-connector-1.0.1/federated_content_connector/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/management/commands/import_course_runs_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.459163 federated-content-connector-1.0.1/federated_content_connector/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/federated_content_connector/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.455163 federated-content-connector-1.0.1/federated_content_connector/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/federated_content_connector/templates/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/templates/federated_content_connector/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.459163 federated-content-connector-1.0.1/federated_content_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8397 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/tests/test_signals.py
```

### Comparing `federated-content-connector-1.0.0/CHANGELOG.rst` & `federated-content-connector-1.0.1/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.0.1 – 2023-06-14
+------------------
+* Update courserun seat sorting logic.
+
 1.0.0 – 2023-06-06
 ------------------
 * Fetch course metadata from discovery and store.
 
 0.2.1 – 2023-06-5
 ------------------
 * Fixed issue with product source data type
```

### Comparing `federated-content-connector-1.0.0/LICENSE.txt` & `federated-content-connector-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.0/PKG-INFO` & `federated-content-connector-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 1.0.0
+Version: 1.0.1
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.0.1 – 2023-06-14
+------------------
+* Update courserun seat sorting logic.
+
 1.0.0 – 2023-06-06
 ------------------
 * Fetch course metadata from discovery and store.
 
 0.2.1 – 2023-06-5
 ------------------
 * Fixed issue with product source data type
```

### Comparing `federated-content-connector-1.0.0/README.rst` & `federated-content-connector-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.0/federated_content_connector/apps.py` & `federated-content-connector-1.0.1/federated_content_connector/apps.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.0/federated_content_connector/course_metadata_importer.py` & `federated-content-connector-1.0.1/federated_content_connector/course_metadata_importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -153,18 +153,21 @@
         return results
 
     @classmethod
     def process_courses_details(cls, courserun_locators, courses_details):
         """
         Parse and extract the minimal data that we need.
         """
+        log_prefix = 'COURSE_METADATA_IMPORTER'
+
         courses = {}
         for courserun_locator in courserun_locators:
             course_key = cls.construct_course_key(courserun_locator)
             courserun_key = str(courserun_locator)
+            logger.info(f'[{log_prefix}] Process. CourserunKey: {courserun_key}, CourseKey: {course_key}')
             course_metadata = cls.find_attr(courses_details, 'key', course_key)
             if not course_metadata:
                 logger.info(f'[COURSE_METADATA_IMPORTER] Metadata not found. CourseKey: {course_key}')
                 continue
 
             course_type = course_metadata.get('course_type') or ''
             product_source = course_metadata.get('product_source') or ''
@@ -182,14 +185,18 @@
             else:
                 course_run = cls.find_attr(course_metadata.get('course_runs'), 'key', courserun_key)
                 if course_run:
                     seat = cls.find_best_mode_seat(course_run.get('seats'))
                     enroll_by = seat.get('upgrade_deadline')
                     start_date = course_run.get('start')
                     end_date = course_run.get('end')
+                else:
+                    logger.info(
+                        f'[{log_prefix}] Courserun not found. CourserunKey: {courserun_key}, CourseKey: {course_key}'
+                    )
 
             course_data = {
                 'course_type': course_type,
                 'product_source': product_source,
                 'enroll_by': enroll_by,
                 'start_date': start_date,
                 'end_date': end_date,
@@ -210,15 +217,25 @@
             )
 
     @classmethod
     def find_best_mode_seat(cls, seats):
         """
         Find the seat by best course mode.
         """
-        return sorted(seats, key=lambda x: BEST_MODE_ORDER.index(x['type']))[0]
+        def sort_key(mode):
+            """
+            Assign a weight to the seat dictionary based on the position of its type in best moode order list.
+            """
+            mode_type = mode['type']
+            if mode_type in BEST_MODE_ORDER:
+                return len(BEST_MODE_ORDER) - BEST_MODE_ORDER.index(mode_type)
+            else:
+                return 0
+
+        return sorted(seats, key=sort_key, reverse=True)[0]
 
     @classmethod
     def chunks(cls, keys, chunk_size=50):
         """
         Yield chunks of size `chunk_size`.
         """
         for i in range(0, len(keys), chunk_size):
```

### Comparing `federated-content-connector-1.0.0/federated_content_connector/filters/pipeline.py` & `federated-content-connector-1.0.1/federated_content_connector/filters/pipeline.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.0/federated_content_connector/migrations/0001_initial.py` & `federated-content-connector-1.0.1/federated_content_connector/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.0/federated_content_connector/models.py` & `federated-content-connector-1.0.1/federated_content_connector/models.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.0/federated_content_connector/signals.py` & `federated-content-connector-1.0.1/federated_content_connector/signals.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.0/federated_content_connector/tasks.py` & `federated-content-connector-1.0.1/federated_content_connector/tasks.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.0/federated_content_connector/templates/federated_content_connector/base.html` & `federated-content-connector-1.0.1/federated_content_connector/templates/federated_content_connector/base.html`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.0/federated_content_connector.egg-info/PKG-INFO` & `federated-content-connector-1.0.1/federated_content_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 1.0.0
+Version: 1.0.1
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.0.1 – 2023-06-14
+------------------
+* Update courserun seat sorting logic.
+
 1.0.0 – 2023-06-06
 ------------------
 * Fetch course metadata from discovery and store.
 
 0.2.1 – 2023-06-5
 ------------------
 * Fixed issue with product source data type
```

### Comparing `federated-content-connector-1.0.0/federated_content_connector.egg-info/SOURCES.txt` & `federated-content-connector-1.0.1/federated_content_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.0/requirements/constraints.txt` & `federated-content-connector-1.0.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.0/setup.py` & `federated-content-connector-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.0/tests/test_signals.py` & `federated-content-connector-1.0.1/tests/test_signals.py`

 * *Files identical despite different names*

