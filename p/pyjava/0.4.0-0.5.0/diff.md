# Comparing `tmp/pyjava-0.4.0.tar.gz` & `tmp/pyjava-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyjava-0.4.0.tar", last modified: Mon May 15 03:00:29 2023, max compression
+gzip compressed data, was "dist/pyjava-0.5.0.tar", last modified: Thu Jun  8 14:36:14 2023, max compression
```

## Comparing `pyjava-0.4.0.tar` & `pyjava-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 03:00:29.000000 pyjava-0.4.0/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      670 2023-05-15 03:00:29.000000 pyjava-0.4.0/PKG-INFO
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 03:00:29.000000 pyjava-0.4.0/pyjava.egg-info/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      670 2023-05-15 03:00:28.000000 pyjava-0.4.0/pyjava.egg-info/PKG-INFO
--rw-r--r--   0 allwefantasy   (501) staff       (20)      596 2023-05-15 03:00:29.000000 pyjava-0.4.0/pyjava.egg-info/SOURCES.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        7 2023-05-15 03:00:28.000000 pyjava-0.4.0/pyjava.egg-info/top_level.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-05-15 03:00:28.000000 pyjava-0.4.0/pyjava.egg-info/dependency_links.txt
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 03:00:29.000000 pyjava-0.4.0/pyjava/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    42222 2022-10-12 14:29:02.000000 pyjava-0.4.0/pyjava/cloudpickle.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6457 2022-10-12 14:29:02.000000 pyjava-0.4.0/pyjava/worker.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      828 2023-05-15 02:59:58.000000 pyjava-0.4.0/pyjava/version.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 03:00:29.000000 pyjava-0.4.0/pyjava/cache/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      489 2021-01-12 02:30:28.000000 pyjava-0.4.0/pyjava/cache/code_cache.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2021-01-12 02:30:28.000000 pyjava-0.4.0/pyjava/cache/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30195 2021-01-12 02:30:28.000000 pyjava-0.4.0/pyjava/serializers.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2612 2023-03-06 01:45:39.000000 pyjava-0.4.0/pyjava/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 03:00:29.000000 pyjava-0.4.0/pyjava/datatype/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2021-01-12 02:30:28.000000 pyjava-0.4.0/pyjava/datatype/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    64554 2021-01-12 02:30:28.000000 pyjava-0.4.0/pyjava/datatype/types.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 03:00:29.000000 pyjava-0.4.0/pyjava/storage/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2825 2022-10-12 14:29:02.000000 pyjava-0.4.0/pyjava/storage/streaming_tar.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2022-10-12 14:29:02.000000 pyjava-0.4.0/pyjava/storage/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3916 2021-10-03 00:16:16.000000 pyjava-0.4.0/pyjava/utils.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 03:00:29.000000 pyjava-0.4.0/pyjava/api/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16024 2023-03-06 01:45:39.000000 pyjava-0.4.0/pyjava/api/mlsql.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      688 2022-10-12 14:29:02.000000 pyjava-0.4.0/pyjava/api/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4524 2023-03-17 14:55:56.000000 pyjava-0.4.0/pyjava/api/serve.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 03:00:29.000000 pyjava-0.4.0/pyjava/udf/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5103 2023-05-15 02:59:58.000000 pyjava-0.4.0/pyjava/udf/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2190 2022-10-12 14:29:02.000000 pyjava-0.4.0/pyjava/rayfix.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 03:00:29.000000 pyjava-0.4.0/pyjava/data/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2022-10-12 14:29:02.000000 pyjava-0.4.0/pyjava/data/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1185 2023-03-19 01:36:05.000000 pyjava-0.4.0/pyjava/data/datasource.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     7048 2021-01-12 02:30:28.000000 pyjava-0.4.0/pyjava/daemon.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      448 2021-01-12 02:30:28.000000 pyjava-0.4.0/README.md
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2955 2022-10-12 14:29:02.000000 pyjava-0.4.0/setup.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)       79 2023-05-15 03:00:29.000000 pyjava-0.4.0/setup.cfg
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      670 2023-06-08 14:36:14.000000 pyjava-0.5.0/PKG-INFO
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava.egg-info/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      670 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava.egg-info/PKG-INFO
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      596 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava.egg-info/SOURCES.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        7 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava.egg-info/top_level.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava.egg-info/dependency_links.txt
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42222 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/cloudpickle.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6457 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/worker.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      828 2023-06-08 14:32:55.000000 pyjava-0.5.0/pyjava/version.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/cache/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      489 2021-01-12 02:30:28.000000 pyjava-0.5.0/pyjava/cache/code_cache.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2021-01-12 02:30:28.000000 pyjava-0.5.0/pyjava/cache/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30195 2021-01-12 02:30:28.000000 pyjava-0.5.0/pyjava/serializers.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2612 2023-03-06 01:45:39.000000 pyjava-0.5.0/pyjava/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/datatype/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2021-01-12 02:30:28.000000 pyjava-0.5.0/pyjava/datatype/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    64554 2021-01-12 02:30:28.000000 pyjava-0.5.0/pyjava/datatype/types.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/storage/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2825 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/storage/streaming_tar.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/storage/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3916 2021-10-03 00:16:16.000000 pyjava-0.5.0/pyjava/utils.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/api/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16024 2023-03-06 01:45:39.000000 pyjava-0.5.0/pyjava/api/mlsql.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      688 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/api/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4524 2023-03-17 14:55:56.000000 pyjava-0.5.0/pyjava/api/serve.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/udf/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5361 2023-06-08 14:32:55.000000 pyjava-0.5.0/pyjava/udf/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2190 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/rayfix.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/data/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/data/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1185 2023-03-19 01:36:05.000000 pyjava-0.5.0/pyjava/data/datasource.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7048 2021-01-12 02:30:28.000000 pyjava-0.5.0/pyjava/daemon.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      448 2021-01-12 02:30:28.000000 pyjava-0.5.0/README.md
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2955 2022-10-12 14:29:02.000000 pyjava-0.5.0/setup.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       79 2023-06-08 14:36:14.000000 pyjava-0.5.0/setup.cfg
```

### Comparing `pyjava-0.4.0/PKG-INFO` & `pyjava-0.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyjava
-Version: 0.4.0
+Version: 0.5.0
 Summary: PyJava Python API
 Home-page: https://github.com/allwefantasy/pyjava
 Author: allwefantasy
 Author-email: allwefantasy@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `pyjava-0.4.0/pyjava.egg-info/PKG-INFO` & `pyjava-0.5.0/pyjava.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyjava
-Version: 0.4.0
+Version: 0.5.0
 Summary: PyJava Python API
 Home-page: https://github.com/allwefantasy/pyjava
 Author: allwefantasy
 Author-email: allwefantasy@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `pyjava-0.4.0/pyjava.egg-info/SOURCES.txt` & `pyjava-0.5.0/pyjava.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/pyjava/cloudpickle.py` & `pyjava-0.5.0/pyjava/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/pyjava/worker.py` & `pyjava-0.5.0/pyjava/worker.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/pyjava/version.py` & `pyjava-0.5.0/pyjava/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
