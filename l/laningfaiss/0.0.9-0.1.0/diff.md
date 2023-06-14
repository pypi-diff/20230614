# Comparing `tmp/laningfaiss-0.0.9.tar.gz` & `tmp/laningfaiss-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/laningfaiss-0.0.9.tar", last modified: Fri Apr  7 03:48:16 2023, max compression
+gzip compressed data, was "dist/laningfaiss-0.1.0.tar", last modified: Wed Jun 14 03:28:25 2023, max compression
```

## Comparing `laningfaiss-0.0.9.tar` & `laningfaiss-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 03:48:16.000000 laningfaiss-0.0.9/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-03-23 06:17:06.000000 laningfaiss-0.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      194 2023-04-07 03:48:16.000000 laningfaiss-0.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-03-23 06:17:06.000000 laningfaiss-0.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 03:48:16.000000 laningfaiss-0.0.9/laningfaiss/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-03-23 06:17:06.000000 laningfaiss-0.0.9/laningfaiss/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9465 2023-04-07 03:46:28.000000 laningfaiss-0.0.9/laningfaiss/requester.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 03:48:16.000000 laningfaiss-0.0.9/laningfaiss.egg-info/
--rw-r--r--   0 root         (0) root         (0)      194 2023-04-07 03:48:16.000000 laningfaiss-0.0.9/laningfaiss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      249 2023-04-07 03:48:16.000000 laningfaiss-0.0.9/laningfaiss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 03:48:16.000000 laningfaiss-0.0.9/laningfaiss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-07 03:48:16.000000 laningfaiss-0.0.9/laningfaiss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 03:48:16.000000 laningfaiss-0.0.9/laningfaiss.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 03:48:16.000000 laningfaiss-0.0.9/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      791 2023-03-23 06:38:33.000000 laningfaiss-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-03-23 06:17:06.000000 laningfaiss-0.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      581 2023-06-14 03:28:06.000000 laningfaiss-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-03-23 06:17:06.000000 laningfaiss-0.1.0/laningfaiss/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10277 2023-06-14 03:28:06.000000 laningfaiss-0.1.0/laningfaiss/requester.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      791 2023-03-23 06:38:33.000000 laningfaiss-0.1.0/setup.py
```

### Comparing `laningfaiss-0.0.9/laningfaiss/requester.py` & `laningfaiss-0.1.0/laningfaiss/requester.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 from typing import List, Any
 
 import faiss
 import numpy as np
 from httpx import AsyncClient
 
 
-class LaningFaissError(Exception):
-    ...
-
-
 class Requester:
     def __init__(self, base_url: str, timeout):
         self.base_url = base_url
         self.timeout = timeout
 
-    async def request(self, method, url, **kwargs):
-        try:
-            async with AsyncClient() as client:
-                response = await client.request(method, url, **kwargs)
-            return response
-        except Exception as e:
-            raise LaningFaissError(f"IO Error: {url}: {e}")
+    async def request(self, method, url, retry=3, **kwargs):
+        response = None
+        exc = None
+        for _ in range(retry):
+            try:
+                async with AsyncClient() as client:
+                    response = await client.request(method, url, **kwargs)
+                    break
+            except Exception as e:
+                exc = e
+
+        if response is None:
+            raise exc
+        return response
 
     @staticmethod
     def parse(response):
         assert response.status_code == 200, f"{response.status_code} {response.reason_phrase}"
         data = response.json()
         assert data["code"] == 0, data["msg"]
         return data
@@ -43,22 +46,33 @@
     async def close(self):
         pass
 
 
 class RequesterContext(Requester):
     def __init__(self, base_url: str, timeout):
         super().__init__(base_url, timeout)
-        self.client = AsyncClient()
-
-    async def request(self, method, url, **kwargs):
-        try:
-            response = await self.client.request(method, url, **kwargs)
-            return response
-        except Exception as e:
-            raise LaningFaissError(f"IO Error: {url}: {e}")
+        self.client = AsyncClient(
+            timeout=timeout,
+            # limits=httpx.Limits(max_keepalive_connections=10, max_connections=20),
+        )
+
+    async def request(self, method, url, retry=3, **kwargs):
+        response = None
+        exc = None
+        for _ in range(retry):
+            try:
+                response = await self.client.request(method, url, **kwargs)
+                break
+            except Exception as e:
+                print(f"laningfaiss exception {e}. Retrying.")
+                exc = e
+
+        if response is None:
+            raise exc
+        return response
 
     async def close(self):
         await self.client.aclose()
 
 
 class Router:
     def __init__(self, base_url, timeout=10):
@@ -104,16 +118,16 @@
 
         payloads = {
             "vectors": searching_vectors.tolist(),
             "radius": threshold
         }
         response = await self.requester.post("range_search", json=payloads)
         res = response["data"]["res"]
-        assert len(res) == len(vectors), \
-            f"The response of engine is incomplete. expect {len(vectors)} but {len(res)}"
+        assert len(res) == searching_vectors.shape[0], \
+            f"The response of engine is incomplete. expect {searching_vectors.shape[0]} but {len(res)}"
 
         searched_mapping = {}
         for ftr_cmp_res, m in zip(res, number_list):
             if ftr_cmp_res:
                 vid = ftr_cmp_res[0][0]
                 sim = ftr_cmp_res[0][1]
                 searched_mapping[m] = (vid, sim)
@@ -211,17 +225,20 @@
 
         payloads = {
             "vectors": vectors_arr.tolist(),
             "radius": radius
         }
         response = await self.requester.post("range_search", json=payloads)
         res = response["data"]["res"]
-        for ftr_cmp_res in res:
-            for pair in ftr_cmp_res:
-                pair[1] = round(pair[1], 3)
+        try:
+            for ftr_cmp_res in res:
+                for pair in ftr_cmp_res:
+                    pair[1] = round(pair[1], 3)
+        except TypeError as e:
+            raise TypeError(f"parse error: {res}")
         return res
 
     async def remove(self, ids: List[int]):
         """
         根据id删除向量
 
         :param ids: 向量id列表
@@ -284,14 +301,26 @@
         }
         try:
             await self.requester.post("cancel", json=payloads)
             return True, None
         except Exception as e:
             return False, str(e)
 
+    async def cancel_all(self):
+        """
+        删除所有索引
+
+        :return:
+        """
+        try:
+            await self.requester.post("cancel_all", json={})
+            return True, None
+        except Exception as e:
+            return False, str(e)
+
     async def info(self) -> tuple:
         """
         获取索引相关信息
 
         :return: (项目名称, minio地址, 存储到minio的周期<秒>)
         """
         response = await self.requester.get("info")
```

### Comparing `laningfaiss-0.0.9/setup.py` & `laningfaiss-0.1.0/setup.py`

 * *Files identical despite different names*

