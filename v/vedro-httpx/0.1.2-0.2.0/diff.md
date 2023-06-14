# Comparing `tmp/vedro-httpx-0.1.2.tar.gz` & `tmp/vedro-httpx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-httpx-0.1.2.tar", last modified: Tue Jun 13 15:51:52 2023, max compression
+gzip compressed data, was "vedro-httpx-0.2.0.tar", last modified: Wed Jun 14 15:18:29 2023, max compression
```

## Comparing `vedro-httpx-0.1.2.tar` & `vedro-httpx-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:51:52.150869 vedro-httpx-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-13 15:51:52.150869 vedro-httpx-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-13 15:51:52.150869 vedro-httpx-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:51:52.146870 vedro-httpx-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/tests/test_async_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/tests/test_format_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/tests/test_sync_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:51:52.150869 vedro-httpx-0.1.2/vedro_httpx/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/_async_http_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/_render_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/_sync_http_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/_vedro_httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:51:52.150869 vedro-httpx-0.1.2/vedro_httpx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-13 15:51:52.000000 vedro-httpx-0.1.2/vedro_httpx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-13 15:51:52.000000 vedro-httpx-0.1.2/vedro_httpx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:51:52.000000 vedro-httpx-0.1.2/vedro_httpx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 15:51:52.000000 vedro-httpx-0.1.2/vedro_httpx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 15:51:52.000000 vedro-httpx-0.1.2/vedro_httpx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:18:29.150343 vedro-httpx-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-14 15:18:29.150343 vedro-httpx-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-14 15:18:29.150343 vedro-httpx-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:18:29.150343 vedro-httpx-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/tests/test_async_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/tests/test_format_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/tests/test_sync_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:18:29.150343 vedro-httpx-0.2.0/vedro_httpx/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/_async_http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/_render_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/_sync_http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/_vedro_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:18:29.150343 vedro-httpx-0.2.0/vedro_httpx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-14 15:18:29.000000 vedro-httpx-0.2.0/vedro_httpx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-14 15:18:29.000000 vedro-httpx-0.2.0/vedro_httpx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:18:29.000000 vedro-httpx-0.2.0/vedro_httpx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-14 15:18:29.000000 vedro-httpx-0.2.0/vedro_httpx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 15:18:29.000000 vedro-httpx-0.2.0/vedro_httpx.egg-info/top_level.txt
```

### Comparing `vedro-httpx-0.1.2/LICENSE` & `vedro-httpx-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.2/PKG-INFO` & `vedro-httpx-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: vedro-httpx
-Version: 0.1.2
+Version: 0.2.0
 Summary: Vedro + HTTPX
 Home-page: https://github.com/vedro-universe/vedro-httpx
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
+Project-URL: Docs, https://vedro.io/docs/integrations/httpx-client
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-httpx
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
@@ -93,7 +94,11 @@
 class Api(AsyncHTTPInterface):
     def __init__(self, base_url: str = "http://localhost:8080") -> None:
         super().__init__(base_url)
 
     async def register(self, creds: dict[str, str]) -> Response:
         return await self._request("POST", "/auth/register", json=creds)
 ```
+
+## Documentation
+
+Check out the [documentation](https://vedro.io/docs/integrations/httpx-client) for additional information about `vedro-httpx`.
```

### Comparing `vedro-httpx-0.1.2/README.md` & `vedro-httpx-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -74,7 +74,11 @@
 class Api(AsyncHTTPInterface):
     def __init__(self, base_url: str = "http://localhost:8080") -> None:
         super().__init__(base_url)
 
     async def register(self, creds: dict[str, str]) -> Response:
         return await self._request("POST", "/auth/register", json=creds)
 ```
+
+## Documentation
+
+Check out the [documentation](https://vedro.io/docs/integrations/httpx-client) for additional information about `vedro-httpx`.
```

### Comparing `vedro-httpx-0.1.2/setup.cfg` & `vedro-httpx-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.2
+current_version = 0.2.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-httpx-0.1.2/setup.py` & `vedro-httpx-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-httpx",
-    version="0.1.2",
+    version="0.2.0",
     description="Vedro + HTTPX",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.8",
     url="https://github.com/vedro-universe/vedro-httpx",
     project_urls={
+        "Docs": "https://vedro.io/docs/integrations/httpx-client",
         "GitHub": "https://github.com/vedro-universe/vedro-httpx",
     },
     license="Apache-2.0",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"vedro_httpx": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
```

### Comparing `vedro-httpx-0.1.2/tests/test_async_interface.py` & `vedro-httpx-0.2.0/tests/test_async_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.2/tests/test_format_response.py` & `vedro-httpx-0.2.0/tests/test_format_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,28 +49,28 @@
     with given:
         response = Response(status_code=200)
 
     with when:
         code, lexer = format_response_body(response)
 
     with then:
-        assert code == "<binary len=0>"
+        assert code == "<binary preview=b'' len=0>"
         assert lexer == ""
 
 
 def test_format_response_no_content_type():
     with given:
