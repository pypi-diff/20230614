# Comparing `tmp/raga-testing-platform-1.0.3.tar.gz` & `tmp/raga-testing-platform-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-testing-platform-1.0.3.tar", last modified: Wed Jun 14 10:07:59 2023, max compression
+gzip compressed data, was "raga-testing-platform-1.0.4.tar", last modified: Wed Jun 14 10:23:10 2023, max compression
```

## Comparing `raga-testing-platform-1.0.3.tar` & `raga-testing-platform-1.0.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.234393 raga-testing-platform-1.0.3/
--rw-r--r--   0 manabroy   (501) staff       (20)     6148 2023-06-14 09:48:34.000000 raga-testing-platform-1.0.3/.DS_Store
--rw-r--r--   0 manabroy   (501) staff       (20)     3095 2023-06-13 13:44:54.000000 raga-testing-platform-1.0.3/.gitignore
--rw-r--r--   0 manabroy   (501) staff       (20)     1073 2023-06-14 05:19:34.000000 raga-testing-platform-1.0.3/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      990 2023-06-14 10:07:59.234143 raga-testing-platform-1.0.3/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      289 2023-06-12 07:17:11.000000 raga-testing-platform-1.0.3/README.md
--rw-r--r--   0 manabroy   (501) staff       (20)     1005 2023-06-14 10:07:43.000000 raga-testing-platform-1.0.3/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.225841 raga-testing-platform-1.0.3/raga/
--rw-r--r--   0 manabroy   (501) staff       (20)     8196 2023-06-14 09:48:39.000000 raga-testing-platform-1.0.3/raga/.DS_Store
--rw-r--r--   0 manabroy   (501) staff       (20)      977 2023-06-13 11:01:16.000000 raga-testing-platform-1.0.3/raga/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1243 2023-06-13 13:01:16.000000 raga-testing-platform-1.0.3/raga/auth.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9087 2023-06-14 09:51:10.000000 raga-testing-platform-1.0.3/raga/dataset.py
--rw-r--r--   0 manabroy   (501) staff       (20)      498 2023-06-12 11:57:49.000000 raga-testing-platform-1.0.3/raga/dataset_creds.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.226843 raga-testing-platform-1.0.3/raga/docs/
--rw-r--r--   0 manabroy   (501) staff       (20)       82 2023-06-12 07:15:42.000000 raga-testing-platform-1.0.3/raga/docs/conf.py
--rw-r--r--   0 manabroy   (501) staff       (20)      160 2023-06-12 09:52:28.000000 raga-testing-platform-1.0.3/raga/docs/index.rst
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.227875 raga-testing-platform-1.0.3/raga/examples/
--rw-r--r--   0 manabroy   (501) staff       (20)      151 2023-06-13 11:37:36.000000 raga-testing-platform-1.0.3/raga/examples/.raga
--rw-r--r--   0 manabroy   (501) staff       (20)     1780 2023-06-12 13:42:21.000000 raga-testing-platform-1.0.3/raga/examples/coco.json
--rw-r--r--   0 manabroy   (501) staff       (20)     1588 2023-06-13 13:07:53.000000 raga-testing-platform-1.0.3/raga/examples/example.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1399 2023-06-13 13:05:33.000000 raga-testing-platform-1.0.3/raga/test_session.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.228829 raga-testing-platform-1.0.3/raga/tests/
--rw-r--r--   0 manabroy   (501) staff       (20)       51 2023-06-12 07:15:00.000000 raga-testing-platform-1.0.3/raga/tests/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)       59 2023-06-12 07:51:37.000000 raga-testing-platform-1.0.3/raga/tests.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.230189 raga-testing-platform-1.0.3/raga/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     3601 2023-06-13 13:06:36.000000 raga-testing-platform-1.0.3/raga/utils/http_client.py
--rw-r--r--   0 manabroy   (501) staff       (20)      929 2023-06-12 12:28:35.000000 raga-testing-platform-1.0.3/raga/utils/raga_config_reader.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.231284 raga-testing-platform-1.0.3/raga/validators/
--rw-r--r--   0 manabroy   (501) staff       (20)      860 2023-06-12 10:10:59.000000 raga-testing-platform-1.0.3/raga/validators/dataset_creds_validations.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1611 2023-06-13 10:18:53.000000 raga-testing-platform-1.0.3/raga/validators/dataset_validations.py
--rw-r--r--   0 manabroy   (501) staff       (20)      715 2023-06-13 09:15:46.000000 raga-testing-platform-1.0.3/raga/validators/test_session_validation.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:07:59.233748 raga-testing-platform-1.0.3/raga_testing_platform.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      990 2023-06-14 10:07:59.000000 raga-testing-platform-1.0.3/raga_testing_platform.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      711 2023-06-14 10:07:59.000000 raga-testing-platform-1.0.3/raga_testing_platform.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-06-14 10:07:59.000000 raga-testing-platform-1.0.3/raga_testing_platform.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       61 2023-06-14 10:07:59.000000 raga-testing-platform-1.0.3/raga_testing_platform.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        5 2023-06-14 10:07:59.000000 raga-testing-platform-1.0.3/raga_testing_platform.egg-info/top_level.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-06-14 10:07:59.234444 raga-testing-platform-1.0.3/setup.cfg
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:23:10.829720 raga-testing-platform-1.0.4/
+-rw-r--r--   0 manabroy   (501) staff       (20)     6148 2023-06-14 10:14:55.000000 raga-testing-platform-1.0.4/.DS_Store
+-rw-r--r--   0 manabroy   (501) staff       (20)     3095 2023-06-13 13:44:54.000000 raga-testing-platform-1.0.4/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)     1073 2023-06-14 05:19:34.000000 raga-testing-platform-1.0.4/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      990 2023-06-14 10:23:10.829545 raga-testing-platform-1.0.4/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      289 2023-06-12 07:17:11.000000 raga-testing-platform-1.0.4/README.md
+-rw-r--r--   0 manabroy   (501) staff       (20)     1005 2023-06-14 10:23:01.000000 raga-testing-platform-1.0.4/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:23:10.825024 raga-testing-platform-1.0.4/raga/
+-rw-r--r--   0 manabroy   (501) staff       (20)     8196 2023-06-14 10:14:38.000000 raga-testing-platform-1.0.4/raga/.DS_Store
+-rw-r--r--   0 manabroy   (501) staff       (20)      998 2023-06-14 10:11:52.000000 raga-testing-platform-1.0.4/raga/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1236 2023-06-14 10:12:53.000000 raga-testing-platform-1.0.4/raga/auth.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9080 2023-06-14 10:13:07.000000 raga-testing-platform-1.0.4/raga/dataset.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      498 2023-06-12 11:57:49.000000 raga-testing-platform-1.0.4/raga/dataset_creds.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:23:10.825659 raga-testing-platform-1.0.4/raga/docs/
+-rw-r--r--   0 manabroy   (501) staff       (20)       82 2023-06-12 07:15:42.000000 raga-testing-platform-1.0.4/raga/docs/conf.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      160 2023-06-12 09:52:28.000000 raga-testing-platform-1.0.4/raga/docs/index.rst
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:23:10.826638 raga-testing-platform-1.0.4/raga/examples/
+-rw-r--r--   0 manabroy   (501) staff       (20)      151 2023-06-13 11:37:36.000000 raga-testing-platform-1.0.4/raga/examples/.raga
+-rw-r--r--   0 manabroy   (501) staff       (20)     1780 2023-06-12 13:42:21.000000 raga-testing-platform-1.0.4/raga/examples/coco.json
+-rw-r--r--   0 manabroy   (501) staff       (20)     1588 2023-06-14 10:20:07.000000 raga-testing-platform-1.0.4/raga/examples/example.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1392 2023-06-14 10:13:12.000000 raga-testing-platform-1.0.4/raga/test_session.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:23:10.826767 raga-testing-platform-1.0.4/raga/tests/
+-rw-r--r--   0 manabroy   (501) staff       (20)       51 2023-06-12 07:15:00.000000 raga-testing-platform-1.0.4/raga/tests/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       59 2023-06-12 07:51:37.000000 raga-testing-platform-1.0.4/raga/tests.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:23:10.827452 raga-testing-platform-1.0.4/raga/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3601 2023-06-13 13:06:36.000000 raga-testing-platform-1.0.4/raga/utils/http_client.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1011 2023-06-14 10:12:33.000000 raga-testing-platform-1.0.4/raga/utils/raga_config_reader.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:23:10.828245 raga-testing-platform-1.0.4/raga/validators/
+-rw-r--r--   0 manabroy   (501) staff       (20)      860 2023-06-12 10:10:59.000000 raga-testing-platform-1.0.4/raga/validators/dataset_creds_validations.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1611 2023-06-13 10:18:53.000000 raga-testing-platform-1.0.4/raga/validators/dataset_validations.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      715 2023-06-13 09:15:46.000000 raga-testing-platform-1.0.4/raga/validators/test_session_validation.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-14 10:23:10.829295 raga-testing-platform-1.0.4/raga_testing_platform.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      990 2023-06-14 10:23:10.000000 raga-testing-platform-1.0.4/raga_testing_platform.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      711 2023-06-14 10:23:10.000000 raga-testing-platform-1.0.4/raga_testing_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-06-14 10:23:10.000000 raga-testing-platform-1.0.4/raga_testing_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       61 2023-06-14 10:23:10.000000 raga-testing-platform-1.0.4/raga_testing_platform.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        5 2023-06-14 10:23:10.000000 raga-testing-platform-1.0.4/raga_testing_platform.egg-info/top_level.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-06-14 10:23:10.829764 raga-testing-platform-1.0.4/setup.cfg
```

### Comparing `raga-testing-platform-1.0.3/.DS_Store` & `raga-testing-platform-1.0.4/.DS_Store`

 * *Files 10% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 000004e0: 6c69 7374 3030 d601 0203 0405 0607 0709  list00..........
 000004f0: 070b 075d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
 00000500: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
 00000510: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
 00000520: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
 00000530: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
 00000540: 6f77 5369 6465 6261 7209 0908 095f 1018  owSidebar...._..
-00000550: 7b7b 3236 302c 2036 327d 2c20 7b31 3034  {{260, 62}, {104
+00000550: 7b7b 3238 392c 2036 327d 2c20 7b31 3034  {{289, 62}, {104
 00000560: 382c 2038 3133 7d7d 0908 1523 2f3b 525f  8, 813}}...#/;R_
 00000570: 6b6c 6d6e 6f8a 0000 0000 0000 0101 0000  klmno...........
 00000580: 0000 0000 000d 0000 0000 0000 0000 0000  ................
 00000590: 0000 0000 008b 0000 0004 0072 0061 0067  ...........r.a.g
 000005a0: 0061 7653 726e 6c6f 6e67 0000 0001 0000  .avSrnlong......
 000005b0: 001e 0072 0061 0067 0061 005f 0074 0065  ...r.a.g.a._.t.e
 000005c0: 0073 0074 0069 006e 0067 005f 0070 006c  .s.t.i.n.g._.p.l
```

