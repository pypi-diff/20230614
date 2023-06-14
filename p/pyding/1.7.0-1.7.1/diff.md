# Comparing `tmp/pyding-1.7.0.tar.gz` & `tmp/pyding-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyding-1.7.0.tar", last modified: Sat Dec 10 17:27:48 2022, max compression
+gzip compressed data, was "pyding-1.7.1.tar", last modified: Wed Jun 14 18:05:56 2023, max compression
```

## Comparing `pyding-1.7.0.tar` & `pyding-1.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 17:27:48.086963 pyding-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-10 17:27:37.000000 pyding-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2022-12-10 17:27:48.086963 pyding-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2022-12-10 17:27:37.000000 pyding-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 17:27:48.082963 pyding-1.7.0/pyding/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2022-12-10 17:27:37.000000 pyding-1.7.0/pyding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2022-12-10 17:27:37.000000 pyding-1.7.0/pyding/event_space.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-10 17:27:37.000000 pyding-1.7.0/pyding/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2022-12-10 17:27:37.000000 pyding-1.7.0/pyding/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2022-12-10 17:27:37.000000 pyding-1.7.0/pyding/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 17:27:48.082963 pyding-1.7.0/pyding.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2022-12-10 17:27:48.000000 pyding-1.7.0/pyding.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-10 17:27:48.000000 pyding-1.7.0/pyding.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-10 17:27:48.000000 pyding-1.7.0/pyding.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-10 17:27:48.000000 pyding-1.7.0/pyding.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-10 17:27:48.086963 pyding-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2022-12-10 17:27:37.000000 pyding-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:05:56.412751 pyding-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 18:05:39.000000 pyding-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-14 18:05:56.412751 pyding-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-14 18:05:39.000000 pyding-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:05:56.412751 pyding-1.7.1/pyding/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-14 18:05:39.000000 pyding-1.7.1/pyding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-14 18:05:39.000000 pyding-1.7.1/pyding/event_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-14 18:05:39.000000 pyding-1.7.1/pyding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-14 18:05:39.000000 pyding-1.7.1/pyding/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-14 18:05:39.000000 pyding-1.7.1/pyding/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:05:56.412751 pyding-1.7.1/pyding.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-14 18:05:56.000000 pyding-1.7.1/pyding.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-14 18:05:56.000000 pyding-1.7.1/pyding.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:05:56.000000 pyding-1.7.1/pyding.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 18:05:56.000000 pyding-1.7.1/pyding.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:05:56.412751 pyding-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-14 18:05:39.000000 pyding-1.7.1/setup.py
```

### Comparing `pyding-1.7.0/LICENSE` & `pyding-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyding-1.7.0/PKG-INFO` & `pyding-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyding
-Version: 1.7.0
+Version: 1.7.1
 Summary: Simpĺe but effective event framework
 Home-page: https://github.com/jaobernardi/pyding
 Author: João Lucas Bernardi
 Author-email: joao_bernardi@outlook.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyding-1.7.0/README.md` & `pyding-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyding-1.7.0/pyding/event_space.py` & `pyding-1.7.1/pyding/event_space.py`

 * *Files identical despite different names*

### Comparing `pyding-1.7.0/pyding/methods.py` & `pyding-1.7.1/pyding/methods.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 on = global_event_space.on
 call = global_event_space.call
 async_call = global_event_space.async_call
 handlers_registered = global_event_space.handler_registered
 register_handler = global_event_space.register_handler
 unregister_from_module = global_event_space.unregister_from_module
 unregister_handler = global_event_space.unregister_handler
-get_handlers = global_event_space.get_handlers
+get_handlers = global_event_space.get_handlers
```

### Comparing `pyding-1.7.0/pyding/structures.py` & `pyding-1.7.1/pyding/structures.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     def handler(self, *args, **kwargs):
         self.output = kwargs
         return
     
     def wait(self):
         while not self.output:
             continue
+        self.unregister()
         return self.output
 
 
 
 # Add support for event calls inside objects
 class EventSupport:
     def __init__(self):
```

### Comparing `pyding-1.7.0/pyding.egg-info/PKG-INFO` & `pyding-1.7.1/pyding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyding
-Version: 1.7.0
+Version: 1.7.1
 Summary: Simpĺe but effective event framework
 Home-page: https://github.com/jaobernardi/pyding
 Author: João Lucas Bernardi
 Author-email: joao_bernardi@outlook.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyding-1.7.0/setup.py` & `pyding-1.7.1/setup.py`

 * *Files identical despite different names*

