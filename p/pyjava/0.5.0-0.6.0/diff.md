# Comparing `tmp/pyjava-0.5.0.tar.gz` & `tmp/pyjava-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyjava-0.5.0.tar", last modified: Thu Jun  8 14:36:14 2023, max compression
+gzip compressed data, was "dist/pyjava-0.6.0.tar", last modified: Wed Jun 14 11:27:27 2023, max compression
```

## Comparing `pyjava-0.5.0.tar` & `pyjava-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      670 2023-06-08 14:36:14.000000 pyjava-0.5.0/PKG-INFO
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava.egg-info/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      670 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava.egg-info/PKG-INFO
--rw-r--r--   0 allwefantasy   (501) staff       (20)      596 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava.egg-info/SOURCES.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        7 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava.egg-info/top_level.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava.egg-info/dependency_links.txt
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    42222 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/cloudpickle.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6457 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/worker.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      828 2023-06-08 14:32:55.000000 pyjava-0.5.0/pyjava/version.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/cache/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      489 2021-01-12 02:30:28.000000 pyjava-0.5.0/pyjava/cache/code_cache.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2021-01-12 02:30:28.000000 pyjava-0.5.0/pyjava/cache/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30195 2021-01-12 02:30:28.000000 pyjava-0.5.0/pyjava/serializers.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2612 2023-03-06 01:45:39.000000 pyjava-0.5.0/pyjava/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/datatype/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2021-01-12 02:30:28.000000 pyjava-0.5.0/pyjava/datatype/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    64554 2021-01-12 02:30:28.000000 pyjava-0.5.0/pyjava/datatype/types.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/storage/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2825 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/storage/streaming_tar.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/storage/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3916 2021-10-03 00:16:16.000000 pyjava-0.5.0/pyjava/utils.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/api/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16024 2023-03-06 01:45:39.000000 pyjava-0.5.0/pyjava/api/mlsql.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      688 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/api/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4524 2023-03-17 14:55:56.000000 pyjava-0.5.0/pyjava/api/serve.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/udf/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5361 2023-06-08 14:32:55.000000 pyjava-0.5.0/pyjava/udf/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2190 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/rayfix.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-08 14:36:14.000000 pyjava-0.5.0/pyjava/data/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2022-10-12 14:29:02.000000 pyjava-0.5.0/pyjava/data/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1185 2023-03-19 01:36:05.000000 pyjava-0.5.0/pyjava/data/datasource.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     7048 2021-01-12 02:30:28.000000 pyjava-0.5.0/pyjava/daemon.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      448 2021-01-12 02:30:28.000000 pyjava-0.5.0/README.md
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2955 2022-10-12 14:29:02.000000 pyjava-0.5.0/setup.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)       79 2023-06-08 14:36:14.000000 pyjava-0.5.0/setup.cfg
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-14 11:27:27.000000 pyjava-0.6.0/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      670 2023-06-14 11:27:27.000000 pyjava-0.6.0/PKG-INFO
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-14 11:27:27.000000 pyjava-0.6.0/pyjava.egg-info/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      670 2023-06-14 11:27:27.000000 pyjava-0.6.0/pyjava.egg-info/PKG-INFO
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      596 2023-06-14 11:27:27.000000 pyjava-0.6.0/pyjava.egg-info/SOURCES.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        7 2023-06-14 11:27:27.000000 pyjava-0.6.0/pyjava.egg-info/top_level.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-06-14 11:27:27.000000 pyjava-0.6.0/pyjava.egg-info/dependency_links.txt
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-14 11:27:27.000000 pyjava-0.6.0/pyjava/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42222 2022-10-12 14:29:02.000000 pyjava-0.6.0/pyjava/cloudpickle.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6457 2022-10-12 14:29:02.000000 pyjava-0.6.0/pyjava/worker.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      828 2023-06-14 11:27:10.000000 pyjava-0.6.0/pyjava/version.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-14 11:27:27.000000 pyjava-0.6.0/pyjava/cache/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      489 2021-01-12 02:30:28.000000 pyjava-0.6.0/pyjava/cache/code_cache.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2021-01-12 02:30:28.000000 pyjava-0.6.0/pyjava/cache/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30195 2021-01-12 02:30:28.000000 pyjava-0.6.0/pyjava/serializers.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2612 2023-03-06 01:45:39.000000 pyjava-0.6.0/pyjava/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-14 11:27:27.000000 pyjava-0.6.0/pyjava/datatype/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2021-01-12 02:30:28.000000 pyjava-0.6.0/pyjava/datatype/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    64554 2021-01-12 02:30:28.000000 pyjava-0.6.0/pyjava/datatype/types.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-14 11:27:27.000000 pyjava-0.6.0/pyjava/storage/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2825 2022-10-12 14:29:02.000000 pyjava-0.6.0/pyjava/storage/streaming_tar.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2022-10-12 14:29:02.000000 pyjava-0.6.0/pyjava/storage/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3916 2021-10-03 00:16:16.000000 pyjava-0.6.0/pyjava/utils.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-14 11:27:27.000000 pyjava-0.6.0/pyjava/api/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16024 2023-03-06 01:45:39.000000 pyjava-0.6.0/pyjava/api/mlsql.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      688 2022-10-12 14:29:02.000000 pyjava-0.6.0/pyjava/api/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4524 2023-03-17 14:55:56.000000 pyjava-0.6.0/pyjava/api/serve.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-14 11:27:27.000000 pyjava-0.6.0/pyjava/udf/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5883 2023-06-14 11:27:10.000000 pyjava-0.6.0/pyjava/udf/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2190 2022-10-12 14:29:02.000000 pyjava-0.6.0/pyjava/rayfix.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-06-14 11:27:27.000000 pyjava-0.6.0/pyjava/data/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2022-10-12 14:29:02.000000 pyjava-0.6.0/pyjava/data/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1185 2023-03-19 01:36:05.000000 pyjava-0.6.0/pyjava/data/datasource.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7048 2021-01-12 02:30:28.000000 pyjava-0.6.0/pyjava/daemon.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      448 2021-01-12 02:30:28.000000 pyjava-0.6.0/README.md
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2955 2022-10-12 14:29:02.000000 pyjava-0.6.0/setup.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       79 2023-06-14 11:27:27.000000 pyjava-0.6.0/setup.cfg
```

### Comparing `pyjava-0.5.0/PKG-INFO` & `pyjava-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyjava
-Version: 0.5.0
+Version: 0.6.0
 Summary: PyJava Python API
 Home-page: https://github.com/allwefantasy/pyjava
 Author: allwefantasy
 Author-email: allwefantasy@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `pyjava-0.5.0/pyjava.egg-info/PKG-INFO` & `pyjava-0.6.0/pyjava.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyjava
-Version: 0.5.0
+Version: 0.6.0
 Summary: PyJava Python API
 Home-page: https://github.com/allwefantasy/pyjava
 Author: allwefantasy
 Author-email: allwefantasy@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `pyjava-0.5.0/pyjava.egg-info/SOURCES.txt` & `pyjava-0.6.0/pyjava.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/pyjava/cloudpickle.py` & `pyjava-0.6.0/pyjava/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/pyjava/worker.py` & `pyjava-0.6.0/pyjava/worker.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/pyjava/version.py` & `pyjava-0.6.0/pyjava/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
