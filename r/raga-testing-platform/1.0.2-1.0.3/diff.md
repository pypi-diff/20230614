# Comparing `tmp/raga-testing-platform-1.0.2.tar.gz` & `tmp/raga-testing-platform-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-testing-platform-1.0.2.tar", last modified: Wed Jun 14 09:52:16 2023, max compression
+gzip compressed data, was "raga-testing-platform-1.0.3.tar", last modified: Wed Jun 14 10:07:59 2023, max compression
```

## Comparing `raga-testing-platform-1.0.2.tar` & `raga-testing-platform-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,38 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.629429 raga-testing-platform-1.0.2/
--rw-r--r--   0 manabroy   (501) staff       (20)     1073 2023-06-14 05:19:34.000000 raga-testing-platform-1.0.2/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      869 2023-06-14 09:52:16.629264 raga-testing-platform-1.0.2/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      289 2023-06-12 07:17:11.000000 raga-testing-platform-1.0.2/README.md
--rw-r--r--   0 manabroy   (501) staff       (20)      565 2023-06-14 09:51:56.000000 raga-testing-platform-1.0.2/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.625072 raga-testing-platform-1.0.2/raga/
--rw-r--r--   0 manabroy   (501) staff       (20)      977 2023-06-13 11:01:16.000000 raga-testing-platform-1.0.2/raga/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1243 2023-06-13 13:01:16.000000 raga-testing-platform-1.0.2/raga/auth.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9087 2023-06-14 09:51:10.000000 raga-testing-platform-1.0.2/raga/dataset.py
--rw-r--r--   0 manabroy   (501) staff       (20)      498 2023-06-12 11:57:49.000000 raga-testing-platform-1.0.2/raga/dataset_creds.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.625567 raga-testing-platform-1.0.2/raga/docs/
--rw-r--r--   0 manabroy   (501) staff       (20)       82 2023-06-12 07:15:42.000000 raga-testing-platform-1.0.2/raga/docs/conf.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.625917 raga-testing-platform-1.0.2/raga/examples/
--rw-r--r--   0 manabroy   (501) staff       (20)     1588 2023-06-13 13:07:53.000000 raga-testing-platform-1.0.2/raga/examples/example.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1399 2023-06-13 13:05:33.000000 raga-testing-platform-1.0.2/raga/test_session.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.626228 raga-testing-platform-1.0.2/raga/tests/
--rw-r--r--   0 manabroy   (501) staff       (20)       51 2023-06-12 07:15:00.000000 raga-testing-platform-1.0.2/raga/tests/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)       59 2023-06-12 07:51:37.000000 raga-testing-platform-1.0.2/raga/tests.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.627013 raga-testing-platform-1.0.2/raga/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     3601 2023-06-13 13:06:36.000000 raga-testing-platform-1.0.2/raga/utils/http_client.py
--rw-r--r--   0 manabroy   (501) staff       (20)      929 2023-06-12 12:28:35.000000 raga-testing-platform-1.0.2/raga/utils/raga_config_reader.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.627949 raga-testing-platform-1.0.2/raga/validators/
--rw-r--r--   0 manabroy   (501) staff       (20)      860 2023-06-12 10:10:59.000000 raga-testing-platform-1.0.2/raga/validators/dataset_creds_validations.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1611 2023-06-13 10:18:53.000000 raga-testing-platform-1.0.2/raga/validators/dataset_validations.py
--rw-r--r--   0 manabroy   (501) staff       (20)      715 2023-06-13 09:15:46.000000 raga-testing-platform-1.0.2/raga/validators/test_session_validation.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.629056 raga-testing-platform-1.0.2/raga_testing_platform.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      869 2023-06-14 09:52:16.000000 raga-testing-platform-1.0.2/raga_testing_platform.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      567 2023-06-14 09:52:16.000000 raga-testing-platform-1.0.2/raga_testing_platform.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-06-14 09:52:16.000000 raga-testing-platform-1.0.2/raga_testing_platform.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        5 2023-06-14 09:52:16.000000 raga-testing-platform-1.0.2/raga_testing_platform.egg-info/top_level.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-06-14 09:52:16.629473 raga-testing-platform-1.0.2/setup.cfg
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.234393 raga-testing-platform-1.0.3/
+-rw-r--r--   0 manabroy   (501) staff       (20)     6148 2023-06-14 09:48:34.000000 raga-testing-platform-1.0.3/.DS_Store
+-rw-r--r--   0 manabroy   (501) staff       (20)     3095 2023-06-13 13:44:54.000000 raga-testing-platform-1.0.3/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)     1073 2023-06-14 05:19:34.000000 raga-testing-platform-1.0.3/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      990 2023-06-14 10:07:59.234143 raga-testing-platform-1.0.3/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      289 2023-06-12 07:17:11.000000 raga-testing-platform-1.0.3/README.md
+-rw-r--r--   0 manabroy   (501) staff       (20)     1005 2023-06-14 10:07:43.000000 raga-testing-platform-1.0.3/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.225841 raga-testing-platform-1.0.3/raga/
+-rw-r--r--   0 manabroy   (501) staff       (20)     8196 2023-06-14 09:48:39.000000 raga-testing-platform-1.0.3/raga/.DS_Store
+-rw-r--r--   0 manabroy   (501) staff       (20)      977 2023-06-13 11:01:16.000000 raga-testing-platform-1.0.3/raga/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1243 2023-06-13 13:01:16.000000 raga-testing-platform-1.0.3/raga/auth.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9087 2023-06-14 09:51:10.000000 raga-testing-platform-1.0.3/raga/dataset.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      498 2023-06-12 11:57:49.000000 raga-testing-platform-1.0.3/raga/dataset_creds.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.226843 raga-testing-platform-1.0.3/raga/docs/
+-rw-r--r--   0 manabroy   (501) staff       (20)       82 2023-06-12 07:15:42.000000 raga-testing-platform-1.0.3/raga/docs/conf.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      160 2023-06-12 09:52:28.000000 raga-testing-platform-1.0.3/raga/docs/index.rst
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.227875 raga-testing-platform-1.0.3/raga/examples/
+-rw-r--r--   0 manabroy   (501) staff       (20)      151 2023-06-13 11:37:36.000000 raga-testing-platform-1.0.3/raga/examples/.raga
+-rw-r--r--   0 manabroy   (501) staff       (20)     1780 2023-06-12 13:42:21.000000 raga-testing-platform-1.0.3/raga/examples/coco.json
+-rw-r--r--   0 manabroy   (501) staff       (20)     1588 2023-06-13 13:07:53.000000 raga-testing-platform-1.0.3/raga/examples/example.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1399 2023-06-13 13:05:33.000000 raga-testing-platform-1.0.3/raga/test_session.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.228829 raga-testing-platform-1.0.3/raga/tests/
+-rw-r--r--   0 manabroy   (501) staff       (20)       51 2023-06-12 07:15:00.000000 raga-testing-platform-1.0.3/raga/tests/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       59 2023-06-12 07:51:37.000000 raga-testing-platform-1.0.3/raga/tests.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.230189 raga-testing-platform-1.0.3/raga/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3601 2023-06-13 13:06:36.000000 raga-testing-platform-1.0.3/raga/utils/http_client.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      929 2023-06-12 12:28:35.000000 raga-testing-platform-1.0.3/raga/utils/raga_config_reader.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.231284 raga-testing-platform-1.0.3/raga/validators/
+-rw-r--r--   0 manabroy   (501) staff       (20)      860 2023-06-12 10:10:59.000000 raga-testing-platform-1.0.3/raga/validators/dataset_creds_validations.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1611 2023-06-13 10:18:53.000000 raga-testing-platform-1.0.3/raga/validators/dataset_validations.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      715 2023-06-13 09:15:46.000000 raga-testing-platform-1.0.3/raga/validators/test_session_validation.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.233748 raga-testing-platform-1.0.3/raga_testing_platform.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      990 2023-06-14 10:07:59.000000 raga-testing-platform-1.0.3/raga_testing_platform.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      711 2023-06-14 10:07:59.000000 raga-testing-platform-1.0.3/raga_testing_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-06-14 10:07:59.000000 raga-testing-platform-1.0.3/raga_testing_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       61 2023-06-14 10:07:59.000000 raga-testing-platform-1.0.3/raga_testing_platform.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        5 2023-06-14 10:07:59.000000 raga-testing-platform-1.0.3/raga_testing_platform.egg-info/top_level.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-06-14 10:07:59.234444 raga-testing-platform-1.0.3/setup.cfg
```

### Comparing `raga-testing-platform-1.0.2/LICENSE` & `raga-testing-platform-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.2/PKG-INFO` & `raga-testing-platform-1.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: raga-testing-platform
-Version: 1.0.2
+Version: 1.0.3
 Summary: Short description or overview of the raga package.
 Author-email: Raga AI <support@ragaai.com>
