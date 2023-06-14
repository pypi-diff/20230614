# Comparing `tmp/computex_cli-0.1.1.tar.gz` & `tmp/computex_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computex_cli-0.1.1.tar", max compression
+gzip compressed data, was "computex_cli-0.1.2.tar", max compression
```

## Comparing `computex_cli-0.1.1.tar` & `computex_cli-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      613 2023-06-13 21:08:54.631293 computex_cli-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-12 13:32:24.984013 computex_cli-0.1.1/cxcli/__init__.py
--rw-r--r--   0        0        0     6202 2023-06-14 13:56:13.757403 computex_cli-0.1.1/cxcli/cli.py
--rw-r--r--   0        0        0      911 2023-06-13 21:08:54.632830 computex_cli-0.1.1/cxcli/config.py
--rw-r--r--   0        0        0      161 2023-06-13 21:08:54.633286 computex_cli-0.1.1/cxcli/exc.py
--rw-r--r--   0        0        0        0 2023-06-13 21:08:54.633381 computex_cli-0.1.1/cxcli/services/__init__.py
--rw-r--r--   0        0        0      950 2023-06-13 21:08:54.634140 computex_cli-0.1.1/cxcli/services/auth.py
--rw-r--r--   0        0        0     1485 2023-06-13 21:08:54.634576 computex_cli-0.1.1/cxcli/services/deployments.py
--rw-r--r--   0        0        0     1912 2023-06-13 21:08:54.635101 computex_cli-0.1.1/cxcli/services/service.py
--rw-r--r--   0        0        0     1236 2023-06-13 21:08:54.635947 computex_cli-0.1.1/cxcli/services/users.py
--rw-r--r--   0        0        0      727 2023-06-14 13:58:16.104380 computex_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 computex_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      613 2023-06-13 21:08:54.631293 computex_cli-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 13:32:24.984013 computex_cli-0.1.2/cxcli/__init__.py
+-rw-r--r--   0        0        0     6085 2023-06-14 16:12:11.890803 computex_cli-0.1.2/cxcli/cli.py
+-rw-r--r--   0        0        0      911 2023-06-13 21:08:54.632830 computex_cli-0.1.2/cxcli/config.py
+-rw-r--r--   0        0        0      161 2023-06-13 21:08:54.633286 computex_cli-0.1.2/cxcli/exc.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:08:54.633381 computex_cli-0.1.2/cxcli/services/__init__.py
+-rw-r--r--   0        0        0      950 2023-06-13 21:08:54.634140 computex_cli-0.1.2/cxcli/services/auth.py
+-rw-r--r--   0        0        0     1485 2023-06-13 21:08:54.634576 computex_cli-0.1.2/cxcli/services/deployments.py
+-rw-r--r--   0        0        0     1912 2023-06-13 21:08:54.635101 computex_cli-0.1.2/cxcli/services/service.py
+-rw-r--r--   0        0        0     1236 2023-06-13 21:08:54.635947 computex_cli-0.1.2/cxcli/services/users.py
+-rw-r--r--   0        0        0      727 2023-06-14 16:12:11.880449 computex_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 computex_cli-0.1.2/PKG-INFO
```

### Comparing `computex_cli-0.1.1/README.md` & `computex_cli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.1/cxcli/cli.py` & `computex_cli-0.1.2/cxcli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,18 +132,17 @@
     num_cpu_cores,
     num_gpu,
     gpu_sku,
     # cpu_sku,
     memory,
     replicas,
 ):
-    registry_credentials = UserServiceV1().get_registry_credentials()
     r = DeployRequest(
         app_name=app_name,
-        container_image=f"{registry_credentials.registry_namespace}/{container_image}",
+        container_image=container_image,
         num_cpu_cores=num_cpu_cores,
         num_gpu=num_gpu,
         gpu_sku=gpu_sku,
         # cpu_sku=cpu_sku,
         memory=memory,
         replicas=replicas,
     )
```

### Comparing `computex_cli-0.1.1/cxcli/config.py` & `computex_cli-0.1.2/cxcli/config.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.1/cxcli/services/auth.py` & `computex_cli-0.1.2/cxcli/services/auth.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.1/cxcli/services/deployments.py` & `computex_cli-0.1.2/cxcli/services/deployments.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.1/cxcli/services/service.py` & `computex_cli-0.1.2/cxcli/services/service.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.1/cxcli/services/users.py` & `computex_cli-0.1.2/cxcli/services/users.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.1/pyproject.toml` & `computex_cli-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "computex-cli"
-version = "0.1.1"
+version = "0.1.2"
 description = "ComputeX CLI tool"
 authors = ["Abate De Mey <abate@computex.ai>"]
 readme = "README.md"
 packages = [{include = "cxcli"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `computex_cli-0.1.1/PKG-INFO` & `computex_cli-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computex-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: ComputeX CLI tool
 Author: Abate De Mey
 Author-email: abate@computex.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

