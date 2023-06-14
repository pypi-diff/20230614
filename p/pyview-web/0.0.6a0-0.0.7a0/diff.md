# Comparing `tmp/pyview_web-0.0.6a0.tar.gz` & `tmp/pyview_web-0.0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyview_web-0.0.6a0.tar", max compression
+gzip compressed data, was "pyview_web-0.0.7a0.tar", max compression
```

## Comparing `pyview_web-0.0.6a0.tar` & `pyview_web-0.0.7a0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0     1071 2023-05-02 00:38:29.733278 pyview_web-0.0.6a0/LICENSE
--rw-r--r--   0        0        0     2032 2023-05-17 01:47:12.158934 pyview_web-0.0.6a0/pyproject.toml
--rw-r--r--   0        0        0      223 2023-05-10 01:04:35.299955 pyview_web-0.0.6a0/pyview/__init__.py
--rw-r--r--   0        0        0     2508 2023-05-02 00:38:29.742232 pyview_web-0.0.6a0/pyview/assets/js/app.js
--rw-r--r--   0        0        0     2425 2023-05-02 00:38:29.742415 pyview_web-0.0.6a0/pyview/assets/package-lock.json
--rw-r--r--   0        0        0      151 2023-05-02 00:38:29.742554 pyview_web-0.0.6a0/pyview/assets/package.json
--rw-r--r--   0        0        0       46 2023-05-02 00:38:29.742781 pyview_web-0.0.6a0/pyview/changesets/__init__.py
--rw-r--r--   0        0        0     1747 2023-05-02 00:38:29.743020 pyview_web-0.0.6a0/pyview/changesets/changesets.py
--rw-r--r--   0        0        0     1119 2023-05-10 01:19:49.350200 pyview_web-0.0.6a0/pyview/csrf.py
--rw-r--r--   0        0        0      125 2023-05-17 01:41:14.565206 pyview_web-0.0.6a0/pyview/events.py
--rw-r--r--   0        0        0      751 2023-05-02 00:38:29.743473 pyview_web-0.0.6a0/pyview/js.py
--rw-r--r--   0        0        0      498 2023-05-02 00:38:29.743607 pyview_web-0.0.6a0/pyview/live_routes.py
--rw-r--r--   0        0        0     3314 2023-05-17 01:34:56.470702 pyview_web-0.0.6a0/pyview/live_socket.py
--rw-r--r--   0        0        0     1207 2023-05-11 13:26:15.707368 pyview_web-0.0.6a0/pyview/live_view.py
--rw-r--r--   0        0        0     3423 2023-05-02 00:38:29.744047 pyview_web-0.0.6a0/pyview/pyview.py
--rw-r--r--   0        0        0   199984 2023-05-02 00:38:29.745551 pyview_web-0.0.6a0/pyview/static/assets/app.js
--rw-r--r--   0        0        0      124 2023-05-02 00:38:29.745832 pyview_web-0.0.6a0/pyview/template/__init__.py
--rw-r--r--   0        0        0     1864 2023-05-02 00:38:29.745961 pyview_web-0.0.6a0/pyview/template/live_template.py
--rw-r--r--   0        0        0      826 2023-05-02 00:38:29.746088 pyview_web-0.0.6a0/pyview/template/serializer.py
--rw-r--r--   0        0        0      684 2023-05-02 00:38:29.746210 pyview_web-0.0.6a0/pyview/test_csrf.py
--rw-r--r--   0        0        0        0 2023-05-02 00:38:29.746312 pyview_web-0.0.6a0/pyview/vendor/__init__.py
--rw-r--r--   0        0        0       39 2023-05-02 00:38:29.746495 pyview_web-0.0.6a0/pyview/vendor/flet/pubsub/__init__.py
--rw-r--r--   0        0        0    10184 2023-05-02 00:38:29.746630 pyview_web-0.0.6a0/pyview/vendor/flet/pubsub/pub_sub.py
--rw-r--r--   0        0        0      455 2023-05-02 00:38:29.746775 pyview_web-0.0.6a0/pyview/vendor/ibis/__init__.py
--rw-r--r--   0        0        0     7220 2023-05-02 00:38:29.746901 pyview_web-0.0.6a0/pyview/vendor/ibis/compiler.py
--rw-r--r--   0        0        0     3613 2023-05-02 00:38:29.747013 pyview_web-0.0.6a0/pyview/vendor/ibis/context.py
--rw-r--r--   0        0        0     1531 2023-05-02 00:38:29.747126 pyview_web-0.0.6a0/pyview/vendor/ibis/errors.py
--rw-r--r--   0        0        0     7042 2023-05-02 00:38:29.747263 pyview_web-0.0.6a0/pyview/vendor/ibis/filters.py
--rw-r--r--   0        0        0     3457 2023-05-02 00:38:29.747371 pyview_web-0.0.6a0/pyview/vendor/ibis/loaders.py
--rw-r--r--   0        0        0    25128 2023-05-02 00:38:29.747569 pyview_web-0.0.6a0/pyview/vendor/ibis/nodes.py
--rw-r--r--   0        0        0     2314 2023-05-02 00:38:29.747704 pyview_web-0.0.6a0/pyview/vendor/ibis/template.py
--rw-r--r--   0        0        0     2293 2023-05-02 00:38:29.747817 pyview_web-0.0.6a0/pyview/vendor/ibis/tree.py
--rw-r--r--   0        0        0     2768 2023-05-02 00:38:29.747930 pyview_web-0.0.6a0/pyview/vendor/ibis/utils.py
--rw-r--r--   0        0        0     4624 2023-05-02 00:38:29.748053 pyview_web-0.0.6a0/pyview/ws_handler.py
--rw-r--r--   0        0        0     3144 2023-05-02 00:38:29.748181 pyview_web-0.0.6a0/readme.md
--rw-r--r--   0        0        0     5059 1970-01-01 00:00:00.000000 pyview_web-0.0.6a0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-02 00:38:29.733278 pyview_web-0.0.7a0/LICENSE
+-rw-r--r--   0        0        0     2032 2023-06-14 00:15:29.628194 pyview_web-0.0.7a0/pyproject.toml
+-rw-r--r--   0        0        0      223 2023-06-02 16:20:26.327598 pyview_web-0.0.7a0/pyview/__init__.py
+-rw-r--r--   0        0        0     2508 2023-05-02 00:38:29.742232 pyview_web-0.0.7a0/pyview/assets/js/app.js
+-rw-r--r--   0        0        0     2425 2023-05-02 00:38:29.742415 pyview_web-0.0.7a0/pyview/assets/package-lock.json
+-rw-r--r--   0        0        0      151 2023-05-02 00:38:29.742554 pyview_web-0.0.7a0/pyview/assets/package.json
+-rw-r--r--   0        0        0       46 2023-05-02 00:38:29.742781 pyview_web-0.0.7a0/pyview/changesets/__init__.py
+-rw-r--r--   0        0        0     1747 2023-05-02 00:38:29.743020 pyview_web-0.0.7a0/pyview/changesets/changesets.py
+-rw-r--r--   0        0        0      789 2023-06-13 01:17:27.976763 pyview_web-0.0.7a0/pyview/csrf.py
+-rw-r--r--   0        0        0      125 2023-06-02 16:20:26.327913 pyview_web-0.0.7a0/pyview/events.py
+-rw-r--r--   0        0        0      751 2023-05-02 00:38:29.743473 pyview_web-0.0.7a0/pyview/js.py
+-rw-r--r--   0        0        0      498 2023-05-02 00:38:29.743607 pyview_web-0.0.7a0/pyview/live_routes.py
+-rw-r--r--   0        0        0     3314 2023-06-02 16:20:26.328472 pyview_web-0.0.7a0/pyview/live_socket.py
+-rw-r--r--   0        0        0     1255 2023-06-13 20:41:53.657377 pyview_web-0.0.7a0/pyview/live_view.py
+-rw-r--r--   0        0        0     3801 2023-06-14 00:15:09.733211 pyview_web-0.0.7a0/pyview/pyview.py
+-rw-r--r--   0        0        0      363 2023-06-13 01:17:27.979329 pyview_web-0.0.7a0/pyview/secret.py
+-rw-r--r--   0        0        0      432 2023-06-13 01:17:27.980035 pyview_web-0.0.7a0/pyview/session.py
+-rw-r--r--   0        0        0   199984 2023-05-02 00:38:29.745551 pyview_web-0.0.7a0/pyview/static/assets/app.js
+-rw-r--r--   0        0        0      124 2023-05-02 00:38:29.745832 pyview_web-0.0.7a0/pyview/template/__init__.py
+-rw-r--r--   0        0        0     1864 2023-05-02 00:38:29.745961 pyview_web-0.0.7a0/pyview/template/live_template.py
+-rw-r--r--   0        0        0      826 2023-05-02 00:38:29.746088 pyview_web-0.0.7a0/pyview/template/serializer.py
+-rw-r--r--   0        0        0      684 2023-05-02 00:38:29.746210 pyview_web-0.0.7a0/pyview/test_csrf.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:38:29.746312 pyview_web-0.0.7a0/pyview/vendor/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-02 00:38:29.746495 pyview_web-0.0.7a0/pyview/vendor/flet/pubsub/__init__.py
+-rw-r--r--   0        0        0    10184 2023-05-02 00:38:29.746630 pyview_web-0.0.7a0/pyview/vendor/flet/pubsub/pub_sub.py
+-rw-r--r--   0        0        0      455 2023-05-02 00:38:29.746775 pyview_web-0.0.7a0/pyview/vendor/ibis/__init__.py
+-rw-r--r--   0        0        0     7220 2023-05-02 00:38:29.746901 pyview_web-0.0.7a0/pyview/vendor/ibis/compiler.py
+-rw-r--r--   0        0        0     3613 2023-05-02 00:38:29.747013 pyview_web-0.0.7a0/pyview/vendor/ibis/context.py
+-rw-r--r--   0        0        0     1531 2023-05-02 00:38:29.747126 pyview_web-0.0.7a0/pyview/vendor/ibis/errors.py
+-rw-r--r--   0        0        0     7042 2023-05-02 00:38:29.747263 pyview_web-0.0.7a0/pyview/vendor/ibis/filters.py
+-rw-r--r--   0        0        0     3457 2023-05-02 00:38:29.747371 pyview_web-0.0.7a0/pyview/vendor/ibis/loaders.py
+-rw-r--r--   0        0        0    25128 2023-05-02 00:38:29.747569 pyview_web-0.0.7a0/pyview/vendor/ibis/nodes.py
+-rw-r--r--   0        0        0     2314 2023-05-02 00:38:29.747704 pyview_web-0.0.7a0/pyview/vendor/ibis/template.py
+-rw-r--r--   0        0        0     2293 2023-05-02 00:38:29.747817 pyview_web-0.0.7a0/pyview/vendor/ibis/tree.py
+-rw-r--r--   0        0        0     2768 2023-05-02 00:38:29.747930 pyview_web-0.0.7a0/pyview/vendor/ibis/utils.py
+-rw-r--r--   0        0        0     4707 2023-06-14 00:15:09.733494 pyview_web-0.0.7a0/pyview/ws_handler.py
+-rw-r--r--   0        0        0     3154 2023-06-13 01:17:27.982729 pyview_web-0.0.7a0/readme.md
+-rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 pyview_web-0.0.7a0/PKG-INFO
```

### Comparing `pyview_web-0.0.6a0/LICENSE` & `pyview_web-0.0.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyproject.toml` & `pyview_web-0.0.7a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "pyview-web"
 
 packages = [
   { include = "pyview" },
 ]
 
