# Comparing `tmp/fastapi_swagger2-0.0.1b3.tar.gz` & `tmp/fastapi_swagger2-0.0.1b4.tar.gz`

## Comparing `fastapi_swagger2-0.0.1b3.tar` & `fastapi_swagger2-0.0.1b4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/.ruff_cache/.gitignore
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/.ruff_cache/.update-informer
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/.ruff_cache/content/10fbfe993ec4be0d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/.ruff_cache/content/1abeadf52d9572ab
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/.ruff_cache/content/8cf332caaea8e79b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/.ruff_cache/content/a8a883be09c5919b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/.ruff_cache/content/c180a20ea5e70786
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/.ruff_cache/content/f16744491f37c6f5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/.ruff_cache/content/f885759af04f4f9e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/.ruff_cache/content/fbcf51701267e364
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/scripts/build.sh
--rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/scripts/clean.sh
--rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/scripts/format.sh
--rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/scripts/lint.sh
--rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/scripts/publish.sh
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/scripts/test.sh
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/src/fastapi_swagger2/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/src/fastapi_swagger2/constants.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/src/fastapi_swagger2/models.py
--rw-r--r--   0        0        0    18659 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/src/fastapi_swagger2/utils.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/LICENSE
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/README.md
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/pyproject.toml
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b3/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/.update-informer
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/10fbfe993ec4be0d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/1abeadf52d9572ab
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/8cf332caaea8e79b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/a8a883be09c5919b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/c180a20ea5e70786
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/f16744491f37c6f5
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/f885759af04f4f9e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.ruff_cache/content/fbcf51701267e364
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/scripts/build.sh
+-rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/scripts/clean.sh
+-rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/scripts/format.sh
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/scripts/lint.sh
+-rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/scripts/publish.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/scripts/test.sh
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/constants.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/models.py
+-rw-r--r--   0        0        0    18659 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/utils.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/LICENSE
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/README.md
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/pyproject.toml
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b4/PKG-INFO
```

### Comparing `fastapi_swagger2-0.0.1b3/src/fastapi_swagger2/__init__.py` & `fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,39 @@
-__version__ = "0.0.1b3"
+__version__ = "0.0.1b4"
 
 from typing import Any, Dict, List, Optional, TypeVar
 
 from fastapi import FastAPI
 from fastapi.openapi.docs import (
     get_redoc_html,
     get_swagger_ui_html,
     get_swagger_ui_oauth2_redirect_html,
 )
 from starlette.requests import Request
 from starlette.responses import HTMLResponse, JSONResponse
 
 from fastapi_swagger2.utils import get_swagger2
 
-AppType = TypeVar("AppType", bound="FastAPI")
+
+# Keep mypy happy with the monkey patching
+class FastAPIEx(FastAPI):
+    swagger2_url: Optional[str]
+    swagger2_tags: Optional[List[Dict[str, Any]]]
+    swagger2_docs_url: Optional[str]
+    swagger2_redoc_url: Optional[str]
+    swagger2_ui_oauth2_redirect_url: Optional[str]
+    swagger2_ui_init_oauth: Optional[Dict[str, Any]]
+    swagger2_ui_parameters: Optional[Dict[str, Any]]
+    swagger2_version: str = "2.0"
+    swagger2_schema: Optional[Dict[str, Any]]
+
+    swagger2: Any
+
+
+AppType = TypeVar("AppType", bound="FastAPIEx")
 
 
 class FastAPISwagger2:
     def __init__(
         self,
         app: AppType,
         swagger2_url: Optional[str] = "/swagger2.json",
@@ -27,100 +43,102 @@
         swagger2_ui_oauth2_redirect_url: Optional[
             str
         ] = "/swagger2/docs/oauth2-redirect",
         swagger2_ui_init_oauth: Optional[Dict[str, Any]] = None,
         swagger2_ui_parameters: Optional[Dict[str, Any]] = None,
     ) -> None:
         self.app = app
-        self.swagger2_url = swagger2_url
-        self.swagger2_tags = swagger2_tags
-        self.swagger2_docs_url = swagger2_docs_url
-        self.swagger2_redoc_url = swagger2_redoc_url
-        self.swagger2_ui_oauth2_redirect_url = swagger2_ui_oauth2_redirect_url
-        self.swagger2_ui_init_oauth = swagger2_ui_init_oauth
-        self.swagger2_ui_parameters = swagger2_ui_parameters
-
-        self.swagger2_version = "2.0"
-        self.swagger2_schema: Optional[Dict[str, Any]] = None
-        if self.swagger2_url:
+        self.app.swagger2_url = swagger2_url
+        self.app.swagger2_tags = swagger2_tags
+        self.app.swagger2_docs_url = swagger2_docs_url
+        self.app.swagger2_redoc_url = swagger2_redoc_url
+        self.app.swagger2_ui_oauth2_redirect_url = swagger2_ui_oauth2_redirect_url
+        self.app.swagger2_ui_init_oauth = swagger2_ui_init_oauth
+        self.app.swagger2_ui_parameters = swagger2_ui_parameters
+
+        self.app.swagger2_version = "2.0"
+        self.app.swagger2_schema = None
+        if self.app.swagger2_url:
             assert (
                 self.app.title
             ), "A title must be provided for Swagger, e.g.: 'My API'"
             assert (
                 self.app.version
             ), "A version must be provided for Swagger, e.g.: '2.1.0'"
 
