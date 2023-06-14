# Comparing `tmp/bs_admin_utils-1.0.4.tar.gz` & `tmp/bs_admin_utils-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_admin_utils-1.0.4.tar", last modified: Mon May 29 06:45:30 2023, max compression
+gzip compressed data, was "bs_admin_utils-1.0.5.tar", last modified: Wed Jun 14 10:42:57 2023, max compression
```

## Comparing `bs_admin_utils-1.0.4.tar` & `bs_admin_utils-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-05-29 06:45:30.391330 bs_admin_utils-1.0.4/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1067 2023-04-07 03:25:03.000000 bs_admin_utils-1.0.4/LICENSE
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       35 2023-04-07 04:04:08.000000 bs_admin_utils-1.0.4/MANIFEST.in
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-05-29 06:45:30.391330 bs_admin_utils-1.0.4/PKG-INFO
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      206 2023-04-07 03:35:29.000000 bs_admin_utils-1.0.4/README.md
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-05-29 06:45:30.391330 bs_admin_utils-1.0.4/bs_admin_utils/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       13 2023-04-07 03:39:05.000000 bs_admin_utils-1.0.4/bs_admin_utils/__init__.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     4216 2023-05-29 06:42:03.000000 bs_admin_utils-1.0.4/bs_admin_utils/api.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      490 2023-04-07 04:11:32.000000 bs_admin_utils-1.0.4/bs_admin_utils/decorators.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1034 2023-04-07 03:48:50.000000 bs_admin_utils-1.0.4/bs_admin_utils/model.py
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-05-29 06:45:30.391330 bs_admin_utils-1.0.4/bs_admin_utils/static/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)   367112 2023-04-07 03:52:07.000000 bs_admin_utils-1.0.4/bs_admin_utils/static/arial.ttf
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2320 2023-04-07 04:36:50.000000 bs_admin_utils-1.0.4/bs_admin_utils/vercode.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2868 2023-04-07 04:10:45.000000 bs_admin_utils-1.0.4/bs_admin_utils/websocket.py
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-05-29 06:45:30.391330 bs_admin_utils-1.0.4/bs_admin_utils.egg-info/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-05-29 06:45:30.000000 bs_admin_utils-1.0.4/bs_admin_utils.egg-info/PKG-INFO
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      448 2023-05-29 06:45:30.000000 bs_admin_utils-1.0.4/bs_admin_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-05-29 06:45:30.000000 bs_admin_utils-1.0.4/bs_admin_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       44 2023-05-29 06:45:30.000000 bs_admin_utils-1.0.4/bs_admin_utils.egg-info/requires.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       15 2023-05-29 06:45:30.000000 bs_admin_utils-1.0.4/bs_admin_utils.egg-info/top_level.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-05-29 06:45:30.000000 bs_admin_utils-1.0.4/bs_admin_utils.egg-info/zip-safe
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-05-29 06:45:30.391330 bs_admin_utils-1.0.4/setup.cfg
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      620 2023-05-29 06:42:17.000000 bs_admin_utils-1.0.4/setup.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-14 10:42:57.431320 bs_admin_utils-1.0.5/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1067 2023-04-07 03:25:03.000000 bs_admin_utils-1.0.5/LICENSE
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       35 2023-04-07 04:04:08.000000 bs_admin_utils-1.0.5/MANIFEST.in
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-06-14 10:42:57.431320 bs_admin_utils-1.0.5/PKG-INFO
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      206 2023-04-07 03:35:29.000000 bs_admin_utils-1.0.5/README.md
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-14 10:42:57.427320 bs_admin_utils-1.0.5/bs_admin_utils/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       13 2023-04-07 03:39:05.000000 bs_admin_utils-1.0.5/bs_admin_utils/__init__.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     4220 2023-06-14 10:41:27.000000 bs_admin_utils-1.0.5/bs_admin_utils/api.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      490 2023-04-07 04:11:32.000000 bs_admin_utils-1.0.5/bs_admin_utils/decorators.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1034 2023-04-07 03:48:50.000000 bs_admin_utils-1.0.5/bs_admin_utils/model.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-14 10:42:57.427320 bs_admin_utils-1.0.5/bs_admin_utils/static/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)   367112 2023-04-07 03:52:07.000000 bs_admin_utils-1.0.5/bs_admin_utils/static/arial.ttf
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2320 2023-04-07 04:36:50.000000 bs_admin_utils-1.0.5/bs_admin_utils/vercode.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2868 2023-04-07 04:10:45.000000 bs_admin_utils-1.0.5/bs_admin_utils/websocket.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-14 10:42:57.427320 bs_admin_utils-1.0.5/bs_admin_utils.egg-info/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-06-14 10:42:57.000000 bs_admin_utils-1.0.5/bs_admin_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      448 2023-06-14 10:42:57.000000 bs_admin_utils-1.0.5/bs_admin_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-06-14 10:42:57.000000 bs_admin_utils-1.0.5/bs_admin_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       44 2023-06-14 10:42:57.000000 bs_admin_utils-1.0.5/bs_admin_utils.egg-info/requires.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       15 2023-06-14 10:42:57.000000 bs_admin_utils-1.0.5/bs_admin_utils.egg-info/top_level.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-06-14 10:42:57.000000 bs_admin_utils-1.0.5/bs_admin_utils.egg-info/zip-safe
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-06-14 10:42:57.431320 bs_admin_utils-1.0.5/setup.cfg
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      620 2023-06-14 10:42:20.000000 bs_admin_utils-1.0.5/setup.py
```

### Comparing `bs_admin_utils-1.0.4/LICENSE` & `bs_admin_utils-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.0.4/bs_admin_utils/api.py` & `bs_admin_utils-1.0.5/bs_admin_utils/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     # Apis
 
     async def delete(self, id: str):
         if model := await self.model.from_id(id):
             await model.delete()
             return self.success
-        return self.error()
+        return self.not_found()
 
     async def get_list(self, rq: Request, fetch_links: bool = True, with_children: bool = True):
         skip, limit = get_data_range(rq)
         models = self.model.find(
             fetch_links=fetch_links,
             limit=limit,
             skip=skip,
```

### Comparing `bs_admin_utils-1.0.4/bs_admin_utils/model.py` & `bs_admin_utils-1.0.5/bs_admin_utils/model.py`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.0.4/bs_admin_utils/static/arial.ttf` & `bs_admin_utils-1.0.5/bs_admin_utils/static/arial.ttf`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.0.4/bs_admin_utils/vercode.py` & `bs_admin_utils-1.0.5/bs_admin_utils/vercode.py`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.0.4/bs_admin_utils/websocket.py` & `bs_admin_utils-1.0.5/bs_admin_utils/websocket.py`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.0.4/setup.py` & `bs_admin_utils-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ],
     packages=find_packages(),
     package_data={
         'bs_admin_utils': ['*.ttf']
     },
     include_package_data=True,
     zip_safe=True,
-    version='1.0.4',
+    version='1.0.5',
     description='Blacksheep admin backend utils classes and function.',
     author='kiki-kanri',
     author_email='a470666@gmail.com',
     keywords=[],
     install_requires=[
         'beanie',
         'blacksheep',
```

