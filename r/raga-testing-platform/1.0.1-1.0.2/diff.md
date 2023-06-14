# Comparing `tmp/raga-testing-platform-1.0.1.tar.gz` & `tmp/raga-testing-platform-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-testing-platform-1.0.1.tar", last modified: Wed Jun 14 05:20:03 2023, max compression
+gzip compressed data, was "raga-testing-platform-1.0.2.tar", last modified: Wed Jun 14 09:52:16 2023, max compression
```

## Comparing `raga-testing-platform-1.0.1.tar` & `raga-testing-platform-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.542548 raga-testing-platform-1.0.1/
--rw-r--r--   0 manabroy   (501) staff       (20)     1073 2023-06-14 05:19:34.000000 raga-testing-platform-1.0.1/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      869 2023-06-14 05:20:03.542344 raga-testing-platform-1.0.1/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      289 2023-06-12 07:17:11.000000 raga-testing-platform-1.0.1/README.md
--rw-r--r--   0 manabroy   (501) staff       (20)      565 2023-06-14 05:19:15.000000 raga-testing-platform-1.0.1/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.538511 raga-testing-platform-1.0.1/raga/
--rw-r--r--   0 manabroy   (501) staff       (20)      977 2023-06-13 11:01:16.000000 raga-testing-platform-1.0.1/raga/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1243 2023-06-13 13:01:16.000000 raga-testing-platform-1.0.1/raga/auth.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9070 2023-06-13 13:27:02.000000 raga-testing-platform-1.0.1/raga/dataset.py
--rw-r--r--   0 manabroy   (501) staff       (20)      498 2023-06-12 11:57:49.000000 raga-testing-platform-1.0.1/raga/dataset_creds.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.538829 raga-testing-platform-1.0.1/raga/docs/
--rw-r--r--   0 manabroy   (501) staff       (20)       82 2023-06-12 07:15:42.000000 raga-testing-platform-1.0.1/raga/docs/conf.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.539148 raga-testing-platform-1.0.1/raga/examples/
--rw-r--r--   0 manabroy   (501) staff       (20)     1588 2023-06-13 13:07:53.000000 raga-testing-platform-1.0.1/raga/examples/example.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1399 2023-06-13 13:05:33.000000 raga-testing-platform-1.0.1/raga/test_session.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.539445 raga-testing-platform-1.0.1/raga/tests/
--rw-r--r--   0 manabroy   (501) staff       (20)       51 2023-06-12 07:15:00.000000 raga-testing-platform-1.0.1/raga/tests/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)       59 2023-06-12 07:51:37.000000 raga-testing-platform-1.0.1/raga/tests.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.540252 raga-testing-platform-1.0.1/raga/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     3601 2023-06-13 13:06:36.000000 raga-testing-platform-1.0.1/raga/utils/http_client.py
--rw-r--r--   0 manabroy   (501) staff       (20)      929 2023-06-12 12:28:35.000000 raga-testing-platform-1.0.1/raga/utils/raga_config_reader.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.541185 raga-testing-platform-1.0.1/raga/validators/
--rw-r--r--   0 manabroy   (501) staff       (20)      860 2023-06-12 10:10:59.000000 raga-testing-platform-1.0.1/raga/validators/dataset_creds_validations.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1611 2023-06-13 10:18:53.000000 raga-testing-platform-1.0.1/raga/validators/dataset_validations.py
--rw-r--r--   0 manabroy   (501) staff       (20)      715 2023-06-13 09:15:46.000000 raga-testing-platform-1.0.1/raga/validators/test_session_validation.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.542075 raga-testing-platform-1.0.1/raga_testing_platform.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      869 2023-06-14 05:20:03.000000 raga-testing-platform-1.0.1/raga_testing_platform.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      567 2023-06-14 05:20:03.000000 raga-testing-platform-1.0.1/raga_testing_platform.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-06-14 05:20:03.000000 raga-testing-platform-1.0.1/raga_testing_platform.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        5 2023-06-14 05:20:03.000000 raga-testing-platform-1.0.1/raga_testing_platform.egg-info/top_level.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-06-14 05:20:03.542604 raga-testing-platform-1.0.1/setup.cfg
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.629429 raga-testing-platform-1.0.2/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1073 2023-06-14 05:19:34.000000 raga-testing-platform-1.0.2/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      869 2023-06-14 09:52:16.629264 raga-testing-platform-1.0.2/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      289 2023-06-12 07:17:11.000000 raga-testing-platform-1.0.2/README.md
+-rw-r--r--   0 manabroy   (501) staff       (20)      565 2023-06-14 09:51:56.000000 raga-testing-platform-1.0.2/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.625072 raga-testing-platform-1.0.2/raga/
+-rw-r--r--   0 manabroy   (501) staff       (20)      977 2023-06-13 11:01:16.000000 raga-testing-platform-1.0.2/raga/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1243 2023-06-13 13:01:16.000000 raga-testing-platform-1.0.2/raga/auth.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9087 2023-06-14 09:51:10.000000 raga-testing-platform-1.0.2/raga/dataset.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      498 2023-06-12 11:57:49.000000 raga-testing-platform-1.0.2/raga/dataset_creds.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.625567 raga-testing-platform-1.0.2/raga/docs/
+-rw-r--r--   0 manabroy   (501) staff       (20)       82 2023-06-12 07:15:42.000000 raga-testing-platform-1.0.2/raga/docs/conf.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.625917 raga-testing-platform-1.0.2/raga/examples/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1588 2023-06-13 13:07:53.000000 raga-testing-platform-1.0.2/raga/examples/example.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1399 2023-06-13 13:05:33.000000 raga-testing-platform-1.0.2/raga/test_session.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.626228 raga-testing-platform-1.0.2/raga/tests/
+-rw-r--r--   0 manabroy   (501) staff       (20)       51 2023-06-12 07:15:00.000000 raga-testing-platform-1.0.2/raga/tests/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       59 2023-06-12 07:51:37.000000 raga-testing-platform-1.0.2/raga/tests.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.627013 raga-testing-platform-1.0.2/raga/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3601 2023-06-13 13:06:36.000000 raga-testing-platform-1.0.2/raga/utils/http_client.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      929 2023-06-12 12:28:35.000000 raga-testing-platform-1.0.2/raga/utils/raga_config_reader.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.627949 raga-testing-platform-1.0.2/raga/validators/
+-rw-r--r--   0 manabroy   (501) staff       (20)      860 2023-06-12 10:10:59.000000 raga-testing-platform-1.0.2/raga/validators/dataset_creds_validations.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1611 2023-06-13 10:18:53.000000 raga-testing-platform-1.0.2/raga/validators/dataset_validations.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      715 2023-06-13 09:15:46.000000 raga-testing-platform-1.0.2/raga/validators/test_session_validation.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 09:52:16.629056 raga-testing-platform-1.0.2/raga_testing_platform.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      869 2023-06-14 09:52:16.000000 raga-testing-platform-1.0.2/raga_testing_platform.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      567 2023-06-14 09:52:16.000000 raga-testing-platform-1.0.2/raga_testing_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-06-14 09:52:16.000000 raga-testing-platform-1.0.2/raga_testing_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        5 2023-06-14 09:52:16.000000 raga-testing-platform-1.0.2/raga_testing_platform.egg-info/top_level.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-06-14 09:52:16.629473 raga-testing-platform-1.0.2/setup.cfg
```

### Comparing `raga-testing-platform-1.0.1/LICENSE` & `raga-testing-platform-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.1/PKG-INFO` & `raga-testing-platform-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-testing-platform
-Version: 1.0.1
+Version: 1.0.2
 Summary: Short description or overview of the raga package.
 Author-email: Raga AI <support@ragaai.com>
 Project-URL: Homepage, https://github.com/whoosh-labs/testing-platform-python-client
 Project-URL: Bug Tracker, https://github.com/whoosh-labs/testing-platform-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `raga-testing-platform-1.0.1/pyproject.toml` & `raga-testing-platform-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "raga-testing-platform"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Raga AI", email="support@ragaai.com" },
 ]
 description = "Short description or overview of the raga package."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `raga-testing-platform-1.0.1/raga/__init__.py` & `raga-testing-platform-1.0.2/raga/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.1/raga/auth.py` & `raga-testing-platform-1.0.2/raga/auth.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.1/raga/dataset.py` & `raga-testing-platform-1.0.2/raga/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             if not locals().get(param):
                 raise ValueError(f"{param.capitalize().replace('_', ' ')} is required.")
         file_dir = os.path.dirname(path_to_file)
         file_name_without_ext, file_extension, file_name = self.get_file_name(path_to_file)
         zip_file_name = os.path.join(file_dir, file_name_without_ext + ".zip")
         with zipfile.ZipFile(zip_file_name, "w") as zip_file:
             zip_file.write(path_to_file, file_name)
-        pre_signed_url = self.get_pre_signed_s3_url(zip_file_name)
+        pre_signed_url = self.get_pre_signed_s3_url(file_name_without_ext + ".zip")
         self.upload_file(
             pre_signed_url,
             zip_file_name,
             success_callback=self.on_upload_success,
             failure_callback=self.on_upload_failed,
         )
         if os.path.exists(zip_file_name):
```

