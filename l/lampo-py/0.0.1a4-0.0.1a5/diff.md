# Comparing `tmp/lampo_py-0.0.1a4.tar.gz` & `tmp/lampo_py-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lampo_py-0.0.1a4.tar", max compression
+gzip compressed data, was "lampo_py-0.0.1a5.tar", max compression
```

## Comparing `lampo_py-0.0.1a4.tar` & `lampo_py-0.0.1a5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      143 2023-05-19 20:34:41.067709 lampo_py-0.0.1a4/README.md
--rw-r--r--   0        0        0       31 2023-05-19 20:34:41.067709 lampo_py-0.0.1a4/lampo_py/__init__.py
--rw-r--r--   0        0        0     2953 2023-05-23 20:36:58.462585 lampo_py-0.0.1a4/lampo_py/lampo.py
--rw-r--r--   0        0        0      432 2023-05-23 21:34:12.275383 lampo_py-0.0.1a4/pyproject.toml
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 lampo_py-0.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-06-09 21:47:37.142795 lampo_py-0.0.1a5/README.md
+-rw-r--r--   0        0        0       31 2023-06-09 21:47:37.142795 lampo_py-0.0.1a5/lampo_py/__init__.py
+-rw-r--r--   0        0        0     3378 2023-06-14 17:21:12.520060 lampo_py-0.0.1a5/lampo_py/lampo.py
+-rw-r--r--   0        0        0      432 2023-06-14 17:23:33.245921 lampo_py-0.0.1a5/pyproject.toml
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 lampo_py-0.0.1a5/PKG-INFO
```

### Comparing `lampo_py-0.0.1a4/lampo_py/lampo.py` & `lampo_py-0.0.1a5/lampo_py/lampo.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,26 +67,39 @@
         home_path = ffi.new("char[]", home_path.encode('ascii'))
         logging.info(f'home path {ffi.string(home_path)}')
         self.__inner = lampod.new_lampod(home_path)
         if self.__inner == ffi.NULL:
             err = ffi.string(lampod.lampo_last_errror())
             raise Exception(err)
 
+    def register_unix_rpc(self):
+        """ ""
+        Run The lightning node!
+        """
+        lampod.add_jsonrpc_on_unixsocket(self.__inner)
+
+
     def listen(self):
         """ ""
         Run The lightning node!
         """
         #lampod.add_jsonrpc_on_unixsocket(self.__inner)
         lampod.lampo_listen(self.__inner)
 
     def call(self, method: str, payload: Dict[str, Any]) -> Dict[str, Any]:
         """ " Perform a call to the lightning node"""
+        logging.info(f"------ call `{method}` with payload `{payload}`")
         result = lampod.lampod_call(self.__inner, bytes(method, "utf-8"), b"{}")
+        if result is None:
+            logging.error("response is null")
+            err = lampod.lampo_last_errror()
+            raise Exception(ffi.string(err))
         logging.debug(f"raw data {result}")
         result = ffi.string(result).decode("utf-8")
+        logging.debug(f"data {result}")
         assert result is not None
         result = json.loads(result)
 
         logging.debug(f"call to `{method}` return {result}")
         return result
 
     def __exit__(self, exc_type, exc_value, traceback):
```

### Comparing `lampo_py-0.0.1a4/PKG-INFO` & `lampo_py-0.0.1a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lampo-py
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: 
 Author: Vincenzo Palazzo
 Author-email: vincenzopalazzodev@gmail.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

