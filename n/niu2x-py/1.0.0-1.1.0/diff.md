# Comparing `tmp/niu2x-py-1.0.0.tar.gz` & `tmp/niu2x-py-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niu2x-py-1.0.0.tar", last modified: Fri Oct  7 14:45:55 2022, max compression
+gzip compressed data, was "niu2x-py-1.1.0.tar", last modified: Sat Oct  8 03:07:13 2022, max compression
```

## Comparing `niu2x-py-1.0.0.tar` & `niu2x-py-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 niu2x     (1000) niu2x     (1000)        0 2022-10-07 14:45:55.423783 niu2x-py-1.0.0/
--rw-rw-r--   0 niu2x     (1000) niu2x     (1000)     1062 2022-04-03 10:20:06.000000 niu2x-py-1.0.0/LICENSE
--rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      644 2022-10-07 14:45:55.423783 niu2x-py-1.0.0/PKG-INFO
--rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      181 2022-08-06 16:54:26.000000 niu2x-py-1.0.0/README.md
--rw-rw-r--   0 niu2x     (1000) niu2x     (1000)       84 2022-04-03 10:42:54.000000 niu2x-py-1.0.0/pyproject.toml
--rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      588 2022-10-07 14:45:55.423783 niu2x-py-1.0.0/setup.cfg
-drwxrwxr-x   0 niu2x     (1000) niu2x     (1000)        0 2022-10-07 14:45:55.419782 niu2x-py-1.0.0/src/
-drwxrwxr-x   0 niu2x     (1000) niu2x     (1000)        0 2022-10-07 14:45:55.423783 niu2x-py-1.0.0/src/niu2x_py.egg-info/
--rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      644 2022-10-07 14:45:55.000000 niu2x-py-1.0.0/src/niu2x_py.egg-info/PKG-INFO
--rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      263 2022-10-07 14:45:55.000000 niu2x-py-1.0.0/src/niu2x_py.egg-info/SOURCES.txt
--rw-rw-r--   0 niu2x     (1000) niu2x     (1000)        1 2022-10-07 14:45:55.000000 niu2x-py-1.0.0/src/niu2x_py.egg-info/dependency_links.txt
--rw-rw-r--   0 niu2x     (1000) niu2x     (1000)        5 2022-10-07 14:45:55.000000 niu2x-py-1.0.0/src/niu2x_py.egg-info/top_level.txt
-drwxrwxr-x   0 niu2x     (1000) niu2x     (1000)        0 2022-10-07 14:45:55.423783 niu2x-py-1.0.0/src/nxpy/
--rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      224 2022-04-03 14:27:09.000000 niu2x-py-1.0.0/src/nxpy/__init__.py
--rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      663 2022-04-03 14:17:57.000000 niu2x-py-1.0.0/src/nxpy/log.py
--rw-rw-r--   0 niu2x     (1000) niu2x     (1000)     1339 2022-08-06 16:55:08.000000 niu2x-py-1.0.0/src/nxpy/misc.py
--rw-rw-r--   0 niu2x     (1000) niu2x     (1000)     1721 2022-04-03 14:30:39.000000 niu2x-py-1.0.0/src/nxpy/subprocess.py
+drwxrwxr-x   0 niu2x     (1000) niu2x     (1000)        0 2022-10-08 03:07:13.725335 niu2x-py-1.1.0/
+-rw-rw-r--   0 niu2x     (1000) niu2x     (1000)     1062 2022-04-06 11:36:14.000000 niu2x-py-1.1.0/LICENSE
+-rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      644 2022-10-08 03:07:13.725335 niu2x-py-1.1.0/PKG-INFO
+-rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      181 2022-10-08 02:38:04.000000 niu2x-py-1.1.0/README.md
+-rw-rw-r--   0 niu2x     (1000) niu2x     (1000)       84 2022-04-06 11:36:14.000000 niu2x-py-1.1.0/pyproject.toml
+-rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      588 2022-10-08 03:07:13.725335 niu2x-py-1.1.0/setup.cfg
+drwxrwxr-x   0 niu2x     (1000) niu2x     (1000)        0 2022-10-08 03:07:13.721335 niu2x-py-1.1.0/src/
+drwxrwxr-x   0 niu2x     (1000) niu2x     (1000)        0 2022-10-08 03:07:13.721335 niu2x-py-1.1.0/src/niu2x_py.egg-info/
+-rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      644 2022-10-08 03:07:13.000000 niu2x-py-1.1.0/src/niu2x_py.egg-info/PKG-INFO
+-rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      263 2022-10-08 03:07:13.000000 niu2x-py-1.1.0/src/niu2x_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 niu2x     (1000) niu2x     (1000)        1 2022-10-08 03:07:13.000000 niu2x-py-1.1.0/src/niu2x_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 niu2x     (1000) niu2x     (1000)        5 2022-10-08 03:07:13.000000 niu2x-py-1.1.0/src/niu2x_py.egg-info/top_level.txt
+drwxrwxr-x   0 niu2x     (1000) niu2x     (1000)        0 2022-10-08 03:07:13.725335 niu2x-py-1.1.0/src/nxpy/
+-rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      407 2022-10-08 03:04:06.000000 niu2x-py-1.1.0/src/nxpy/__init__.py
+-rw-rw-r--   0 niu2x     (1000) niu2x     (1000)      663 2022-04-06 11:36:14.000000 niu2x-py-1.1.0/src/nxpy/log.py
+-rw-rw-r--   0 niu2x     (1000) niu2x     (1000)     2196 2022-10-08 03:04:06.000000 niu2x-py-1.1.0/src/nxpy/misc.py
+-rw-rw-r--   0 niu2x     (1000) niu2x     (1000)     1854 2022-10-08 03:04:06.000000 niu2x-py-1.1.0/src/nxpy/subprocess.py
```

### Comparing `niu2x-py-1.0.0/LICENSE` & `niu2x-py-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `niu2x-py-1.0.0/PKG-INFO` & `niu2x-py-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niu2x-py
-Version: 1.0.0
+Version: 1.1.0
 Summary: niu2x's python library
 Home-page: https://gitee.com/niu2x/nxpy
 Author: niu2x
 Author-email: niu2x@icloud.com
 Project-URL: Bug Tracker, https://gitee.com/niu2x/nxpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `niu2x-py-1.0.0/setup.cfg` & `niu2x-py-1.1.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = niu2x-py
