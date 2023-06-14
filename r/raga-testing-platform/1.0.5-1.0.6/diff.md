# Comparing `tmp/raga-testing-platform-1.0.5.tar.gz` & `tmp/raga-testing-platform-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-testing-platform-1.0.5.tar", last modified: Wed Jun 14 11:23:55 2023, max compression
+gzip compressed data, was "raga-testing-platform-1.0.6.tar", last modified: Wed Jun 14 12:01:00 2023, max compression
```

## Comparing `raga-testing-platform-1.0.5.tar` & `raga-testing-platform-1.0.6.tar`

### file list

```diff
@@ -1,38 +1,36 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 11:23:55.493055 raga-testing-platform-1.0.5/
--rw-r--r--   0 manabroy   (501) staff       (20)     6148 2023-06-14 10:14:55.000000 raga-testing-platform-1.0.5/.DS_Store
--rw-r--r--   0 manabroy   (501) staff       (20)     3095 2023-06-13 13:44:54.000000 raga-testing-platform-1.0.5/.gitignore
--rw-r--r--   0 manabroy   (501) staff       (20)     1073 2023-06-14 05:19:34.000000 raga-testing-platform-1.0.5/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      990 2023-06-14 11:23:55.492811 raga-testing-platform-1.0.5/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      289 2023-06-12 07:17:11.000000 raga-testing-platform-1.0.5/README.md
--rw-r--r--   0 manabroy   (501) staff       (20)     1005 2023-06-14 11:23:39.000000 raga-testing-platform-1.0.5/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 11:23:55.486653 raga-testing-platform-1.0.5/raga/
--rw-r--r--   0 manabroy   (501) staff       (20)     8196 2023-06-14 10:14:38.000000 raga-testing-platform-1.0.5/raga/.DS_Store
--rw-r--r--   0 manabroy   (501) staff       (20)     1012 2023-06-14 11:02:43.000000 raga-testing-platform-1.0.5/raga/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1236 2023-06-14 10:12:53.000000 raga-testing-platform-1.0.5/raga/auth.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9319 2023-06-14 11:21:31.000000 raga-testing-platform-1.0.5/raga/dataset.py
--rw-r--r--   0 manabroy   (501) staff       (20)      498 2023-06-12 11:57:49.000000 raga-testing-platform-1.0.5/raga/dataset_creds.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 11:23:55.487382 raga-testing-platform-1.0.5/raga/docs/
--rw-r--r--   0 manabroy   (501) staff       (20)       82 2023-06-12 07:15:42.000000 raga-testing-platform-1.0.5/raga/docs/conf.py
--rw-r--r--   0 manabroy   (501) staff       (20)      160 2023-06-12 09:52:28.000000 raga-testing-platform-1.0.5/raga/docs/index.rst
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 11:23:55.488563 raga-testing-platform-1.0.5/raga/examples/
--rw-r--r--   0 manabroy   (501) staff       (20)      151 2023-06-13 11:37:36.000000 raga-testing-platform-1.0.5/raga/examples/.raga
--rw-r--r--   0 manabroy   (501) staff       (20)     1780 2023-06-12 13:42:21.000000 raga-testing-platform-1.0.5/raga/examples/coco.json
--rw-r--r--   0 manabroy   (501) staff       (20)     1588 2023-06-14 11:22:06.000000 raga-testing-platform-1.0.5/raga/examples/example.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1392 2023-06-14 10:13:12.000000 raga-testing-platform-1.0.5/raga/test_session.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 11:23:55.488732 raga-testing-platform-1.0.5/raga/tests/
--rw-r--r--   0 manabroy   (501) staff       (20)       51 2023-06-12 07:15:00.000000 raga-testing-platform-1.0.5/raga/tests/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)       59 2023-06-12 07:51:37.000000 raga-testing-platform-1.0.5/raga/tests.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 11:23:55.489463 raga-testing-platform-1.0.5/raga/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     3601 2023-06-13 13:06:36.000000 raga-testing-platform-1.0.5/raga/utils/http_client.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2055 2023-06-14 11:17:43.000000 raga-testing-platform-1.0.5/raga/utils/raga_config_reader.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 11:23:55.490447 raga-testing-platform-1.0.5/raga/validators/
--rw-r--r--   0 manabroy   (501) staff       (20)      860 2023-06-12 10:10:59.000000 raga-testing-platform-1.0.5/raga/validators/dataset_creds_validations.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1611 2023-06-13 10:18:53.000000 raga-testing-platform-1.0.5/raga/validators/dataset_validations.py
--rw-r--r--   0 manabroy   (501) staff       (20)      715 2023-06-13 09:15:46.000000 raga-testing-platform-1.0.5/raga/validators/test_session_validation.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 11:23:55.492060 raga-testing-platform-1.0.5/raga_testing_platform.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      990 2023-06-14 11:23:55.000000 raga-testing-platform-1.0.5/raga_testing_platform.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      711 2023-06-14 11:23:55.000000 raga-testing-platform-1.0.5/raga_testing_platform.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-06-14 11:23:55.000000 raga-testing-platform-1.0.5/raga_testing_platform.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       61 2023-06-14 11:23:55.000000 raga-testing-platform-1.0.5/raga_testing_platform.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        5 2023-06-14 11:23:55.000000 raga-testing-platform-1.0.5/raga_testing_platform.egg-info/top_level.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-06-14 11:23:55.493111 raga-testing-platform-1.0.5/setup.cfg
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 12:01:00.414315 raga-testing-platform-1.0.6/
+-rw-r--r--   0 manabroy   (501) staff       (20)     6148 2023-06-14 11:27:52.000000 raga-testing-platform-1.0.6/.DS_Store
+-rw-r--r--   0 manabroy   (501) staff       (20)     3095 2023-06-13 13:44:54.000000 raga-testing-platform-1.0.6/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)     1073 2023-06-14 05:19:34.000000 raga-testing-platform-1.0.6/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)     3110 2023-06-14 12:01:00.414118 raga-testing-platform-1.0.6/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)     2408 2023-06-14 11:59:49.000000 raga-testing-platform-1.0.6/README.md
+-rw-r--r--   0 manabroy   (501) staff       (20)     1005 2023-06-14 12:00:46.000000 raga-testing-platform-1.0.6/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 12:01:00.407857 raga-testing-platform-1.0.6/raga/
+-rw-r--r--   0 manabroy   (501) staff       (20)     8196 2023-06-14 10:14:38.000000 raga-testing-platform-1.0.6/raga/.DS_Store
+-rw-r--r--   0 manabroy   (501) staff       (20)     1054 2023-06-14 11:27:11.000000 raga-testing-platform-1.0.6/raga/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1236 2023-06-14 10:12:53.000000 raga-testing-platform-1.0.6/raga/auth.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9319 2023-06-14 11:21:31.000000 raga-testing-platform-1.0.6/raga/dataset.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      498 2023-06-12 11:57:49.000000 raga-testing-platform-1.0.6/raga/dataset_creds.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 12:01:00.408609 raga-testing-platform-1.0.6/raga/docs/
+-rw-r--r--   0 manabroy   (501) staff       (20)       82 2023-06-12 07:15:42.000000 raga-testing-platform-1.0.6/raga/docs/conf.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      160 2023-06-12 09:52:28.000000 raga-testing-platform-1.0.6/raga/docs/index.rst
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 12:01:00.408980 raga-testing-platform-1.0.6/raga/examples/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1588 2023-06-14 11:22:06.000000 raga-testing-platform-1.0.6/raga/examples/example.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1392 2023-06-14 10:13:12.000000 raga-testing-platform-1.0.6/raga/test_session.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 12:01:00.409752 raga-testing-platform-1.0.6/raga/tests/
+-rw-r--r--   0 manabroy   (501) staff       (20)       51 2023-06-12 07:15:00.000000 raga-testing-platform-1.0.6/raga/tests/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       59 2023-06-12 07:51:37.000000 raga-testing-platform-1.0.6/raga/tests.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 12:01:00.410756 raga-testing-platform-1.0.6/raga/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3601 2023-06-13 13:06:36.000000 raga-testing-platform-1.0.6/raga/utils/http_client.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2055 2023-06-14 11:17:43.000000 raga-testing-platform-1.0.6/raga/utils/raga_config_reader.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 12:01:00.411972 raga-testing-platform-1.0.6/raga/validators/
+-rw-r--r--   0 manabroy   (501) staff       (20)      860 2023-06-12 10:10:59.000000 raga-testing-platform-1.0.6/raga/validators/dataset_creds_validations.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1611 2023-06-13 10:18:53.000000 raga-testing-platform-1.0.6/raga/validators/dataset_validations.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      715 2023-06-13 09:15:46.000000 raga-testing-platform-1.0.6/raga/validators/test_session_validation.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 12:01:00.413663 raga-testing-platform-1.0.6/raga_testing_platform.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3110 2023-06-14 12:01:00.000000 raga-testing-platform-1.0.6/raga_testing_platform.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      667 2023-06-14 12:01:00.000000 raga-testing-platform-1.0.6/raga_testing_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-06-14 12:01:00.000000 raga-testing-platform-1.0.6/raga_testing_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       61 2023-06-14 12:01:00.000000 raga-testing-platform-1.0.6/raga_testing_platform.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        5 2023-06-14 12:01:00.000000 raga-testing-platform-1.0.6/raga_testing_platform.egg-info/top_level.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-06-14 12:01:00.414359 raga-testing-platform-1.0.6/setup.cfg
```

### Comparing `raga-testing-platform-1.0.5/.gitignore` & `raga-testing-platform-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.5/LICENSE` & `raga-testing-platform-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.5/pyproject.toml` & `raga-testing-platform-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-testing-platform"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Raga AI", email="support@ragaai.com" },
 ]
 maintainers = [{ name = "Raga AI", email = "support@ragaai.com" }]
 dependencies = [
     "pandas==2.0.2",
     "urllib3==1.26.7",
```

### Comparing `raga-testing-platform-1.0.5/raga/.DS_Store` & `raga-testing-platform-1.0.6/raga/.DS_Store`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.5/raga/__init__.py` & `raga-testing-platform-1.0.6/raga/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,21 @@
         level=logging.DEBUG
     )
 else:
     logging.basicConfig(
         format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
         level=logging.INFO
     )
+if debug_mode:
+    # Add a file handler to log messages to a file
+    file_handler = logging.FileHandler('debug.log')
+    file_handler.setLevel(logging.DEBUG)
+    file_handler.setFormatter(logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s'))
 
-# Add a file handler to log messages to a file
-file_handler = logging.FileHandler('debug.log')
-file_handler.setLevel(logging.DEBUG)
-file_handler.setFormatter(logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s'))
-
-# Add the file handler to the logger
-logger = logging.getLogger(__name__)
-logger.addHandler(file_handler)
+    # Add the file handler to the logger
+    logger = logging.getLogger(__name__)
+    logger.addHandler(file_handler)
 
 from .auth import *
 from .test_session import *
 from .dataset_creds import *
 from .dataset import *
```

### Comparing `raga-testing-platform-1.0.5/raga/auth.py` & `raga-testing-platform-1.0.6/raga/auth.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.5/raga/dataset.py` & `raga-testing-platform-1.0.6/raga/dataset.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.5/raga/examples/example.py` & `raga-testing-platform-1.0.6/raga/examples/example.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.5/raga/test_session.py` & `raga-testing-platform-1.0.6/raga/test_session.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.5/raga/utils/http_client.py` & `raga-testing-platform-1.0.6/raga/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.5/raga/utils/raga_config_reader.py` & `raga-testing-platform-1.0.6/raga/utils/raga_config_reader.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.5/raga/validators/dataset_creds_validations.py` & `raga-testing-platform-1.0.6/raga/validators/dataset_creds_validations.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.5/raga/validators/dataset_validations.py` & `raga-testing-platform-1.0.6/raga/validators/dataset_validations.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.5/raga/validators/test_session_validation.py` & `raga-testing-platform-1.0.6/raga/validators/test_session_validation.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.5/raga_testing_platform.egg-info/SOURCES.txt` & `raga-testing-platform-1.0.6/raga_testing_platform.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 raga/auth.py
 raga/dataset.py
 raga/dataset_creds.py
 raga/test_session.py
 raga/tests.py
 raga/docs/conf.py
 raga/docs/index.rst
-raga/examples/.raga
-raga/examples/coco.json
 raga/examples/example.py
 raga/tests/__init__.py
 raga/utils/http_client.py
 raga/utils/raga_config_reader.py
 raga/validators/dataset_creds_validations.py
 raga/validators/dataset_validations.py
 raga/validators/test_session_validation.py
```

