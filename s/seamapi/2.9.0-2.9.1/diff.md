# Comparing `tmp/seamapi-2.9.0.tar.gz` & `tmp/seamapi-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamapi-2.9.0.tar", max compression
+gzip compressed data, was "seamapi-2.9.1.tar", max compression
```

## Comparing `seamapi-2.9.0.tar` & `seamapi-2.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      574 2023-03-17 18:41:36.615127 seamapi-2.9.0/pyproject.toml
--rw-r--r--   0        0        0       61 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/__init__.py
--rw-r--r--   0        0        0    11927 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/access_codes.py
--rw-r--r--   0        0        0     3639 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/action_attempts.py
--rw-r--r--   0        0        0     4233 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/connect_webviews.py
--rw-r--r--   0        0        0     4558 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/connected_accounts.py
--rw-r--r--   0        0        0     5599 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/devices.py
--rw-r--r--   0        0        0     3310 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/events.py
--rw-r--r--   0        0        0     4795 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/locks.py
--rw-r--r--   0        0        0      828 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/routes.py
--rw-r--r--   0        0        0     3861 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/seam.py
--rw-r--r--   0        0        0     9181 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/types.py
--rw-r--r--   0        0        0        0 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/utils/__init__.py
--rw-r--r--   0        0        0     1426 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/utils/convert_to_id.py
--rw-r--r--   0        0        0      864 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/utils/deep_attr_dict.py
--rw-r--r--   0        0        0      117 2023-03-17 18:41:19.834808 seamapi-2.9.0/seamapi/utils/get_sentry_dsn.py
--rw-r--r--   0        0        0      518 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/utils/report_error.py
--rw-r--r--   0        0        0     2977 2023-03-17 18:40:57.070386 seamapi-2.9.0/seamapi/workspaces.py
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 seamapi-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0      574 2023-03-17 18:48:29.995762 seamapi-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/__init__.py
+-rw-r--r--   0        0        0    11927 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/access_codes.py
+-rw-r--r--   0        0        0     3639 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/action_attempts.py
+-rw-r--r--   0        0        0     4257 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/connect_webviews.py
+-rw-r--r--   0        0        0     4558 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/connected_accounts.py
+-rw-r--r--   0        0        0     5599 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/devices.py
+-rw-r--r--   0        0        0     3310 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/events.py
+-rw-r--r--   0        0        0     4795 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/locks.py
+-rw-r--r--   0        0        0      828 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/routes.py
+-rw-r--r--   0        0        0     3861 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/seam.py
+-rw-r--r--   0        0        0     9181 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/types.py
+-rw-r--r--   0        0        0        0 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/utils/__init__.py
+-rw-r--r--   0        0        0     1426 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/utils/convert_to_id.py
+-rw-r--r--   0        0        0      864 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/utils/deep_attr_dict.py
+-rw-r--r--   0        0        0      117 2023-03-17 18:48:12.347622 seamapi-2.9.1/seamapi/utils/get_sentry_dsn.py
+-rw-r--r--   0        0        0      518 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/utils/report_error.py
+-rw-r--r--   0        0        0     2977 2023-03-17 18:47:52.071442 seamapi-2.9.1/seamapi/workspaces.py
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 seamapi-2.9.1/PKG-INFO
```

### Comparing `seamapi-2.9.0/pyproject.toml` & `seamapi-2.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seamapi"
-version = "2.9.0"
+version = "2.9.1"
 description = "A Python Library for Seam's API https://getseam.com"
 authors = ["Severin Ibarluzea <seveibar@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 requests = "^2.26.0"
```

### Comparing `seamapi-2.9.0/seamapi/access_codes.py` & `seamapi-2.9.1/seamapi/access_codes.py`

 * *Files identical despite different names*

### Comparing `seamapi-2.9.0/seamapi/action_attempts.py` & `seamapi-2.9.1/seamapi/action_attempts.py`

 * *Files identical despite different names*

### Comparing `seamapi-2.9.0/seamapi/connect_webviews.py` & `seamapi-2.9.1/seamapi/connect_webviews.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         res = self.seam.make_request(
             "GET",
             "/connect_webviews/list",
         )
         json_webviews = res["connect_webviews"]
 
         return [
-            ConnectWebview(**json_webview) for json_webview in json_webviews
+            ConnectWebview.from_dict(json_webview) for json_webview in json_webviews
         ]
 
     @report_error
     def get(
         self, connect_webview: Union[ConnectWebviewId, ConnectWebview]
     ) -> ConnectWebview:
         """Gets a connect webview.
@@ -96,15 +96,15 @@
         res = self.seam.make_request(
             "GET",
             "/connect_webviews/get",
             params={"connect_webview_id": connect_webview_id},
         )
         json_webview = res["connect_webview"]
 
-        return ConnectWebview(**json_webview)
+        return ConnectWebview.from_dict(json_webview)
 
     @report_error
     def create(
         self,
         accepted_providers: List[AcceptedProvider],
         custom_redirect_url: Optional[str] = None,
         custom_redirect_failure_url: Optional[str] = None,
@@ -148,8 +148,8 @@
         res = self.seam.make_request(
             "POST",
             "/connect_webviews/create",
             json=create_payload,
         )
         json_webview = res["connect_webview"]
 
-        return ConnectWebview(**json_webview)
+        return ConnectWebview.from_dict(json_webview)
```

### Comparing `seamapi-2.9.0/seamapi/connected_accounts.py` & `seamapi-2.9.1/seamapi/connected_accounts.py`

 * *Files identical despite different names*

### Comparing `seamapi-2.9.0/seamapi/devices.py` & `seamapi-2.9.1/seamapi/devices.py`

 * *Files identical despite different names*

### Comparing `seamapi-2.9.0/seamapi/events.py` & `seamapi-2.9.1/seamapi/events.py`

 * *Files identical despite different names*

### Comparing `seamapi-2.9.0/seamapi/locks.py` & `seamapi-2.9.1/seamapi/locks.py`

 * *Files identical despite different names*

### Comparing `seamapi-2.9.0/seamapi/routes.py` & `seamapi-2.9.1/seamapi/routes.py`

 * *Files identical despite different names*

### Comparing `seamapi-2.9.0/seamapi/seam.py` & `seamapi-2.9.1/seamapi/seam.py`

 * *Files identical despite different names*

### Comparing `seamapi-2.9.0/seamapi/types.py` & `seamapi-2.9.1/seamapi/types.py`

 * *Files identical despite different names*

### Comparing `seamapi-2.9.0/seamapi/utils/convert_to_id.py` & `seamapi-2.9.1/seamapi/utils/convert_to_id.py`

 * *Files identical despite different names*

### Comparing `seamapi-2.9.0/seamapi/utils/deep_attr_dict.py` & `seamapi-2.9.1/seamapi/utils/deep_attr_dict.py`

 * *Files identical despite different names*

### Comparing `seamapi-2.9.0/seamapi/utils/report_error.py` & `seamapi-2.9.1/seamapi/utils/report_error.py`

 * *Files identical despite different names*

### Comparing `seamapi-2.9.0/seamapi/workspaces.py` & `seamapi-2.9.1/seamapi/workspaces.py`

 * *Files identical despite different names*

### Comparing `seamapi-2.9.0/PKG-INFO` & `seamapi-2.9.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamapi
-Version: 2.9.0
+Version: 2.9.1
 Summary: A Python Library for Seam's API https://getseam.com
 License: MIT
 Author: Severin Ibarluzea
 Author-email: seveibar@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

