# Comparing `tmp/antchain_nftx-1.8.2.tar.gz` & `tmp/antchain_nftx-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_nftx-1.8.2.tar", last modified: Thu Jun  8 03:51:06 2023, max compression
+gzip compressed data, was "dist/antchain_nftx-1.8.3.tar", last modified: Wed Jun 14 04:59:30 2023, max compression
```

## Comparing `antchain_nftx-1.8.2.tar` & `antchain_nftx-1.8.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_nftx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_nftx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_nftx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_nftx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_nftx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_nftx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_sdk_nftx/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_sdk_nftx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52197 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_sdk_nftx/client.py
--rw-r--r--   0 root         (0) root         (0)   105809 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_sdk_nftx/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 04:59:30.000000 antchain_nftx-1.8.3/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-14 04:59:29.000000 antchain_nftx-1.8.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-14 04:59:29.000000 antchain_nftx-1.8.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-14 04:59:30.000000 antchain_nftx-1.8.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-14 04:59:29.000000 antchain_nftx-1.8.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-14 04:59:29.000000 antchain_nftx-1.8.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 04:59:30.000000 antchain_nftx-1.8.3/antchain_nftx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-14 04:59:30.000000 antchain_nftx-1.8.3/antchain_nftx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-14 04:59:30.000000 antchain_nftx-1.8.3/antchain_nftx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 04:59:30.000000 antchain_nftx-1.8.3/antchain_nftx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-14 04:59:30.000000 antchain_nftx-1.8.3/antchain_nftx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-14 04:59:30.000000 antchain_nftx-1.8.3/antchain_nftx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 04:59:30.000000 antchain_nftx-1.8.3/antchain_sdk_nftx/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-14 04:59:29.000000 antchain_nftx-1.8.3/antchain_sdk_nftx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52197 2023-06-14 04:59:29.000000 antchain_nftx-1.8.3/antchain_sdk_nftx/client.py
+-rw-r--r--   0 root         (0) root         (0)   107073 2023-06-14 04:59:29.000000 antchain_nftx-1.8.3/antchain_sdk_nftx/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-14 04:59:30.000000 antchain_nftx-1.8.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-06-14 04:59:29.000000 antchain_nftx-1.8.3/setup.py
```

### Comparing `antchain_nftx-1.8.2/LICENSE` & `antchain_nftx-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.2/PKG-INFO` & `antchain_nftx-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_nftx
-Version: 1.8.2
+Version: 1.8.3
 Summary: Ant Chain NFTX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftx-1.8.2/README-CN.md` & `antchain_nftx-1.8.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.2/README.md` & `antchain_nftx-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.2/antchain_nftx.egg-info/PKG-INFO` & `antchain_nftx-1.8.3/antchain_nftx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-nftx
-Version: 1.8.2
+Version: 1.8.3
 Summary: Ant Chain NFTX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftx-1.8.2/antchain_sdk_nftx/client.py` & `antchain_nftx-1.8.3/antchain_sdk_nftx/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.2',
+                    'sdk_version': '1.8.3',
                     '_prod_code': 'NFTX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.2',
