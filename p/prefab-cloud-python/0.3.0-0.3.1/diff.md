# Comparing `tmp/prefab_cloud_python-0.3.0.tar.gz` & `tmp/prefab_cloud_python-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefab_cloud_python-0.3.0.tar", max compression
+gzip compressed data, was "prefab_cloud_python-0.3.1.tar", max compression
```

## Comparing `prefab_cloud_python-0.3.0.tar` & `prefab_cloud_python-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1054 2023-06-12 23:27:33.699244 prefab_cloud_python-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0      768 2023-05-08 23:50:45.418057 prefab_cloud_python-0.3.0/README.md
--rw-r--r--   0        0        0      117 2023-05-08 23:50:45.419706 prefab_cloud_python-0.3.0/prefab_cloud_python/__init__.py
--rw-r--r--   0        0        0     3495 2023-06-12 23:26:42.576839 prefab_cloud_python-0.3.0/prefab_cloud_python/_processors.py
--rw-r--r--   0        0        0     3499 2023-06-12 23:26:42.576967 prefab_cloud_python-0.3.0/prefab_cloud_python/client.py
--rw-r--r--   0        0        0     6654 2023-06-12 23:26:42.577111 prefab_cloud_python-0.3.0/prefab_cloud_python/config_client.py
--rw-r--r--   0        0        0     2288 2023-06-12 23:26:42.577338 prefab_cloud_python-0.3.0/prefab_cloud_python/config_loader.py
--rw-r--r--   0        0        0     4963 2023-04-12 22:57:29.416107 prefab_cloud_python-0.3.0/prefab_cloud_python/config_parser.py
--rw-r--r--   0        0        0     1476 2023-05-08 23:50:45.420741 prefab_cloud_python-0.3.0/prefab_cloud_python/config_resolver.py
--rw-r--r--   0        0        0     1107 2023-05-08 23:50:45.421081 prefab_cloud_python-0.3.0/prefab_cloud_python/config_value_unwrapper.py
--rw-r--r--   0        0        0     3305 2023-05-08 23:50:45.421401 prefab_cloud_python-0.3.0/prefab_cloud_python/context.py
--rw-r--r--   0        0        0     4010 2023-06-12 23:26:42.577562 prefab_cloud_python-0.3.0/prefab_cloud_python/criteria_evaluator.py
--rw-r--r--   0        0        0     1344 2023-06-12 23:26:42.577722 prefab_cloud_python-0.3.0/prefab_cloud_python/feature_flag_client.py
--rw-r--r--   0        0        0     2367 2023-06-12 23:26:42.577835 prefab_cloud_python-0.3.0/prefab_cloud_python/log_path_collector.py
--rw-r--r--   0        0        0     2497 2023-06-12 23:26:42.577957 prefab_cloud_python-0.3.0/prefab_cloud_python/logger_client.py
--rw-r--r--   0        0        0     5843 2023-06-12 23:26:42.578086 prefab_cloud_python-0.3.0/prefab_cloud_python/options.py
--rw-r--r--   0        0        0     1321 2023-05-23 23:23:40.055365 prefab_cloud_python-0.3.0/prefab_cloud_python/read_write_lock.py
--rw-r--r--   0        0        0     1099 2023-05-08 23:50:45.422222 prefab_cloud_python-0.3.0/prefab_cloud_python/weighted_value_resolver.py
--rw-r--r--   0        0        0      443 2023-05-25 23:50:08.502938 prefab_cloud_python-0.3.0/prefab_cloud_python/yaml_parser.py
--rw-r--r--   0        0        0    13403 2023-05-06 18:25:23.417081 prefab_cloud_python-0.3.0/prefab_pb2.py
--rw-r--r--   0        0        0      159 2023-05-06 18:25:29.960098 prefab_cloud_python-0.3.0/prefab_pb2_grpc.py
--rw-r--r--   0        0        0      950 2023-06-12 23:35:48.923244 prefab_cloud_python-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 prefab_cloud_python-0.3.0/setup.py
--rw-r--r--   0        0        0     1932 1970-01-01 00:00:00.000000 prefab_cloud_python-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-06-13 00:50:55.374694 prefab_cloud_python-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0      768 2023-05-08 23:50:45.418057 prefab_cloud_python-0.3.1/README.md
+-rw-r--r--   0        0        0      117 2023-05-08 23:50:45.419706 prefab_cloud_python-0.3.1/prefab_cloud_python/__init__.py
+-rw-r--r--   0        0        0     3496 2023-06-13 22:01:06.563045 prefab_cloud_python-0.3.1/prefab_cloud_python/_processors.py
+-rw-r--r--   0        0        0     3581 2023-06-13 22:01:06.563279 prefab_cloud_python-0.3.1/prefab_cloud_python/client.py
+-rw-r--r--   0        0        0     7242 2023-06-13 22:01:06.563523 prefab_cloud_python-0.3.1/prefab_cloud_python/config_client.py
+-rw-r--r--   0        0        0     2288 2023-06-12 23:26:42.577338 prefab_cloud_python-0.3.1/prefab_cloud_python/config_loader.py
+-rw-r--r--   0        0        0     4963 2023-04-12 22:57:29.416107 prefab_cloud_python-0.3.1/prefab_cloud_python/config_parser.py
+-rw-r--r--   0        0        0     1476 2023-05-08 23:50:45.420741 prefab_cloud_python-0.3.1/prefab_cloud_python/config_resolver.py
+-rw-r--r--   0        0        0     1107 2023-05-08 23:50:45.421081 prefab_cloud_python-0.3.1/prefab_cloud_python/config_value_unwrapper.py
+-rw-r--r--   0        0        0     3305 2023-05-08 23:50:45.421401 prefab_cloud_python-0.3.1/prefab_cloud_python/context.py
+-rw-r--r--   0        0        0     4010 2023-06-12 23:26:42.577562 prefab_cloud_python-0.3.1/prefab_cloud_python/criteria_evaluator.py
+-rw-r--r--   0        0        0     1344 2023-06-12 23:26:42.577722 prefab_cloud_python-0.3.1/prefab_cloud_python/feature_flag_client.py
+-rw-r--r--   0        0        0     2367 2023-06-13 00:36:56.487397 prefab_cloud_python-0.3.1/prefab_cloud_python/log_path_collector.py
+-rw-r--r--   0        0        0     2497 2023-06-12 23:26:42.577957 prefab_cloud_python-0.3.1/prefab_cloud_python/logger_client.py
+-rw-r--r--   0        0        0     5843 2023-06-12 23:26:42.578086 prefab_cloud_python-0.3.1/prefab_cloud_python/options.py
+-rw-r--r--   0        0        0     1594 2023-06-13 22:01:06.563757 prefab_cloud_python-0.3.1/prefab_cloud_python/read_write_lock.py
+-rw-r--r--   0        0        0     1099 2023-05-08 23:50:45.422222 prefab_cloud_python-0.3.1/prefab_cloud_python/weighted_value_resolver.py
+-rw-r--r--   0        0        0      443 2023-05-25 23:50:08.502938 prefab_cloud_python-0.3.1/prefab_cloud_python/yaml_parser.py
+-rw-r--r--   0        0        0    13403 2023-05-06 18:25:23.417081 prefab_cloud_python-0.3.1/prefab_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-06 18:25:29.960098 prefab_cloud_python-0.3.1/prefab_pb2_grpc.py
+-rw-r--r--   0        0        0      950 2023-06-13 22:01:06.563982 prefab_cloud_python-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 prefab_cloud_python-0.3.1/setup.py
+-rw-r--r--   0        0        0     1932 1970-01-01 00:00:00.000000 prefab_cloud_python-0.3.1/PKG-INFO
```

### Comparing `prefab_cloud_python-0.3.0/LICENSE.txt` & `prefab_cloud_python-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/README.md` & `prefab_cloud_python-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/_processors.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/_processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,21 +61,22 @@
 
 def log_or_drop(_, method, event_dict):
     location = event_dict["location"]
     config_client = event_dict["config_client"]
     closest_log_level = get_severity(location, config_client)
     called_method_level = python_to_prefab_log_levels[method]
 
