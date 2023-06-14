# Comparing `tmp/lampo_py-0.0.1a6.tar.gz` & `tmp/lampo_py-0.0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lampo_py-0.0.1a6.tar", max compression
+gzip compressed data, was "lampo_py-0.0.1a7.tar", max compression
```

## Comparing `lampo_py-0.0.1a6.tar` & `lampo_py-0.0.1a7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      143 2023-06-09 21:47:37.142795 lampo_py-0.0.1a6/README.md
--rw-r--r--   0        0        0       31 2023-06-09 21:47:37.142795 lampo_py-0.0.1a6/lampo_py/__init__.py
--rw-r--r--   0        0        0     3366 2023-06-14 17:28:31.344822 lampo_py-0.0.1a6/lampo_py/lampo.py
--rw-r--r--   0        0        0      432 2023-06-14 17:25:08.759863 lampo_py-0.0.1a6/pyproject.toml
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 lampo_py-0.0.1a6/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-06-09 21:47:37.142795 lampo_py-0.0.1a7/README.md
+-rw-r--r--   0        0        0       31 2023-06-09 21:47:37.142795 lampo_py-0.0.1a7/lampo_py/__init__.py
+-rw-r--r--   0        0        0     3370 2023-06-14 17:44:10.632644 lampo_py-0.0.1a7/lampo_py/lampo.py
+-rw-r--r--   0        0        0      432 2023-06-14 17:44:20.416369 lampo_py-0.0.1a7/pyproject.toml
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 lampo_py-0.0.1a7/PKG-INFO
```

### Comparing `lampo_py-0.0.1a6/lampo_py/lampo.py` & `lampo_py-0.0.1a7/lampo_py/lampo.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         #lampod.add_jsonrpc_on_unixsocket(self.__inner)
         lampod.lampo_listen(self.__inner)
 
     def call(self, method: str, payload: Dict[str, Any] = {}) -> Dict[str, Any]:
         """ " Perform a call to the lightning node"""
         payload = json.dumps(payload)
         result = lampod.lampod_call(self.__inner, bytes(method, "utf-8"), bytes(payload, "utf-8"))
-        if result is None:
+        if result == ffi.NULL:
             logging.error("response is null")
             err = lampod.lampo_last_errror()
             raise Exception(ffi.string(err))
         logging.debug(f"raw data {result}")
         result = ffi.string(result).decode("utf-8")
         logging.debug(f"data {result}")
         assert result is not None
```

### Comparing `lampo_py-0.0.1a6/PKG-INFO` & `lampo_py-0.0.1a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lampo-py
-Version: 0.0.1a6
+Version: 0.0.1a7
 Summary: 
 Author: Vincenzo Palazzo
 Author-email: vincenzopalazzodev@gmail.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