-version = "0.0.6a"
+version = "0.0.7a"
 description = "LiveView in Python"
 authors = ["Larry Ogrodnek <ogrodnek@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://pyview.rocks"
 repository = "https://github.com/ogrodnek/pyview"
 keywords = ["web", "api", "LiveView"]
```

### Comparing `pyview_web-0.0.6a0/pyview/assets/js/app.js` & `pyview_web-0.0.7a0/pyview/assets/js/app.js`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/assets/package-lock.json` & `pyview_web-0.0.7a0/pyview/assets/package-lock.json`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/changesets/changesets.py` & `pyview_web-0.0.7a0/pyview/changesets/changesets.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/csrf.py` & `pyview_web-0.0.7a0/pyview/csrf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,25 @@
 from itsdangerous import BadData, SignatureExpired, URLSafeTimedSerializer
-import secrets
 from typing import Optional
 import hmac
-import os
+from pyview.secret import get_secret
 
 
 def generate_csrf_token(value: str, salt: Optional[str] = None) -> str:
     """
     Generate a CSRF token.
     """
-    s = URLSafeTimedSerializer(_get_secret(), salt=salt or "pyview-csrf-token")
+    s = URLSafeTimedSerializer(get_secret(), salt=salt or "pyview-csrf-token")
     return s.dumps(value)  # type: ignore
 
 
 def validate_csrf_token(data: str, expected: str, salt: Optional[str] = None) -> bool:
     """
     Validate a CSRF token.
     """
-    s = URLSafeTimedSerializer(_get_secret(), salt=salt or "pyview-csrf-token")
+    s = URLSafeTimedSerializer(get_secret(), salt=salt or "pyview-csrf-token")
     try:
         token = s.loads(data, max_age=3600)
         return hmac.compare_digest(token, expected)
     except (BadData, SignatureExpired) as e:
         print(e)
         return False
-
-
-_SECRET = None
-
-
-def _get_secret() -> str:
-    """
-    Get the secret key from the environment, or generate a new one.
-    """
-    global _SECRET
-    if _SECRET is None:
-        secret = os.environ.get("PYVIEW_SECRET")
-        if secret is None:
-            secret = secrets.token_urlsafe(16)
-        _SECRET = secret
-
-    return _SECRET
```

### Comparing `pyview_web-0.0.6a0/pyview/js.py` & `pyview_web-0.0.7a0/pyview/js.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/live_socket.py` & `pyview_web-0.0.7a0/pyview/live_socket.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/live_view.py` & `pyview_web-0.0.7a0/pyview/live_view.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from typing import TypeVar, Generic, Optional, Union
+from typing import TypeVar, Generic, Optional, Union, Any
 from .live_socket import LiveViewSocket, UnconnectedSocket
 from pyview.template import LiveTemplate, template_file, RenderedContent, LiveRender
 import inspect
 from pyview.events import InfoEvent
 
 T = TypeVar("T")
 
 AnySocket = Union[LiveViewSocket[T], UnconnectedSocket[T]]
+Session = dict[str, Any]
 
 
 class LiveView(Generic[T]):
     def __init__(self):
         pass
 
-    async def mount(self, socket: AnySocket):
+    async def mount(self, socket: AnySocket, session: Session):
         pass
 
     async def handle_event(self, event, payload, socket: LiveViewSocket[T]):
         pass
 
     async def handle_info(self, event: InfoEvent, socket: LiveViewSocket[T]):
         pass
```

### Comparing `pyview_web-0.0.6a0/pyview/pyview.py` & `pyview_web-0.0.7a0/pyview/pyview.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from starlette.applications import Starlette
 from fastapi import WebSocket
 from fastapi.responses import HTMLResponse
 from starlette.middleware.gzip import GZipMiddleware
+from starlette.middleware.sessions import SessionMiddleware
 from starlette.routing import Route
+from starlette.requests import Request
 import uuid
 from urllib.parse import parse_qs
 
 from pyview.live_socket import UnconnectedSocket
 from pyview.csrf import generate_csrf_token
+from pyview.session import serialize_session
+from pyview.secret import get_secret
 from .ws_handler import LiveSocketHandler
 from .live_view import LiveView
 from .live_routes import LiveViewLookup
 from typing import Callable, Optional, TypedDict
 
 
 class RootTemplateContext(TypedDict):
     id: str
     content: str
     title: Optional[str]
     css: Optional[str]
     csrf_token: str
+    session: Optional[str]
 
 
 RootTemplate = Callable[[RootTemplateContext], str]
 
 
 class PyView(Starlette):
     rootTemplate: RootTemplate
@@ -35,44 +40,45 @@
         self.live_handler = LiveSocketHandler(self.view_lookup)
 
         async def live_websocket_endpoint(websocket: WebSocket):
             await self.live_handler.handle(websocket)
 
         self.add_websocket_route("/live/websocket", live_websocket_endpoint)
         self.add_middleware(GZipMiddleware)
+        # self.add_middleware(SessionMiddleware, secret_key=get_secret())
 
     def add_live_view(self, path: str, view: Callable[[], LiveView]):
-        async def lv(request):
-            return await liveview_container(
-                self.rootTemplate, self.view_lookup, request
-            )
+        async def lv(request: Request):
+            return await liveview_container(self.rootTemplate, self.view_lookup, request)
 
         self.view_lookup.add(path, view)
         self.routes.append(Route(path, lv, methods=["GET"]))
 
 
-async def liveview_container(
-    template: RootTemplate, view_lookup: LiveViewLookup, request
-):
+async def liveview_container(template: RootTemplate, view_lookup: LiveViewLookup, request: Request):
     url = request.url
     path = url.path
     lv: LiveView = view_lookup.get(path)
     s = UnconnectedSocket()
-    await lv.mount(s)
+
+    session = request.session if "session" in request.scope else {}
+
+    await lv.mount(s, session)
     await lv.handle_params(url, parse_qs(url.query), s)
     r = await lv.render(s.context)
 
     id = str(uuid.uuid4())
 
     context: RootTemplateContext = {
         "id": id,
         "content": r.text(),
         "title": s.live_title,
         "csrf_token": generate_csrf_token("lv:phx-" + id),
         "css": None,
+        "session": serialize_session(session),
     }
 
     return HTMLResponse(template(context))
 
 
 def defaultRootTemplate(css: str) -> RootTemplate:
     def template(context: RootTemplateContext) -> str:
@@ -80,19 +86,15 @@
         return _defaultRootTemplate(context)
 
     return template
 
 
 def _defaultRootTemplate(context: RootTemplateContext) -> str:
     suffix = " | LiveView"
-    render_title = (
-        (context["title"] + suffix)  # type: ignore
-        if context.get("title", None) is not None
-        else "LiveView"
-    )
+    render_title = (context["title"] + suffix) if context.get("title", None) is not None else "LiveView"  # type: ignore
     css = context["css"] if context.get("css", None) is not None else ""
     return f"""
 <!DOCTYPE html>
 <html lang="en">
     <head>
       <title data-suffix="{suffix}">{render_title}</title>
       <meta name="csrf-token" content="{context['csrf_token']}" />
@@ -103,15 +105,15 @@
       {css}
     </head>
     <body>
     <div>
       <a href="/">Home</a>
       <div
         data-phx-main="true"
-        data-phx-session=""
+        data-phx-session="{context['session']}"
         data-phx-static=""
         id="phx-{context['id']}"
         >
         {context['content']}
     </div>
     </div>
     </body>
```

### Comparing `pyview_web-0.0.6a0/pyview/static/assets/app.js` & `pyview_web-0.0.7a0/pyview/static/assets/app.js`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/template/live_template.py` & `pyview_web-0.0.7a0/pyview/template/live_template.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/template/serializer.py` & `pyview_web-0.0.7a0/pyview/template/serializer.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/test_csrf.py` & `pyview_web-0.0.7a0/pyview/test_csrf.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/vendor/flet/pubsub/pub_sub.py` & `pyview_web-0.0.7a0/pyview/vendor/flet/pubsub/pub_sub.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/vendor/ibis/compiler.py` & `pyview_web-0.0.7a0/pyview/vendor/ibis/compiler.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/vendor/ibis/context.py` & `pyview_web-0.0.7a0/pyview/vendor/ibis/context.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/vendor/ibis/errors.py` & `pyview_web-0.0.7a0/pyview/vendor/ibis/errors.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/vendor/ibis/filters.py` & `pyview_web-0.0.7a0/pyview/vendor/ibis/filters.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/vendor/ibis/loaders.py` & `pyview_web-0.0.7a0/pyview/vendor/ibis/loaders.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/vendor/ibis/nodes.py` & `pyview_web-0.0.7a0/pyview/vendor/ibis/nodes.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/vendor/ibis/template.py` & `pyview_web-0.0.7a0/pyview/vendor/ibis/template.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/vendor/ibis/tree.py` & `pyview_web-0.0.7a0/pyview/vendor/ibis/tree.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/vendor/ibis/utils.py` & `pyview_web-0.0.7a0/pyview/vendor/ibis/utils.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.6a0/pyview/ws_handler.py` & `pyview_web-0.0.7a0/pyview/ws_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional
 from fastapi import WebSocket, WebSocketDisconnect
 import json
 from urllib.parse import urlparse, parse_qs
 from pyview.live_socket import LiveViewSocket
 from pyview.live_routes import LiveViewLookup
 from pyview.csrf import validate_csrf_token
+from pyview.session import deserialize_session
 
 
 class LiveSocketHandler:
     def __init__(self, routes: LiveViewLookup):
         self.routes = routes
         self.manager = ConnectionManager()
         self.sessions = 0
@@ -27,15 +28,19 @@
                 url = urlparse(payload["url"])
                 lv = self.routes.get(url.path)
                 socket = LiveViewSocket(websocket, topic, lv)
 
                 if not validate_csrf_token(payload["params"]["_csrf_token"], topic):
                     raise Exception("Invalid CSRF token")
 
-                await lv.mount(socket)
+                session = {}
+                if "session" in payload:
+                    session = deserialize_session(payload["session"])
+
+                await lv.mount(socket, session)
                 await lv.handle_params(url, parse_qs(url.query), socket)
 
                 rendered = await _render(socket)
 
                 resp = [
                     joinRef,
                     mesageRef,
@@ -62,17 +67,15 @@
                 resp = [
                     None,
                     mesageRef,
                     "phoenix",
                     "phx_reply",
                     {"response": {}, "status": "ok"},
                 ]
-                await self.manager.send_personal_message(
-                    json.dumps(resp), socket.websocket
-                )
+                await self.manager.send_personal_message(json.dumps(resp), socket.websocket)
                 continue
 
             if event == "event":
                 value = payload["value"]
                 if payload["type"] == "form":
                     value = parse_qs(value)
 
@@ -82,17 +85,15 @@
                 resp = [
                     joinRef,
                     mesageRef,
                     topic,
                     "phx_reply",
                     {"response": {"diff": rendered}, "status": "ok"},
                 ]
-                await self.manager.send_personal_message(
-                    json.dumps(resp), socket.websocket
-                )
+                await self.manager.send_personal_message(json.dumps(resp), socket.websocket)
                 continue
 
             if event == "live_patch":
                 lv = socket.liveview
                 url = urlparse(payload["url"])
 
                 await lv.handle_params(url, parse_qs(url.query), socket)
@@ -101,17 +102,15 @@
                 resp = [
                     joinRef,
                     mesageRef,
                     topic,
                     "phx_reply",
                     {"response": {"diff": rendered}, "status": "ok"},
                 ]
-                await self.manager.send_personal_message(
-                    json.dumps(resp), socket.websocket
-                )
+                await self.manager.send_personal_message(json.dumps(resp), socket.websocket)
                 continue
 
 
 async def _render(socket: LiveViewSocket):
     rendered = (await socket.liveview.render(socket.context)).tree()
 
     if socket.live_title:
```

### Comparing `pyview_web-0.0.6a0/readme.md` & `pyview_web-0.0.7a0/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 class CountContext(TypedDict):
     count: int
 
 
 class CountLiveView(LiveView[CountContext]):
-    async def mount(self, socket: LiveViewSocket[CountContext]):
+    async def mount(self, socket: LiveViewSocket[CountContext], _session):
         socket.context = {"count": 0}
 
     async def handle_event(self, event, payload, socket: LiveViewSocket[CountContext]):
         if event == "decrement":
             socket.context["count"] -= 1
 
         if event == "increment":
```

### Comparing `pyview_web-0.0.6a0/PKG-INFO` & `pyview_web-0.0.7a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyview-web
-Version: 0.0.6a0
+Version: 0.0.7a0
 Summary: LiveView in Python
 Home-page: https://pyview.rocks
 License: MIT
 Keywords: web,api,LiveView
 Author: Larry Ogrodnek
 Author-email: ogrodnek@gmail.com
 Requires-Python: >=3.9.16,<4.0.0
@@ -75,15 +75,15 @@
 
 
 class CountContext(TypedDict):
     count: int
 
 
 class CountLiveView(LiveView[CountContext]):
-    async def mount(self, socket: LiveViewSocket[CountContext]):
+    async def mount(self, socket: LiveViewSocket[CountContext], _session):
         socket.context = {"count": 0}
 
     async def handle_event(self, event, payload, socket: LiveViewSocket[CountContext]):
         if event == "decrement":
             socket.context["count"] -= 1
 
         if event == "increment":
```