### Comparing `raga-testing-platform-1.0.1/raga/examples/example.py` & `raga-testing-platform-1.0.2/raga/examples/example.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.1/raga/test_session.py` & `raga-testing-platform-1.0.2/raga/test_session.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.1/raga/utils/http_client.py` & `raga-testing-platform-1.0.2/raga/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.1/raga/utils/raga_config_reader.py` & `raga-testing-platform-1.0.2/raga/utils/raga_config_reader.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.1/raga/validators/dataset_creds_validations.py` & `raga-testing-platform-1.0.2/raga/validators/dataset_creds_validations.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.1/raga/validators/dataset_validations.py` & `raga-testing-platform-1.0.2/raga/validators/dataset_validations.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.1/raga/validators/test_session_validation.py` & `raga-testing-platform-1.0.2/raga/validators/test_session_validation.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.1/raga_testing_platform.egg-info/PKG-INFO` & `raga-testing-platform-1.0.2/raga_testing_platform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-testing-platform
-Version: 1.0.1
+Version: 1.0.2
 Summary: Short description or overview of the raga package.
 Author-email: Raga AI <support@ragaai.com>
 Project-URL: Homepage, https://github.com/whoosh-labs/testing-platform-python-client
 Project-URL: Bug Tracker, https://github.com/whoosh-labs/testing-platform-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `raga-testing-platform-1.0.1/raga_testing_platform.egg-info/SOURCES.txt` & `raga-testing-platform-1.0.2/raga_testing_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