### Comparing `raga-testing-platform-1.0.3/.gitignore` & `raga-testing-platform-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.3/LICENSE` & `raga-testing-platform-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.3/PKG-INFO` & `raga-testing-platform-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-testing-platform
-Version: 1.0.3
+Version: 1.0.4
 Summary: Short description or overview of the raga package.
 Author-email: Raga AI <support@ragaai.com>
 Maintainer-email: Raga AI <support@ragaai.com>
 Project-URL: Homepage, https://github.com/whoosh-labs/testing-platform-python-client
 Project-URL: Bug Tracker, https://github.com/whoosh-labs/testing-platform-python-client/issues
 Keywords: testing-platform,raga-testing-platform,model-testing,AB_testing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `raga-testing-platform-1.0.3/pyproject.toml` & `raga-testing-platform-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-testing-platform"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Raga AI", email="support@ragaai.com" },
 ]
 maintainers = [{ name = "Raga AI", email = "support@ragaai.com" }]
 dependencies = [
     "pandas==2.0.2",
     "urllib3==1.26.7",
```

### Comparing `raga-testing-platform-1.0.3/raga/.DS_Store` & `raga-testing-platform-1.0.4/raga/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -293,15 +293,15 @@
 00001240: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
 00001250: 0405 0607 0709 070b 075d 5368 6f77 5374  .........]ShowSt
 00001260: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
 00001270: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00001280: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00001290: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 000012a0: 6e64 735b 5368 6f77 5369 6465 6261 7209  nds[ShowSidebar.
-000012b0: 0908 095f 1018 7b7b 3236 302c 2036 327d  ..._..{{260, 62}
+000012b0: 0908 095f 1018 7b7b 3238 392c 2036 327d  ..._..{{289, 62}
 000012c0: 2c20 7b31 3034 382c 2038 3133 7d7d 0908  , {1048, 813}}..
 000012d0: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
 000012e0: 0000 0101 0000 0000 0000 000d 0000 0000  ................
 000012f0: 0000 0000 0000 0000 0000 008b 0000 0008  ................
 00001300: 0065 0078 0061 006d 0070 006c 0065 0073  .e.x.a.m.p.l.e.s
 00001310: 7653 726e 6c6f 6e67 0000 0001 0000 000f  vSrnlong........
 00001320: 0074 0065 0073 0074 005f 0073 0065 0073  .t.e.s.t._.s.e.s
```

### Comparing `raga-testing-platform-1.0.3/raga/__init__.py` & `raga-testing-platform-1.0.4/raga/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Initialization file for the testing_platform package."""
 import os
 import logging
 
+RAGA_FILE = ".raga"
+
 # Get the value of the DEBUG environment variable
 debug_mode = os.environ.get('DEBUG')
 
 # Configure the logging format and level based on the DEBUG environment variable
 if debug_mode:
     logging.basicConfig(
         format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
```

### Comparing `raga-testing-platform-1.0.3/raga/auth.py` & `raga-testing-platform-1.0.4/raga/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from raga.validators.test_session_validation import TestSessionValidator
 from raga.utils.http_client import HTTPClient
 from raga.utils.raga_config_reader import read_raga_config, get_config_value
 
-config_data = read_raga_config(".raga")
+config_data = read_raga_config()
 
 class Auth:
     def __init__(self):
         self.http_client = HTTPClient(get_config_value(config_data, 'default', 'api_host'))
         self.raga_access_key_id = get_config_value(config_data, 'default', 'raga_access_key_id')
         self.raga_secret_access_key = get_config_value(config_data, 'default', 'raga_secret_access_key')
         self.token = self.create_token()
```

### Comparing `raga-testing-platform-1.0.3/raga/dataset.py` & `raga-testing-platform-1.0.4/raga/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from raga.utils.http_client import HTTPClient
 from raga.dataset_creds import DatasetCreds
 from raga.utils.raga_config_reader import read_raga_config, get_config_value
 import logging
 import zipfile
 
 logger = logging.getLogger(__name__)
-config_data = read_raga_config(".raga")
+config_data = read_raga_config()
 
 
 class FileUploadError(Exception):
     pass
 
 
 class Dataset:
```

### Comparing `raga-testing-platform-1.0.3/raga/examples/coco.json` & `raga-testing-platform-1.0.4/raga/examples/coco.json`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.3/raga/examples/example.py` & `raga-testing-platform-1.0.4/raga/examples/example.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # Create an instance of the Schema class
 schema = Schema()
 
 # Create an instance of the Auth class
 auth = Auth()
 
 # Create an instance of the TestSession class
-test_experiment = TestSession(auth.token, 1, "test_experiment1")
+test_experiment = TestSession(auth.token, 1, "test_experiment7")
 
 # Create an instance of the Dataset class
 test_ds = Dataset(auth.token, test_experiment.experiment_id, test_df, schema, "TestDB")
 
 # Load labels from a file
 test_ds.load_labels_from_file(
     "/Users/manabroy/localhost/observance/raga/testing_platform/testing-platform-python-client/raga/examples/coco.json",
```

### Comparing `raga-testing-platform-1.0.3/raga/test_session.py` & `raga-testing-platform-1.0.4/raga/test_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from raga.validators.test_session_validation import TestSessionValidator
 from raga.utils.http_client import HTTPClient
 from raga.utils.raga_config_reader import read_raga_config, get_config_value
 
-config_data = read_raga_config(".raga")
+config_data = read_raga_config()
 
 class TestSession:
     def __init__(self, token: str, project_id: str, run_name: str):
         self.token = TestSessionValidator.validate_token(token)
         self.project_id = TestSessionValidator.validate_project_id(project_id)
         self.run_name = TestSessionValidator.validate_run_name(run_name)
         self.http_client = HTTPClient(get_config_value(config_data, 'default', 'api_host'))
```

### Comparing `raga-testing-platform-1.0.3/raga/utils/http_client.py` & `raga-testing-platform-1.0.4/raga/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.3/raga/utils/raga_config_reader.py` & `raga-testing-platform-1.0.4/raga/utils/raga_config_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import configparser
 import os
+from raga import RAGA_FILE
 
-def read_raga_config(config_file_path):
+def read_raga_config():
+    config_file_path = os.path.expanduser(os.path.join("~", RAGA_FILE))
     if not os.path.isfile(config_file_path):
         raise FileNotFoundError(f"Config file '{config_file_path}' not found.")
 
     config = configparser.ConfigParser()
     try:
         config.read(config_file_path)
     except configparser.Error as e:
@@ -22,8 +24,7 @@
         section_data = config_data[section]
         if option in section_data:
             return section_data[option]
         else:
             raise KeyError(f"Option '{option}' not found in section '{section}'.")
     else:
         raise KeyError(f"Section '{section}' not found in config data.")
-
```

### Comparing `raga-testing-platform-1.0.3/raga/validators/dataset_creds_validations.py` & `raga-testing-platform-1.0.4/raga/validators/dataset_creds_validations.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.3/raga/validators/dataset_validations.py` & `raga-testing-platform-1.0.4/raga/validators/dataset_validations.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.3/raga/validators/test_session_validation.py` & `raga-testing-platform-1.0.4/raga/validators/test_session_validation.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.3/raga_testing_platform.egg-info/PKG-INFO` & `raga-testing-platform-1.0.4/raga_testing_platform.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-testing-platform
-Version: 1.0.3
+Version: 1.0.4
 Summary: Short description or overview of the raga package.
 Author-email: Raga AI <support@ragaai.com>
 Maintainer-email: Raga AI <support@ragaai.com>
 Project-URL: Homepage, https://github.com/whoosh-labs/testing-platform-python-client
 Project-URL: Bug Tracker, https://github.com/whoosh-labs/testing-platform-python-client/issues
 Keywords: testing-platform,raga-testing-platform,model-testing,AB_testing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `raga-testing-platform-1.0.3/raga_testing_platform.egg-info/SOURCES.txt` & `raga-testing-platform-1.0.4/raga_testing_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