+                    'sdk_version': '1.8.3',
                     '_prod_code': 'NFTX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_nftx-1.8.2/antchain_sdk_nftx/models.py` & `antchain_nftx-1.8.3/antchain_sdk_nftx/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,58 @@
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
 
 
+class CToMResourceImg(TeaModel):
+    def __init__(
+        self,
+        thumbnail_url: str = None,
+        high_definition_url: str = None,
+        key: str = None,
+    ):
+        # 预览图
+        self.thumbnail_url = thumbnail_url
+        # 高清图
+        self.high_definition_url = high_definition_url
+        # key
+        self.key = key
+
+    def validate(self):
+        self.validate_required(self.thumbnail_url, 'thumbnail_url')
+        self.validate_required(self.high_definition_url, 'high_definition_url')
+        self.validate_required(self.key, 'key')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.thumbnail_url is not None:
+            result['thumbnail_url'] = self.thumbnail_url
+        if self.high_definition_url is not None:
+            result['high_definition_url'] = self.high_definition_url
+        if self.key is not None:
+            result['key'] = self.key
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('thumbnail_url') is not None:
+            self.thumbnail_url = m.get('thumbnail_url')
+        if m.get('high_definition_url') is not None:
+            self.high_definition_url = m.get('high_definition_url')
+        if m.get('key') is not None:
+            self.key = m.get('key')
+        return self
+
+
 class UserAsset(TeaModel):
     def __init__(
         self,
         sku_id: int = None,
         nft_id: str = None,
         sku_name: str = None,
         author_name: str = None,
@@ -2562,17 +2606,16 @@
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         nft_id: str = None,
         sku_name: str = None,
         uni_hash: str = None,
         creation_time: str = None,
-        thumbnail_urls: List[str] = None,
+        img_urls: List[CToMResourceImg] = None,
         high_definition_status: int = None,
-        high_definition_urls: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
@@ -2580,27 +2623,28 @@
         self.nft_id = nft_id
         # 具体藏品名称，type为NFT时有值
         self.sku_name = sku_name
         # nftId 的 算法计算的hash，该藏品唯一标识，type为NFT时有值
         self.uni_hash = uni_hash
         # Date	藏品铸造上链生成时间，例如2021.09.22 20:22:19，type为NFT时有值
         self.creation_time = creation_time
-        # 缩略图url列表
-        self.thumbnail_urls = thumbnail_urls
+        # url列表
+        self.img_urls = img_urls
         # int	高清图状态
         # 0 需要等待
         # 1 已完成
         self.high_definition_status = high_definition_status
-        # 在highDefinitionStatus为1时有值
-        # 高清图列表
-        self.high_definition_urls = high_definition_urls
 
     def validate(self):
         if self.creation_time is not None:
             self.validate_pattern(self.creation_time, 'creation_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
+        if self.img_urls:
+            for k in self.img_urls:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -2614,20 +2658,20 @@
             result['nft_id'] = self.nft_id
         if self.sku_name is not None:
             result['sku_name'] = self.sku_name
         if self.uni_hash is not None:
             result['uni_hash'] = self.uni_hash
         if self.creation_time is not None:
             result['creation_time'] = self.creation_time
-        if self.thumbnail_urls is not None:
-            result['thumbnail_urls'] = self.thumbnail_urls
+        result['img_urls'] = []
+        if self.img_urls is not None:
+            for k in self.img_urls:
+                result['img_urls'].append(k.to_map() if k else None)
         if self.high_definition_status is not None:
             result['high_definition_status'] = self.high_definition_status
-        if self.high_definition_urls is not None:
-            result['high_definition_urls'] = self.high_definition_urls
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -2638,20 +2682,21 @@
             self.nft_id = m.get('nft_id')
         if m.get('sku_name') is not None:
             self.sku_name = m.get('sku_name')
         if m.get('uni_hash') is not None:
             self.uni_hash = m.get('uni_hash')
         if m.get('creation_time') is not None:
             self.creation_time = m.get('creation_time')
-        if m.get('thumbnail_urls') is not None:
-            self.thumbnail_urls = m.get('thumbnail_urls')
+        self.img_urls = []
+        if m.get('img_urls') is not None:
+            for k in m.get('img_urls'):
+                temp_model = CToMResourceImg()
+                self.img_urls.append(temp_model.from_map(k))
         if m.get('high_definition_status') is not None:
             self.high_definition_status = m.get('high_definition_status')
-        if m.get('high_definition_urls') is not None:
-            self.high_definition_urls = m.get('high_definition_urls')
         return self
 
 
 class ApplyOauthTokenRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
```

### Comparing `antchain_nftx-1.8.2/setup.py` & `antchain_nftx-1.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_nftx.
 
-Created on 08/06/2023
+Created on 14/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_nftx"
 NAME = "antchain_nftx" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain NFTX SDK Library for Python"
```