```

### Comparing `pyjava-0.4.0/pyjava/serializers.py` & `pyjava-0.5.0/pyjava/serializers.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/pyjava/__init__.py` & `pyjava-0.5.0/pyjava/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/pyjava/datatype/types.py` & `pyjava-0.5.0/pyjava/datatype/types.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/pyjava/storage/streaming_tar.py` & `pyjava-0.5.0/pyjava/storage/streaming_tar.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/pyjava/utils.py` & `pyjava-0.5.0/pyjava/utils.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/pyjava/api/mlsql.py` & `pyjava-0.5.0/pyjava/api/mlsql.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/pyjava/api/__init__.py` & `pyjava-0.5.0/pyjava/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/pyjava/api/serve.py` & `pyjava-0.5.0/pyjava/api/serve.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/pyjava/udf/__init__.py` & `pyjava-0.5.0/pyjava/udf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import time
 from typing import Any, NoReturn, Callable, Dict, List
 import ray
 from ray.util.client.common import ClientActorHandle, ClientObjectRef
 
 from pyjava.api.mlsql import RayContext
 from pyjava.storage import streaming_tar
-
+import threading
 
 @ray.remote
 class UDFMaster(object):
     def __init__(self, num: int, conf: Dict[str, str],
                  init_func: Callable[[List[ClientObjectRef], Dict[str, str]], Any],
                  apply_func: Callable[[Any, Any], Any]):