+        self.app.swagger2 = self.swagger2
+
         self.setup()
 
     def setup(self) -> None:
-        if self.swagger2_url:
+        if self.app.swagger2_url:
             urls = (server_data.get("url") for server_data in self.app.servers)
             server_urls = {url for url in urls if url}
 
             async def swagger2(req: Request) -> JSONResponse:
                 root_path = req.scope.get("root_path", "").rstrip("/")
                 if root_path not in server_urls:
                     if root_path and self.app.root_path_in_servers:
                         self.app.servers.insert(0, {"url": root_path})
                         server_urls.add(root_path)
                 return JSONResponse(self.swagger2())
 
-            self.app.add_route(self.swagger2_url, swagger2, include_in_schema=False)
+            self.app.add_route(self.app.swagger2_url, swagger2, include_in_schema=False)
 
-        if self.swagger2_url and self.swagger2_docs_url:
+        if self.app.swagger2_url and self.app.swagger2_docs_url:
 
             async def swagger_ui_html(req: Request) -> HTMLResponse:
                 root_path = req.scope.get("root_path", "").rstrip("/")
-                swagger2_url = root_path + self.swagger2_url
-                oauth2_redirect_url = self.swagger2_ui_oauth2_redirect_url
+                swagger2_url = root_path + self.app.swagger2_url
+                oauth2_redirect_url = self.app.swagger2_ui_oauth2_redirect_url
                 if oauth2_redirect_url:
                     oauth2_redirect_url = root_path + oauth2_redirect_url
                 return get_swagger_ui_html(
                     openapi_url=swagger2_url,
                     title=self.app.title + " - Swagger UI",
                     oauth2_redirect_url=oauth2_redirect_url,
-                    init_oauth=self.swagger2_ui_init_oauth,
-                    swagger_ui_parameters=self.swagger2_ui_parameters,
+                    init_oauth=self.app.swagger2_ui_init_oauth,
+                    swagger_ui_parameters=self.app.swagger2_ui_parameters,
                 )
 
             self.app.add_route(
-                self.swagger2_docs_url, swagger_ui_html, include_in_schema=False
+                self.app.swagger2_docs_url, swagger_ui_html, include_in_schema=False
             )
 
-            if self.swagger2_ui_oauth2_redirect_url:
+            if self.app.swagger2_ui_oauth2_redirect_url:
 
                 async def swagger_ui_redirect(req: Request) -> HTMLResponse:
                     return get_swagger_ui_oauth2_redirect_html()
 
                 self.app.add_route(
-                    self.swagger2_ui_oauth2_redirect_url,
+                    self.app.swagger2_ui_oauth2_redirect_url,
                     swagger_ui_redirect,
                     include_in_schema=False,
                 )
-        if self.swagger2_url and self.swagger2_redoc_url:
+        if self.app.swagger2_url and self.app.swagger2_redoc_url:
 
             async def redoc_html(req: Request) -> HTMLResponse:
                 root_path = req.scope.get("root_path", "").rstrip("/")
-                swagger2_url = root_path + self.swagger2_url
+                swagger2_url = root_path + self.app.swagger2_url
                 return get_redoc_html(
                     openapi_url=swagger2_url, title=self.app.title + " - ReDoc"
                 )
 
             self.app.add_route(
-                self.swagger2_redoc_url, redoc_html, include_in_schema=False
+                self.app.swagger2_redoc_url, redoc_html, include_in_schema=False
             )
 
     def swagger2(self) -> Dict[str, Any]:
-        if not self.swagger2_schema:
-            self.swagger2_schema = get_swagger2(
+        if not self.app.swagger2_schema:
+            self.app.swagger2_schema = get_swagger2(
                 title=self.app.title,
                 version=self.app.version,
-                swagger2_version=self.swagger2_version,
+                swagger2_version=self.app.swagger2_version,
                 description=self.app.description,
                 terms_of_service=self.app.terms_of_service,
                 contact=self.app.contact,
                 license_info=self.app.license_info,
                 routes=self.app.routes,
-                tags=self.swagger2_tags,
+                tags=self.app.swagger2_tags,
             )
 
-        return self.swagger2_schema
+        return self.app.swagger2_schema
```

### Comparing `fastapi_swagger2-0.0.1b3/src/fastapi_swagger2/models.py` & `fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b3/src/fastapi_swagger2/utils.py` & `fastapi_swagger2-0.0.1b4/src/fastapi_swagger2/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b3/.gitignore` & `fastapi_swagger2-0.0.1b4/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b3/LICENSE` & `fastapi_swagger2-0.0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b3/README.md` & `fastapi_swagger2-0.0.1b4/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b3/pyproject.toml` & `fastapi_swagger2-0.0.1b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b3/PKG-INFO` & `fastapi_swagger2-0.0.1b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_swagger2
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: Swagger2 support for FastAPI framework
 Project-URL: Homepage, https://github.com/virajkanwade/fastapi_swagger2
 Project-URL: Documentation, https://github.com/virajkanwade/fastapi_swagger2
 Author-email: Viraj Kanwade <virajk.oib@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Viraj Kanwade
```

