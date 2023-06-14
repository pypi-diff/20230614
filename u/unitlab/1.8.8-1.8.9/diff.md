# Comparing `tmp/unitlab-1.8.8.tar.gz` & `tmp/unitlab-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-1.8.8.tar", last modified: Tue Jun 13 12:52:23 2023, max compression
+gzip compressed data, was "unitlab-1.8.9.tar", last modified: Wed Jun 14 10:48:11 2023, max compression
```

## Comparing `unitlab-1.8.8.tar` & `unitlab-1.8.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 12:52:23.083466 unitlab-1.8.8/
--rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.8.8/LICENSE.md
--rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.8.8/MANIFEST.in
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-06-13 12:52:23.083466 unitlab-1.8.8/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)     1431 2023-06-13 08:13:23.000000 unitlab-1.8.8/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2023-06-13 12:52:23.083466 unitlab-1.8.8/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1108 2023-06-13 11:16:56.000000 unitlab-1.8.8/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 12:52:23.083466 unitlab-1.8.8/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 12:52:23.083466 unitlab-1.8.8/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)      214 2023-05-23 13:05:07.000000 unitlab-1.8.8/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)     2112 2023-06-13 12:01:49.000000 unitlab-1.8.8/src/unitlab/cli.py
--rw-rw-r--   0 me        (1000) me        (1000)    12257 2023-06-13 12:34:06.000000 unitlab-1.8.8/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)      656 2023-06-13 10:04:19.000000 unitlab-1.8.8/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     1785 2023-06-13 12:01:36.000000 unitlab-1.8.8/src/unitlab/run.py
--rw-rw-r--   0 me        (1000) me        (1000)     2089 2023-06-13 12:43:07.000000 unitlab-1.8.8/src/unitlab/utils.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 12:52:23.083466 unitlab-1.8.8/src/unitlab.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-06-13 12:52:23.000000 unitlab-1.8.8/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      394 2023-06-13 12:52:23.000000 unitlab-1.8.8/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2023-06-13 12:52:23.000000 unitlab-1.8.8/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       44 2023-06-13 12:52:23.000000 unitlab-1.8.8/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       55 2023-06-13 12:52:23.000000 unitlab-1.8.8/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2023-06-13 12:52:23.000000 unitlab-1.8.8/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 10:48:11.913919 unitlab-1.8.9/
+-rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.8.9/LICENSE.md
+-rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.8.9/MANIFEST.in
+-rw-rw-r--   0 me        (1000) me        (1000)      685 2023-06-14 10:48:11.913919 unitlab-1.8.9/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     1431 2023-06-13 08:13:23.000000 unitlab-1.8.9/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2023-06-14 10:48:11.913919 unitlab-1.8.9/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1108 2023-06-14 10:47:45.000000 unitlab-1.8.9/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 10:48:11.909919 unitlab-1.8.9/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 10:48:11.913919 unitlab-1.8.9/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)      214 2023-05-23 13:05:07.000000 unitlab-1.8.9/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)     2112 2023-06-13 12:01:49.000000 unitlab-1.8.9/src/unitlab/cli.py
+-rw-rw-r--   0 me        (1000) me        (1000)    12257 2023-06-13 12:34:06.000000 unitlab-1.8.9/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)      656 2023-06-13 10:04:19.000000 unitlab-1.8.9/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1785 2023-06-13 12:01:36.000000 unitlab-1.8.9/src/unitlab/run.py
+-rw-rw-r--   0 me        (1000) me        (1000)     2103 2023-06-14 10:47:11.000000 unitlab-1.8.9/src/unitlab/utils.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 10:48:11.913919 unitlab-1.8.9/src/unitlab.egg-info/
+-rw-rw-r--   0 me        (1000) me        (1000)      685 2023-06-14 10:48:11.000000 unitlab-1.8.9/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      394 2023-06-14 10:48:11.000000 unitlab-1.8.9/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2023-06-14 10:48:11.000000 unitlab-1.8.9/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       45 2023-06-14 10:48:11.000000 unitlab-1.8.9/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       55 2023-06-14 10:48:11.000000 unitlab-1.8.9/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2023-06-14 10:48:11.000000 unitlab-1.8.9/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-1.8.8/LICENSE.md` & `unitlab-1.8.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.8/README.md` & `unitlab-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.8/setup.py` & `unitlab-1.8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="1.8.8",
+    version="1.8.9",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
```

### Comparing `unitlab-1.8.8/src/unitlab/cli.py` & `unitlab-1.8.9/src/unitlab/cli.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.8/src/unitlab/client.py` & `unitlab-1.8.9/src/unitlab/client.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.8/src/unitlab/exceptions.py` & `unitlab-1.8.9/src/unitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.8/src/unitlab/run.py` & `unitlab-1.8.9/src/unitlab/run.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.8/src/unitlab/utils.py` & `unitlab-1.8.9/src/unitlab/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     "cli_task_statistics": "/api/cli/tasks/{}/statistics/",
     "cli_datasets": "/api/cli/datasets/",
 }
 
 
 def send_request(request, session=None):
     endpoint = request.pop("endpoint")
-    if base_url := os.environ.get("UNITLAB_BASE_URL"):
-        request["url"] = base_url + endpoint
+    if os.environ.get("UNITLAB_BASE_URL"):
+        request["url"] = os.environ.get("UNITLAB_BASE_URL") + endpoint
         response = (
             session.request(**request) if session else requests.request(**request)
         )
         if response.ok:
             return response
 
     request["url"] = "https://api.unitlab.ai" + endpoint
```

