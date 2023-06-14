# Comparing `tmp/oexp-0.7.6.tar.gz` & `tmp/oexp-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.7.6.tar", last modified: Mon Jun 12 16:34:28 2023, max compression
+gzip compressed data, was "oexp-0.8.0.tar", last modified: Wed Jun 14 01:07:12 2023, max compression
```

## Comparing `oexp-0.7.6.tar` & `oexp-0.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 16:34:28.828978 oexp-0.7.6/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 16:34:28.828737 oexp-0.7.6/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.7.6/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 16:34:28.827412 oexp-0.7.6/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.7.6/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    80316 2023-06-12 16:34:05.000000 oexp-0.7.6/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-12 16:34:04.000000 oexp-0.7.6/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2011 2023-06-12 01:50:22.000000 oexp-0.7.6/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 16:34:28.828525 oexp-0.7.6/oexp/util/
--rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.7.6/oexp/util/__init__.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2650 2023-06-12 14:09:05.000000 oexp-0.7.6/oexp/util/ops.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.7.6/oexp/util/vals.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 16:34:28.828110 oexp-0.7.6/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 16:34:28.000000 oexp-0.7.6/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-12 16:34:28.000000 oexp-0.7.6/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-12 16:34:28.000000 oexp-0.7.6/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-12 16:34:28.000000 oexp-0.7.6/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-12 16:34:28.000000 oexp-0.7.6/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-12 16:34:24.000000 oexp-0.7.6/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-12 16:34:28.829051 oexp-0.7.6/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-14 01:07:12.805117 oexp-0.8.0/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-14 01:07:12.804897 oexp-0.8.0/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.8.0/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-14 01:07:12.803465 oexp-0.8.0/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.8.0/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    80838 2023-06-14 01:06:38.000000 oexp-0.8.0/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-14 01:06:36.000000 oexp-0.8.0/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2011 2023-06-12 01:50:22.000000 oexp-0.8.0/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-14 01:07:12.804644 oexp-0.8.0/oexp/util/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.8.0/oexp/util/__init__.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2650 2023-06-12 14:09:05.000000 oexp-0.8.0/oexp/util/ops.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.8.0/oexp/util/vals.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-14 01:07:12.804241 oexp-0.8.0/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-14 01:07:12.000000 oexp-0.8.0/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-14 01:07:12.000000 oexp-0.8.0/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-14 01:07:12.000000 oexp-0.8.0/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-14 01:07:12.000000 oexp-0.8.0/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-14 01:07:12.000000 oexp-0.8.0/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-14 01:07:08.000000 oexp-0.8.0/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-14 01:07:12.805169 oexp-0.8.0/setup.cfg
```

### Comparing `oexp-0.7.6/oexp/access.py` & `oexp-0.8.0/oexp/access.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     global _SAFE_PROCESS, _SAFE_THREAD
     if current_process().pid != _SAFE_PROCESS or current_thread().ident != _SAFE_THREAD:
         raise Exception(
             f"Python-Kotlin communication is currently not safe to use across multiple threads or processes. If you need this feature, please let me know."
         )
 
 
-JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/530/oexp-front-0-all.jar"
+JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/533/oexp-front-0-all.jar"
 
 
 class OexpExitSocketHeaders(Enum):
     EXIT = b"\x00"
 
 
 EXIT = b"\x00"
@@ -572,34 +572,48 @@
         _check_required_parameters(**dict())
         _sendall(CALL_FUN)
         _send_long(self._id._id)
         _send_int(7)
         _recv_exception_check()
         return _recv_object(SubjectData, nullable=False)
 
+    # [[matt.oexp.front.api.Experiment#uploadImage]]
+    def upload_image(self, local_abs_path=NO_DEFAULT, remote_rel_path=NO_DEFAULT):
+        _ensure_synchronized()
+        _check_required_parameters(
+            **dict(local_abs_path=local_abs_path, remote_rel_path=remote_rel_path)
+        )
+        _sendall(CALL_FUN)
+        _send_long(self._id._id)
+        _send_int(8)
+        _send_string(local_abs_path)
+        _send_string(remote_rel_path)
+        _recv_exception_check()
+        return _recv_confirmation()
+
     # [[matt.oexp.front.api.Experiment#uploadImages]]
     def upload_images(self, root_dir=NO_DEFAULT) -> List[str]:
         _ensure_synchronized()
         _check_required_parameters(**dict(root_dir=root_dir))
         _sendall(CALL_FUN)
         _send_long(self._id._id)
-        _send_int(8)
+        _send_int(9)
         _send_string(root_dir)
         _recv_exception_check()
         return _recv_list(
             elementReceiveFun=lambda: _recv_string(nullable=False), nullable=False
         )
 
     # [[matt.oexp.front.api.Experiment#viewImage]]
     def view_image(self, path=NO_DEFAULT):
         _ensure_synchronized()
         _check_required_parameters(**dict(path=path))
         _sendall(CALL_FUN)
         _send_long(self._id._id)
-        _send_int(9)
+        _send_int(10)
         _send_string(path)
         _recv_exception_check()
         return _recv_confirmation()
 
     # [[matt.oexp.front.api.Experiment]]
     def __eq__(self, other):
         _ensure_synchronized()
```

### Comparing `oexp-0.7.6/oexp/jbridge.py` & `oexp-0.8.0/oexp/jbridge.py`

 * *Files identical despite different names*

### Comparing `oexp-0.7.6/oexp/util/ops.py` & `oexp-0.8.0/oexp/util/ops.py`

 * *Files identical despite different names*

### Comparing `oexp-0.7.6/oexp/util/vals.py` & `oexp-0.8.0/oexp/util/vals.py`

 * *Files identical despite different names*

