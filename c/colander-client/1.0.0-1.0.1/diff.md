# Comparing `tmp/colander-client-1.0.0.tar.gz` & `tmp/colander-client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colander-client-1.0.0.tar", last modified: Wed May 10 17:33:48 2023, max compression
+gzip compressed data, was "colander-client-1.0.1.tar", last modified: Wed Jun 14 07:30:25 2023, max compression
```

## Comparing `colander-client-1.0.0.tar` & `colander-client-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:33:48.181079 colander-client-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 17:33:34.000000 colander-client-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-05-10 17:33:48.181079 colander-client-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-05-10 17:33:34.000000 colander-client-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:33:48.177079 colander-client-1.0.0/colander_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 17:33:34.000000 colander-client-1.0.0/colander_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9191 2023-05-10 17:33:34.000000 colander-client-1.0.0/colander_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:33:48.177079 colander-client-1.0.0/colander_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-05-10 17:33:47.000000 colander-client-1.0.0/colander_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-10 17:33:48.000000 colander-client-1.0.0/colander_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 17:33:47.000000 colander-client-1.0.0/colander_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 17:33:47.000000 colander-client-1.0.0/colander_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 17:33:47.000000 colander-client-1.0.0/colander_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 17:33:48.181079 colander-client-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-10 17:33:34.000000 colander-client-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:30:25.192037 colander-client-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 07:30:13.000000 colander-client-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-14 07:30:25.192037 colander-client-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-14 07:30:13.000000 colander-client-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:30:25.192037 colander-client-1.0.1/colander_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 07:30:13.000000 colander-client-1.0.1/colander_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-06-14 07:30:13.000000 colander-client-1.0.1/colander_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:30:25.192037 colander-client-1.0.1/colander_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-14 07:30:25.000000 colander-client-1.0.1/colander_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-14 07:30:25.000000 colander-client-1.0.1/colander_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:30:25.000000 colander-client-1.0.1/colander_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 07:30:25.000000 colander-client-1.0.1/colander_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 07:30:25.000000 colander-client-1.0.1/colander_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 07:30:25.192037 colander-client-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-14 07:30:13.000000 colander-client-1.0.1/setup.py
```

### Comparing `colander-client-1.0.0/LICENSE.txt` & `colander-client-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `colander-client-1.0.0/PKG-INFO` & `colander-client-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colander-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: Colander REST API Python client
 Home-page: https://github.com/PiRogueToolSuite/colander-python-client.git
 Author: U+039b
 Author-email: esther@pts-project.org
 License: UNKNOWN
 Description: # Colander Python 3 client
```

### Comparing `colander-client-1.0.0/README.md` & `colander-client-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `colander-client-1.0.0/colander_client/client.py` & `colander-client-1.0.1/colander_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,17 +172,22 @@
                             'addr': addr
                         },
                         encoding="multipart/form-data"
                     )
 
                     addr += len(buf)
 
-        if not last_response['eof'] or not last_response['status'] == 'SUCCEEDED':
-            progress_callback(filepath, 100, 'failed')
-            raise Exception("Upload failed somehow")
+        if last_response is None:
+            if size > 0:
+                progress_callback(filepath, 100, 'failed')
+                raise Exception("Upload failed with no response but stuff to do")
+        else:
+            if not last_response['eof'] or not last_response['status'] == 'SUCCEEDED':
+                progress_callback(filepath, 100, 'failed')
+                raise Exception("Upload failed somehow")
 
         progress_callback(filepath, 100, 'complete')
 
         new_artifact = self._action(
             ['artifacts', 'create'],
             params={
                 **{
```

### Comparing `colander-client-1.0.0/colander_client.egg-info/PKG-INFO` & `colander-client-1.0.1/colander_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colander-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: Colander REST API Python client
 Home-page: https://github.com/PiRogueToolSuite/colander-python-client.git
 Author: U+039b
 Author-email: esther@pts-project.org
 License: UNKNOWN
 Description: # Colander Python 3 client
```

### Comparing `colander-client-1.0.0/setup.py` & `colander-client-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 install_requires = [
     'coreapi',
 ]
 
 setup(
     name='colander-client',
-    version='1.0.0',
+    version='1.0.1',
     description='Colander REST API Python client',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='U+039b',
     author_email='esther@pts-project.org',
     url='https://github.com/PiRogueToolSuite/colander-python-client.git',
     packages=find_packages(exclude=['*.tests', '*.tests.*', 'test*', 'tests']),
```