-        body = b"{}"
+        body = b"a04e8431ff62"
         response = Response(status_code=200, content=body)
 
     with when:
         code, lexer = format_response_body(response)
 
     with then:
-        assert code == f"<binary len={len(body)}>"
+        assert code == f"<binary preview={body[:10]} len={len(body)}>"
         assert lexer == ""
 
 
 def test_format_response_text():
     with given:
         body = b"Hello, world!"
         response = Response(status_code=200, content=body, headers={
```

### Comparing `vedro-httpx-0.1.2/tests/test_response.py` & `vedro-httpx-0.2.0/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.2/tests/test_sync_interface.py` & `vedro-httpx-0.2.0/tests/test_sync_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.2/vedro_httpx/_async_http_interface.py` & `vedro-httpx-0.2.0/vedro_httpx/_async_http_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,18 +38,19 @@
 
 
 class AsyncHTTPInterface(vedro.Interface):
     def __init__(self, base_url: Union[URL, str] = "") -> None:
         super().__init__()
         self._base_url = base_url
 
-    # Docs https://www.python-httpx.org/advanced/
+    # Docs https://www.python-httpx.org/api/#asyncclient
     def _client(self, **kwargs: Any) -> AsyncClient:
         return AsyncClient(**kwargs)
 
+    # Arguments are duplicated to provide auto-completion
     async def _request(self,
                        method: str,
                        url: Union[URL, str],
                        *,
                        content: Optional[RequestContent] = None,
                        data: Optional[RequestData] = None,
                        files: Optional[RequestFiles] = None,
```

### Comparing `vedro-httpx-0.1.2/vedro_httpx/_render_response.py` & `vedro-httpx-0.2.0/vedro_httpx/_render_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 def render_response(response: Response, *,
                     theme: str = "ansi_dark", code_width: int = 1024 ** 2) -> RenderResult:
     yield "Response:"
     headers, http_lexer = format_response_headers(response)
     yield Syntax(headers, http_lexer, theme=theme, code_width=code_width)
 
     body, lexer = format_response_body(response)
-    yield Syntax(body, lexer, theme=theme, background_color="default",
-                 indent_guides=True, code_width=code_width)
+    yield Syntax(body, lexer, theme=theme, indent_guides=True, code_width=code_width)
 
 
 def format_response_headers(response: Response) -> Tuple[str, Lexer]:
     lines = [f"{response.http_version} {response.status_code} {response.reason_phrase}"]
     for header in response.headers:
         values = response.headers.get_list(header)
         for value in values:
@@ -35,15 +34,16 @@
 
 def format_response_body(response: Response) -> Tuple[Any, Union[Lexer, str]]:
     content_type = response.headers.get("Content-Type", "")
     mime_type, *_ = content_type.split(";")
     try:
         lexer = get_lexer_for_mimetype(mime_type.strip())
     except ClassNotFound:
-        return f"<binary len={len(response.content)}>", ""
+        preview = response.content[:10]
+        return f"<binary preview={preview!r} len={len(response.content)}>", ""
 
     code = response.text
     if isinstance(lexer, JsonLexer):
         try:
             code = json.dumps(response.json(), indent=4)
         except BaseException:
             return code, TextLexer()
```

### Comparing `vedro-httpx-0.1.2/vedro_httpx/_sync_http_interface.py` & `vedro-httpx-0.2.0/vedro_httpx/_sync_http_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,18 +37,19 @@
 
 
 class SyncHTTPInterface(vedro.Interface):
     def __init__(self, base_url: Union[URL, str] = "") -> None:
         super().__init__()
         self._base_url = base_url
 
-    # Docs https://www.python-httpx.org/advanced/
+    # Docs https://www.python-httpx.org/api/#client
     def _client(self, **kwargs: Any) -> SyncClient:
         return SyncClient(**kwargs)
 
+    # Arguments are duplicated to provide auto-completion
     def _request(self,
                  method: str,
                  url: Union[URL, str],
                  *,
                  content: Optional[RequestContent] = None,
                  data: Optional[RequestData] = None,
                  files: Optional[RequestFiles] = None,
```

### Comparing `vedro-httpx-0.1.2/vedro_httpx.egg-info/PKG-INFO` & `vedro-httpx-0.2.0/vedro_httpx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: vedro-httpx
-Version: 0.1.2
+Version: 0.2.0
 Summary: Vedro + HTTPX
 Home-page: https://github.com/vedro-universe/vedro-httpx
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
+Project-URL: Docs, https://vedro.io/docs/integrations/httpx-client
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-httpx
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
@@ -93,7 +94,11 @@
 class Api(AsyncHTTPInterface):
     def __init__(self, base_url: str = "http://localhost:8080") -> None:
         super().__init__(base_url)
 
     async def register(self, creds: dict[str, str]) -> Response:
         return await self._request("POST", "/auth/register", json=creds)
 ```
+
+## Documentation
+
+Check out the [documentation](https://vedro.io/docs/integrations/httpx-client) for additional information about `vedro-httpx`.
```

### Comparing `vedro-httpx-0.1.2/vedro_httpx.egg-info/SOURCES.txt` & `vedro-httpx-0.2.0/vedro_httpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