-    if closest_log_level > called_method_level:
-        raise DropEvent
-
     if event_dict["log_path_collector"] and not event_dict["skip_collector"]:
         event_dict["log_path_collector"].push(
             event_dict["location"], Prefab.LogLevel.Name(called_method_level)
         )
+
+    if closest_log_level > called_method_level:
+        raise DropEvent
+
     return event_dict
 
 
 def get_severity(location, config_client):
     context = Context.get_current() or {}
     default = Prefab.LogLevel.Value("WARN")
     closest_log_level = config_client.get(
```

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/client.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,19 +26,24 @@
         )
         self.log_path_collector.client = self
         self.log_path_collector.start_periodic_sync()
         self.namespace = options.namespace
         self.api_url = options.prefab_api_url
         self.grpc_url = options.prefab_grpc_url
         if options.is_local_only():
-            self.logger.info("Prefab running in local-only mode")
+            self.logger.log_internal("info", "Prefab running in local-only mode")
         else:
-            self.logger.info(
+            self.logger.log_internal(
+                "info",
                 "Prefab connecting to %s and %s, secure %s"
-                % (options.prefab_api_url, options.prefab_grpc_url, options.http_secure)
+                % (
+                    options.prefab_api_url,
+                    options.prefab_grpc_url,
+                    options.http_secure,
+                ),
             )
 
         self.context().clear()
         self.config_client()
 
     def get(self, key, default="NO_DEFAULT_PROVIDED", context="NO_CONTEXT_PROVIDED"):
         if self.is_ff(key):
@@ -75,15 +80,14 @@
 
     def scoped_context(context):
         return Context.scope(context)
 
     @functools.cache
     def config_client(self):
         client = ConfigClient(self, timeout=5.0)
-        self.logger.set_config_client(client)
         return client
 
     @functools.cache
     def feature_flag_client(self):
         return FeatureFlagClient(self)
 
     def post(self, path, body):
```

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/config_client.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/config_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,32 +64,42 @@
         value = self.__get(key, None, {}, context=context)
         if value is not None:
             return ConfigValueUnwrapper.unwrap(value, key, context)
         else:
             return self.handle_default(key, default)
 
     def __get(self, key, lookup_key, properties, context=Context.get_current()):
-        return self.config_resolver.get(key, context=context)
+        try:
+            with self.init_lock.read_locked():
+                return self.config_resolver.get(key, context=context)
+        except Exception:
+            if self.options.on_connection_failure == "RAISE":
+                raise InitializationTimeoutException(
+                    self.options.connection_timeout_seconds, key
+                )
+            self.base_client.logger().warn(
+                f"Couldn't initialize in {self.options.connection_timeout_seconds}. Key {key}. Returning what we have."
+            )
+            self.init_lock.release_write()
+            return self.config_resolver.get(key, context=context)
 
     def handle_default(self, key, default):
         if default != "NO_DEFAULT_PROVIDED":
             return default
         if self.options.on_no_default == "RAISE":
             raise MissingDefaultException(key)
         return None
 
     def load_checkpoint(self):
         if self.load_checkpoint_from_api_cdn():
             return
         self.base_client.logger.log_internal("warn", "No success loading checkpoints")
 
     def start_checkpointing_thread(self):
-        self.checkpointing_thread = threading.Thread(
-            target=self.checkpointing_loop
-        )  # , daemon=True).start()
+        self.checkpointing_thread = threading.Thread(target=self.checkpointing_loop)
         self.checkpointing_thread.daemon = True
         self.checkpointing_thread.start()
 
     def start_streaming(self):
         self.streaming_thread = threading.Thread(target=self.streaming_loop)
         self.streaming_thread.daemon = True
         self.streaming_thread.start()
@@ -162,12 +172,13 @@
         self.finish_init(source)
 
     def finish_init(self, source):
         if not self.init_lock._write_locked:
             return
         self.base_client.logger.log_internal("info", f"Unlocked config via {source}")
         self.init_lock.release_write()
+        self.base_client.logger.set_config_client(self)
 
     @functools.cache
     def grpc_channel(self):
         creds = grpc.ssl_channel_credentials()
         return grpc.secure_channel(self.options.prefab_grpc_url, creds)
```

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/config_loader.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/config_loader.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/config_parser.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/config_parser.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/config_resolver.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/config_resolver.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/config_value_unwrapper.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/config_value_unwrapper.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/context.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/context.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/criteria_evaluator.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/criteria_evaluator.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/feature_flag_client.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/feature_flag_client.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/log_path_collector.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/log_path_collector.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/logger_client.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/logger_client.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/options.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/options.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/read_write_lock.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/read_write_lock.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import threading
+from contextlib import contextmanager
 
 
 # source: https://www.oreilly.com/library/view/python-cookbook/0596001673/ch06s04.html
 class ReadWriteLock:
     """A lock object that allows many simultaneous "read locks", but
     only one "write lock." """
 
@@ -26,14 +27,23 @@
         try:
             self._readers -= 1
             if not self._readers:
                 self._read_ready.notify_all()
         finally:
             self._read_ready.release()
 
+    @contextmanager
+    def read_locked(self):
+        """This method is designed to be used via the `with` statement."""
+        try:
+            self.acquire_read()
+            yield
+        finally:
+            self.release_read()
+
     def acquire_write(self):
         """Acquire a write lock. Blocks until there are no
         acquired read or write locks."""
         self._read_ready.acquire()
         while self._readers > 0:
             self._read_ready.wait()
         self._write_locked = True
```

### Comparing `prefab_cloud_python-0.3.0/prefab_cloud_python/weighted_value_resolver.py` & `prefab_cloud_python-0.3.1/prefab_cloud_python/weighted_value_resolver.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/prefab_pb2.py` & `prefab_cloud_python-0.3.1/prefab_pb2.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.0/pyproject.toml` & `prefab_cloud_python-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prefab-cloud-python"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python client for Prefab Feature Flags, Dynamic log levels, and Config as a Service: https://www.prefab.cloud"
 license = "MIT"
 authors = ["Michael Berkowitz <michael.berkowitz@gmail.com>"]
 maintainers = ["Michael Berkowitz <michael.berkowitz@gmail.com>"]
 readme = "README.md"
 homepage = "https://www.prefab.cloud"
 repository = "https://github.com/prefab-cloud/prefab-cloud-python"
```

### Comparing `prefab_cloud_python-0.3.0/setup.py` & `prefab_cloud_python-0.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'sseclient-py>=1.7.2,<2.0.0',
  'structlog>=22.3,<23.0',
  'timecop>=0.5.0dev,<0.6.0',
  'urllib3>=2.0,<3.0']
 
 setup_kwargs = {
     'name': 'prefab-cloud-python',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Python client for Prefab Feature Flags, Dynamic log levels, and Config as a Service: https://www.prefab.cloud',
     'long_description': '# prefab-cloud-python\n\nPython client for prefab.cloud, providing Config, FeatureFlags as a Service\n\n**Note: This library is under active development and not quite ready for production usage**\n\n[Sign up to be notified when this library releases](https://forms.gle/2qsjMFvjGnkTnA9T8)\n\n## Example usage\n\n```python\nfrom prefab_cloud_python import Client, Options\n\noptions = Options(\n    prefab_api_key="your-prefab-api-key"\n)\n\ncontext = {\n  "user": {\n    "team_id": 432,\n    "id": 123,\n    "subscription_level": \'pro\',\n    "email": "alice@example.com"\n  }\n}\n\nclient = Client(options)\n\nresult = client.enabled("my-first-feature-flag", context=context)\n\nprint("my-first-feature-flag is:", result)\n```\n\nSee full documentation https://docs.prefab.cloud/docs/python-sdk/python\n',
     'author': 'Michael Berkowitz',
     'author_email': 'michael.berkowitz@gmail.com',
     'maintainer': 'Michael Berkowitz',
     'maintainer_email': 'michael.berkowitz@gmail.com',
     'url': 'https://www.prefab.cloud',
```

### Comparing `prefab_cloud_python-0.3.0/PKG-INFO` & `prefab_cloud_python-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefab-cloud-python
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python client for Prefab Feature Flags, Dynamic log levels, and Config as a Service: https://www.prefab.cloud
 Home-page: https://www.prefab.cloud
 License: MIT
 Author: Michael Berkowitz
 Author-email: michael.berkowitz@gmail.com
 Maintainer: Michael Berkowitz
 Maintainer-email: michael.berkowitz@gmail.com
```

