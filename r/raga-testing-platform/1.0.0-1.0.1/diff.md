# Comparing `tmp/raga-testing-platform-1.0.0.tar.gz` & `tmp/raga-testing-platform-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-testing-platform-1.0.0.tar", last modified: Wed Jun 14 05:10:31 2023, max compression
+gzip compressed data, was "raga-testing-platform-1.0.1.tar", last modified: Wed Jun 14 05:20:03 2023, max compression
```

## Comparing `raga-testing-platform-1.0.0.tar` & `raga-testing-platform-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,31 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:10:31.811833 raga-testing-platform-1.0.0/
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-06-12 07:11:03.000000 raga-testing-platform-1.0.0/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      621 2023-06-14 05:10:31.811645 raga-testing-platform-1.0.0/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      289 2023-06-12 07:17:11.000000 raga-testing-platform-1.0.0/README.md
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:10:31.809867 raga-testing-platform-1.0.0/raga/
--rw-r--r--   0 manabroy   (501) staff       (20)      977 2023-06-13 11:01:16.000000 raga-testing-platform-1.0.0/raga/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1243 2023-06-13 13:01:16.000000 raga-testing-platform-1.0.0/raga/auth.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9070 2023-06-13 13:27:02.000000 raga-testing-platform-1.0.0/raga/dataset.py
--rw-r--r--   0 manabroy   (501) staff       (20)      498 2023-06-12 11:57:49.000000 raga-testing-platform-1.0.0/raga/dataset_creds.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1399 2023-06-13 13:05:33.000000 raga-testing-platform-1.0.0/raga/test_session.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:10:31.810270 raga-testing-platform-1.0.0/raga/tests/
--rw-r--r--   0 manabroy   (501) staff       (20)       51 2023-06-12 07:15:00.000000 raga-testing-platform-1.0.0/raga/tests/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)       59 2023-06-12 07:51:37.000000 raga-testing-platform-1.0.0/raga/tests.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:10:31.811374 raga-testing-platform-1.0.0/raga_testing_platform.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      621 2023-06-14 05:10:31.000000 raga-testing-platform-1.0.0/raga_testing_platform.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      376 2023-06-14 05:10:31.000000 raga-testing-platform-1.0.0/raga_testing_platform.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-06-14 05:10:31.000000 raga-testing-platform-1.0.0/raga_testing_platform.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       32 2023-06-14 05:10:31.000000 raga-testing-platform-1.0.0/raga_testing_platform.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        5 2023-06-14 05:10:31.000000 raga-testing-platform-1.0.0/raga_testing_platform.egg-info/top_level.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-06-14 05:10:31.811889 raga-testing-platform-1.0.0/setup.cfg
--rw-r--r--   0 manabroy   (501) staff       (20)      831 2023-06-14 05:10:11.000000 raga-testing-platform-1.0.0/setup.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.542548 raga-testing-platform-1.0.1/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1073 2023-06-14 05:19:34.000000 raga-testing-platform-1.0.1/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      869 2023-06-14 05:20:03.542344 raga-testing-platform-1.0.1/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      289 2023-06-12 07:17:11.000000 raga-testing-platform-1.0.1/README.md
+-rw-r--r--   0 manabroy   (501) staff       (20)      565 2023-06-14 05:19:15.000000 raga-testing-platform-1.0.1/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.538511 raga-testing-platform-1.0.1/raga/
+-rw-r--r--   0 manabroy   (501) staff       (20)      977 2023-06-13 11:01:16.000000 raga-testing-platform-1.0.1/raga/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1243 2023-06-13 13:01:16.000000 raga-testing-platform-1.0.1/raga/auth.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9070 2023-06-13 13:27:02.000000 raga-testing-platform-1.0.1/raga/dataset.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      498 2023-06-12 11:57:49.000000 raga-testing-platform-1.0.1/raga/dataset_creds.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.538829 raga-testing-platform-1.0.1/raga/docs/
+-rw-r--r--   0 manabroy   (501) staff       (20)       82 2023-06-12 07:15:42.000000 raga-testing-platform-1.0.1/raga/docs/conf.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.539148 raga-testing-platform-1.0.1/raga/examples/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1588 2023-06-13 13:07:53.000000 raga-testing-platform-1.0.1/raga/examples/example.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1399 2023-06-13 13:05:33.000000 raga-testing-platform-1.0.1/raga/test_session.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.539445 raga-testing-platform-1.0.1/raga/tests/
+-rw-r--r--   0 manabroy   (501) staff       (20)       51 2023-06-12 07:15:00.000000 raga-testing-platform-1.0.1/raga/tests/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       59 2023-06-12 07:51:37.000000 raga-testing-platform-1.0.1/raga/tests.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.540252 raga-testing-platform-1.0.1/raga/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3601 2023-06-13 13:06:36.000000 raga-testing-platform-1.0.1/raga/utils/http_client.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      929 2023-06-12 12:28:35.000000 raga-testing-platform-1.0.1/raga/utils/raga_config_reader.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.541185 raga-testing-platform-1.0.1/raga/validators/
+-rw-r--r--   0 manabroy   (501) staff       (20)      860 2023-06-12 10:10:59.000000 raga-testing-platform-1.0.1/raga/validators/dataset_creds_validations.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1611 2023-06-13 10:18:53.000000 raga-testing-platform-1.0.1/raga/validators/dataset_validations.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      715 2023-06-13 09:15:46.000000 raga-testing-platform-1.0.1/raga/validators/test_session_validation.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 05:20:03.542075 raga-testing-platform-1.0.1/raga_testing_platform.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      869 2023-06-14 05:20:03.000000 raga-testing-platform-1.0.1/raga_testing_platform.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      567 2023-06-14 05:20:03.000000 raga-testing-platform-1.0.1/raga_testing_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-06-14 05:20:03.000000 raga-testing-platform-1.0.1/raga_testing_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        5 2023-06-14 05:20:03.000000 raga-testing-platform-1.0.1/raga_testing_platform.egg-info/top_level.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-06-14 05:20:03.542604 raga-testing-platform-1.0.1/setup.cfg
```

### Comparing `raga-testing-platform-1.0.0/raga/__init__.py` & `raga-testing-platform-1.0.1/raga/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.0/raga/auth.py` & `raga-testing-platform-1.0.1/raga/auth.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.0/raga/dataset.py` & `raga-testing-platform-1.0.1/raga/dataset.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.0/raga/test_session.py` & `raga-testing-platform-1.0.1/raga/test_session.py`

 * *Files identical despite different names*

