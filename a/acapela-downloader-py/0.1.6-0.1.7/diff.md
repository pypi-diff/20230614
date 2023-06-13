# Comparing `tmp/acapela_downloader_py-0.1.6.tar.gz` & `tmp/acapela_downloader_py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acapela_downloader_py-0.1.6.tar", last modified: Tue Jun 13 17:13:39 2023, max compression
+gzip compressed data, was "acapela_downloader_py-0.1.7.tar", last modified: Tue Jun 13 23:23:28 2023, max compression
```

## Comparing `acapela_downloader_py-0.1.6.tar` & `acapela_downloader_py-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:13:39.711011 acapela_downloader_py-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 17:13:17.000000 acapela_downloader_py-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 17:13:39.711011 acapela_downloader_py-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 17:13:17.000000 acapela_downloader_py-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 17:13:17.000000 acapela_downloader_py-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:13:39.711011 acapela_downloader_py-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:13:39.711011 acapela_downloader_py-0.1.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-13 17:13:17.000000 acapela_downloader_py-0.1.6/src/acapela.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:13:39.711011 acapela_downloader_py-0.1.6/src/acapela_downloader_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 17:13:39.000000 acapela_downloader_py-0.1.6/src/acapela_downloader_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 17:13:39.000000 acapela_downloader_py-0.1.6/src/acapela_downloader_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:13:39.000000 acapela_downloader_py-0.1.6/src/acapela_downloader_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 17:13:39.000000 acapela_downloader_py-0.1.6/src/acapela_downloader_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-13 17:13:17.000000 acapela_downloader_py-0.1.6/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:23:28.366222 acapela_downloader_py-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 23:23:18.000000 acapela_downloader_py-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 23:23:28.366222 acapela_downloader_py-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 23:23:18.000000 acapela_downloader_py-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 23:23:18.000000 acapela_downloader_py-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:23:28.366222 acapela_downloader_py-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:23:28.366222 acapela_downloader_py-0.1.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-13 23:23:18.000000 acapela_downloader_py-0.1.7/src/acapela.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:23:28.366222 acapela_downloader_py-0.1.7/src/acapela_downloader_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 23:23:28.000000 acapela_downloader_py-0.1.7/src/acapela_downloader_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 23:23:28.000000 acapela_downloader_py-0.1.7/src/acapela_downloader_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:23:28.000000 acapela_downloader_py-0.1.7/src/acapela_downloader_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 23:23:28.000000 acapela_downloader_py-0.1.7/src/acapela_downloader_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-13 23:23:18.000000 acapela_downloader_py-0.1.7/src/utils.py
```

### Comparing `acapela_downloader_py-0.1.6/LICENSE` & `acapela_downloader_py-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `acapela_downloader_py-0.1.6/PKG-INFO` & `acapela_downloader_py-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acapela_downloader_py
-Version: 0.1.6
+Version: 0.1.7
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.1.6/src/acapela_downloader_py.egg-info/PKG-INFO` & `acapela_downloader_py-0.1.7/src/acapela_downloader_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acapela-downloader-py
-Version: 0.1.6
+Version: 0.1.7
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.1.6/src/utils.py` & `acapela_downloader_py-0.1.7/src/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         fake_email = fake_email.replace(" ", "")
         nonce_response = post(NONCE_ENDPOINT, json={
             "googleid": fake_email
         })
 
         if debug_mode:
             print("DEBUG: " + fake_email)
+            print("DEBUG: " + nonce_response.json()["nonce"])
 
         if len(nonce_response.json()["nonce"]) > 1:
             cached_nonce = nonce_response.json()["nonce"]
             cached_email = fake_email
             finished = True
```