```

### Comparing `pyjava-0.5.0/pyjava/serializers.py` & `pyjava-0.6.0/pyjava/serializers.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/pyjava/__init__.py` & `pyjava-0.6.0/pyjava/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/pyjava/datatype/types.py` & `pyjava-0.6.0/pyjava/datatype/types.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/pyjava/storage/streaming_tar.py` & `pyjava-0.6.0/pyjava/storage/streaming_tar.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/pyjava/utils.py` & `pyjava-0.6.0/pyjava/utils.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/pyjava/api/mlsql.py` & `pyjava-0.6.0/pyjava/api/mlsql.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/pyjava/api/__init__.py` & `pyjava-0.6.0/pyjava/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/pyjava/api/serve.py` & `pyjava-0.6.0/pyjava/api/serve.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/pyjava/udf/__init__.py` & `pyjava-0.6.0/pyjava/udf/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,23 +28,28 @@
 
         if len(custom_resources) > 0:
             udf_worker_conf["resources"] = dict(custom_resources)
                 
         standalone = conf.get("standalone", "false") == "true"
         
         model_refs = []
-        print(f"standalone: {standalone} modelServers: {'modelServers' in conf}") 
+
+        udf_name  = conf["UDF_CLIENT"] if "UDF_CLIENT" in conf else "UNKNOW MODEL"
+                
         if "modelServers" in conf and not standalone:
-            model_servers = RayContext.parse_servers(conf["modelServers"])
-            print(f"Pull model from {model_servers[0].host}:{model_servers[0].port}")
+            model_servers = RayContext.parse_servers(conf["modelServers"])  
+            print(f"MODEL[{udf_name}] Transfer model from {model_servers[0].host}:{model_servers[0].port} to Ray Object Store")                       
             time1 = time.time()
-            items = RayContext.collect_from(model_servers)
-            model_refs = [ray.put(item) for item in items]
+            items = RayContext.collect_from(model_servers)            
+            for item in items:
+                if len(model_refs) % 5000:
+                    print(f"MODEL[{udf_name}] Transfer model from {model_servers[0].host}:{model_servers[0].port} to Ray Object Store, current count: {len(model_refs)}")
+                model_refs.append(ray.put(item))            
             time2 = time.time()
-            print(f"Success to pull model, time taken:{time2-time1}s. The total refs: {len(model_refs)}")    
+            print(f"MODEL[{udf_name}] Successful to put the model in Ray, time taken:{time2-time1}s. The total refs: {len(model_refs)}")    
             
 
         self.actors = dict(
             [(index,
               UDFWorker.options(**udf_worker_conf).remote(model_refs, conf, init_func,
                                                           apply_func)) for index in
              range(num)])
@@ -68,19 +73,22 @@
 @ray.remote
 class UDFWorker(object):
     def __init__(self,
                  model_refs: List[ClientObjectRef],
                  conf: Dict[str, str],
                  init_func: Callable[[List[ClientObjectRef], Dict[str, str]], Any],
                  apply_func: Callable[[Any, Any], Any]):
-        print("Init model....")
+        
+        udf_name  = conf["UDF_CLIENT"] if "UDF_CLIENT" in conf else "UNKNOW MODEL"
+
+        print(f"MODEL[{udf_name}] Init Model,It make take a while.")
         time1 = time.time()
         self.model = init_func(model_refs, conf)
         time2 = time.time()
-        print(f"Success to init model. Time taken: {time2 - time1}s")
+        print(f"MODEL[{udf_name}] Successful to init model, time taken:{time2-time1}s")
         self.apply_func = apply_func
 
     def apply(self, v: Any) -> Any:
         return self.apply_func(self.model, v)
 
     def shutdown(self):
         ray.actor.exit_actor()
```

### Comparing `pyjava-0.5.0/pyjava/rayfix.py` & `pyjava-0.6.0/pyjava/rayfix.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/pyjava/data/datasource.py` & `pyjava-0.6.0/pyjava/data/datasource.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/pyjava/daemon.py` & `pyjava-0.6.0/pyjava/daemon.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.5.0/setup.py` & `pyjava-0.6.0/setup.py`

 * *Files identical despite different names*