-version = 1.0.0
+version = 1.1.0
 author = niu2x
 author_email = niu2x@icloud.com
 description = niu2x's python library
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitee.com/niu2x/nxpy
 project_urls =
```

### Comparing `niu2x-py-1.0.0/src/niu2x_py.egg-info/PKG-INFO` & `niu2x-py-1.1.0/src/niu2x_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niu2x-py
-Version: 1.0.0
+Version: 1.1.0
 Summary: niu2x's python library
 Home-page: https://gitee.com/niu2x/nxpy
 Author: niu2x
 Author-email: niu2x@icloud.com
 Project-URL: Bug Tracker, https://gitee.com/niu2x/nxpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `niu2x-py-1.0.0/src/nxpy/log.py` & `niu2x-py-1.1.0/src/nxpy/log.py`

 * *Files identical despite different names*

### Comparing `niu2x-py-1.0.0/src/nxpy/subprocess.py` & `niu2x-py-1.1.0/src/nxpy/subprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     """
     proc = subprocess.Popen(cmd, stdin=subprocess.PIPE, stdout=subprocess.PIPE,
                             stderr=subprocess.PIPE, shell=True, **kwargs)
     children_process[proc] = cmd + str(kwargs)
     return proc
 
 
+def run(cmd, stop_if_child_fail=True, quite=False, **kwargs):
+    return wait(spawn(cmd, **kwargs), quite, "", stop_if_child_fail)
+
+
 def kill_all():
     """ """
     for proc in children_process:
         proc.kill()
     children_process.clear()
```