+        self.lock = threading.Lock()         
         udf_worker_conf = {}
 
         if "num_cpus" in conf:
             udf_worker_conf["num_cpus"] = float(conf["num_cpus"])
 
         if "num_gpus" in conf:
             udf_worker_conf["num_gpus"] = float(conf["num_gpus"])
@@ -47,20 +48,22 @@
               UDFWorker.options(**udf_worker_conf).remote(model_refs, conf, init_func,
                                                           apply_func)) for index in
              range(num)])
         self._idle_actors = [index for index in range(num)]
 
     def get(self) -> List[Any]:
         while len(self._idle_actors) == 0:
-            time.sleep(0.001)
-        index = self._idle_actors.pop()
+                time.sleep(0.001)
+        with self.lock:            
+            index = self._idle_actors.pop()        
         return [index, self.actors[index]]
 
     def give_back(self, v) -> NoReturn:
-        self._idle_actors.append(v)
+        with self.lock:
+            self._idle_actors.append(v)
 
     def shutdown(self) -> NoReturn:
         [ray.kill(self.actors[index]) for index in self._idle_actors]
 
 
 @ray.remote
 class UDFWorker(object):
@@ -87,14 +90,15 @@
     @staticmethod
     def build(ray_context: RayContext,
               init_func: Callable[[List[ClientObjectRef], Dict[str, str]], Any],
               apply_func: Callable[[Any, Any], Any]) -> NoReturn:
         conf = ray_context.conf()
         udf_name = conf["UDF_CLIENT"]
         max_concurrency = int(conf.get("maxConcurrency", "3"))
+        masterMaxConcurrency = int(conf.get("masterMaxConcurrency", "1000"))
 
         try:
             stop_flag = True
             counter = 30
             temp_udf_master = ray.get_actor(udf_name)
             ray.kill(temp_udf_master)
             while stop_flag or counter < 0:
@@ -106,15 +110,15 @@
                     counter = counter - 1
 
         except Exception as inst:
             print(inst)
             pass
                 
         UDFMaster.options(name=udf_name, lifetime="detached",
-                          max_concurrency=max_concurrency).remote(
+                          max_concurrency=masterMaxConcurrency).remote(
             max_concurrency, conf, init_func, apply_func)
         ray_context.build_result([])
 
     @staticmethod
     def apply(ray_context: RayContext):
         conf = ray_context.conf()
         udf_name = conf["UDF_CLIENT"]
@@ -122,15 +126,16 @@
         [index, worker] = ray.get(udf_master.get.remote())
         input_value = [row["value"] for row in ray_context.python_context.fetch_once_as_rows()]
         try:
             res = ray.get(worker.apply.remote(input_value))
         except Exception as inst:
             res = {}
             print(inst)
-        udf_master.give_back.remote(index)
+        finally:    
+            ray.get(udf_master.give_back.remote(index))
         ray_context.build_result([res])
 
 
 class UDFBuildInFunc(object):
     @staticmethod
     def init_tf(model_refs: List[ClientObjectRef], conf: Dict[str, str]) -> Any:
         from tensorflow.keras import models
```

### Comparing `pyjava-0.4.0/pyjava/rayfix.py` & `pyjava-0.5.0/pyjava/rayfix.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/pyjava/data/datasource.py` & `pyjava-0.5.0/pyjava/data/datasource.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/pyjava/daemon.py` & `pyjava-0.5.0/pyjava/daemon.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.4.0/setup.py` & `pyjava-0.5.0/setup.py`

 * *Files identical despite different names*