+Maintainer-email: Raga AI <support@ragaai.com>
 Project-URL: Homepage, https://github.com/whoosh-labs/testing-platform-python-client
 Project-URL: Bug Tracker, https://github.com/whoosh-labs/testing-platform-python-client/issues
+Keywords: testing-platform,raga-testing-platform,model-testing,AB_testing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # testing_platform
 
 Short description or overview of the my_package package.
```

### Comparing `raga-testing-platform-1.0.2/raga/__init__.py` & `raga-testing-platform-1.0.3/raga/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.2/raga/auth.py` & `raga-testing-platform-1.0.3/raga/auth.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.2/raga/dataset.py` & `raga-testing-platform-1.0.3/raga/dataset.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.2/raga/examples/example.py` & `raga-testing-platform-1.0.3/raga/examples/example.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.2/raga/test_session.py` & `raga-testing-platform-1.0.3/raga/test_session.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.2/raga/utils/http_client.py` & `raga-testing-platform-1.0.3/raga/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.2/raga/utils/raga_config_reader.py` & `raga-testing-platform-1.0.3/raga/utils/raga_config_reader.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.2/raga/validators/dataset_creds_validations.py` & `raga-testing-platform-1.0.3/raga/validators/dataset_creds_validations.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.2/raga/validators/dataset_validations.py` & `raga-testing-platform-1.0.3/raga/validators/dataset_validations.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.2/raga/validators/test_session_validation.py` & `raga-testing-platform-1.0.3/raga/validators/test_session_validation.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.2/raga_testing_platform.egg-info/PKG-INFO` & `raga-testing-platform-1.0.3/raga_testing_platform.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: raga-testing-platform
-Version: 1.0.2
+Version: 1.0.3
 Summary: Short description or overview of the raga package.
 Author-email: Raga AI <support@ragaai.com>
+Maintainer-email: Raga AI <support@ragaai.com>
 Project-URL: Homepage, https://github.com/whoosh-labs/testing-platform-python-client
 Project-URL: Bug Tracker, https://github.com/whoosh-labs/testing-platform-python-client/issues
+Keywords: testing-platform,raga-testing-platform,model-testing,AB_testing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # testing_platform
 
 Short description or overview of the my_package package.
```

